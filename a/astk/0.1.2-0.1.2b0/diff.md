# Comparing `tmp/astk-0.1.2.tar.gz` & `tmp/astk-0.1.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astk-0.1.2.tar", last modified: Sun Nov 27 07:33:36 2022, max compression
+gzip compressed data, was "astk-0.1.2b0.tar", last modified: Sat May  6 06:49:18 2023, max compression
```

## Comparing `astk-0.1.2.tar` & `astk-0.1.2b0.tar`

### file list

```diff
@@ -1,424 +1,419 @@
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.432768 astk-0.1.2/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1527 2022-11-03 01:59:44.000000 astk-0.1.2/LICENSE
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       44 2022-11-03 01:59:44.000000 astk-0.1.2/MANIFEST.in
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      164 2022-11-27 07:33:36.431768 astk-0.1.2/PKG-INFO
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      393 2022-11-03 01:59:44.000000 astk-0.1.2/README.md
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.059768 astk-0.1.2/astk/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)  4012487 2022-11-03 01:59:44.000000 astk-0.1.2/astk/ChromHMM.jar
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      810 2022-11-03 01:59:44.000000 astk-0.1.2/astk/ChromHMM.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.092768 astk-0.1.2/astk/R/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      756 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/ChromHMM_hm.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3672 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/CoSpliceNet.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1778 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/barplot.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      168 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/dl_keggdata.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2553 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/enrich.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2795 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/enrichCompare.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10069 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/epiFeature.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2239 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/epiProfile.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2502 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/gsea.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1048 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/gseaPlot.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1965 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/heatmap.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2678 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/install.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      462 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/makeTxDb.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2048 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/motifEnrich.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2095 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/motifFind.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3259 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/motifMap.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      631 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/motifPlot.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1747 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/pca.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      689 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/seqLogo.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1163 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/signalCompare.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1670 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/signalHeatmap.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1182 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/signalProfile.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1635 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/upset.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    14862 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/utils.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1324 2022-11-03 01:59:44.000000 astk-0.1.2/astk/R/volcano.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      691 2022-11-03 01:59:44.000000 astk-0.1.2/astk/__init__.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.094768 astk-0.1.2/astk/cli/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2946 2022-11-20 08:22:21.000000 astk-0.1.2/astk/cli/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5376 2022-11-03 01:59:44.000000 astk-0.1.2/astk/cli/as_event.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6025 2022-11-03 01:59:44.000000 astk-0.1.2/astk/cli/config.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5836 2022-11-03 01:59:44.000000 astk-0.1.2/astk/cli/draw.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9832 2022-11-03 01:59:44.000000 astk-0.1.2/astk/cli/epi.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8064 2022-11-03 02:11:49.000000 astk-0.1.2/astk/cli/gsea.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5451 2022-11-20 08:30:11.000000 astk-0.1.2/astk/cli/motif.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      928 2022-11-03 01:59:44.000000 astk-0.1.2/astk/cli/net.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8175 2022-11-22 13:13:19.000000 astk-0.1.2/astk/cli/seqfeature.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5139 2022-11-14 08:14:14.000000 astk-0.1.2/astk/cli/suppa.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6302 2022-11-03 01:59:44.000000 astk-0.1.2/astk/cli/utils.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4548 2022-11-03 01:59:44.000000 astk-0.1.2/astk/constant.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:35.960768 astk-0.1.2/astk/data/
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.127768 astk-0.1.2/astk/data/maxent/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)  1595043 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/maxent/ss3_score.json
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   472299 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/maxent/ss5seq_score.json
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:35.961768 astk-0.1.2/astk/data/motif/
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.205768 astk-0.1.2/astk/data/motif/ATtRACT/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4459 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Arabidopsis_thaliana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1251 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Aspergillus_nidulans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      634 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Bombyx_mori.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      571 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Bos_taurus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      506 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Brachypodium_distachyon.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    32322 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Caenorhabditis_elegans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      502 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Chaetomium_thermophilum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      921 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Cricetulus_griseus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2679 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Danio_rerio.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    47701 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Drosophila_melanogaster.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6358 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Gallus_gallus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   674737 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Homo_sapiens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2388 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Leishmania_major.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1454 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Mesocricetus_auratus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29005 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Mus_musculus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      738 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Naegleria_gruberi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      776 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Nematostella_vectensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1309 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Neurospora_crassa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2523 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Oryctolagus_cuniculus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1352 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Oryzias_latipes.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1274 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Ostreococcus_tauri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1937 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Physcomitrella_patens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      716 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Phytophthora_ramorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4695 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Plasmodium_falciparum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11158 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Rattus_norvegicus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      670 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Rhizopus_oryzae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    43405 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      629 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae_s288c.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      682 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Schistosoma_mansoni.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1540 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Spodoptera_frugiperda.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1307 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Tetraodon_nigroviridis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      687 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Thalassiosira_pseudonana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3021 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Trichomonas_vaginalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4015 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Trypanosoma_brucei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      836 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Vanderwaltozyma_polyspora.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6096 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Xenopus_laevis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4865 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Xenopus_tropicalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2441 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ATtRACT/Zea_mays.meme
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.361768 astk-0.1.2/astk/data/motif/CISBP-RNA/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    14270 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Acyrtosiphon_pisum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    18150 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aedes_aegypti.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1703 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Agaricus_bisporus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37235 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ailuropoda_melanoleuca.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1143 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Allomyces_macrogynus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2163 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Alternaria_brassicicola.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5774 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Amphimedon_queenslandica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31421 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Anolis_carolinensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    18154 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Anopheles_gambiae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20491 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Apis_mellifera.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4315 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Arabidopsis_lyrata.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3679 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Arabidopsis_thaliana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Arthroderma_benhamiae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2438 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ashbya_gossypii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2211 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_carbonarius.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_clavatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1664 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_flavus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2175 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_fumigatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2101 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_nidulans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_niger.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1157 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_oryzae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_terreus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1188 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Aureococcus_anophagefferens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1216 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Batrachochytrium_dendrobatidis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Blastomyces_dermatitidis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    13085 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Bombyx_mori.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38156 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Bos_taurus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Botrytis_cinerea.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3742 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Brachypodium_distachyon.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    19275 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Branchiostoma_floridae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5171 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Brugia_malayi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9824 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_brenneri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10312 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_briggsae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10846 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_elegans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8805 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_japonica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9823 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_remanei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    40543 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Callithrix_jacchus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      637 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_albicans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_dubliniensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_glabrata.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_guilliermondii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_lusitaniae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_parapsilosis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_tropicalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37241 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Canis_familiaris.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3721 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Cannabis_sativa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15084 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Capitella_teleta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1143 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Capsaspora_owczarzaki.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37866 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Cavia_porcellus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Chaetomium_globosum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1157 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Chlamydomonas_reinhardtii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1655 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Chlorella_NC64A.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1172 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Chlorella_vulgaris.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21518 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Choloepus_hoffmanni.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9963 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ciona_intestinalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9399 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ciona_savignyi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Coccidioides_immitis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Coccidioides_posadasii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1172 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Coccomyxa_C_169.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2236 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Cochliobolus_heterostrophus_C5.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Colletotrichum_graminicola.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Coprinopsis_cinerea.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2760 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Cryphonectria_parasitica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Cryptosporidium_hominis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      642 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Cryptosporidium_parvum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4245 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Cucumis_sativus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15784 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Culex_pipiens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15604 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Culex_quinquefasciatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    33623 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Danio_rerio.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15219 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Daphnia_pulex.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23518 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Dasypus_novemcinctus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Debaryomyces_hansenii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      639 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Dictyostelium_discoideum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Dictyostelium_purpureum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31954 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Dipodomys_ordii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23747 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_ananassae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22774 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_erecta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21646 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_grimshawi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26626 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_melanogaster.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24185 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_mojavensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    19664 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_persimilis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22874 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_pseudoobscura.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23799 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_sechellia.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20806 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_simulans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21658 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_virilis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22709 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_willistoni.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24840 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_yakuba.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28911 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Echinops_telfairi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1218 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Emiliania_huxleyi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35839 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Equus_caballus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24489 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Erinaceus_europaeus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20944 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Felis_catus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      659 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Fragilariopsis_cylindrus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Fusarium_graminearum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Fusarium_oxysporum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Fusarium_verticillioides.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30729 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Gallus_gallus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31435 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Gasterosteus_aculeatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4280 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Glycine_max.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37787 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Gorilla_gorilla.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11728 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Helobdella_robusta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Heterobasidion_annosum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Histoplasma_capsulatum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    46774 2022-11-21 03:15:49.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Homo_sapiens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5292 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Hydra_magnipapillata.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9004 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ixodes_scapularis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Kluyveromyces_lactis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Kluyveromyces_thermotolerans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2451 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Kluyveromyces_waltii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1666 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Laccaria_bicolor.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Lachancea_kluyveri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3189 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Leishmania_braziliensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2680 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Leishmania_infantum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3043 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Leishmania_major.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3171 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Leishmania_mexicana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6695 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Loa_loa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Lodderomyces_elongisporus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    13348 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Lottia_gigantea.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3269 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Lotus_japonicus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35812 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Loxodonta_africana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37085 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Macaca_mulatta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26202 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Macropus_eugenii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2713 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Magnaporthe_oryzae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Malassezia_globosa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3760 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Malus_x_domestica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3796 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Manihot_esculenta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3746 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Medicago_truncatula.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1189 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Melampsora_laricis_populina.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28964 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Meleagris_gallopavo.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5218 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Meloidogyne_incognita.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Microcebus_murinus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1162 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Micromonas_pusilla.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Microsporum_canis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Microsporum_gypseum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3780 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Mimulus_guttatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37066 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Monodelphis_domestica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1177 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Monosiga_brevicollis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1709 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Mucor_circinelloides.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38188 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Mus_musculus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2802 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Myceliophthora_thermophila.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1693 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Mycosphaerella_fijiensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1719 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Mycosphaerella_graminicola.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28910 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Myotis_lucifugus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      622 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Naegleria_gruberi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    16833 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Nasonia_vitripennis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2833 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Nectria_haematococca.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10051 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Nematostella_vectensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Neosartorya_fischeri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Neospora_caninum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2642 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Neurospora_crassa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2234 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Neurospora_discreta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2799 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Neurospora_tetrasperma.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    27878 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ochotona_princeps.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4841 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Oikopleura_dioica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29248 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ornithorhynchus_anatinus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37518 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Oryctolagus_cuniculus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2733 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Oryza_indica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3242 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Oryza_sativa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31120 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Oryzias_latipes.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1656 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ostreococcus_RCC809.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1153 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ostreococcus_lucimarinus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2134 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ostreococcus_tauri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22825 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Otolemur_garnettii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38413 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pan_troglodytes.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Paracoccidioides_brasiliensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    16093 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pediculus_humanus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Penicillium_chrysogenum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Penicillium_marneffei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      649 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Phaeodactylum_tricornutum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Phaeosphaeria_nodorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1683 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Phanerochaete_chrysosporium.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1720 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Phoenix_dactylifera.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2209 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Phycomyces_blakesleeanus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3736 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Physcomitrella_patens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1173 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Phytophthora_capsici.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Phytophthora_infestans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1145 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Phytophthora_ramorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      638 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Phytophthora_sojae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      647 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pichia_pastoris.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      711 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pichia_stipitis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3812 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_berghei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4317 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_chabaudi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3995 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_falciparum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3791 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_knowlesi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3791 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_vivax.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2756 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_yoelii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1705 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pleurotus_ostreatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1674 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pneumocystis_carinii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2714 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Podospora_anserina.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1200 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Polysphondylium_pallidum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37096 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pongo_pygmaeus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4245 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Populus_trichocarpa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1713 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Postia_placenta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4162 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pristionchus_pacificus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26820 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Procavia_capensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3739 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Prunus_persica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35919 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pteropus_vampyrus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Pyrenophora_tritici_repentis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6506 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/RNAcompete_CONSTRUCTS.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38860 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Rattus_norvegicus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1616 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Rhizopus_oryzae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3749 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ricinus_communis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_bayanus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1914 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_castellii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2310 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_cerevisiae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1217 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_kudriavzevii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_mikatae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_paradoxus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1644 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Salpingoeca_rosetta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Saprolegnia_parasitica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3721 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Schistosoma_japonicum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5826 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Schistosoma_mansoni.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2215 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Schizophyllum_commune.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Schizosaccharomyces_cryophilus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Schizosaccharomyces_japonicus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Schizosaccharomyces_octosporus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      639 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Schizosaccharomyces_pombe.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Sclerotinia_sclerotiorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3271 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Selaginella_moellendorfii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1702 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Serpula_lacrymans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23198 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Sorex_araneus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3224 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Sorghum_bicolor.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20742 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Spermophilus_tridecemlineatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2145 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Spizellomyces_punctatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Sporobolomyces_roseus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Stagonospora_nodorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10832 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Strongylocentrotus_purpuratus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29388 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Sus_scrofa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    32434 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Taeniopygia_guttata.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30452 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Takifugu_rubripes.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26504 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Tarsius_syrichta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31987 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Tetraodon_nigroviridis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1125 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Thalassiosira_pseudonana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Thecamonas_trahens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2817 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Thielavia_terrestris.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Toxoplasma_gondii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Tremella_mesenterica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1715 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Tribolium_castaneum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2207 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trichoderma_atroviride.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2786 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trichoderma_reesei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2794 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trichoderma_virens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2546 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trichomonas_vaginalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trichophyton_equinum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trichophyton_rubrum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trichophyton_tonsurans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trichophyton_verrucosum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6932 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trichoplax_adhaerens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5682 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trypanosoma_brucei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4326 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trypanosoma_congolense.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2773 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trypanosoma_cruzi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2735 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Trypanosoma_vivax.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1682 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Tuber_melanosporum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23608 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Tupaia_belangeri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    34596 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Tursiops_truncatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Uncinocarpus_reesii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1146 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Ustilago_maydis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Vanderwaltozyma_polyspora.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Verticillium_albo_atrum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2212 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Verticillium_dahliae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26009 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Vicugna_pacos.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3777 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Vitis_vinifera.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Volvox_carteri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5691 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Wuchereria_bancrofti.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30403 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Xenopus_laevis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    34934 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Xenopus_tropicalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Yarrowia_lipolytica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3236 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Zea_mays.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/CISBP-RNA/Zygosaccharomyces_rouxii.meme
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.418768 astk-0.1.2/astk/data/motif/ELM/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    79014 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ELM/elm_classes.tsv
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   855778 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ELM/elm_instances.tsv
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003) 11720265 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ELM/hg38_alter_exon_seq.json
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)  4375026 2022-11-03 01:59:44.000000 astk-0.1.2/astk/data/motif/ELM/mm10_alter_exon_seq.json
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.425768 astk-0.1.2/astk/draw/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      123 2022-11-03 01:59:44.000000 astk-0.1.2/astk/draw/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3097 2022-11-03 01:59:44.000000 astk-0.1.2/astk/draw/_func.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.425768 astk-0.1.2/astk/epi/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      253 2022-11-03 01:59:44.000000 astk-0.1.2/astk/epi/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11719 2022-11-03 01:59:44.000000 astk-0.1.2/astk/epi/_func.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.426768 astk-0.1.2/astk/event/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      127 2022-11-03 01:59:44.000000 astk-0.1.2/astk/event/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5219 2022-11-03 01:59:44.000000 astk-0.1.2/astk/event/_cli_func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3083 2022-11-14 08:15:26.000000 astk-0.1.2/astk/event/eid.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.426768 astk-0.1.2/astk/gsea/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      237 2022-11-03 02:11:49.000000 astk-0.1.2/astk/gsea/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7118 2022-11-21 04:21:25.000000 astk-0.1.2/astk/gsea/_func.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.427768 astk-0.1.2/astk/motif/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      151 2022-11-03 01:59:44.000000 astk-0.1.2/astk/motif/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6138 2022-11-21 03:08:32.000000 astk-0.1.2/astk/motif/_func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1641 2022-11-03 01:59:44.000000 astk-0.1.2/astk/motif/elm.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.427768 astk-0.1.2/astk/network/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      132 2022-11-03 01:59:44.000000 astk-0.1.2/astk/network/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2358 2022-11-03 01:59:44.000000 astk-0.1.2/astk/network/_func.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.428768 astk-0.1.2/astk/seqfeature/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      121 2022-11-03 01:59:44.000000 astk-0.1.2/astk/seqfeature/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5366 2022-11-22 13:47:57.000000 astk-0.1.2/astk/seqfeature/_compare.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3862 2022-11-03 01:59:44.000000 astk-0.1.2/astk/seqfeature/_feature.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3979 2022-11-20 08:34:02.000000 astk-0.1.2/astk/seqfeature/_splice_score.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4095 2022-11-03 01:59:44.000000 astk-0.1.2/astk/seqfeature/feature.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.429768 astk-0.1.2/astk/suppa/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31571 2022-11-10 11:53:35.000000 astk-0.1.2/astk/suppa/AS_event.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      105 2022-11-03 01:59:44.000000 astk-0.1.2/astk/suppa/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7067 2022-11-14 08:14:12.000000 astk-0.1.2/astk/suppa/_func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1264 2022-11-09 03:17:16.000000 astk-0.1.2/astk/suppa/event_psi.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4434 2022-11-03 01:59:44.000000 astk-0.1.2/astk/suppa/gtf_parse.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.430768 astk-0.1.2/astk/suppa/lib/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       84 2022-11-03 01:59:44.000000 astk-0.1.2/astk/suppa/lib/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23418 2022-11-03 01:59:44.000000 astk-0.1.2/astk/suppa/lib/diff_tools.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24715 2022-11-03 01:59:44.000000 astk-0.1.2/astk/suppa/lib/event.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8048 2022-11-03 01:59:44.000000 astk-0.1.2/astk/suppa/lib/gtf_store.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    12030 2022-11-03 01:59:44.000000 astk-0.1.2/astk/suppa/lib/optics.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22325 2022-11-03 01:59:44.000000 astk-0.1.2/astk/suppa/lib/tools.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24158 2022-11-03 01:59:44.000000 astk-0.1.2/astk/suppa/lib/var_event.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      221 2022-11-03 01:59:44.000000 astk-0.1.2/astk/types.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.431768 astk-0.1.2/astk/utils/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      173 2022-11-03 01:59:44.000000 astk-0.1.2/astk/utils/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4534 2022-11-20 08:39:05.000000 astk-0.1.2/astk/utils/_cli_func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8465 2022-11-10 08:16:02.000000 astk-0.1.2/astk/utils/_coord.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      502 2022-11-20 07:25:11.000000 astk-0.1.2/astk/utils/_getfasta.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15361 2022-11-20 07:00:42.000000 astk-0.1.2/astk/utils/func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4629 2022-11-03 01:59:44.000000 astk-0.1.2/astk/utils/meta_template.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5161 2022-11-03 01:59:44.000000 astk-0.1.2/astk/utils/select.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2022-11-27 07:33:36.060768 astk-0.1.2/astk.egg-info/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      164 2022-11-27 07:33:35.000000 astk-0.1.2/astk.egg-info/PKG-INFO
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    17679 2022-11-27 07:33:35.000000 astk-0.1.2/astk.egg-info/SOURCES.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        1 2022-11-27 07:33:35.000000 astk-0.1.2/astk.egg-info/dependency_links.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       42 2022-11-27 07:33:35.000000 astk-0.1.2/astk.egg-info/entry_points.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      180 2022-11-27 07:33:35.000000 astk-0.1.2/astk.egg-info/requires.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        5 2022-11-27 07:33:35.000000 astk-0.1.2/astk.egg-info/top_level.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       38 2022-11-27 07:33:36.432768 astk-0.1.2/setup.cfg
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      936 2022-11-20 08:52:45.000000 astk-0.1.2/setup.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.221081 astk-0.1.2b0/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1527 2022-11-03 01:59:44.000000 astk-0.1.2b0/LICENSE
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       44 2022-11-03 01:59:44.000000 astk-0.1.2b0/MANIFEST.in
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1036 2023-05-06 06:49:18.220081 astk-0.1.2b0/PKG-INFO
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      762 2023-05-05 06:43:18.000000 astk-0.1.2b0/README.md
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.134081 astk-0.1.2b0/astk/
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.137081 astk-0.1.2b0/astk/R/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3672 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/R/CoSpliceNet.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      168 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/R/dl_keggdata.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2968 2023-05-04 06:15:41.000000 astk-0.1.2b0/astk/R/enrich.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3294 2023-05-04 06:46:26.000000 astk-0.1.2b0/astk/R/enrichCompare.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2869 2023-04-14 02:29:46.000000 astk-0.1.2b0/astk/R/gsea.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1048 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/R/gseaPlot.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2613 2023-04-30 07:09:14.000000 astk-0.1.2b0/astk/R/install.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      462 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/R/makeTxDb.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3259 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/R/motifMap.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      631 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/R/motifPlot.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      689 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/R/seqLogo.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1635 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/R/upset.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    14912 2023-05-03 02:48:27.000000 astk-0.1.2b0/astk/R/utils.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        0 2023-02-20 01:59:46.000000 astk-0.1.2b0/astk/__init__.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.139081 astk-0.1.2b0/astk/cli/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      235 2023-03-11 08:22:05.000000 astk-0.1.2b0/astk/cli/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      491 2023-03-26 13:53:39.000000 astk-0.1.2b0/astk/cli/aliases.ini
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5031 2023-03-16 14:16:18.000000 astk-0.1.2b0/astk/cli/as_event.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8716 2023-05-03 06:40:12.000000 astk-0.1.2b0/astk/cli/config.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6144 2023-05-05 07:14:52.000000 astk-0.1.2b0/astk/cli/draw.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3445 2023-04-30 14:54:26.000000 astk-0.1.2b0/astk/cli/epi.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1816 2023-03-30 12:17:52.000000 astk-0.1.2b0/astk/cli/experiment.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7458 2023-05-04 06:46:28.000000 astk-0.1.2b0/astk/cli/gsea.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9104 2023-04-30 14:36:22.000000 astk-0.1.2b0/astk/cli/ml.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5632 2023-02-20 01:59:46.000000 astk-0.1.2b0/astk/cli/motif.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      928 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/cli/net.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8307 2023-04-10 12:32:20.000000 astk-0.1.2b0/astk/cli/seqfeature.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5551 2023-04-07 06:56:36.000000 astk-0.1.2b0/astk/cli/suppa.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11856 2023-03-13 06:26:06.000000 astk-0.1.2b0/astk/cli/utils.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4617 2023-03-04 08:32:09.000000 astk-0.1.2b0/astk/constant.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      237 2023-03-17 02:36:37.000000 astk-0.1.2b0/astk/ctypes.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.132081 astk-0.1.2b0/astk/data/
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.141081 astk-0.1.2b0/astk/data/maxent/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)  1595043 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/maxent/ss3_score.json
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   472299 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/maxent/ss5seq_score.json
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.132081 astk-0.1.2b0/astk/data/motif/
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.149081 astk-0.1.2b0/astk/data/motif/ATtRACT/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4459 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Arabidopsis_thaliana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1251 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Aspergillus_nidulans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      634 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Bombyx_mori.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      571 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Bos_taurus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      506 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Brachypodium_distachyon.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    32322 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Caenorhabditis_elegans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      502 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Chaetomium_thermophilum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      921 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Cricetulus_griseus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2679 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Danio_rerio.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    47701 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Drosophila_melanogaster.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6358 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Gallus_gallus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   674737 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Homo_sapiens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2388 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Leishmania_major.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1454 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Mesocricetus_auratus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29005 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Mus_musculus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      738 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Naegleria_gruberi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      776 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Nematostella_vectensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1309 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Neurospora_crassa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2523 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Oryctolagus_cuniculus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1352 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Oryzias_latipes.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1274 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Ostreococcus_tauri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1937 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Physcomitrella_patens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      716 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Phytophthora_ramorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4695 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Plasmodium_falciparum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11158 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Rattus_norvegicus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      670 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Rhizopus_oryzae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    43405 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      629 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae_s288c.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      682 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Schistosoma_mansoni.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1540 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Spodoptera_frugiperda.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1307 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Tetraodon_nigroviridis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      687 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Thalassiosira_pseudonana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3021 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Trichomonas_vaginalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4015 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Trypanosoma_brucei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      836 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Vanderwaltozyma_polyspora.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6096 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Xenopus_laevis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4865 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Xenopus_tropicalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2441 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ATtRACT/Zea_mays.meme
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.194081 astk-0.1.2b0/astk/data/motif/CISBP-RNA/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    14270 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Acyrtosiphon_pisum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    18150 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aedes_aegypti.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1703 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Agaricus_bisporus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37235 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ailuropoda_melanoleuca.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1143 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Allomyces_macrogynus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2163 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Alternaria_brassicicola.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5774 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Amphimedon_queenslandica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31421 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Anolis_carolinensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    18154 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Anopheles_gambiae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20491 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Apis_mellifera.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4315 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Arabidopsis_lyrata.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3679 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Arabidopsis_thaliana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Arthroderma_benhamiae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2438 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ashbya_gossypii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2211 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_carbonarius.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_clavatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1664 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_flavus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2175 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_fumigatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2101 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_nidulans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_niger.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1157 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_oryzae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_terreus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1188 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aureococcus_anophagefferens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1216 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Batrachochytrium_dendrobatidis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Blastomyces_dermatitidis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    13085 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Bombyx_mori.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38156 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Bos_taurus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Botrytis_cinerea.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3742 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Brachypodium_distachyon.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    19275 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Branchiostoma_floridae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5171 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Brugia_malayi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9824 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_brenneri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10312 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_briggsae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10846 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_elegans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8805 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_japonica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9823 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_remanei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    40543 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Callithrix_jacchus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      637 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_albicans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_dubliniensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_glabrata.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_guilliermondii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_lusitaniae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_parapsilosis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_tropicalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37241 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Canis_familiaris.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3721 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cannabis_sativa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15084 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Capitella_teleta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1143 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Capsaspora_owczarzaki.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37866 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cavia_porcellus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Chaetomium_globosum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1157 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Chlamydomonas_reinhardtii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1655 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Chlorella_NC64A.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1172 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Chlorella_vulgaris.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21518 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Choloepus_hoffmanni.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9963 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ciona_intestinalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9399 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ciona_savignyi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Coccidioides_immitis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Coccidioides_posadasii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1172 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Coccomyxa_C_169.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2236 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cochliobolus_heterostrophus_C5.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Colletotrichum_graminicola.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Coprinopsis_cinerea.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2760 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cryphonectria_parasitica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cryptosporidium_hominis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      642 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cryptosporidium_parvum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4245 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cucumis_sativus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15784 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Culex_pipiens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15604 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Culex_quinquefasciatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    33623 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Danio_rerio.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15219 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Daphnia_pulex.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23518 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Dasypus_novemcinctus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Debaryomyces_hansenii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      639 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Dictyostelium_discoideum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Dictyostelium_purpureum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31954 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Dipodomys_ordii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23747 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_ananassae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22774 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_erecta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21646 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_grimshawi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26626 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_melanogaster.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24185 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_mojavensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    19664 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_persimilis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22874 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_pseudoobscura.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23799 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_sechellia.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20806 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_simulans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21658 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_virilis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22709 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_willistoni.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24840 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_yakuba.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28911 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Echinops_telfairi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1218 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Emiliania_huxleyi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35839 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Equus_caballus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24489 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Erinaceus_europaeus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20944 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Felis_catus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      659 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Fragilariopsis_cylindrus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Fusarium_graminearum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Fusarium_oxysporum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Fusarium_verticillioides.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30729 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Gallus_gallus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31435 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Gasterosteus_aculeatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4280 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Glycine_max.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37787 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Gorilla_gorilla.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11728 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Helobdella_robusta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Heterobasidion_annosum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Histoplasma_capsulatum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    46774 2022-11-21 03:15:49.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Homo_sapiens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5292 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Hydra_magnipapillata.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9004 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ixodes_scapularis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Kluyveromyces_lactis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Kluyveromyces_thermotolerans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2451 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Kluyveromyces_waltii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1666 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Laccaria_bicolor.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Lachancea_kluyveri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3189 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Leishmania_braziliensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2680 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Leishmania_infantum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3043 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Leishmania_major.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3171 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Leishmania_mexicana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6695 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Loa_loa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Lodderomyces_elongisporus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    13348 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Lottia_gigantea.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3269 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Lotus_japonicus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35812 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Loxodonta_africana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37085 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Macaca_mulatta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26202 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Macropus_eugenii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2713 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Magnaporthe_oryzae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Malassezia_globosa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3760 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Malus_x_domestica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3796 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Manihot_esculenta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3746 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Medicago_truncatula.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1189 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Melampsora_laricis_populina.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28964 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Meleagris_gallopavo.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5218 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Meloidogyne_incognita.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Microcebus_murinus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1162 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Micromonas_pusilla.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Microsporum_canis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Microsporum_gypseum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3780 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mimulus_guttatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37066 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Monodelphis_domestica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1177 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Monosiga_brevicollis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1709 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mucor_circinelloides.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38188 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mus_musculus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2802 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Myceliophthora_thermophila.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1693 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mycosphaerella_fijiensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1719 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mycosphaerella_graminicola.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28910 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Myotis_lucifugus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      622 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Naegleria_gruberi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    16833 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Nasonia_vitripennis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2833 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Nectria_haematococca.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10051 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Nematostella_vectensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neosartorya_fischeri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neospora_caninum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2642 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neurospora_crassa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2234 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neurospora_discreta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2799 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neurospora_tetrasperma.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    27878 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ochotona_princeps.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4841 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oikopleura_dioica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29248 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ornithorhynchus_anatinus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37518 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oryctolagus_cuniculus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2733 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oryza_indica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3242 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oryza_sativa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31120 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oryzias_latipes.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1656 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ostreococcus_RCC809.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1153 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ostreococcus_lucimarinus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2134 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ostreococcus_tauri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22825 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Otolemur_garnettii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38413 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pan_troglodytes.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Paracoccidioides_brasiliensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    16093 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pediculus_humanus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Penicillium_chrysogenum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Penicillium_marneffei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      649 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phaeodactylum_tricornutum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phaeosphaeria_nodorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1683 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phanerochaete_chrysosporium.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1720 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phoenix_dactylifera.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2209 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phycomyces_blakesleeanus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3736 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Physcomitrella_patens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1173 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phytophthora_capsici.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phytophthora_infestans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1145 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phytophthora_ramorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      638 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phytophthora_sojae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      647 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pichia_pastoris.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      711 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pichia_stipitis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3812 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_berghei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4317 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_chabaudi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3995 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_falciparum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3791 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_knowlesi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3791 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_vivax.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2756 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_yoelii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1705 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pleurotus_ostreatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1674 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pneumocystis_carinii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2714 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Podospora_anserina.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1200 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Polysphondylium_pallidum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37096 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pongo_pygmaeus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4245 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Populus_trichocarpa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1713 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Postia_placenta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4162 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pristionchus_pacificus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26820 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Procavia_capensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3739 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Prunus_persica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35919 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pteropus_vampyrus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pyrenophora_tritici_repentis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6506 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/RNAcompete_CONSTRUCTS.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38860 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Rattus_norvegicus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1616 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Rhizopus_oryzae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3749 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ricinus_communis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_bayanus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1914 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_castellii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2310 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_cerevisiae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1217 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_kudriavzevii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_mikatae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_paradoxus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1644 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Salpingoeca_rosetta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saprolegnia_parasitica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3721 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schistosoma_japonicum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5826 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schistosoma_mansoni.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2215 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizophyllum_commune.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_cryophilus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_japonicus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_octosporus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      639 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_pombe.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sclerotinia_sclerotiorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3271 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Selaginella_moellendorfii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1702 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Serpula_lacrymans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23198 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sorex_araneus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3224 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sorghum_bicolor.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20742 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Spermophilus_tridecemlineatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2145 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Spizellomyces_punctatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sporobolomyces_roseus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Stagonospora_nodorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10832 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Strongylocentrotus_purpuratus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29388 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sus_scrofa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    32434 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Taeniopygia_guttata.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30452 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Takifugu_rubripes.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26504 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tarsius_syrichta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31987 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tetraodon_nigroviridis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1125 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Thalassiosira_pseudonana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Thecamonas_trahens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2817 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Thielavia_terrestris.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Toxoplasma_gondii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tremella_mesenterica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1715 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tribolium_castaneum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2207 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichoderma_atroviride.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2786 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichoderma_reesei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2794 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichoderma_virens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2546 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichomonas_vaginalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichophyton_equinum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichophyton_rubrum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichophyton_tonsurans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichophyton_verrucosum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6932 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichoplax_adhaerens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5682 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trypanosoma_brucei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4326 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trypanosoma_congolense.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2773 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trypanosoma_cruzi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2735 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trypanosoma_vivax.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1682 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tuber_melanosporum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23608 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tupaia_belangeri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    34596 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tursiops_truncatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Uncinocarpus_reesii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1146 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ustilago_maydis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Vanderwaltozyma_polyspora.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Verticillium_albo_atrum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2212 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Verticillium_dahliae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26009 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Vicugna_pacos.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3777 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Vitis_vinifera.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Volvox_carteri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5691 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Wuchereria_bancrofti.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30403 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Xenopus_laevis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    34934 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Xenopus_tropicalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Yarrowia_lipolytica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3236 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Zea_mays.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/CISBP-RNA/Zygosaccharomyces_rouxii.meme
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.208081 astk-0.1.2b0/astk/data/motif/ELM/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    79014 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ELM/elm_classes.tsv
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   855778 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ELM/elm_instances.tsv
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003) 11720265 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ELM/hg38_alter_exon_seq.json
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)  4375026 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/data/motif/ELM/mm10_alter_exon_seq.json
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.213081 astk-0.1.2b0/astk/draw/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      123 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/draw/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6863 2023-05-05 07:15:54.000000 astk-0.1.2b0/astk/draw/_func.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.214081 astk-0.1.2b0/astk/epi/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      236 2023-04-30 14:39:09.000000 astk-0.1.2b0/astk/epi/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7159 2023-04-30 14:52:01.000000 astk-0.1.2b0/astk/epi/_func.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.214081 astk-0.1.2b0/astk/event/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      152 2023-02-27 08:00:31.000000 astk-0.1.2b0/astk/event/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6026 2023-03-17 02:40:47.000000 astk-0.1.2b0/astk/event/_cli_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3009 2023-04-07 12:22:47.000000 astk-0.1.2b0/astk/event/eid.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.215081 astk-0.1.2b0/astk/gsea/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      237 2022-11-28 11:24:56.000000 astk-0.1.2b0/astk/gsea/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6330 2023-05-03 13:57:59.000000 astk-0.1.2b0/astk/gsea/_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1537 2023-03-08 12:39:17.000000 astk-0.1.2b0/astk/lazy_loader.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.215081 astk-0.1.2b0/astk/ml/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       89 2023-03-26 13:56:20.000000 astk-0.1.2b0/astk/ml/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2713 2023-03-26 13:56:20.000000 astk-0.1.2b0/astk/ml/_chunk_permutation_importance.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2869 2023-03-26 13:56:20.000000 astk-0.1.2b0/astk/ml/_metric.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4506 2023-03-30 12:07:57.000000 astk-0.1.2b0/astk/ml/_tools.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.216081 astk-0.1.2b0/astk/motif/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      151 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/motif/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6099 2023-03-11 07:50:42.000000 astk-0.1.2b0/astk/motif/_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1641 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/motif/elm.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.216081 astk-0.1.2b0/astk/network/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      132 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/network/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2358 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/network/_func.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.217081 astk-0.1.2b0/astk/seqfeature/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      121 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/seqfeature/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5220 2023-04-30 07:04:25.000000 astk-0.1.2b0/astk/seqfeature/_compare.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3774 2023-04-10 07:31:13.000000 astk-0.1.2b0/astk/seqfeature/_feature.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3735 2023-03-10 02:43:17.000000 astk-0.1.2b0/astk/seqfeature/_splice_score.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4067 2023-04-24 12:34:54.000000 astk-0.1.2b0/astk/seqfeature/feature.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.218081 astk-0.1.2b0/astk/suppa/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31571 2023-01-22 11:43:29.000000 astk-0.1.2b0/astk/suppa/AS_event.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       54 2023-04-07 08:57:38.000000 astk-0.1.2b0/astk/suppa/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7043 2023-04-07 12:40:54.000000 astk-0.1.2b0/astk/suppa/_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1236 2023-02-20 01:59:46.000000 astk-0.1.2b0/astk/suppa/event_psi.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4413 2023-02-20 01:59:46.000000 astk-0.1.2b0/astk/suppa/gtf_parse.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.219081 astk-0.1.2b0/astk/suppa/lib/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       84 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/suppa/lib/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23418 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/suppa/lib/diff_tools.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24715 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/suppa/lib/event.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8048 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/suppa/lib/gtf_store.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    12030 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/suppa/lib/optics.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22325 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/suppa/lib/tools.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24158 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/suppa/lib/var_event.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.220081 astk-0.1.2b0/astk/utils/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      173 2022-11-03 01:59:44.000000 astk-0.1.2b0/astk/utils/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3711 2023-04-30 14:57:10.000000 astk-0.1.2b0/astk/utils/_cli_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9589 2023-04-10 12:32:19.000000 astk-0.1.2b0/astk/utils/_coord.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      537 2023-02-20 01:59:46.000000 astk-0.1.2b0/astk/utils/_getfasta.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15326 2023-05-03 13:44:10.000000 astk-0.1.2b0/astk/utils/func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4513 2023-02-28 07:54:41.000000 astk-0.1.2b0/astk/utils/meta_template.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3970 2023-02-27 07:37:24.000000 astk-0.1.2b0/astk/utils/select.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 06:49:18.135081 astk-0.1.2b0/astk.egg-info/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1036 2023-05-06 06:49:18.000000 astk-0.1.2b0/astk.egg-info/PKG-INFO
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    17588 2023-05-06 06:49:18.000000 astk-0.1.2b0/astk.egg-info/SOURCES.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        1 2023-05-06 06:49:18.000000 astk-0.1.2b0/astk.egg-info/dependency_links.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       42 2023-05-06 06:49:18.000000 astk-0.1.2b0/astk.egg-info/entry_points.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      189 2023-05-06 06:49:18.000000 astk-0.1.2b0/astk.egg-info/requires.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        5 2023-05-06 06:49:18.000000 astk-0.1.2b0/astk.egg-info/top_level.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       38 2023-05-06 06:49:18.221081 astk-0.1.2b0/setup.cfg
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1190 2023-05-05 03:57:27.000000 astk-0.1.2b0/setup.py
```

### Comparing `astk-0.1.2/LICENSE` & `astk-0.1.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/R/CoSpliceNet.R` & `astk-0.1.2b0/astk/R/CoSpliceNet.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/R/enrich.R` & `astk-0.1.2b0/astk/R/enrich.R`

 * *Files 19% similar despite different names*

```diff
@@ -11,38 +11,50 @@
 parser$add_argument("--database", help="database")
 parser$add_argument("--ontology", help="ontology")
 parser$add_argument("--orgdb", help="orgdb")
 parser$add_argument("--genetype", help="gene type")
 parser$add_argument("--organism", help="kegg organism")
 parser$add_argument("--file", help="dpsi files")
 parser$add_argument("--simple", action='store_true', help="simple")
+parser$add_argument("--app", help="software output")
 
 args <- parser$parse_args()
 
 out.dir <- args$outdir
 pval  <- args$pval
 qval  <- args$qval
 db <- args$database
 ontology <- args$ontology
 gene_type <- args$genetype
 org_db <- args$orgdb
 organism <- args$organism
 dpsi_file <- args$file
+app <- args$app
 
 suppressMessages(library(org_db, character.only = T))
 
+if (app == "SUPPA2"){
+    dpsi <- read_tsv(dpsi_file, 
+                    skip      = 1, 
+                    col_names = F,
+                    col_types = cols("c", "d", "d"))
+
+    colnames(dpsi) = c("event_id", "dpsi", "pval")
+    genes <- gsub("\\..*", "",  dpsi$event_id)  
+} else if (app == "rMATS"){
+    df  <-  read_tsv(dpsi_file)
+    genes <- gsub("\\..*", "",  df$GeneID)   
+} else if (app == "EventPointer"){
+    df  <-  read_csv(dpsi_file)
+    if (! "Gene" %in% colnames(df)){
+        df  <-  read.table(dpsi_file)  
+    }
+    genes <- gsub("\\..*", "",  df$Gene) 
+}
 
-dpsi <- read_tsv(dpsi_file, 
-                skip      = 1, 
-                col_names = F,
-                col_types = cols("c", "d", "d"))
-
-colnames(dpsi) = c("event_id", "dpsi", "pval")
-
-genes <- gsub("\\..*", "",  dpsi$event_id) 
 
 if (db == "GO"){
     p <- enrichGOSep(genes, 
                 out.dir,
                 org_db, 
                 name    = "GO",
                 ont     = ontology,
```

### Comparing `astk-0.1.2/astk/R/enrichCompare.R` & `astk-0.1.2b0/astk/R/enrichCompare.R`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 parser$add_argument("--database", help="database")
 parser$add_argument("--ontology", help="ontology")
 parser$add_argument("--orgdb", help="orgdb")
 parser$add_argument("--genetype", help="gene type")
 parser$add_argument("--organism", help="organism")
 parser$add_argument("--files",  nargs='+', help="dpsi files")
 parser$add_argument("--xlabel",  nargs='+', help="dpsi files")
+parser$add_argument("--app", help="software output")
 
 args <- parser$parse_args()
 
 out.dir <- args$outdir
 pval  <- args$pval
 qval  <- args$qval
 database <- args$database
 orgdb <- args$orgdb
 gene_type <- args$genetype
 organism <- args$organism
 dpsi_files <- args$files
 xlabel <- args$xlabel
 ontology <- args$ontology
+app <- args$app
 
 suppressMessages(library(orgdb, character.only = T))
 
 
 filenames <- unlist(lapply(dpsi_files, function(file){
                             tools::file_path_sans_ext(basename(file))
                         }))   
@@ -40,21 +42,33 @@
     filenames <- xlabel
 } else if (length(filenames) != length(unique(filenames))) {
    filenames <- paste(filenames, seq(1, length(filenames)), sep=".") 
 } else {
    filenames <- filenames
 }
 
-
 gene_ls <- lapply(dpsi_files, function(file){
-    dpsi <- read_tsv(file, 
-                    skip      = 1, 
-                    col_names = F,
-                    col_types = cols("c", "d", "d"))
-    genes <- unique(gsub("\\..*", "",  dpsi$X1))   
+    if (app == "SUPPA2"){
+        dpsi <- read_tsv(file, 
+                        skip      = 1, 
+                        col_names = F,
+                        col_types = cols("c", "d", "d")
+                        )
+        colnames(dpsi) = c("event_id", "dpsi", "pval")
+        genes <- gsub("\\..*", "",  dpsi$event_id)  
+    } else if (app == "rMATS"){
+        df  <-  read_tsv(file)
+        genes <- gsub("\\..*", "",  df$GeneID)   
+    } else if (app == "EventPointer"){
+    df  <-  read_csv(file)
+    if (! "Gene" %in% colnames(df)){
+        df  <-  read.table(file) 
+    }
+        genes <- gsub("\\..*", "",  df$Gene) 
+    }
     return(genes)
 })
 
 names(gene_ls) <- filenames
 
 if (database == "GO"){
     compareClusterSep(gene_ls,
```

### Comparing `astk-0.1.2/astk/R/gsea.R` & `astk-0.1.2b0/astk/R/gsea.R`

 * *Files 7% similar despite different names*

```diff
@@ -9,32 +9,43 @@
 org_db <- args[8]
 ont <- args[9]
 gene_type <- args[10]
 name <- args[11]
 database <- args[12]
 organism <- args[13]
 dpsi_file <- args[14]
+app <- args[15]
 
 script_path  <- str_split(args[4], "=")[[1]][2]
 source(file.path(dirname(script_path), "utils.R"))
 
 OrgDb <- load_OrgDb(org_db)
 
-dpsi_df <- read_tsv(dpsi_file, 
-                    skip      = 1, 
-                    col_names = F,
-                    col_types = cols("c", "d", "d")) %>% 
-                    drop_na()
+if (app == "SUPPA2"){
+    dpsi_df <- read_tsv(dpsi_file, 
+                        skip      = 1, 
+                        col_names = F,
+                        col_types = cols("c", "d", "d")) %>% 
+                        drop_na()      
+} else if (app == "rMATS"){
+    dpsi_df  <-  read_tsv(dpsi_file) %>%
+                select(GeneID, FDR, IncLevelDifference) %>%
+                drop_na()
+} else if (app == "EventPointer"){
+    dpsi_df  <-  read_csv(dpsi_file) %>%
+                select(Gene, Pvalue, `Delta PSI`) %>%
+                drop_na()  
+}
 
-colnames(dpsi_df) = c("event_id", "dpsi", "pval")
+colnames(dpsi_df) = c("gene", "dpsi", "pval")
 
 if (gene_type == "ENSEMBL"){
-    dpsi_df$gene <- gsub("\\..*", "",  dpsi_df$event_id) 
+    dpsi_df$gene <- gsub("\\..*", "",  dpsi_df$gene) 
 } else {
-    dpsi_df$gene <- gsub(";.*", "",  dpsi_df$event_id)
+    dpsi_df$gene <- gsub(";.*", "",  dpsi_df$gene)
 }
 
 
 dpis_gene <- sapply(unique(dpsi_df$gene), function(x){
     scores <- dpsi_df[dpsi_df$gene == x, ]$dpsi
     pos_score <- sum(scores[scores > 0])
     neg_score <- sum(scores[scores < 0])
```

### Comparing `astk-0.1.2/astk/R/gseaPlot.R` & `astk-0.1.2b0/astk/R/gseaPlot.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/R/heatmap.R` & `astk-0.1.2b0/astk/R/upset.R`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,58 @@
-suppressMessages(library(ComplexHeatmap))
-
-
 script_path  <- stringr::str_split(commandArgs()[4], "=")[[1]][2]
 source(file.path(dirname(script_path), "utils.R"))
 
 
 parser <- fig_cmd_parser()
 
-parser$add_argument("--file", nargs="+", help="psi file path")
-parser$add_argument("--clusterinfo", help="cluster info file path")
+parser$add_argument("--file", nargs='+', help="file names")
+parser$add_argument("--name", nargs='+', help="file path")
+parser$add_argument("--dg", action='store_true', help="dg")
 
 
 args <- parser$parse_args()
 
+files <- args$file
+names(files) <- args$name
 
-psi_df_ls <- lapply(args$file, function(file){
-    psi_df <- read.delim(file, row.names = 1) # col_types = cols("c", "d", "d")
-    return(psi_df)
-})
+if (args$dg){
+    evnet_id.ls <- lapply(files, function(x){
+        df <- readr::read_tsv(x, skip = 1, show_col_types = FALSE)
+        colnames(df)[1] <- "event_id"
+        list(pos = df[df[2]>0, ]$event_id,
+             neg = df[df[2]<0, ]$event_id)
+    })
+    evnet_id.ls <- unlist(evnet_id.ls, recursive = F)
+    repN <- 2 
 
-
-my_inner_join <- function(x, y){
-    rows <- intersect(rownames(x), rownames(y))
-    cbind(x[rows, ], y[rows, ])
+} else {
+    evnet_id.ls <- lapply(files, function(x){
+        df <- readr::read_tsv(x, skip = 1, show_col_types = FALSE)
+        colnames(df)[1] <- "event_id"
+        df$event_id
+    })  
+    repN <- 1 
 }
 
-dat <- Reduce(my_inner_join, psi_df_ls)
-dat <- na.omit(dat)
 
-if (file.exists(args$clusterinfo)){
+pre_colors <- c("#a1d9f9", "#d69bc5", "#ff9999", "#ffc799", "#99d1b8")
 
-    cls_ext <- tools::file_ext(args$clusterinfo)
+colors <- pre_colors[1:length(files)]
+colors[is.na(colors)] <- "black"
+colors <- rep(colors, each=repN)
 
-    if (cls_ext == "tsv"){
-        exon_cluster <- read.delim(args$clusterinfo, row.names = 1)
-    } else if (cls_ext == "csv") {
-        exon_cluster <- read.delim(args$clusterinfo, row.names = 1)
-    }
-
-    exon_cluster <- as.data.frame(exon_cluster)
-    rownames(exon_cluster) <- exon_cluster$event_id
-
-    exon_cluster[rownames(dat), ]$cluster
-    split <- paste("Cluster", exon_cluster[rownames(dat), ]$cluster, sep = "")
-} else {
-   split <- NULL
-}
 
+p <- UpSetR::upset(UpSetR::fromList(evnet_id.ls), 
+                   nsets          = length(files), 
+                   keep.order     = TRUE, 
+                   sets           = names(evnet_id.ls), 
+                   matrix.color   = "red", 
+                   main.bar.color = "black",
+                   sets.bar.color = colors)
 
-col_fun <- circlize::colorRamp2(seq(0, 1, length.out = 9), 
-                c('#0077B6', '#00B4D8', '#90E0EF',
-                  '#CAF0F8', '#FAE0E4', '#F9BEC7',
-                  '#FF99AC', '#FF7096', '#FF477E'))
-
-p <- Heatmap(as.matrix(dat), 
-             name            = "Heatmap", 
-             show_row_dend   = T, 
-             border          = TRUE, 
-             col             = col_fun,
-             cluster_columns = F, 
-             show_row_names  = F,
-             row_split       = split, 
-             row_gap         = unit(c(3), "mm"))
 
 save_fig(p, 
         args$output, 
         format = args$fmt,
         width  = args$width, 
         height = args$height, 
         units  = "in",
```

### Comparing `astk-0.1.2/astk/R/install.R` & `astk-0.1.2b0/astk/R/install.R`

 * *Files 8% similar despite different names*

```diff
@@ -34,17 +34,16 @@
         message('Installing package: ', i)
         install.packages(i, dependencies = T)
     } else 
         next
     }
     ## Install packages from Bioconductor
 
-    bioconductor.packages <- c('ComplexHeatmap', 'clusterProfiler', 'org.Mm.eg.db',
-             'org.Hs.eg.db', 'simplifyEnrichment', 'universalmotif', 'memes',"tximport",
-             "DESeq2", "metagene2")
+    bioconductor.packages <- c('clusterProfiler', 'org.Mm.eg.db', 'org.Hs.eg.db',
+             'simplifyEnrichment', 'universalmotif', 'memes')
 
     if (!requireNamespace("BiocManager", quietly = TRUE))
         install.packages("BiocManager")
     for(i in bioconductor.packages){
         if(!(i %in% rownames(installed.packages()))){
             message('Installing package: ', i)
             BiocManager::install(i, dependencies = T)
```

### Comparing `astk-0.1.2/astk/R/motifMap.R` & `astk-0.1.2b0/astk/R/motifMap.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/R/motifPlot.R` & `astk-0.1.2b0/astk/R/motifPlot.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/R/seqLogo.R` & `astk-0.1.2b0/astk/R/seqLogo.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/R/utils.R` & `astk-0.1.2b0/astk/R/utils.R`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                       panel.grid.major.x = element_blank())                                      
     }else {
        p <- dotplot(ego, showCategory=30, title = p_title) + 
                 scale_color_gradientn(colours = c("#b3eebe", "#46bac2", "#371ea3"),
                                       guide   = guide_colorbar(reverse=TRUE, order=1)) +
                 guides(size = guide_legend(override.aes=list(shape=1))) +
                 theme(panel.grid.major.y = element_line(linetype='dotted', color='#808080'),
-                      panel.grid.major.x = element_blank())                          
+                      panel.grid.major.x = element_blank()) + scale_y_discrete(labels=function(x) str_wrap(x, width=40))                 
 
       if (simple){
           simple.ego <- clusterProfiler::simplify(ego, cutoff=0.7, by="p.adjust", select_fun=min)
           simple.ego <- enrichplot::pairwise_termsim(simple.ego)           
           simgo.dir <- file.path(output, "simgo")
           if (!dir.exists(simgo.dir)) {
             dir.create(simgo.dir, recursive = T)
@@ -166,22 +166,20 @@
 
           if (dim(as.data.frame(cpk))[1] == 0){
 
             pdf(out.pdf ,width = 12, height = 10)
             dev.off()
             next()           
           }
-
           p <- dotplot(cpk, title = sprintf("%s_%s",name, ont.i)) + 
                 scale_color_gradientn(colours = c("#b3eebe", "#46bac2", "#371ea3"),
                                       guide   = guide_colorbar(reverse=TRUE, order=1)) +
                 guides(size = guide_legend(override.aes=list(shape=1))) +
                 theme(panel.grid.major.y = element_line(linetype='dotted', color='#808080'),
                       panel.grid.major.x = element_blank())
-
           save_fig(p, 
               out.pdf, 
               format = format,
               width  = width, 
               height = height, 
               units  = "in")
         }
```

### Comparing `astk-0.1.2/astk/cli/as_event.py` & `astk-0.1.2b0/astk/cli/as_event.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,85 @@
 from .config import *
-from astk.event import _cli_func as et
+import astk.event as et
 
 
-@click.command(help="length distribution")
+@cli_fun.command(name="lenDist", help="length distribution; short alias: ld")
 @click.option('-i', '--input', 'infile', type=click.Path(exists=True),
                 required=True,  help='AS ioe file')
 @click.option('-o', '--output', required=True, help="output path")
 @click.option('-cl', '--custom_len', 'custom_len', cls=MultiOption, type=int, help="custom length")
 @click.option('-nc', '--cluster', type=int, default=4, help="number of cluster")
 @click.option('-bw', '--width', type=int, default=3, help="bin width")
 @click.option('-lw', '--len_weight', type=float, default=2, help="length weight")
 @click.option('--max_len', type=int, default=500, help="the max length of exon in clustering")
 @click.option('-fmt', '--format', "fmt", type=click.Choice(['png', 'jpeg', 'pdf', 'tiff']), 
                 default="png", help="output figure format")
 def len_dist(*args, **kwargs):
     et.len_dist(*args, **kwargs)
 
 
-@click.command(help="length cluster")
+@cli_fun.command(name="lenCluster", help="length cluster; short alias: lc")
 @click.option('-i', '--input', "files", cls=MultiOption, type=click.Path(exists=True),
                 help="input dpsi files")
 @click.option('-id', '--inDir', type=click.Path(exists=True), help='input direcory')
 @click.option('-od', '--outdir', required=True, help="output directory")
 @click.option('-lr', '--lenRange', cls=MultiOption, type=int,
                 default=(1, ), help="custom length")
 def len_cluster(*args, **kwargs):
     et.len_cluster(*args, **kwargs)
 
 
-@click.command(help="pick AS event with specific length")
+@cli_fun.command(name="lenPick", help="pick AS event with specific length; short alias: lp")
 @click.option('-i', '--input', 'infile', type=click.Path(exists=True), help='AS ioe file')
 @click.option('-o', '--output', help="output path")
 @click.option('-rg', '--range', "len_range", type=(int, int), required=True, help="length range")
 def len_pick(*args, **kwargs):
     et.len_pick(*args, **kwargs)
 
 
-# it is deprecated
-@click.command(help="filter significant result")
-@click.option('-i', '--input', "files", cls=MultiOption, type=click.Path(exists=True),
-                help="input dpsi files")
-@click.option('-od', '--outDir', required=True, help="output directory")
-@click.option('-dpsi', '--dpsi', type=float, default=0, help="dpsi threshold value")
-@click.option('-p', '--pval', type=float, default=0.05, help="pval threshold value")
-@click.option('-adpsi', '--abs_dpsi', type=float, default=0, help="absulte dpsi threshold value")
-@click.option('-pf1', '--psiFile1', cls=MultiOption, type=click.Path(exists=True),
-                default=(), help="psi files of condtion 1")
-@click.option('-pf2', '--psiFile2', cls=MultiOption, type=click.Path(exists=True),
-                default=(), help="psi files of condtion 2")
-@click.option('-fmt', '--format', "fmt", type=click.Choice(['csv', 'tsv']), 
-                default="tsv", help="out  file format ")
-@click.option('-app','--app', required=True, type=click.Choice(["auto", "SUPPA2", "rMATS"]),
-                default="auto", help="the program that generates event file")
-def _sigfilter(*args, **kwargs):
-    et.sigfilter(*args, **kwargs)
-
-
-@click.command(help="filter psi result")
-@click.option('-i', '--input', "file", type=click.Path(exists=True),
+@cli_fun.command(name="psiFilter", help="filter psi result; short alias: pf")
+@click.option('-i', '--input', "file", required=True, type=click.Path(exists=True),
                 help="input psi file")
-#@click.option('-md', '--metadata', type=click.Path(exists=True), help="metadata file")
 @click.option('-o', '--output', required=True, help="output path")
-@click.option('-psi', '--psi', type=float, default=0, help="psi threshold value, defualt=0")
-@click.option('-qt', '--quantile', type=float, default=0, help="quantile threshold value, defualt=0")
-# @click.option('-fmt', '--format', "fmt", type=click.Choice(['csv', 'tsv']), 
-#                 default="tsv", help="out  file format ")
+@click.option('-minv', '--minValue', "minv", type=click.FloatRange(min=0, max=1), 
+                default=0, show_default=True, help="minimum PSI threshold value")
+@click.option('-maxv', '--maxValue', "maxv", type=click.FloatRange(min=0, max=1), 
+                default=1, show_default=True,  help="maximal PSI threshold value")
+@click.option('-minq', '--minQuantile', "minq", type=click.FloatRange(min=0, max=1), 
+                default=0, show_default=True, help="minimum quantile threshold value")
+@click.option('-maxq', '--maxQuantile', "maxq", type=click.FloatRange(min=0, max=1), 
+                default=1, show_default=True, help="maximal quantile threshold value")
+@click.option('-app','--app', default="auto", type=click.Choice(["auto", "SUPPA2", "rMATS"]),
+                show_default=True, help="the program that generates event file")
 def psi_filter(*args, **kwargs):
     et.psi_filter(*args, **kwargs)
 
- 
-@click.command(help="intersect AS event")
+
+@cli_fun.command(help="intersect AS event")
 @click.option('-a', "file_a", type=click.Path(exists=True), required=True, help="dpsi or psi file A")
 @click.option('-b', "file_b", type=click.Path(exists=True), help="dpsi or psi file B")
 @click.option('-o', "--output", required=True, help="output suffix")
 @click.option('-ioeb', "--ioeB", type=click.Path(exists=True), help="ioe file file B")
 @click.option('-ib', "--ignoreB", type=bool, default=False, help="ignore file B intersection output")
 def intersect(*args, **kwargs):
     if any([kwargs.get("file_b"), kwargs.get("ioeb")]):
         et.intersect(*args, **kwargs)
 
 
-@click.command(help="filter significant result")
-@click.option('-i', '--input', "file", type=click.Path(exists=True),
+@cli_fun.command(name="sigFilter", help="filter significant result; short alias: sf")
+@click.option('-i', '--input', "file", required=True, type=click.Path(exists=True),
                 help="input dpsi file")
-@click.option('-o', '--output', help="output directory")
-@click.option('-dpsi', '--dpsi', type=float, default=0, help="dpsi threshold value, defualt=0")
-@click.option('-p', '--pval', type=float, default=0.05, help="pval threshold value, defualt=0.05")
-@click.option('-q', '--qval', type=float, default=1, help="qval threshold value, defualt=1")
-@click.option('-adpsi', '--abs_dpsi', type=float, default=0, 
-                help="absulte dpsi threshold value, defualt=0")
-@click.option('-sep', '--sep', "sep", is_flag=True, default=False, 
+@click.option('-o', '--output', required=True, type=click.Path(), help="output directory")
+@click.option('-dpsi', '--dpsi', type=click.FloatRange(min=-1, max=1), default=0, 
+                show_default=True, help="dpsi threshold value")
+@click.option('-p', '--pval', type=click.FloatRange(min=0, max=1), default=0.05, 
+                show_default=True, help="pval threshold value")
+@click.option('-q', '--qval', type=click.FloatRange(min=0, max=1), default=1, 
+                show_default=True, help="qval threshold value")
+@click.option('-adpsi', '--abs_dpsi', type=click.FloatRange(min=0, max=1), default=0, 
+                show_default=True, help="absulte dpsi threshold value")
+@click.option('-sep', '--sep', "sep", is_flag=True, default=False, show_default=True, 
                 help="split file into two files according to dpsi > 0 and dpsi < 0")
-@click.option('-app','--app', required=True, type=click.Choice(["auto", "SUPPA2", "rMATS"]),
-                default="auto", help="the program that generates event file, defualt='auto'")
+@click.option('-app','--app', type=click.Choice(["auto", "SUPPA2", "rMATS"]),
+                default="auto", show_default=True, help="the program that generates event file")
 def sigfilter(*args, **kwargs):
-    et.sigfilter(*args, **kwargs)
+    et.sigfilter(*args, **kwargs)
```

### Comparing `astk-0.1.2/astk/cli/gsea.py` & `astk-0.1.2b0/astk/cli/gsea.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,120 @@
+from click_option_group import optgroup
+
 from .config import *
 from astk.constant import NEASE_DATABASE
 from astk import gsea
+from astk.utils import detect_file_info
 
 
-@click.command(help="Gene Set Enrichment Analysis")
+@cli_fun.command(name="gsea", help="Gene Set Enrichment Analysis")
 @click.option('-i', '--input', "file", type=click.Path(exists=True),
-                help="input dpsi files")
+                required=True, help="input dpsi files")
 @click.option('-od', '--outdir', default=".", help="outdir")
 @click.option('-n', '--name', default="GSEA", help="output name prefix")
-@click.option('-pval', '--pvalue', type=float, default=0.2, help="pvalue cutoff, defualt=0.2")
-@click.option('-db', '--database', type=click.Choice(['GO']), 
-                default="GO", help="enrich database, defualt='GO'")
-@click.option('-gt', '--geneId', type=click.Choice(['ENSEMBL', 'ENTREZID', 'SYMBOL']), 
-                default="ENSEMBL", help="gene ID type, defualt='ENSEMBL'")                      
-@click.option('-orgdb', '--orgdb', required=True,
-                help="OrgDb for GO annotation, such as: hs for Human, mm for Mouse. \
-                    run 'astk ls -org' to view more ")
-@click.option('-ont', type=click.Choice(['BP', 'MF', 'CC']), 
-                default="BP", help="one of 'BP', 'MF', and 'CC' subontologies.")  
-@click.option('-org', '--keggOrganism', "organism", default = "",
-                help="KEGG organism short alias.This is required if -db is KEGG.\
-                    Organism list in http://www.genome.jp/kegg/catalog/org_list.html")                            
+@click.option('-pval', '--pvalue', type=float, default=0.2, show_default=True, help="pvalue cutoff")
+@click.option('-db', '--database', type=click.Choice(['GO']), show_default=True, 
+                default="GO", help="enrich database")
+@click.option('-gt', '--gene-id', type=click.Choice(['ENSEMBL', 'ENTREZID', 'SYMBOL']), 
+                default="ENSEMBL", show_default=True, help="gene ID type, defualt='ENSEMBL'") 
+@click.option('-ont', '--ontology', type=click.Choice(['BP', 'MF', 'CC']), show_default=True, 
+                default="BP", help="one of 'BP', 'MF', and 'CC' subontologies, or 'ALL' for all three")  
+@click.option('-org', '--organism', type=click.Choice(['hs', 'mm']), required=True,  help="organism")
+@click.option('-app','--app', required=True, type=click.Choice(["SUPPA2", "rMATS", "EventPointer"]), 
+                help="the software that generates event file")                 
 def gsea_fun(*args, **kwargs):
+    if kwargs["app"] is None: # it will not run
+        kwargs["app"] = detect_file_info(kwargs["file"])["app"] 
     gsea.gsea_fun(*args, **kwargs)
 
 
-@click.command(help="Over representation enrichment analysis")
+@cli_fun.command(help="Over representation enrichment analysis")
 @click.option('-i', '--input', "file", type=click.Path(exists=True),
-                help="input dpsi files")
+                required=True, help="input dpsi files")
 @click.option('-od', '--outdir', default=".", help="outdir")
-@click.option('-pval', '--pvalue', type=float, default=0.1, help="pvalue cutoff, default=0.1")
-@click.option('-qval', '--qvalue', type=float, default=0.1, help="pvalue cutoff, default=0.1")
+@click.option('-pval', '--pvalue', type=float, default=0.1, show_default=True, help="pvalue cutoff")
+@click.option('-qval', '--qvalue', type=float, default=0.1, show_default=True, help="qvalue cutoff")
 @click.option('-db', '--database', type=click.Choice(['GO', 'KEGG', 'Reactome']), 
-                default="GO", help="enrich database GO|KEGG|Reactome, default=GO")
-@click.option('-ont', '--ontology', type=click.Choice(['ALL', 'BP', 'CC','MF']), default="BP",
-                help="One of 'BP', 'MF', and 'CC' subontologies, or 'ALL' for all three. default=BP")                
-@click.option('-gene_id', '-gene_id', type=click.Choice(['ENSEMBL', 'ENTREZID', 'SYMBOL']), 
-                default="ENSEMBL", help="gene ID type")
-@click.option('-org', '--organism', type=click.Choice(['hs', 'mm']), 
-                required=True, help="organism")
-@click.option('--simple', is_flag=True, help="simplify GO enrichment")
-@click.option('-fmt', '--format', "fmt", type=click.Choice(['png', 'pdf', 'pptx']),
-                 default="pdf", help="output figure format") 
-@click.option('-w', '--width', default=10, help="fig width, default=10 inches")
-@click.option('--height', default=12, help="fig height, default=12 inches")    
+                default="GO", show_default=True, help="enrich database")
+@click.option('-ont', '--ontology', type=click.Choice(['ALL', 'BP', 'CC','MF']), default="BP", show_default=True,
+                help="One of 'BP', 'MF', and 'CC' subontologies, or 'ALL' for all three")                
+@click.option('-gi', '--gene-id', type=click.Choice(['ENSEMBL', 'ENTREZID', 'SYMBOL']), 
+                default="ENSEMBL", show_default=True, help="gene ID type")
+@click.option('-org', '--organism', type=click.Choice(['hs', 'mm']), required=True, 
+                show_default=True, help="organism")
+@click.option('--simple', is_flag=True, default=False, show_default=True, help="simplify GO enrichment")
+@click.option('-app','--app', type=click.Choice(["auto", "SUPPA2", "rMATS", "EventPointer"]), 
+                default="auto", show_default=True, help="the software that generates event file")
+@fig_common_options()          
 def enrich(*args, **kwargs):
+    if kwargs["app"] == "auto":
+        kwargs["app"] = detect_file_info(kwargs["file"])["app"]
+    if kwargs["figfmt"] == "auto":
+        kwargs["figfmt"] = "png"
     gsea.enrich(*args, **kwargs)
 
 
-@click.command()
+@cli_fun.command(name="enrichCompare", help="function enrichment comparison; short alias: ecmp")
 @click.option('-i', '--input', "files", cls=MultiOption, type=click.Path(exists=True),
-                help="input dpsi files")
+                required=True, help="input dpsi files")
 @click.option('-od', '--outdir', required=True, help="output directory")          
 @click.option('-db', '--database', type=click.Choice(['GO', 'KEGG', 'Reactome']), 
-                default="GO", help="enrich database, default='GO'")
-@click.option('-ont', '--ontology', type=click.Choice(['ALL', 'BP', 'CC','MF']), default="BP",
-                help="One of 'BP', 'MF', and 'CC' subontologies, or 'ALL' for all three. default=BP")                  
-@click.option('-pval', '--pvalue', type=float, default=0.1, help="pvalue cutoff")
-@click.option('-qval', '--qvalue', type=float, default=0.1, help="pvalue cutoff")
+                default="GO", show_default=True, help="enrich database")
+@click.option('-ont', '--ontology', type=click.Choice(['ALL', 'BP', 'CC','MF']), default="BP", show_default=True,
+                help="One of 'BP', 'MF', and 'CC' subontologies, or 'ALL' for all three.")                  
+@click.option('-pval', '--pvalue', type=float, default=0.1, show_default=True, help="pvalue cutoff")
+@click.option('-qval', '--qvalue', type=float, default=0.1, show_default=True, help="qvalue cutoff")
 @click.option('-xl', '--xlabel', cls=MultiOption, type=str, help="xlabel")
-@click.option('-gene_id', '--gene_id', type=click.Choice(['ENSEMBL', 'ENTREZID', 'SYMBOL']), 
-                default="ENSEMBL", help="gene ID type")                      
-@click.option('-org', '--organism', type=click.Choice(['hs', 'mm']), required=True,
-                help="organism: hs|mm")
-@click.option('-fmt', '--format', "fmt", type=click.Choice(['png', 'pdf', 'pptx']),
-                default="pdf", help="output figure format")
-@click.option('-fw', '--width', type=float, help="figure width")
-@click.option('-fh', '--height', type=float, help="figure height")
+@click.option('-gi', '--gene-id', type=click.Choice(['ENSEMBL', 'ENTREZID', 'SYMBOL']), 
+                default="ENSEMBL", show_default=True, help="gene ID type")
+@click.option('-org', '--organism', type=click.Choice(['hs', 'mm']), required=True, 
+                show_default=True, help="organism")
+@click.option('-app','--app', type=click.Choice(["auto", "SUPPA2", "rMATS", "EventPointer"]), 
+                default="auto", show_default=True, help="the software that generates event file")
+@fig_common_options()
 def enrich_cmp(*args, **kwargs):
+    if kwargs["app"] == "auto": 
+        # Assuming that the input files are all in the same format
+        kwargs["app"] = detect_file_info(kwargs["files"][0])["app"]
+    if kwargs["figfmt"] == "auto":
+        kwargs["figfmt"] = "png"
     gsea.enrich_cmp(*args, **kwargs)
 
 
-@click.command()
-@click.option('-i', '--input', "files", cls=MultiOption, type=click.Path(exists=True),
-                help="input dpsi files")
-@click.option('-od', '--outdir', required=True, help="output directory")
-@click.option('-cls', '--cluster', type=click.Path(exists=True),
-                required=True, help="cluster information file")
-@click.option('-m', '--merge', is_flag=True, help="enrich with multiple merged files")              
-@click.option('-db', '--database', type=click.Choice(['GO']), 
-                default="GO", help="enrich database")
-@click.option('-pval', '--pvalue', type=float, default=0.1, help="pvalue cutoff")
-@click.option('-qval', '--qvalue', type=float, default=0.1, help="pvalue cutoff")
-@click.option('-gene_id', '--geneId', "gene_id", type=click.Choice(['ENSEMBL', 'ENTREZID', 'SYMBOL']), 
-                default="ENSEMBL", help="gene ID type")                      
-@click.option('-orgdb', '--orgdb', required=True,
-                help="OrgDb for GO annotation, such as: hs for Human, mm for Mouse. \
-                    run 'astk ls -orgdb' to view more ")
-@click.option('-org', '--keggOrganism', "kegg_organism",
-                help="KEGG organism short alias.This is required if -db is KEGG.\
-                    Organism list in http://www.genome.jp/kegg/catalog/org_list.html") 
-def enrich_lc(*args, **kwargs):
-    pass
-
-
-@click.command(help="Functional enrichment with NEASE")
+@cli_fun.command(name="nease", help="Functional enrichment with NEASE")
 @click.option('-i', '--input', "file", type=click.Path(exists=True),
-                help="input dpsi files")
+                required=True, help="input dpsi files")
 @click.option('-od', '--outdir', required=True, help="output directory")
 @click.option('-pval', '--pvalue', type=float, default=0.1, help="pvalue cutoff")
 @click.option('-db', '--database', cls=MultiOption, type=click.Choice(NEASE_DATABASE), 
                 default=["Reactome"], help="nease enrich database, \
                 [PharmGKB|HumanCyc|Wikipathways|Reactome|KEGG|SMPDB|Signalink|NetPath|EHMN|INOH|BioCarta|PID]")
 @click.option('-org', '--organism', default='Human', type=click.Choice(['Human']),
                 help="organism")
 def nease_sc(*args, **kwargs):
     gsea.nease_sc(*args, **kwargs)
 
 
-@click.command(help="Functional enrichment comparision with NEASE")
+@cli_fun.command(name="neaseCompare", 
+                help="Functional enrichment comparision with NEASE; short alias: ncmp")
 @click.option('-i', '--input', "files", cls=MultiOption, type=click.Path(exists=True),
                 help="input dpsi files")
 @click.option('-od', '--outdir', required=True, help="output directory")
 @click.option('-n', '--showNumber', 'num', type=int, default=15, help="qvalue cutoff")
 @click.option('-qval', '--qvalue', type=float, default=0.1, help="qvalue cutoff")
 @click.option('-db', '--database', cls=MultiOption, type=click.Choice(NEASE_DATABASE), 
                 default=["Reactome"], help="nease enrich database, \
                 [PharmGKB|HumanCyc|Wikipathways|Reactome|KEGG|SMPDB|Signalink|NetPath|EHMN|INOH|BioCarta|PID]")
 @click.option('-org', '--organism', default='Human', type=click.Choice(['Human']),
                 help="organism")
 @click.option('-xl', '--xlabel', cls=MultiOption, type=str, help="xlabel")
 @click.option('-ff', '--figFormat', type=click.Choice(['png', 'pdf', 'tiff', 'jpeg']), 
                 default="png", help="output figure format")
-@click.option('-fw', '--width', type=float, help="figure width")
-@click.option('-fh', '--height', type=float, help="figure height")           
+@click.option('-fw', '--width', type=float, default=6, help="figure width, default=6 inches")
+@click.option('-fh', '--height', type=float, default=6, help="figure height, default=6 inches")        
 def sc_neasecmp(*args, **kwargs):
     fn = len(kwargs["files"])
     if kwargs["xlabel"] is None:
         kwargs["xlabel"] = [f"c{i+1}" for i in range(fn)]
     if fn < 2:
         raise UsageError("for -i/--input should be more than two files")
     gsea.neasecmp(*args, **kwargs)
```

### Comparing `astk-0.1.2/astk/cli/motif.py` & `astk-0.1.2b0/astk/cli/motif.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .config import *
 import astk.motif as mo
 
 
-@click.command(["motifEnrich", "me"], help = "Motif Enrichment")
+@cli_fun.command(name="motifEnrich", help="Motif Enrichment; short alias: me")
 @click.option('-te', "--tevent", type=click.Path(exists=True), 
                 required=True, help="treatment event file")
 @click.option('-ce', "--cevent", type=click.Path(exists=True), 
                 help="control  event file")  
 @click.option('-od', '--outdir', type=click.Path(), default=".", help="output directory")
 @click.option('-db', '--database', type=click.Choice(['ATtRACT', 'CISBP-RNA']),
                  default="CISBP-RNA", help="RBP motif database default=CISBP-RNA")
@@ -17,15 +17,15 @@
                  default="centrimo", help="Motif enrichment method, default=centrimo")
 # @click.option('-mm', '--meme', type=click.Path(exists=True), 
 #                 required=True, help="path to .meme format file")
 def motif_enrich(*args, **kwargs):
     mo.motif_enrich(*args, **kwargs)
 
 
-@click.command(help = "Motif Discovery and similarity comparision")
+@cli_fun.command(name="motifFind", help="Motif Discovery and similarity comparision; short alias: mf")
 @click.option('-te', "--tevent", type=click.Path(exists=True), 
                 required=True, help="AS treatment event file")
 @click.option('-ce', "--cevent", type=click.Path(exists=True), 
                 help="AS treatment control event files")
 @click.option('-od', '--outdir', type=click.Path(), default=".",
                  help="output directory")
 @click.option('-db', '--database', type=click.Choice(['ATtRACT', 'CISBP-RNA']),
@@ -43,60 +43,60 @@
                 help="Input FASTA file. if set, the fasta sequence will be extracted")
 @click.option('-mcmp', '--motifcmp', is_flag=True, 
                 default = False, help="motif similarity comparision")
 def motif_find(*args, **kwargs):
     mo.motif_find(*args, **kwargs)
 
 
-@click.command(help = "Motif plot")
+@cli_fun.command(name="motifPlot", help="Motif plot; short alias: mp")
 @click.option('-mi', "--motifId", "motifid", type=str, # cls=MultiOption, multiple motif plot will ccause bug
                 required=True, help="motif id")
 @click.option('-db', '--database', type=click.Choice(['ATtRACT', 'CISBP-RNA']),
                 help="RBP motif database")
 @click.option('-org', '--organism', help="RBP organism")
 @click.option('-mm', "--meme", type=click.Path(exists=True), 
                 help="meme motif file")
 @click.option('-o', '--output', type=click.Path(), required=True,
                  help="output path")
 @click.option('-fmt', '--format', "fmt", type=click.Choice(['png', 'pdf', 'pptx']),
                  default="png", help="output figure format")
-@click.option('-w', '--width', default=6, help="fig width, default=6 inches")
-@click.option('--height', default=6, help="fig height, default=6 inches")
+@click.option('-fw', '--width', default=6, help="fig width, default=6 inches")
+@click.option('-fh', '--height', default=6, help="fig height, default=6 inches")
 @click.option('-res', '--resolution', default=72, help="resolution, default=72 ppi")
 def motif_plot(*args, **kwargs):
     mo.motif_plot(*args, **kwargs)
 
 
-@click.command(help = "generate motif map")
-@click.option('-e', "--event", type=click.Path(exists=True), 
-                required=True, help="AS event file")
-@click.option('-fi', '--fasta', type=click.Path(exists=True), 
-                required=True, help="genome fasta file")
-@click.option('-n', '--name', cls=MultiOption, type=str,
-                help="fasta file names")
-@click.option('-c', '--center', cls=MultiOption, type=str,
-                help="fasta files names")
-@click.option('-mm', '--meme', required=True, type=click.Path(exists=True), 
-                help="meme motif file")
-@click.option('-od', '--outdir', default=".", type=click.Path(), 
-                help="output directory")
-@click.option('-b', '--binsize', default=20, 
-                help="the window width for scanning motif, default=20")
-@click.option('-s', '--step', default=10, 
-                help="the slide window size, default=10")                
-@click.option('-fmt', '--format', "fmt", type=click.Choice(['png', 'pdf', 'pptx']),
-                 default="png", help="out figure format")
-@click.option('-w', '--width', default=8, help="fig width, default=8 inches")
-@click.option('--height', default=4, help="fig height, default=4 inches")
-@click.option('-res', '--resolution', default=72, help="resolution, default=72 ppi")
-def mmap(*args, **kwargs):
-    mo.mmap(*args, **kwargs)
+# @cli_fun.command(help = "generate motif map")
+# @click.option('-e', "--event", type=click.Path(exists=True), 
+#                 required=True, help="AS event file")
+# @click.option('-fi', '--fasta', type=click.Path(exists=True), 
+#                 required=True, help="genome fasta file")
+# @click.option('-n', '--name', cls=MultiOption, type=str,
+#                 help="fasta file names")
+# @click.option('-c', '--center', cls=MultiOption, type=str,
+#                 help="fasta files names")
+# @click.option('-mm', '--meme', required=True, type=click.Path(exists=True), 
+#                 help="meme motif file")
+# @click.option('-od', '--outdir', default=".", type=click.Path(), 
+#                 help="output directory")
+# @click.option('-b', '--binsize', default=20, 
+#                 help="the window width for scanning motif, default=20")
+# @click.option('-s', '--step', default=10, 
+#                 help="the slide window size, default=10")                
+# @click.option('-fmt', '--format', "fmt", type=click.Choice(['png', 'pdf', 'pptx']),
+#                  default="png", help="out figure format")
+# @click.option('-w', '--width', default=8, help="fig width, default=8 inches")
+# @click.option('--height', default=4, help="fig height, default=4 inches")
+# @click.option('-res', '--resolution', default=72, help="resolution, default=72 ppi")
+# def mmap(*args, **kwargs):
+#     mo.mmap(*args, **kwargs)
 
 
-@click.command(help="Eukaryotic Linear Motif Searching")
+@cli_fun.command(name="elmSearch", help="Eukaryotic Linear Motif Searching; short alias: elms")
 @click.option('-i', '--input', "file", type=click.Path(exists=True),
                 help="input file")
 @click.option('-o', '--output', type=click.Path(), help="output path")
 @click.option('-g', '--genome', type=click.Choice(['mm10', 'hg38']),
                   required=True, help="genome assembly")
 def elms(*args, **kwargs):
     mo.search_elm(*args, **kwargs)
```

### Comparing `astk-0.1.2/astk/cli/net.py` & `astk-0.1.2b0/astk/cli/net.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/cli/seqfeature.py` & `astk-0.1.2b0/astk/cli/seqfeature.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,139 +2,150 @@
 astk.cli.seqfeature
 ~~~~~~~~~~~~~~~~~
 This module provide sequence feature extraction cli api
 """
 
 from .config import *
 import astk.seqfeature.feature as sf
+import astk.utils as ul
 from astk.seqfeature import splice_score, get_elen, get_gcc
-from astk.seqfeature import cmp_sss, cmp_value
+from astk.seqfeature import cmp_value
 
 
-@click.command(help = "extract DNA sequence feature ")
+@cli_fun.command(name="seqfeature", help = "extract DNA sequence feature; short alias: seqf")
 @click.option('-fa', '--fasta', cls=MultiOption, type=click.Path(exists=True), 
                 required=True, help="DNA sequence fasta file")
 @click.option('-o', '--output', type=click.Path(), 
                 help="output path")                
 @click.option('-k', '--kmer', type=int, default=1, help="K-tuple or k-mer value, default=1")
 @click.option('-g', '--gap', type=int, default=0, help="gap value, default=0")
 @click.option('-l', '--lambda', "lambda_", type=int, default=0, help="lambda-correlation value, default=0")
 @click.option('--count', is_flag=True, default=False, help="feature count")
 @click.option('-FM', "--featureMerge", is_flag=True, default=False, help="feature count")
 def sc_extract(*args, **kwargs):
     sf.seq_extract(*args, **kwargs)
 
 
-@click.command(help = "draw seqLogo")
+@cli_fun.command(name="seqlogo", help = "draw seqLogo")
 @click.option('-fa', '--fasta', type=click.Path(exists=True), 
                 required=True, help="DNA sequence fasta file")
 @click.option('-o', '--output', type=click.Path(), 
                 help="output path")
 @click.option('-fmt', '--format', "fmt", type=click.Choice(['png', 'pdf', 'pptx']),
                  default="png", help="out figure format")
 @click.option('-w', '--width', default=8, help="fig width, default=8 inches")
 @click.option('-h', '--height', default=4, help="fig height, default=4 inches")
 @click.option('-res', '--resolution', default=72, help="resolution, default=72 ppi")                
 def sc_seqlogo(*args, **kwargs):
     sf.seq_pcm(*args, **kwargs)
 
 
-@click.command(["spliceScore", "ss"], help="Compute 5/3 Splice site strength")
-@click.option('-e', "--event", 'file', type=click.Path(exists=True), required=True,
+@cli_fun.command(name="spliceScore", help="Compute 5/3 Splice site strength; short alias: sss")
+@click.option('-e', "--event", type=click.Path(exists=True), required=True,
                 help="event file")
 @click.option('-od', '--outdir', type=click.Path(), default=".", help="output directory")
-@click.option('-fi', 'gfasta', type=click.Path(exists=True), help="genome fasta")
-@click.option('-app','--app', required=True, type=click.Choice(["auto", "SUPPA2", "rMATS"]), 
-                default="auto", help="the program that generates event file")
-@click.option('-p', '--process', default=4, help="process number, default=4")
+@click.option('-fi', "--fasta",'gfasta', type=click.Path(exists=True), help="genome fasta")
+@click.option('-si', '--siteIndex', "sites", cls=MultiOption, type=int,
+                default=[], help="splice site index, 0-index")
+@click.option('-alt', '--altIdx', is_flag=True, default=False, show_default=True,
+                help="get alternative splicing sites index")
+@click.option('-app','--app', type=click.Choice(["auto", "SUPPA2", "rMATS"]), 
+                default="auto", show_default=True, help="the program that generates event file")
+@click.option('-p', '--process', type=int, default=4, show_default=True, help="process number")
 def sc_splice_score(*args, **kwargs):
-    splice_score(*args, **kwargs)
+    coor_dic = ul.get_ss_bed(
+        kwargs["event"], 
+        sss=True,
+        app=kwargs["app"],
+        ss_idx=[i+1 for i in kwargs["sites"]],
+        altidx=kwargs["altidx"]        
+    )
+    splice_score(
+        coor_dic,
+        kwargs["outdir"],
+        kwargs["gfasta"],
+        kwargs["process"]
+    )
 
 
-@click.command(["getlen"], help="Compute element length")
+@cli_fun.command(name="getlen", help="Compute element length")
 @click.option('-e', "--event", 'file', type=click.Path(exists=True), required=True,
                 help="event file")
 @click.option('-od', '--outdir', type=click.Path(), default=".", help="output directory")
-@click.option('-log', "--log", is_flag=True, default=False, help="log2 transformation")
+@click.option('--scale', type=click.Choice(["log", "MinMaxScaler"]), help="length value scale method")
+@click.option('--mode', type=click.Choice(["near", "junction"]), default="near", show_default=True,
+                help="the mode to compute the length, the junction mode is specific to the MX type")
 @click.option('-app','--app', required=True, type=click.Choice(["auto", "SUPPA2", "rMATS"]), 
                 default="auto", help="the program that generates event file")
 def sc_get_elen(*args, **kwargs):
     get_elen(*args, **kwargs)
 
 
-@click.command(["gcc"], help="Compute GC content")
-@click.option('-e', "--event", 'file', type=click.Path(exists=True), required=True,
+@cli_fun.command(name="gcc", help="Compute GC content")
+@click.option('-e', "--event", type=click.Path(exists=True), required=True,
                 help="event file")
 @click.option('-od', '--outdir', type=click.Path(), default=".", help="output directory")
-@click.option('-fi', 'gfasta', type=click.Path(exists=True), help="genome fasta")
-@click.option('-bs', '--binsize', default=0, help="use bin size or slide window to compute exon/intron GC content")
-@click.option('-ef', '--exonFlank', default=150, help="the exon flank width")
-@click.option('-if', '--intronFlank', default=150, help="the intron flank width")
+@click.option('-fi', '--fasta', 'gfasta', type=click.Path(exists=True), help="genome fasta")
+@click.option('-si', '--siteIndex', "sites", cls=MultiOption, type=int,
+                default=[], help="splice site index, 1-index")
+@click.option('-alt', '--altIdx', is_flag=True, default=False, show_default=True,
+                help="get alternative splicing sites index")
+@click.option('-bs', '--binsize', default=15, 
+                help="use bin size or slide window to compute exon/intron GC content, default=15")
+@click.option('-ef', '--exonFlank', default=150, help="the exon flank width, default=150")
+@click.option('-if', '--intronFlank', default=150, help="the intron flank width, default=150")
 @click.option('--includeSS', is_flag=True, default=False, help="include splice site flank region")
 # @click.option('-ele', '--element', is_flag=True, default=False, help="compute the whole exon/intron GC content")
 @click.option('-app','--app', required=True, type=click.Choice(["auto", "SUPPA2", "rMATS"]), 
-                default="auto", help="the program that generates event file")
+                default="auto", help="the program that generates event file, default='auto'")
 @click.option('-p', '--process', default=4, help="process number, default=4")
-def sc_get_gcc(*args, **kwargs):
-    get_gcc(*args, **kwargs)
-
-
-@click.command(["ssscmp"], help="Compare Splice site strength between two conditions")
-@click.option('-e', "--events", 'files', type=click.Path(exists=True), cls=MultiOption, 
-                required=True, help="event files")
-@click.option('-o', '--output', type=click.Path(), help="output path")
-@click.option('-test', '--test', default="Mann-Whitney", 
-                type=click.Choice(['Mann-Whitney', 't-test_ind', 't-test_welch', "Wilcoxon"]), 
-                help=" statistical test method, default='Mann-Whitney'")
-@click.option('-gn', '--groupNames', cls=MultiOption, type=str, 
-                help="group names, default= g1 g2 ")
-@click.option('-ft', '--figType',  default="box", help="figure display type",
-                type=click.Choice(["point", 'strip', 'box', 'boxen', 'violin', 'bar']))
-@click.option('-ff', '--figFormat', type=click.Choice(['auto', 'png', 'pdf', 'tiff', 'jpeg']), 
-                default="auto", help="output figure format")       
-def sc_ssscmp(*args, **kwargs):
-    fn = len(kwargs["files"])
-    if fn != 2:
-        raise UsageError("only support two files for -e/--events")
-    if gn := kwargs.get("groupnames"):
-        if len(gn) != fn:
-            raise UsageError("-gn/--groupNames parameter number must be same as -e/--events")
-    else:
-        kwargs["groupnames"] = [f"g{i}" for i in range(1, fn+1)]
-    cmp_sss(*args, **kwargs)
+def sc_get_gcc(*args, **kwargs):  
+    coor_dic = ul.get_ss_bed(
+        kwargs["event"], 
+        split=True,
+        app=kwargs["app"],
+        excludeSS=(not kwargs["includess"]),
+        exon_width=kwargs["exonflank"],
+        intron_width=kwargs["intronflank"],
+        ss_idx=[i+1 for i in kwargs["sites"]],
+        altidx=kwargs["altidx"]          
+    )    
+    get_gcc(
+        coor_dic,
+        kwargs["outdir"],
+        kwargs["gfasta"],
+        kwargs["binsize"]
+    )
 
 
-@click.command(["vcmp"], help="Compare sequence feature value between two conditions")
+@cli_fun.command(name="vcmp", help="Compare sequence feature value among multiple conditions")
 @click.option('-e', "--events", 'files', type=click.Path(exists=True), cls=MultiOption, 
                 required=True, help="event files")
 @click.option('-o', '--output', type=click.Path(), help="output path")
-@click.option('-test', '--test', default="Mann-Whitney", 
+@click.option('-test', '--test', default="Mann-Whitney", show_default=True, 
                 type=click.Choice(['Mann-Whitney', 't-test_ind', 't-test_welch', "Wilcoxon"]), 
-                help=" statistical test method, default='Mann-Whitney'") 
-@click.option('-facet', "--facet", is_flag=True, default=False, 
+                help=" statistical test method") 
+@click.option('-facet', "--facet", is_flag=True, default=False, show_default=True, 
                 help="If true, the facets will not x axes across rows.")
-@click.option('-log', "--log", is_flag=True, default=False, help="log2 transformation")
+@click.option('-log', "--log", is_flag=True, default=False, show_default=True, help="log2 transformation")
 @click.option('-gn', '--groupNames', cls=MultiOption, type=str, 
-                help="group names, default= g1 g2 ")
-@click.option("--merge-ss", is_flag=True, default=False, help="merge 5'/3' splice sites")      
+                help="group names, default= g1 g2... ")
+@click.option("--merge-ss", is_flag=True, default=False, show_default=True, help="merge 5'/3' splice sites")      
 @click.option('-mc', '--multiCorrect', type=click.Choice(['bonf', 'HB', 'holm', 'BH' ,'BY']), 
                 help="multiple test correction method")
 @click.option('--pvalText', type=click.Choice(['star', 'simple']), default="star",
-                help="p-value display format, default='star'")
-@click.option('--xtitle', default="item", help="x title, default='item'")
-@click.option('--ytitle', default="value", help="y title, default='value'")
+                show_default=True, help="p-value display format")
+@click.option('--xtitle', default="xtitle", show_default=True, help="x title")
+@click.option('--ytitle', default="ytitle", show_default=True, help="y title")
 @click.option('--xlabel', cls=MultiOption, type= str, help="x labels, default is input file colnames")
-@click.option('--xrotation', type=int, default=0, help="x tick labels rotation")
+@click.option('--xrotation', type=float, default=0, show_default=True, help="x tick labels rotation")
 @click.option('-fs', '--figSize', type=(float, float), help="figure size")
-@click.option('-ft', '--figType',  default="box", help="figure display type",
+@click.option('-ft', '--figType',  default="box", show_default=True, help="figure display type",
                 type=click.Choice(["point", 'strip', 'box', 'boxen', 'violin', 'bar']))
-@click.option('-ff', '--figFormat', type=click.Choice(['auto', 'png', 'pdf', 'tiff', 'jpeg']),
-                default="auto", help="output figure format")
-@click.option('-fw', '--width', type=float, help="figure width")
-@click.option('-fh', '--height', type=float, help="figure height")  
+@fig_common_options()
 def sc_cmp_value(*args, **kwargs):
     fn = len(kwargs["files"])
     if fn < 2:
         raise UsageError("-e/--events input must be greater than one file")
     if gn := kwargs.get("groupnames"):
         if len(gn) != fn:
             raise UsageError("-gn/--groupNames parameter number must be same as -e/--events")
```

### Comparing `astk-0.1.2/astk/cli/suppa.py` & `astk-0.1.2b0/astk/cli/suppa.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,80 +5,84 @@
 """
 
 from .config import *
 from astk.suppa import *
 from astk.constant import AS_TYPE
 
 
-@click.command(help="generate the events from the GTF file")
+@cli_fun.command(name="generateEvents", help="generate the events from the GTF file; short alias:ge")
 @click.option('-gtf', '--gtf', type=click.Path(exists=True), help="a GTF format file")
 @click.option('-et', '--eventType', "event_types", type=click.Choice(['ALL'] + AS_TYPE), 
                 default="ALL", help="AS event Type")
 @click.option('-o', '--output', required=True, 
                 help="name of the output file without any extension")
-@click.option('--idType', default="SUPPA2", type=click.Choice(["SUPPA2"]), 
+@click.option('--id-type', default="SUPPA2", type=click.Choice(["SUPPA2"]), 
                 help="output event ID type, default='SUPPA2'") 
 @click.option('-ep','--event-pos', type=click.Choice(['body', 'FT', 'LT']), 
                 help="AS event exon that overlapping the transcript first or last \
                         terminal exon startCodon and stopCodon will save separately")
 def generateEvents(*args, **kwargs):
     generate_events(*args, **kwargs)
 
 
-@click.command(help="calculates AS events PSI values")
-@click.option('-o', '--output', type=click.Path(), help="output file path")
+@cli_fun.command(name="generatePsi", help="calculates AS events PSI values; alias: ge, psiPerEvent")
+@click.option('-o', '--output', type=click.Path(), required=True, help="output file path")
 @click.option('-ioe', '--ioe', type=click.Path(exists=True), help="ioe file path")
 @click.option('-qf', '--quantifyFile', "tpm_files", cls=MultiOption, type=click.Path(exists=True),
-                help="transcript quantification files from salmon")
-@click.option('--tpmThreshold', "tpm_th", type=float, default=0, 
-                help="minimum transcript TPM value that using for calculates PSI, default=0")                
-@click.option('--tpmCol', "tpm_col", type=int, default=4, help="TPM columns index,0-based, default=4")
-@click.option('--txCol', "tx_col", type=int, default=0, 
-                help="transcript ID columns index, 0-based")
-def compute_psi(*args, **kwargs):
+                help="transcript quantification files")
+@click.option('--tpmThreshold', "tpm_th", type=float, default=0, show_default=True,
+                help="minimum transcript TPM value that using for calculates PSI")                
+@click.option('--tpm-col', "tpm_col", type=int, default=4, show_default=True, 
+                help="TPM columns index, 1-based")
+@click.option('--txCol', "tx_col", type=int, default=0, show_default=True,
+                help="transcript ID columns index, 1-based")
+def generatePsi(*args, **kwargs):
     from pathlib import Path
     
     output = kwargs.pop("output")
     psi_df, tpm_df = calculate_psi(*args, **kwargs)
     psi_df.to_csv(output, sep="\t")
     tpm_df.to_csv(Path(output).with_suffix(".tpm"), sep="\t", index_label=False)
 
 
-@click.command(help="differential splicing analysis")
-@click.option('-psi', '--psiFile', "psi_files", cls=MultiOption, 
+@cli_fun.command(name="diffSplice", help="differential splicing analysis; short alias: ds")
+@click.option('-psi', '--psiFile', "psi_files", cls=MultiOption, required=True, 
                 type=click.Path(exists=True),  help="AS event PSI files")
-@click.option('-exp', '--expressFile', "exp_files", cls=MultiOption, 
-                type=click.Path(exists=True), help="transcript quantification files from salmon")
+@click.option('-exp', '--expressFile', "exp_files", cls=MultiOption, required=True, 
+                type=click.Path(exists=True), help="transcript TPM quantification files")
 @click.option('-ref', '--reference', type=click.Path(exists=True),
                 help="ioe reference file")
 @click.option('-o', '--output', help="output directory")
 @click.option('-m', '--method', type=click.Choice(['empirical', 'classical']), default="empirical",
                 help="The method to calculate the significance, default=empirical")
 def diffSplice(*args, **kwargs):
     diff_splice(*args, **kwargs)
 
 
-@click.command(help="differential splicing analysis workflow")
-@click.option('-od', '--outdir', help="output directory")
+@cli_fun.command(help="differential splicing analysis workflow")
+@click.option('-od', '--outdir', required=True, help="output directory")
 @click.option('-md', '--metadata', type=click.Path(exists=True),
              help="contrast group metadata, generated by meta")
 @click.option('-gtf', '--gtf', type=click.Path(exists=True), help="gene annotation gtf file")
 @click.option('-et', '--event-type', type=click.Choice(['ALL']+AS_TYPE), cls=MultiOption,
-                default="ALL", help="gene annotation gtf file")
+                default="ALL", show_default=True, help="AS event type")
 @click.option('-m', '--method', type=click.Choice(['empirical', 'classical']), default="empirical",
-                help="The method to calculate the significance, default=empirical")
-@click.option('-p', '--pval', type=float, default=0.05, help="pval threshold value, default=0.05")
-@click.option('-adpsi', '--abs-dpsi', type=float, default=0.1, help="absulte dpsi threshold value, default=0.1")
+                show_default=True, help="The method to calculate the significance")
+@click.option('-p', '--pval', type=click.FloatRange(min=0, max=1), 
+                default=0.05, show_default=True, help="pval threshold  value")
+@click.option('-adpsi', '--abs-dpsi', type=click.FloatRange(min=0, max=1), 
+                default=0.1, show_default=True, help="absulte dpsi threshold value")
 @click.option('--id-type', default="SUPPA2", type=click.Choice(["SUPPA2"]), 
-                help="output event ID type, default='SUPPA2'")          
+                show_default=True, help="output event ID type")          
 @click.option('--exon-len', type=int, default=100,
              help="Defines the number of nucleotides to display in the output GTF. (Default: 100 nt)")             
 @click.option('-pg', '--pool-genes', default=False, is_flag=True, 
              help="pool together overlapping genes")
-@click.option('--tpm-col', type=int, help="TPM columns index, default=4")
+@click.option('--tpm-col', "tpm_col", type=int, default=4, show_default=True, 
+                help="TPM columns index, 1-based")
 @click.option('--tpm-threshold', type=float, default=0, 
                 help="Minimum TPM value to be included in the analysis. default=0")
 @click.option('-ep','--event-pos', type=click.Choice(['body', 'FT', 'LT']), 
                 help="AS event exon that overlapping the transcript first or last \
                         terminal exon startCodon and stopCodon will save separately")                
 def dsflow(*args, **kwargs):
     if "ALL" in kwargs.get("event_type"):
@@ -90,9 +94,10 @@
         etypes,
         kwargs.get("outdir"),
         kwargs.get("method"),
         kwargs.get("id_type"),
         kwargs.get("pval"),
         kwargs.get("abs_dpsi"),
         kwargs.get("tpm_threshold"),
-        kwargs.get("event_pos")
+        kwargs.get("event_pos"),
+        kwargs.get("tpm_col")
     )
```

### Comparing `astk-0.1.2/astk/cli/utils.py` & `astk-0.1.2b0/astk/cli/draw.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,128 +1,124 @@
-"""
-astk.cli.utils
-~~~~~~~~~~~~~~~~~
-This module provide some utility function
-"""
-
-from email.policy import default
 from .config import *
-import astk.utils._cli_func as ul
-
+from astk import draw
+from astk.utils import sniff_fig_fmt
 
-@click.command(help="generate metadata template file")
-@click.option('-c1', '--ctrl', cls=MultiOption, type=click.Path(exists=True),
-                required=True, help="file path for condtion 1")
-@click.option('-c2', '--case', cls=MultiOption, type=click.Path(exists=True),
-                required=True, help="file path for condtion 2")
-@click.option('-gn', '--groupName', cls=MultiOption, type=str,
-                default=(), help="group name")                
-@click.option('-repN', '--replicate', cls=MultiOption, type=int,
-                help="replicate, number")
-@click.option('-o', '--output', required=True, type=click.Path(),
-                help='metadata output path')                
-@click.option('-repN1', '--replicate1', cls=MultiOption, type=int,
-                help="replicate1, number")
-@click.option('-repN2', '--replicate2', cls=MultiOption, type=int, 
-                help="replicate2, number")
-@click.option('--condition', cls=MultiOption, type=str, help="condition name")
-@click.option('-fn', '--filename', 'is_fn', is_flag=True, help="file name")
-@click.option('--split', cls=MultiOption, type=str, help="name split symbol and index")    
-def meta(*args, **kwargs):
-    ul.meta(*args, **kwargs)
-
-
-@click.command(help = "install R packages")
-@click.option('-r', '--requirement', is_flag=True, default=False,
-                help="install astk requirement R packages")
-@click.option('-OrgDb', '--OrgDb', "OrgDb", cls=MultiOption, type=str, 
-                default=(), help="install Genome wide annotation package")
-@click.option('-cran', '--cran', cls=MultiOption, type=str, 
-                default=(), help="install CRAN package")
-@click.option('-bioc', '--bioconductor', cls=MultiOption, type=str, 
-                default=(),help="install Bioconductor package")
-@click.option('-j', '--java',  is_flag=True, help="install java software")
-@click.option('-m', '--mirror',  is_flag=True, default=False,
-                help="use tsinghua mirrors.")
-@click.option('--conda',  is_flag=True, default=False,
-                help="install packages via conda")
-def install(*args, **kwargs):
-    ul.install(*args, **kwargs)
-
-
-@click.command(help = "get motif from meme file")
-@click.argument('motifId', nargs=-1, required=True)   
-@click.option('-mm', '--meme', type=click.Path(exists=True), help="meme motif file")
-@click.option('-db', '--database', type=click.Choice(['ATtRACT', 'CISBP-RNA']),
-                help="RBP motif database")
-@click.option('-org', '--organism', help="RBP organism")
-@click.option('-o', '--output', required=True, help="output path")
-def getmeme(*args, **kwargs):
 
-    ul.getmeme(*args, **kwargs)
-
-@click.command(help = "list OrgDb")
-@click.option('-orgdb', '--OrgDb', "OrgDb", is_flag=True, help="list OrgDb")
-@click.option('-rbpsp', '--RBPSp', "RBPSp", is_flag=True, help="RNA binding protein  ")
-def list_(*args, **kwargs):
-    ul.list_(*args, **kwargs)
-
-
-@click.command(help = "generate ChromHMM anchor file")
-@click.argument('file', type=click.Path(exists=True), required=True)
-@click.option('-o', '--output', required=True, help="file output path")
-@click.option('-idx', '--index', type=int, help="element index")
-@click.option('-si', '--sideIndex', type=(int, int), help="the center of two side index")
-@click.option('-u', '--upstreamOffset', "offset5", type=int, default=0, help="upstream offset")
-@click.option('-d', '--downstreamOffset', "offset3", type=int, default=0, help="downstream offset")
-@click.option('-ss', '--strandSpecifc', "strand_sp", is_flag=True, help="strand specifc")
-def anchor(*args, **kwargs):
-    ul.anchor(*args, **kwargs)
- 
-
-@click.command(help = "generate bed file according to selected coordinates")
-@click.option('-i', '--input', 'file', type=click.Path(exists=True),
-                required=True,  help='AS event file')
-@click.option('-o', '--output', required=True, help="file output path")
-@click.option('-a', '--anchor', cls=MultiOption, type=int, 
-                help="splice site index. if not set, it will use all splice sites. 1-based")
-@click.option('-uw', '--upstreamWidth', "upstream_w", type=int, default=50,
-                help="flank width of splice site upstream")
-@click.option('-dw', '--downstreamWidth', "downstream_w", type=int, default=50,
-                help="flank width of splice site downstream")
-@click.option('--interval', type=(int, int), default=(None, None),
-                help="splice site start and end index, 1-based")
-@click.option('--strandSpecifc', "strand_sp", is_flag=True, help="strand specifc")
-@click.option('-fi', 'fasta', type=click.Path(exists=True), 
-                help="Input FASTA file. if set, the fasta sequence will be extracted")
-def getcoor(*args, **kwargs):
-    ul.getcoor(*args, **kwargs)
-
-
-@click.command(help = "Make the TxDb object")
-@click.argument('gtf', type=click.Path(exists=True), required=True)
-@click.option('-org', '--organism', required=True, help="organism")
-@click.option('-o', '--output', help="file output path")
-def mktxdb(*args, **kwargs):
-    ul.mkTxDb(*args, **kwargs)
-
-
-@click.command(help = "get gene ID from AS event file")
-@click.argument('file', type=click.Path(exists=True), required=True)
-@click.option('-o', '--output', type=click.Path(), help="file output path")
-@click.option('-u', '--unique', is_flag=True, help="only save unique gene ID")
-def getgene(*args, **kwargs):
-    ul.getgene(*args, **kwargs)
-
-
-@click.command(["merge"], help="merge file")
-@click.option('-i','--input', 'files' ,cls=MultiOption, type=click.Path(exists=True),
-                required=True , help="input files")
+@cli_fun.command(help="Gene Set Enrichment Analysis ploting")
+@click.option('-id', '--id', "termid", cls=MultiOption, type=str, 
+                required=True, help="term id")
+@click.option('-o', '--output', help="output figure path")
+@click.option('-rd', '--RData', help="output figure path")
+@click.option('-fmt', '--format', "fmt", type=click.Choice(['auto', 'png', 'pdf', 'pptx']),
+                default="auto", help="output figure format") 
+@click.option('-fw', '--width', default=6, help="fig width, default=6 inches")
+@click.option('-fh', '--height', default=6, help="fig height, default=6 inches")
+@click.option('-res', '--resolution', default=72, help="resolution, default=72 ppi")
+def gseplot(*args, **kwargs):
+    if kwargs["fmt"] == "auto":
+        kwargs["fmt"] = sniff_fig_fmt(kwargs["output"])
+    draw.gseplot(*args, **kwargs)
+
+
+@cli_fun.command(help="draw UpSet plots for AS events")
+@click.option('-i', '--input', "files", cls=MultiOption, type=click.Path(exists=True),
+                help="input psi files")           
+@click.option('-o', '--output', required=True, help="output figure path")
+@click.option('-xl', '--xlabel', cls=MultiOption, type=str,  help="x xlabel")
+@click.option('-dg', '--dg', is_flag=True, default = False,
+              help=("AS events can be divided into two groups based on dPSI values \
+                   (group +: dPSI > 0, group -: dPSI < 0)"))                 
+@click.option('-fmt', '--format', "fmt", type=click.Choice(['auto', 'png', 'pdf', 'pptx']),
+                default="auto", help="output figure format") 
+@click.option('-fw', '--width', default=6, help="fig width, default=6 inches")
+@click.option('-fh', '--height', default=6, help="fig height, default=6 inches")
+@click.option('-res', '--resolution', default=72, help="resolution, default=72 ppi")
+def upset(*args, **kwargs):
+    if kwargs["fmt"] == "auto":
+        kwargs["fmt"] = sniff_fig_fmt(kwargs["output"])    
+    draw.upset(*args, **kwargs)
+
+
+@cli_fun.command(name="volcano", help="Volcano plot analysis for dPSI; short alias: vol")
+@click.option('-i', '--input', "file", type=click.Path(exists=True),
+                required=True, help="input psi files")    
 @click.option('-o', '--output', type=click.Path(), help="output path")
-@click.option('-axis', '--axis', type=click.IntRange(min=0, max=1), default=0,
-                help="merge direction, 0 for row merge and 1 for column merge")
-@click.option('-rmdup', '--rmdup', type=click.Choice(["index", 'all', 'content']), 
-                help="remove duplicate rows")
-@click.option('-rmna', '--rmna', is_flag=True, help="remove NA data")                
-def sub_merge_files(*args, **kwargs):
-    from astk.utils.func import merge_files
-    merge_files(*args, **kwargs)
+@click.option('-adpsi', '--adpsi', default=0.1, help="absolute dpsi cut-off value")
+@click.option('-pval', '--pvalue', default=0.05, help="p-value cut-off value")
+@fig_common_options()
+def sc_volcano(*args, **kwargs):
+    if kwargs["figfmt"] == "auto":
+        kwargs["figfmt"] = sniff_fig_fmt(kwargs["output"])       
+    draw.volcano(*args, **kwargs)
+
+
+@cli_fun.command(name="pca", help="PCA analysis for PSI")
+@click.option('-i', '--input', "files", cls=MultiOption, type=click.Path(exists=True),
+                required=True, help="input psi files")
+@click.option('-o', '--output', required=True, help="figure output path")
+@click.option('-gl', '--groupLabel', cls=MultiOption, type=str, help="file label")
+@click.option('-sep', '--sep', type=click.Choice([",", r"\t"]), 
+                help="separator of file content")
+@click.option('-gb', '--groupBy', type=click.Choice(["row", "col"]), required=True, 
+                help=("this option is used to choose whether the sample information is stored in rows or columns;"
+                       "AS event PSI use col, feature values use row"))
+@fig_common_options()
+def sc_pca(*args, **kwargs):
+    import pandas as pd
+    from .ml import plot_pca
+
+    if kwargs["figfmt"] == "auto":
+        kwargs["figfmt"] = sniff_fig_fmt(kwargs["output"])
+    if gn := kwargs.get("grouplabel", []):
+        if len(gn) != len(kwargs["files"]):
+            raise UsageError("-gl/--groupLabel number must be same as -i/--input")
+    else:
+        gn = [idx for idx, _ in enumerate(kwargs["files"])]
+    if kwargs["sep"] in ("\\t", "t"):
+        sep = "\t"
+    else:
+        sep = kwargs["sep"]
+    axis = 1 if kwargs["groupby"] == "col" else 0
+    dfs, labels = [], []
+    for idx, file in enumerate(kwargs["files"]):
+        df = pd.read_csv(file, sep=sep, index_col=0)
+        labels.extend([gn[idx]] * df.shape[axis])
+        dfs.append(df)
+    dfm = pd.concat(dfs, axis=axis, join='inner').dropna()
+    dfm = dfm.T if axis == 1 else dfm
+    plot_pca(kwargs["output"], dfm, labels)
+
+
+@cli_fun.command(help="Heatmap plot for PSI; short alias: hm")
+@click.option('-i', '--input', "files", cls=MultiOption, type=click.Path(exists=True),
+                required=True, help="input psi files")
+@click.option('-o', '--output', type=click.Path(), required=True, help="figure output path")
+@click.option('-cmap', '--colormap', default="crest", help="matplotlib colormap name")
+@fig_common_options()
+def heatmap(*args, **kwargs):
+    from matplotlib.pyplot import colormaps
+
+    if kwargs["figfmt"] == "auto":
+        kwargs["figfmt"] = sniff_fig_fmt(kwargs["output"])
+    if kwargs["colormap"] not in colormaps()+["crest"]:
+        msg  = f"'{kwargs['colormap']}' is not a valid value for colormap name"
+        msg += f"; supported values are {', '.join(map(repr, colormaps()))}"        
+        raise BadParameter(msg)
+    draw.heatmap(*args, **kwargs)
+
+
+@cli_fun.command(help="barplot")
+@click.option('-i', '--input', "files", cls=MultiOption, type=click.Path(exists=True),
+                required=True, help="input psi/dpsi files")
+@click.option('-o', '--output', required=True, help="output path")
+@click.option('-xl', '--xlabel', cls=MultiOption, type=str,
+             help="x tick labels for files")
+@click.option('-dg', '--dg', is_flag=True, default=False,
+              help=("AS events can be divided into two groups based on dPSI values \
+                   (group +: dPSI > 0, group -: dPSI < 0)"))
+@click.option('-app','--app', required=True, type=click.Choice(["SUPPA2"]), 
+                default="SUPPA2", help="the program that generates event file")                   
+@fig_common_options()
+def barplot(*args, **kwargs):
+    if kwargs["figfmt"] == "auto":
+        kwargs["figfmt"] = sniff_fig_fmt(kwargs["output"])
+    draw.barplot(*args, **kwargs)
```

### Comparing `astk-0.1.2/astk/constant.py` & `astk-0.1.2b0/astk/constant.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,24 +89,14 @@
         "MXE": [23, 9, 23, 9, 23, 9, 23, 9],
         "A5SS": [23, 9, 9, 23, 9],
         "A3SS": [23, 9, 23, 23, 9],
         "RI": [23, 9, 23, 9],           
     }
 }
 
-rMATS_EXON_COLS = {
-    "SE": [
-            "upstreamES", "upstreamEE", "exonStart_0base", "exonEnd",
-            "downstreamES", "downstreamEE"
-        ],
-    "A5SS": [
-        "longExonStart_0base","longExonEnd","shortES","shortEE","flankingES","flankingEE"
-    ]
-}
-
 rMATS_POS_COLS = {
     "A5SS": {
         "+": ["longExonStart_0base", "shortEE", "longExonEnd", "flankingES", "flankingEE"],
         "-": ["longExonEnd", "shortES", "longExonStart_0base", "flankingEE", "flankingES"]
     },
     "A3SS": {
         "+": ["flankingES", "flankingEE", "longExonStart_0base", "shortES", "longExonEnd"],
@@ -127,7 +117,26 @@
         ]
     },
     "RI": {
         "+": ["upstreamES", "upstreamEE", "downstreamES", "downstreamEE"],
         "-": ["downstreamEE", "downstreamES", "upstreamEE", "upstreamES"],
     }
 }
+
+ALT_IDX = {
+    "rMATS": {
+        "SE": [2, 3],
+        "A5SS": [1, 2],
+        "A3SS": [2, 3],
+        "MXE": [2, 3, 4, 5],
+        "RI": [1, 2]
+    },
+    "SUPPA2": {
+        "SE": [1, 2],
+        "MX": [1, 2, 3, 4],
+        "A5": [0, 1],
+        "A3": [1, 2],
+        "RI": [1, 2],
+        "AF": [1, 3],
+        "AL": [1, 3]
+    }
+}
```

### Comparing `astk-0.1.2/astk/data/maxent/ss3_score.json` & `astk-0.1.2b0/astk/data/maxent/ss3_score.json`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/maxent/ss5seq_score.json` & `astk-0.1.2b0/astk/data/maxent/ss5seq_score.json`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Arabidopsis_thaliana.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Arabidopsis_thaliana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Aspergillus_nidulans.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Aspergillus_nidulans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Bombyx_mori.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Bombyx_mori.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Bos_taurus.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Bos_taurus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Caenorhabditis_elegans.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Caenorhabditis_elegans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Cricetulus_griseus.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Cricetulus_griseus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Danio_rerio.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Danio_rerio.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Drosophila_melanogaster.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Drosophila_melanogaster.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Gallus_gallus.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Gallus_gallus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Homo_sapiens.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Homo_sapiens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Leishmania_major.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Leishmania_major.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Mesocricetus_auratus.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Mesocricetus_auratus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Mus_musculus.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Mus_musculus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Naegleria_gruberi.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Naegleria_gruberi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Nematostella_vectensis.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Nematostella_vectensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Neurospora_crassa.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Neurospora_crassa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Oryctolagus_cuniculus.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Oryctolagus_cuniculus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Oryzias_latipes.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Oryzias_latipes.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Ostreococcus_tauri.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Ostreococcus_tauri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Physcomitrella_patens.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Physcomitrella_patens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Phytophthora_ramorum.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Phytophthora_ramorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Plasmodium_falciparum.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Plasmodium_falciparum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Rattus_norvegicus.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Rattus_norvegicus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Rhizopus_oryzae.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Rhizopus_oryzae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae_s288c.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae_s288c.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Schistosoma_mansoni.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Schistosoma_mansoni.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Spodoptera_frugiperda.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Spodoptera_frugiperda.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Tetraodon_nigroviridis.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Tetraodon_nigroviridis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Thalassiosira_pseudonana.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Thalassiosira_pseudonana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Trichomonas_vaginalis.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Trichomonas_vaginalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Trypanosoma_brucei.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Trypanosoma_brucei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Vanderwaltozyma_polyspora.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Vanderwaltozyma_polyspora.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Xenopus_laevis.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Xenopus_laevis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Xenopus_tropicalis.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Xenopus_tropicalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ATtRACT/Zea_mays.meme` & `astk-0.1.2b0/astk/data/motif/ATtRACT/Zea_mays.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Acyrtosiphon_pisum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Acyrtosiphon_pisum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aedes_aegypti.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aedes_aegypti.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Agaricus_bisporus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Agaricus_bisporus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ailuropoda_melanoleuca.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ailuropoda_melanoleuca.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Allomyces_macrogynus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Allomyces_macrogynus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Alternaria_brassicicola.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Alternaria_brassicicola.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Amphimedon_queenslandica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Amphimedon_queenslandica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Anolis_carolinensis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Anolis_carolinensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Anopheles_gambiae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Anopheles_gambiae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Apis_mellifera.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Apis_mellifera.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Arabidopsis_lyrata.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Arabidopsis_lyrata.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Arabidopsis_thaliana.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Arabidopsis_thaliana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Arthroderma_benhamiae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Arthroderma_benhamiae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ashbya_gossypii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ashbya_gossypii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_carbonarius.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_carbonarius.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_clavatus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_clavatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_flavus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_flavus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_fumigatus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_fumigatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_nidulans.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_nidulans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_niger.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_niger.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_oryzae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_oryzae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aspergillus_terreus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aspergillus_terreus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Aureococcus_anophagefferens.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Aureococcus_anophagefferens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Batrachochytrium_dendrobatidis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Batrachochytrium_dendrobatidis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Blastomyces_dermatitidis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Blastomyces_dermatitidis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Bombyx_mori.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Bombyx_mori.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Bos_taurus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Bos_taurus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Botrytis_cinerea.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Botrytis_cinerea.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Brachypodium_distachyon.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Brachypodium_distachyon.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Branchiostoma_floridae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Branchiostoma_floridae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Brugia_malayi.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Brugia_malayi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_brenneri.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_brenneri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_briggsae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_briggsae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_elegans.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_elegans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_japonica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_japonica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Caenorhabditis_remanei.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Caenorhabditis_remanei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Callithrix_jacchus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Callithrix_jacchus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_albicans.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_albicans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_dubliniensis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_dubliniensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_glabrata.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_glabrata.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_guilliermondii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_guilliermondii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_lusitaniae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_lusitaniae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_parapsilosis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_parapsilosis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Candida_tropicalis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Candida_tropicalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Canis_familiaris.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Canis_familiaris.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Cannabis_sativa.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cannabis_sativa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Capitella_teleta.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Capitella_teleta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Capsaspora_owczarzaki.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Capsaspora_owczarzaki.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Cavia_porcellus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cavia_porcellus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Chaetomium_globosum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Chaetomium_globosum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Chlamydomonas_reinhardtii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Chlamydomonas_reinhardtii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Chlorella_NC64A.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Chlorella_NC64A.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Chlorella_vulgaris.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Chlorella_vulgaris.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Choloepus_hoffmanni.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Choloepus_hoffmanni.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ciona_intestinalis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ciona_intestinalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ciona_savignyi.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ciona_savignyi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Coccidioides_immitis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Coccidioides_immitis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Coccidioides_posadasii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Coccidioides_posadasii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Coccomyxa_C_169.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Coccomyxa_C_169.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Cochliobolus_heterostrophus_C5.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cochliobolus_heterostrophus_C5.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Colletotrichum_graminicola.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Colletotrichum_graminicola.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Coprinopsis_cinerea.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Coprinopsis_cinerea.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Cryphonectria_parasitica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cryphonectria_parasitica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Cryptosporidium_hominis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cryptosporidium_hominis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Cryptosporidium_parvum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cryptosporidium_parvum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Cucumis_sativus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Cucumis_sativus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Culex_pipiens.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Culex_pipiens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Culex_quinquefasciatus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Culex_quinquefasciatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Danio_rerio.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Danio_rerio.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Daphnia_pulex.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Daphnia_pulex.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Dasypus_novemcinctus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Dasypus_novemcinctus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Debaryomyces_hansenii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Debaryomyces_hansenii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Dictyostelium_discoideum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Dictyostelium_discoideum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Dictyostelium_purpureum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Dictyostelium_purpureum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Dipodomys_ordii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Dipodomys_ordii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_ananassae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_ananassae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_erecta.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_erecta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_grimshawi.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_grimshawi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_melanogaster.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_melanogaster.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_mojavensis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_mojavensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_persimilis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_persimilis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_pseudoobscura.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_pseudoobscura.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_sechellia.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_sechellia.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_simulans.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_simulans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_virilis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_virilis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_willistoni.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_willistoni.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Drosophila_yakuba.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Drosophila_yakuba.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Echinops_telfairi.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Echinops_telfairi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Emiliania_huxleyi.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Emiliania_huxleyi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Equus_caballus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Equus_caballus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Erinaceus_europaeus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Erinaceus_europaeus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Felis_catus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Felis_catus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Fragilariopsis_cylindrus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Fragilariopsis_cylindrus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Fusarium_graminearum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Fusarium_graminearum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Fusarium_oxysporum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Fusarium_oxysporum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Fusarium_verticillioides.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Fusarium_verticillioides.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Gallus_gallus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Gallus_gallus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Gasterosteus_aculeatus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Gasterosteus_aculeatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Glycine_max.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Glycine_max.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Gorilla_gorilla.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Gorilla_gorilla.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Helobdella_robusta.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Helobdella_robusta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Heterobasidion_annosum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Heterobasidion_annosum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Histoplasma_capsulatum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Histoplasma_capsulatum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Homo_sapiens.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Homo_sapiens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Hydra_magnipapillata.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Hydra_magnipapillata.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ixodes_scapularis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ixodes_scapularis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Kluyveromyces_lactis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Kluyveromyces_lactis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Kluyveromyces_thermotolerans.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Kluyveromyces_thermotolerans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Kluyveromyces_waltii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Kluyveromyces_waltii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Laccaria_bicolor.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Laccaria_bicolor.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Lachancea_kluyveri.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Lachancea_kluyveri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Leishmania_braziliensis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Leishmania_braziliensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Leishmania_infantum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Leishmania_infantum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Leishmania_major.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Leishmania_major.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Leishmania_mexicana.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Leishmania_mexicana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Loa_loa.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Loa_loa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Lodderomyces_elongisporus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Lodderomyces_elongisporus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Lottia_gigantea.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Lottia_gigantea.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Lotus_japonicus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Lotus_japonicus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Loxodonta_africana.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Loxodonta_africana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Macaca_mulatta.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Macaca_mulatta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Macropus_eugenii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Macropus_eugenii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Magnaporthe_oryzae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Magnaporthe_oryzae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Malassezia_globosa.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Malassezia_globosa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Malus_x_domestica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Malus_x_domestica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Manihot_esculenta.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Manihot_esculenta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Medicago_truncatula.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Medicago_truncatula.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Melampsora_laricis_populina.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Melampsora_laricis_populina.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Meleagris_gallopavo.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Meleagris_gallopavo.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Meloidogyne_incognita.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Meloidogyne_incognita.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Microcebus_murinus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Microcebus_murinus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Micromonas_pusilla.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Micromonas_pusilla.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Microsporum_canis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Microsporum_canis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Microsporum_gypseum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Microsporum_gypseum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Mimulus_guttatus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mimulus_guttatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Monodelphis_domestica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Monodelphis_domestica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Monosiga_brevicollis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Monosiga_brevicollis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Mucor_circinelloides.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mucor_circinelloides.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Mus_musculus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mus_musculus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Myceliophthora_thermophila.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Myceliophthora_thermophila.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Mycosphaerella_fijiensis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mycosphaerella_fijiensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Mycosphaerella_graminicola.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Mycosphaerella_graminicola.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Myotis_lucifugus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Myotis_lucifugus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Naegleria_gruberi.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Naegleria_gruberi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Nasonia_vitripennis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Nasonia_vitripennis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Nectria_haematococca.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Nectria_haematococca.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Nematostella_vectensis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Nematostella_vectensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Neosartorya_fischeri.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neosartorya_fischeri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Neospora_caninum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neospora_caninum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Neurospora_crassa.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neurospora_crassa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Neurospora_discreta.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neurospora_discreta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Neurospora_tetrasperma.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Neurospora_tetrasperma.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ochotona_princeps.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ochotona_princeps.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Oikopleura_dioica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oikopleura_dioica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ornithorhynchus_anatinus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ornithorhynchus_anatinus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Oryctolagus_cuniculus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oryctolagus_cuniculus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Oryza_indica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oryza_indica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Oryza_sativa.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oryza_sativa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Oryzias_latipes.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Oryzias_latipes.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ostreococcus_RCC809.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ostreococcus_RCC809.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ostreococcus_lucimarinus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ostreococcus_lucimarinus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ostreococcus_tauri.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ostreococcus_tauri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Otolemur_garnettii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Otolemur_garnettii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pan_troglodytes.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pan_troglodytes.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Paracoccidioides_brasiliensis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Paracoccidioides_brasiliensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pediculus_humanus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pediculus_humanus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Penicillium_chrysogenum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Penicillium_chrysogenum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Penicillium_marneffei.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Penicillium_marneffei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Phaeodactylum_tricornutum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phaeodactylum_tricornutum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Phaeosphaeria_nodorum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phaeosphaeria_nodorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Phanerochaete_chrysosporium.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phanerochaete_chrysosporium.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Phoenix_dactylifera.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phoenix_dactylifera.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Phycomyces_blakesleeanus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phycomyces_blakesleeanus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Physcomitrella_patens.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Physcomitrella_patens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Phytophthora_capsici.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phytophthora_capsici.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Phytophthora_infestans.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phytophthora_infestans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Phytophthora_ramorum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phytophthora_ramorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Phytophthora_sojae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Phytophthora_sojae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pichia_pastoris.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pichia_pastoris.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pichia_stipitis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pichia_stipitis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_berghei.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_berghei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_chabaudi.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_chabaudi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_falciparum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_falciparum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_knowlesi.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_knowlesi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_vivax.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_vivax.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Plasmodium_yoelii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Plasmodium_yoelii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pleurotus_ostreatus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pleurotus_ostreatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pneumocystis_carinii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pneumocystis_carinii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Podospora_anserina.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Podospora_anserina.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Polysphondylium_pallidum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Polysphondylium_pallidum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pongo_pygmaeus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pongo_pygmaeus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Populus_trichocarpa.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Populus_trichocarpa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Postia_placenta.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Postia_placenta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pristionchus_pacificus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pristionchus_pacificus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Procavia_capensis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Procavia_capensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Prunus_persica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Prunus_persica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pteropus_vampyrus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pteropus_vampyrus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Pyrenophora_tritici_repentis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Pyrenophora_tritici_repentis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/RNAcompete_CONSTRUCTS.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/RNAcompete_CONSTRUCTS.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Rattus_norvegicus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Rattus_norvegicus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Rhizopus_oryzae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Rhizopus_oryzae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ricinus_communis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ricinus_communis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_bayanus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_bayanus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_castellii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_castellii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_cerevisiae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_cerevisiae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_kudriavzevii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_kudriavzevii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_mikatae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_mikatae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Saccharomyces_paradoxus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saccharomyces_paradoxus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Salpingoeca_rosetta.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Salpingoeca_rosetta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Saprolegnia_parasitica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Saprolegnia_parasitica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Schistosoma_japonicum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schistosoma_japonicum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Schistosoma_mansoni.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schistosoma_mansoni.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Schizophyllum_commune.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizophyllum_commune.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Schizosaccharomyces_cryophilus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_cryophilus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Schizosaccharomyces_japonicus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_japonicus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Schizosaccharomyces_octosporus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_octosporus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Schizosaccharomyces_pombe.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_pombe.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Sclerotinia_sclerotiorum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sclerotinia_sclerotiorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Selaginella_moellendorfii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Selaginella_moellendorfii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Serpula_lacrymans.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Serpula_lacrymans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Sorex_araneus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sorex_araneus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Sorghum_bicolor.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sorghum_bicolor.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Spermophilus_tridecemlineatus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Spermophilus_tridecemlineatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Spizellomyces_punctatus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Spizellomyces_punctatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Sporobolomyces_roseus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sporobolomyces_roseus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Stagonospora_nodorum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Stagonospora_nodorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Strongylocentrotus_purpuratus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Strongylocentrotus_purpuratus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Sus_scrofa.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Sus_scrofa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Taeniopygia_guttata.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Taeniopygia_guttata.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Takifugu_rubripes.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Takifugu_rubripes.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Tarsius_syrichta.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tarsius_syrichta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Tetraodon_nigroviridis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tetraodon_nigroviridis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Thalassiosira_pseudonana.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Thalassiosira_pseudonana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Thecamonas_trahens.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Thecamonas_trahens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Thielavia_terrestris.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Thielavia_terrestris.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Toxoplasma_gondii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Toxoplasma_gondii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Tremella_mesenterica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tremella_mesenterica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Tribolium_castaneum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tribolium_castaneum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trichoderma_atroviride.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichoderma_atroviride.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trichoderma_reesei.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichoderma_reesei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trichoderma_virens.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichoderma_virens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trichomonas_vaginalis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichomonas_vaginalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trichophyton_equinum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichophyton_equinum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trichophyton_rubrum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichophyton_rubrum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trichophyton_tonsurans.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichophyton_tonsurans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trichophyton_verrucosum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichophyton_verrucosum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trichoplax_adhaerens.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trichoplax_adhaerens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trypanosoma_brucei.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trypanosoma_brucei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trypanosoma_congolense.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trypanosoma_congolense.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trypanosoma_cruzi.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trypanosoma_cruzi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Trypanosoma_vivax.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Trypanosoma_vivax.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Tuber_melanosporum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tuber_melanosporum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Tupaia_belangeri.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tupaia_belangeri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Tursiops_truncatus.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Tursiops_truncatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Uncinocarpus_reesii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Uncinocarpus_reesii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Ustilago_maydis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Ustilago_maydis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Vanderwaltozyma_polyspora.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Vanderwaltozyma_polyspora.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Verticillium_albo_atrum.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Verticillium_albo_atrum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Verticillium_dahliae.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Verticillium_dahliae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Vicugna_pacos.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Vicugna_pacos.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Vitis_vinifera.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Vitis_vinifera.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Volvox_carteri.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Volvox_carteri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Wuchereria_bancrofti.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Wuchereria_bancrofti.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Xenopus_laevis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Xenopus_laevis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Xenopus_tropicalis.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Xenopus_tropicalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Yarrowia_lipolytica.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Yarrowia_lipolytica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Zea_mays.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Zea_mays.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/CISBP-RNA/Zygosaccharomyces_rouxii.meme` & `astk-0.1.2b0/astk/data/motif/CISBP-RNA/Zygosaccharomyces_rouxii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ELM/elm_classes.tsv` & `astk-0.1.2b0/astk/data/motif/ELM/elm_classes.tsv`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ELM/elm_instances.tsv` & `astk-0.1.2b0/astk/data/motif/ELM/elm_instances.tsv`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ELM/hg38_alter_exon_seq.json` & `astk-0.1.2b0/astk/data/motif/ELM/hg38_alter_exon_seq.json`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/data/motif/ELM/mm10_alter_exon_seq.json` & `astk-0.1.2b0/astk/data/motif/ELM/mm10_alter_exon_seq.json`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/event/_cli_func.py` & `astk-0.1.2b0/astk/event/_cli_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 import astk.utils.func  as ul
 import astk.utils.select as sl
-from astk.types import FilePath
+from astk.ctypes import FilePath
 from .eid import SuppaEventID
 
 
 def len_dist(infile, output, custom_len, cluster, width, len_weight, max_len, fmt):
     import pandas as pd
 
     if not (pdir:= Path(output).parent).exists():
@@ -18,35 +18,30 @@
     cluster_ls = []
     clens = [0] + list(custom_len)
     print(clens)
     for i in range(1, len(clens)):
         print( clens[i-1], clens[i])
         subset = [l for l in  ae_lens if clens[i-1] < l <= clens[i]]
         cluster_ls.append(subset)
-    else:
-        subset = [l for l in  ae_lens if l > clens[-1]]
-        cluster_ls.append(subset)
+    subset = [l for l in  ae_lens if l > clens[-1]]
+    cluster_ls.append(subset)
     output = Path(output).with_suffix(f".{fmt}")
     ul.plot_hist_cluster(output, cluster_ls, bin_edges)
 
 
 def len_cluster(files, indir, outdir, lenrange):
 
     outdir = Path(outdir)
     outdir = Path(outdir).absolute()
     outdir.mkdir(exist_ok=True)
 
     lrs = list(map(int, lenrange))
     coor_ls = [(lrs[i], lrs[i+1]) for i in range(len(lrs)-1)]
 
-    if indir:
-        files = list(Path(indir).glob("*psi"))
-    else:
-        files = [Path(i) for i in files]
-    
+    files = list(Path(indir).glob("*psi")) if indir else [Path(i) for i in files]
     if len(files) == 1:
         file = Path(files[0])
         outdir.mkdir(exist_ok=True)
         for s, e in coor_ls:
             outfile = outdir / f"{file.stem}_{s}-{e}{file.suffix}"
             ul.df_len_select(file, outfile, s, e)
     else:
@@ -118,28 +113,54 @@
     if sep and abs_dpsi:
         pos_df = df_fil.loc[df_fil[dpsi_col] > 0, ]
         neg_df = df_fil.loc[df_fil[dpsi_col] < 0, ]
         pos_df.to_csv(pos_out, sep="\t")
         neg_df.to_csv(neg_out, sep="\t")
 
 
-def psi_filter(file, output, psi, quantile):
+def psi_filter(
+    file: str, 
+    output: str, 
+    minv: float = 0, 
+    maxv: float = 1, 
+    minq: float = 0, 
+    maxq: float = 1, 
+    app: str = "auto"
+):
+    from pandas import read_csv
+
+    def _rmats_mean_psi(vstr):
+        strings = vstr.split(",")
+        values = [float(i) for i in strings if i != "NA"]
+        return sum(values) / len(values)
+        
+    dpsi_df = read_csv(file, sep="\t", index_col=0).dropna()
+    if app == "auto":
+        app = ul.detect_file_info(file)["app"]
+    if app == "rMATS":        
+        dpsi_df["PSI"] = dpsi_df["IncLevel1"].apply(_rmats_mean_psi)
+    elif app == "SUPPA2":
+        dpsi_df["PSI"] = dpsi_df.apply(lambda row: sum(row)/len(row), axis=1)
+
+    min_psi = max([dpsi_df["PSI"].quantile(minq), minv])
+    max_psi = min([dpsi_df["PSI"].quantile(maxq), maxv])
+    keep = (dpsi_df["PSI"] >= min_psi) & (dpsi_df["PSI"] <= max_psi)
+    df_fil = dpsi_df.loc[keep, ]
+    del df_fil["PSI"]
+    df_fil.to_csv(output, sep="\t")
+    return df_fil
 
-    if file:
-        pf = sl.PsiFilter(file, output, psi, quantile)
-        pf.run()
-  
 
 def intersect(
     file_a: FilePath,
     file_b: FilePath,
     output: FilePath, 
     ioeb: FilePath, 
     ignoreb: bool
-    ) -> None:
+) -> None:
 
     from pandas import read_csv
 
     outname = Path(output).stem
     outdir = Path(output).parent
     fa = Path(file_a)
     dfa = read_csv(fa, sep="\t", index_col=0)
```

### Comparing `astk-0.1.2/astk/event/eid.py` & `astk-0.1.2b0/astk/event/eid.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,16 +60,14 @@
             e2, s3, e1, _ = map(int, nums)
             coors = (e1, e2, s3)
             self.alter_element_coor = (e1, e2)
         elif A5_rs or A3_fs:
             e1, s2, _, s3 = map(int, nums)
             coors = (e1, s2, s3)
             self.alter_element_coor = (s2, s3)
-        else:
-            coors = ()
         return coors
 
     def _parse_RI_coor(self):
         nums = self.coordinate_str.split("-")
         s1, e1, s2, e2 = map(int, nums)
         self.alter_element_coor = (e1, s2)
         return (s1, e1, s2, e2)
@@ -86,11 +84,9 @@
             s1, e1, s3, s2, e2, _ = map(int, nums)
             coors = (s1, e1, s2, e2, s3)
             self.alter_element_coor = (s1, e1)
         elif AF_rs or AL_fs:
             e1, s2, e2, _, s3, e3 = map(int, nums)
             coors = (e1, s2, e2, s3, e3)
             self.alter_element_coor = (s3, e3)
-        else:
-            coors = ()
         return coors
```

### Comparing `astk-0.1.2/astk/gsea/_func.py` & `astk-0.1.2b0/astk/gsea/_func.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 import subprocess
 from pathlib import Path
 from typing import Sequence
 
 from astk.constant import BASE_DIR, PATHWAY_DB_ORG
 import astk.utils.func  as ul
-from astk.types import FilePath
+from astk.ctypes import FilePath
 from astk.event import SuppaEventID
-                
-def gsea_fun(file, outdir, name, pvalue, database, geneid, orgdb, ont, organism):
-    Path(outdir).mkdir(exist_ok=True)
-    if not (org_db := ul.select_OrgDb(orgdb)):
-        print(f"{orgdb} is wrong! Please run 'astk ls -org' to view more")
 
+
+def gsea_fun(
+    file: FilePath, 
+    outdir: FilePath, 
+    name: str, 
+    pvalue: float, 
+    database: str, 
+    gene_id: str, 
+    ontology: str, 
+    organism: str,
+    app: str
+):
+    Path(outdir).mkdir(exist_ok=True)
+    if not (org_db := ul.select_OrgDb(organism)):
+        print(f"{organism} is wrong! Please run 'astk ls -org' to view more")
+    if database in {"KEGG", "Reactome"}:
+        organism = PATHWAY_DB_ORG[database].get(organism, None)
     rscript = BASE_DIR / "R" / "gsea.R"
-    params = [outdir, str(pvalue), org_db, ont, geneid, name, database, organism, file]
+    params = [outdir, str(pvalue), org_db, ontology, 
+                gene_id, name, database, organism, file, app]
     info = subprocess.Popen([ul.Rscript_bin(), str(rscript), *params])
     info.wait()
 
    
 def enrich(
     file: FilePath,
     outdir: FilePath, 
     pvalue: float, 
     qvalue: float, 
     database: str, 
     ontology: str,  
     gene_id: str, 
     organism: str, 
     simple: bool,
-    fmt: str, 
+    figfmt: str, 
     width: float, 
-    height: float
+    height: float,
+    app: str
 ) -> None:
     rscript = BASE_DIR / "R" / "enrich.R"
     if not (org_db := ul.select_OrgDb(organism)):
         print(f"{organism} is wrong! Please run 'astk ls -org' to view more")
-    if database in ["KEGG", "Reactome"]:
+    if database in {"KEGG", "Reactome"}:
         organism = PATHWAY_DB_ORG[database].get(organism, None)
     Path(outdir).mkdir(exist_ok=True)
     param_dic = {
         "file": file,
         "outdir": outdir, 
         "orgdb": org_db,
         "database": database,
@@ -47,38 +61,40 @@
         "qval": qvalue,
         "organism": organism,
         "genetype": gene_id,
         "ontology": ontology,
         "simple": simple,
         "width": width,
         "height": height,
-        "fmt": fmt
+        "fmt": figfmt,
+        "app": app
     }
     param_ls = ul.parse_cmd_r(**param_dic)
     subprocess.run([ul.Rscript_bin(), rscript, *param_ls])
 
-             
+
 def enrich_cmp(
     files: Sequence[FilePath],
     outdir: FilePath, 
     database: str, 
     ontology: str,
     pvalue: float,
     qvalue: float, 
     xlabel: Sequence[str],
     gene_id: str,
     organism: str,
-    fmt: str,
+    figfmt: str,
     width: float,
-    height: float
+    height: float,
+    app: str
 ) -> None:
 
     if not (org_db := ul.select_OrgDb(organism)):
         print(f"{organism} is wrong! Please run 'astk ls -orgdb' to view more")
-    if database in ["KEGG", "Reactome"]:
+    if database in {"KEGG", "Reactome"}:
         organism = PATHWAY_DB_ORG[database].get(organism, None)
     rscript = BASE_DIR / "R" / "enrichCompare.R"
     Path(outdir).mkdir(exist_ok=True)
     param_dic = {
         "files": files,
         "outdir": outdir, 
         "orgdb": org_db,
@@ -87,51 +103,24 @@
         "qval": qvalue,
         "xlabel": xlabel, 
         "organism": organism,
         "genetype": gene_id,
         "ontology": ontology,
         "width": width,
         "height": height,
-        "fmt": fmt
+        "fmt": figfmt,
+        "app": app
     }
     param_ls = ul.parse_cmd_r(**param_dic)
     subprocess.run([ul.Rscript_bin(), rscript, *param_ls])
 
 
-def enrich_lc(files, outdir, cluster, merge, database, pvalue, qvalue,
-              gene_id, orgdb, kegg_organism):
-    if not (org_db := ul.select_OrgDb(orgdb)):
-        print(f"{orgdb} is wrong! Please run 'astk ls -orgdb' to view more")                
-    if database == "KEGG":
-        ul.check_kegg_RData(kegg_organism)
-        if not kegg_organism:
-            print("Error: --kegg_organism is required!")
-            exit()
-    else:
-        kegg_organism = "0"
-    rscript = BASE_DIR / "R" / "enrichLenCluster.R"
-    Path(outdir).mkdir(exist_ok=True)
-    merge = "1" if merge else "0"
-    for file in files:
-        params = [outdir, str(pvalue), str(qvalue), database, cluster,
-                 org_db, gene_id, kegg_organism, file]
-        info = subprocess.Popen([ul.Rscript_bin(), str(rscript), *params])
-        if database == "KEGG" and not ul.check_kegg_RData(kegg_organism):
-             info.wait() 
-    else:
-        if merge:
-            params = [outdir, str(pvalue), str(qvalue), database, cluster,
-                 org_db, gene_id, kegg_organism, *files]
-            merge_info = subprocess.Popen([ul.Rscript_bin(), str(rscript), *params])
-            merge_info.wait()
-        else:
-            info.wait()
-
-
-def nease_enrich(nease_input, outdir, n=15, database=['Reactome'], organism='Human', cutoff=0.05):
+def nease_enrich(nease_input, outdir, n=15, database=None, organism='Human', cutoff=0.05):
+    if database is None:
+        database = ['Reactome']
     import nease
     import numpy as np
     import matplotlib.pyplot as plt
 
     events = nease.run(nease_input, organism=organism, p_value_cutoff=cutoff)
 
     outdir = Path(outdir)
@@ -193,13 +182,14 @@
     # dfl = pd.concat([df_top, df_share])
     dfl = df_top
     dfl["Pathway name"] = dfl["Pathway name"].apply(lambda x: x.split("- Homo")[0])
     if all([width, height]):
         fig, ax = plt.subplots(figsize=(width, height))
     else:
         ax = None
+    plt.grid(linestyle='dotted', axis='y', color='#808080', dashes=(1, 6), zorder=1)
     palette = sns.color_palette("crest", as_cmap=True)
-    ax = sns.scatterplot(data=dfl, x="cluster", y="Pathway name",palette=palette,
+    ax = sns.scatterplot(data=dfl, x="cluster", y="Pathway name", palette=palette, zorder=2,
                          ax=ax, size="Nease score", hue="adj p_value", sizes=(50, 250))
     ax.legend(bbox_to_anchor=(1.05, 1.0), loc='upper left')
-    ax.set_xlim(-0.5, len(top_res_ls)-0.5)
+    ax.set_xlim(-0.5, len(top_res_ls)-0.5)    
     plt.savefig(outdir / f"cmp_enrichment.{figformat}", bbox_inches='tight')
```

### Comparing `astk-0.1.2/astk/motif/_func.py` & `astk-0.1.2b0/astk/motif/_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,15 @@
     }
     param_ls = ul.parse_cmd_r(**param_dic)
     exe_bin = "centrimo"
     subprocess.run([exe_bin, *param_ls, tfa, motif])
 
 
 def _ame_enrich(outdir, tfa, cfa, motif):
-    param_dic = {
-        "oc": outdir,
-        "control": cfa if cfa else "--shuffle--",
-        "text": True
-    }
+    param_dic = {"oc": outdir, "control": cfa or "--shuffle--", "text": True}
     param_ls = ul.parse_cmd_r(**param_dic)
     exe_bin = "ame"
     subprocess.run([exe_bin, *param_ls, tfa, motif])
 
 
 def _streme_enrich(outdir, tfa, cfa, pvalue, evalue, maxw, minw):
     param_dic = {
```

### Comparing `astk-0.1.2/astk/motif/elm.py` & `astk-0.1.2b0/astk/motif/elm.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/network/_func.py` & `astk-0.1.2b0/astk/network/_func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/seqfeature/_compare.py` & `astk-0.1.2b0/astk/seqfeature/_compare.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         df["condition"] = gns[i]
 
     df = pd.concat(df_ls)
     dft = df.melt(id_vars=["condition"], var_name="splice_site", value_name="score")
     sns.set_theme()
     pairs = [[(i, gn) for gn in gns] for i in df.columns[:-1]]
     fig_type = kwargs.get("figtype", "point")
-    if fig_type == "strip":
-        fig_kwargs = {"split": True}
-    else:
-        fig_kwargs = {}
+    fig_kwargs = {"split": True} if fig_type == "strip" else {}
     if all([kwargs["width"], kwargs["height"]]):
         fig_kwargs["height"] = kwargs["height"]
         fig_kwargs["aspect"] = kwargs["width"] / kwargs["height"]
     g = sns.catplot(
         data=dft, x="splice_site", y="score", 
         hue="condition", kind=fig_type, legend=False, **fig_kwargs
     )
@@ -36,53 +33,52 @@
     annotator.apply_test()
     annotator.annotate()
     plt.legend(loc='upper left', bbox_to_anchor=(1.03, 1))
     fig_fmt = kwargs.get("figformat", "auto")
     if fig_fmt == "auto":
         fig_fmt = sniff_fig_fmt(output, fmts=['png', 'pdf', 'tiff', 'jpeg'])
 
-    output = Path(output).with_suffix(f".{fig_fmt}")    
+    output = Path(output).with_suffix(f".{fig_fmt}")
     plt.savefig(output, dpi=300, bbox_inches='tight', facecolor="w")  
 
 
 def cmp_value(files, output, test, **kwargs):
     import numpy as np
-    import pandas as pd    
+    import pandas as pd
     import seaborn as sns
     import matplotlib.pyplot as plt
     from statannotations.Annotator import Annotator
 
     df_ls = [pd.read_csv(file, index_col=0) for file in files]
     gns = kwargs.get("groupnames")
     origin_col = df_ls[0].columns
     for i, df in enumerate(df_ls):
         if kwargs.get("log", False):
             df.iloc[:, :df.shape[1]] = np.log2(df)
         xlabel = kwargs["xlabel"]
         if (xlabel is not None) and (len(xlabel) == df.shape[1]):
             if len(xlabel) == len(set(xlabel)):
-                columns = [(i, j) for i,j in zip(xlabel, xlabel)]
+                columns = list(zip(xlabel, xlabel))
             else:
-                columns = [(i, j) for i,j in zip(origin_col, xlabel)]
+                columns = list(zip(origin_col, xlabel))
         else:            
             columns = [(col, "_".join(col.split("_")[:2])) for col in origin_col]
         columns = pd.MultiIndex.from_tuples(columns)
         df.columns = columns
         df["condition"] = gns[i]
     df = pd.concat(df_ls)
     ss_cols = df.columns[:-1]
-    xn, yn = kwargs["xtitle"], kwargs["ytitle"]    
+    xn, yn = kwargs["xtitle"], kwargs["ytitle"]
     dft = df.melt(id_vars=["condition"]) # var_name=xn, value_name=yn
     if kwargs.pop("merge_ss"):
         ss_df = dft["variable_0"].str.split("_", n=1, expand=True)
         dft["variable_0"] = ss_df[1]
         dft["variable_1"] = ss_df[1]
         ss_cols = [["5SS", "5SS"], ["3SS","3SS"]]
     dft.rename(columns={"variable_0": xn, "variable_1": "item", "value": yn}, inplace=True)
-    sns.set_theme()
     pairs = []
     for col in ss_cols:
         for gn_c in combinations(gns, 2):
             pairs.append(((col[0], gn_c[0]), (col[0], gn_c[1])))
     fig_kwargs = {}
     if (fig_type := kwargs["figtype"]) == "strip":
         fig_kwargs["split"] = True
@@ -90,29 +86,29 @@
         fig_kwargs["sharex"] = False
         fig_kwargs["sharey"] = False
         fig_kwargs["col"] = "item"
     if all([kwargs["width"], kwargs["height"]]):
         fig_kwargs["height"] = kwargs["height"]
         fig_kwargs["aspect"] = kwargs["width"] / kwargs["height"]
     g = sns.catplot(
-        data=dft, kind=fig_type, x=xn, y=yn, 
+        data=dft, kind=fig_type, x=xn, y=yn,
         hue="condition", legend=False, **fig_kwargs)
     test_kwargs = {
         "comparisons_correction": kwargs["multicorrect"], 
         "show_test_name": False,
         "text_format": kwargs["pvaltext"]
-    }        
+    }
     if kwargs.get("facet", False):
         l_col_dic = {}
         for s_col, l_col in ss_cols:
             l_col_dic.setdefault(l_col, [])
             l_col_dic[l_col].append(s_col)
         s_col_dic = dict(ss_cols)
-        l_col_ls = [lcol for lcol in l_col_dic.keys()]
-        for i, pair in enumerate(pairs):            
+        l_col_ls = list(l_col_dic.keys())
+        for pair in pairs:
             col_g1 = pair[0][0]
             ax = g.axes[0][l_col_ls.index(s_col_dic[col_g1])]
             annotator = Annotator(ax, [pair],
                     data=dft.loc[dft["item"]==s_col_dic[col_g1],],  x=xn, y=yn, 
                     hue="condition",order=l_col_dic[s_col_dic[col_g1]])
             annotator.configure(test=test, **test_kwargs)
             annotator.apply_test()
@@ -121,13 +117,13 @@
         annotator = Annotator(
                 g.ax, pairs,  data=dft, 
                 x=xn, y=yn, hue="condition")
         annotator.configure(test=test, **test_kwargs)
         annotator.apply_test()
         annotator.annotate() 
     plt.legend(loc='upper left', bbox_to_anchor=(1.03, 1))
-    fig_fmt = kwargs.get("figformat", "auto")
+    fig_fmt = kwargs.get("figfmt", "auto")
     if fig_fmt == "auto":
         fig_fmt = sniff_fig_fmt(output, fmts=['png', 'pdf', 'tiff', 'jpeg'])
     output = Path(output).with_suffix(f".{fig_fmt}")
     plt.xticks(rotation=kwargs["xrotation"])
     plt.savefig(output, dpi=300, bbox_inches='tight', facecolor="w")
```

### Comparing `astk-0.1.2/astk/seqfeature/_feature.py` & `astk-0.1.2b0/astk/seqfeature/_feature.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from pathlib import Path
 import multiprocessing as mp
 
 import astk.utils as ul
+from astk.lazy_loader import LazyLoader
+
+np = LazyLoader("np", globals(), "numpy")
+pd = LazyLoader("pd", globals(), "pandas")
+plt = LazyLoader("plt", globals(), "matplotlib.pyplot")
 
 
 def _seq_gcc(seq):
     seq = seq.upper()
     GN = seq.count("G")
     GC = seq.count("C")
     return( GN + GC) / len(seq)
@@ -16,44 +21,30 @@
         gcc = [_seq_gcc(seq)]
     else:
         gcc = [_seq_gcc(seq[i:i+binsize]) for i in range(len(seq)-binsize-1)]
     return gcc
 
 
 def get_seq_gcc(fasta, binsize, process=4):
-    from pandas import DataFrame
-
     with open(fasta, "r") as rh:
         seqs = ul.read_fasta(rh)
         pool = mp.Pool(process)
         gccs = [pool.apply(_get_seq_gcc, args=(seq[1], binsize)) for seq in seqs]
         pool.close()
     
-    return DataFrame(gccs)
+    return pd.DataFrame(gccs)
 
 
-def get_gcc(file, outdir, gfasta, binsize, **kwargs):
-    import matplotlib.pyplot as plt
-    from pandas import concat
-    
-    if app := kwargs.get("app", "auto") == "auto":
-        app = ul.detect_file_info(file)["app"]
-
-    kwargs = {
-             "split": True,
-             "excludeSS": not kwargs["includess"],
-             "exon_width": kwargs["exonflank"],
-             "intron_width": kwargs["intronflank"]
-             }
+def get_gcc(coor_dic, outdir, gfasta, binsize):
     outdir = Path(outdir)
     Path(outdir).mkdir(exist_ok=True)
-    coord_dic = ul.get_ss_bed(file, app=app, **kwargs)
+
     df_ls = []
-    fig, axes = plt.subplots(1, len(coord_dic), figsize= (10, 5))
-    for idx, (ssn, (df_up, df_dw)) in enumerate(coord_dic.items()):
+    fig, axes = plt.subplots(1, len(coor_dic), figsize= (10, 5))
+    for idx, (ssn, (df_up, df_dw)) in enumerate(coor_dic.items()):
         ss_dir = outdir / ssn
         ss_dir.mkdir(exist_ok=True)
         ul.get_coor_fa(df_up, gfasta, ss_dir / f"{ssn}_ups.fa", strandedness=True)
         ul.get_coor_fa(df_dw, gfasta, ss_dir / f"{ssn}_dws.fa", strandedness=True)
 
         df_up.to_csv(ss_dir / f"{ssn}_ups.bed", index=False, header=False, sep="\t")
         df_dw.to_csv(ss_dir / f"{ssn}_dws.bed", index=False, header=False, sep="\t")
@@ -72,39 +63,41 @@
         elif "3SS" in ssn:
             if binsize == 0:
                 ups_gcc.columns = [f"{ssn}_intron"]
                 dws_gcc.columns = [f"{ssn}_exon"]
             else:
                 ups_gcc.columns = [f"{ssn}_intron_b{i}" for i in range(-ups_gcc.shape[1], 0)]
                 dws_gcc.columns = [f"{ssn}_exon_b{i}" for i in range(dws_gcc.shape[1])]
-        df = concat([ups_gcc, dws_gcc], axis=1)
+        df = pd.concat([ups_gcc, dws_gcc], axis=1)
+        # df.index = df_up.iloc[:, 3]
+        df.index = df_up.index
         gcc_mean = df.mean()
         gcc_mean.index = range(-ups_gcc.shape[1], dws_gcc.shape[1])
         axes[idx].plot(gcc_mean)
         axes[idx].set_ylim([min(0.35, min(gcc_mean)), max(0.65, max(gcc_mean))])
         df_ls.append(df)
-    dfs = df = concat(df_ls, axis=1)
+    dfs = pd.concat(df_ls, axis=1)
     dfs.to_csv(outdir / "gcc.csv")
     plt.tight_layout()
     plt.savefig(outdir / "gcc.png")
 
 
-def get_elen(file, outdir, app, log):
-    import matplotlib.pyplot as plt
-    import numpy as np
-
+def get_elen(file, outdir, scale, mode, app):
     outdir = Path(outdir)
     Path(outdir).mkdir(exist_ok=True)
-
-    df_len = ul.get_ss_range(file, app)
+    df_len = ul.get_all_ss_distance(file, mode, app)
+    ylabel = "length"
+    if scale == "log":
+        ylabel = "log2(length)"
+        df_len = np.log2(df_len)
+    elif scale == "MinMaxScaler":
+        from sklearn.preprocessing import MinMaxScaler
+        df_len.iloc[:] = MinMaxScaler().fit_transform(np.log2(df_len))
+        ylabel = "scale(length)"
     df_len.to_csv(outdir / "element_len.csv")
-    ylabel = "log2(length)" if log else "length"
     fig, axes = plt.subplots(1, df_len.shape[1], sharey=True)
     for idx in range(df_len.shape[1]):
-        if log:
-            data = np.log2(df_len.iloc[:, idx])
-        else:
-            data = df_len.iloc[:, idx]
+        data = df_len.iloc[:, idx]
         axes[idx].boxplot(data)
         axes[idx].set_ylabel(ylabel)
-    plt.tight_layout() 
+    plt.tight_layout()
     plt.savefig(outdir / "element_len.png")
```

### Comparing `astk-0.1.2/astk/seqfeature/_splice_score.py` & `astk-0.1.2b0/astk/seqfeature/_splice_score.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import json
 from math import log2
 from pathlib import Path
 import multiprocessing as mp
 
 from astk.constant import BASE_DIR
 from astk.utils._getfasta import get_coor_fa
-from astk.utils import get_ss_bed, read_fasta, detect_file_info
+from astk.utils import read_fasta
 
 
 def ss5_consensus_score(seq):
     bdg = {"A": 0.27, "C": 0.23, "G": 0.23, "T": 0.27}
     cons1 = {'A': 0.004, 'C': 0.0032, 'G': 0.9896, 'T': 0.0032}
     cons2 = {'A': 0.0034, 'C': 0.0039, 'G': 0.0042, 'T': 0.9884}
-    addscore = cons1[seq[3]] * cons2[seq[4]] /( bdg[seq[3]] * bdg[seq[4]])
-    return addscore
+    return cons1[seq[3]] * cons2[seq[4]] /( bdg[seq[3]] * bdg[seq[4]])
 
 
 def ss5_score(seq):
     ss5_score_json = BASE_DIR / "data/maxent/ss5seq_score.json"
     with open(ss5_score_json, "r") as f:
-        ss5_score_dic = json.load(f)    
+        ss5_score_dic = json.load(f)
     seq = seq.upper()[:9]
-    score = log2(ss5_consensus_score(seq) * ss5_score_dic.get(seq[:3]+seq[5:], 1e-12))
-    return score
+    return log2(
+        ss5_consensus_score(seq) * ss5_score_dic.get(seq[:3] + seq[5:], 1e-12)
+    )
 
 
 def ss5_seqs_score(fasta, process=4):
     with open(fasta, "r") as rh:
         seqs = read_fasta(rh)
         pool = mp.Pool(process)
         scores = [pool.apply(ss5_score, args=(seq[1],)) for seq in seqs]
@@ -47,72 +47,65 @@
         num += seqn[seq[i]] * four[slen-i-1]
     return num
 
 
 def ss3_consensus_score(seq):
     bdg = {"A": 0.27, "C": 0.23, "G": 0.23, "T": 0.27}
     cons1 = {'A': 0.9903, 'C': 0.0032, 'G': 0.0034, 'T': 0.0030}
-    cons2 = {'A': 0.0027, 'C': 0.0037, 'G': 0.9905, 'T': 0.0030}    
-    addscore = cons1[seq[18]] * cons2[seq[19]]/ (bdg[seq[18]] * bdg[seq[19]]) 
-    return addscore
+    cons2 = {'A': 0.0027, 'C': 0.0037, 'G': 0.9905, 'T': 0.0030}
+    return cons1[seq[18]] * cons2[seq[19]]/ (bdg[seq[18]] * bdg[seq[19]])
 
 
 def ss3_maxentscore(seq):
     ss3_score_json = BASE_DIR / "data/maxent/ss3_score.json"
     with open(ss3_score_json, "r") as f:
         ss3_score_dic = json.load(f)
     sc = [0] * 9
-    sc[0] = ss3_score_dic['0'][hashseq(seq[0:7])]
+    sc[0] = ss3_score_dic['0'][hashseq(seq[:7])]
     sc[1] = ss3_score_dic['1'][hashseq(seq[7:7+7])]
     sc[2] = ss3_score_dic['2'][hashseq(seq[14:14+7])]
     sc[3] = ss3_score_dic['3'][hashseq(seq[4:4+7])]
     sc[4] = ss3_score_dic['4'][hashseq(seq[11:11+7])]
     sc[5] = ss3_score_dic['5'][hashseq(seq[4:4+3])]
     sc[6] = ss3_score_dic['6'][hashseq(seq[7:7+4])]
     sc[7] = ss3_score_dic['7'][hashseq(seq[11:11+3])]
     sc[8] = ss3_score_dic['8'][hashseq(seq[14:14+4])]
-    finalscore = sc[0]*sc[1]*sc[2]*sc[3]*sc[4]/(sc[5]*sc[6]*sc[7]*sc[8])
-    return finalscore
+    return sc[0]*sc[1]*sc[2]*sc[3]*sc[4]/(sc[5]*sc[6]*sc[7]*sc[8])
 
 
 def ss3_score(seq):
     seq = seq.upper()[:23]
-    score = log2(ss3_consensus_score(seq) * ss3_maxentscore(seq[:18]+seq[20:]))
-    return score
+    return log2(ss3_consensus_score(seq) * ss3_maxentscore(seq[:18]+seq[20:]))
 
 
 def ss3_seqs_score(fasta, process=4):
     with open(fasta, "r") as rh:
         seqs = read_fasta(rh)
         # scores = [ss3_score(seq[1]) for seq in seqs]
         pool = mp.Pool(process)
         scores = [pool.apply(ss3_score, args=(seq[1],)) for seq in seqs]
         pool.close()
     return scores     
 
 
-def splice_score(file, outdir, gfasta, app, process):
+def splice_score(coor_dic, outdir, gfasta, process):
     from pandas import DataFrame
 
-    if app == "auto":
-        app = detect_file_info(file)["app"]
-
     outdir = Path(outdir)
     Path(outdir).mkdir(exist_ok=True)
-    coord_dic = get_ss_bed(file, sss=True, app=app)
-
     df_score = DataFrame()
-    for idx, (ssn, df) in enumerate(coord_dic.items()):
+    for ssn, df in coor_dic.items():
         ss_dir = outdir / ssn
         ss_dir.mkdir(exist_ok=True)
         get_coor_fa(df, gfasta, ss_dir / f"{ssn}.fa", strandedness=True)
         df.to_csv(ss_dir / f"{ssn}.bed", index=False, header=False, sep="\t")
         if ssn.endswith("5SS"):
             df_score[ssn] = ss5_seqs_score(ss_dir / f"{ssn}.fa", process)
         elif ssn.endswith("3SS"):
             df_score[ssn] = ss3_seqs_score(ss_dir / f"{ssn}.fa", process)
 
-    df_score.index = df.iloc[:, 3]
+    # df_score.index = df.iloc[:, 3]
+    df_score.index = df.index
     df_score.to_csv(outdir / "splice_scores.csv")
     ax = df_score.plot.box()
     fig = ax.get_figure()
     fig.savefig(outdir / "splice_scores_box.png")
```

### Comparing `astk-0.1.2/astk/seqfeature/feature.py` & `astk-0.1.2b0/astk/seqfeature/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,24 @@
     :param count:
     :return:
     """
     NT = ["A", "T", "G", "C"]
     def three_f(idx, k, gap, lam, seq_dic):
         a = (seq_dic.get(idx+idx*gap+(lam+1)*i, '') for i in range(k))
         return ''.join(a)
-    seq_dic = {i: v for i,v in enumerate(seq)}
+
+    seq_dic = dict(enumerate(seq))
     nt = [''.join(n) for n in product(NT, repeat=k)]
     f3 = partial(three_f, gap=gap, k=k, lam=lam, seq_dic=seq_dic)
     nt_list = [f3(i) for i in range(len(seq))]
     nt_list = [i for i in nt_list if len(i) ==k]
     nt_dict = Counter(nt_list)
     all_count = len(nt_list)
     if count:
-        all_count = 1 
+        all_count = 1
     nt_fre = [nt_dict[i] / all_count for i in nt]
     return nt_fre
 
 
 def read_fasta(seq):
     seq_ls = []
     for line in seq:
@@ -79,15 +80,15 @@
                 featuremerge: bool
     ):
     iscount = count
     k, gap, lam = kmer, gap, lambda_
 
     xy_ls = []
     # aa_ls = [''.join(aa) for aa in product(raa, repeat=k)]
-    for idx, file in enumerate(fasta):
+    for file in fasta:
         feature_file = Path(file)
         xy = extract_feature(feature_file, k, gap, lam, count=iscount)
         # new_aa_ls = aa_ls
 
         xy_ls.append(xy)
     # new_aa_ls.insert(0, 'label') if args.label_f else 0
     # header = ','.join(new_aa_ls)
```

### Comparing `astk-0.1.2/astk/suppa/AS_event.py` & `astk-0.1.2b0/astk/suppa/AS_event.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/suppa/_func.py` & `astk-0.1.2b0/astk/suppa/_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import hashlib
 import sys
 import json
 from pathlib import Path
 
-from astk.types import *
+from astk.ctypes import *
 import astk.utils.select as sl
 from .AS_event import make_events
 from .event_psi import get_ioe_psi
 from .gtf_parse import construct_genome
 from astk.suppa.lib.diff_tools import multiple_conditions_analysis as mca
+from astk.lazy_loader import LazyLoader
+
+pd = LazyLoader("pd", globals(), "pandas")
 
 
 def check_gtf_used(gtf):
     gtf = Path(gtf)
     gtf_hash = hashlib.blake2b()
     gtf_size = gtf.stat().st_size
     gtf_hash.update(str(gtf_size).encode('utf-8'))
-    f = gtf.open("rb")
+    f = gtf.open("rb") 
     for _ in range(10):
         gtf_hash.update(f.readline().strip())
-    hash_val = gtf_hash.hexdigest()
-    return hash_val
+    return gtf_hash.hexdigest()
 
 
 def gtf_parse_cache(gtf):
     home = Path.home()
-    astk_cache_dir = home / f".astk"
+    astk_cache_dir = home / ".astk"
     astk_cache_dir.mkdir(exist_ok=True)
     gtf_hash = check_gtf_used(gtf)
     gtf_cache_path = astk_cache_dir / "gtfParse"
     gtf_cache_path.mkdir(exist_ok=True)
-    pkl = (gtf_cache_path / gtf_hash).with_suffix(".pkl")
-    return pkl
+    return (gtf_cache_path / gtf_hash).with_suffix(".pkl")
 
 
 def generate_events(gtf, event_types, output, idtype, event_pos):
     genome = construct_genome(gtf)
     if event_types == "ALL":
         event_types =  ['SE', "A5", "A3", "MX", "RI", 'AF', 'AL']
     else:
@@ -52,42 +53,37 @@
 ):
     if str(output).endswith(".dpsi"):
         output = str(output)[:-5]
     mca(method, psi_files, exp_files, reference, 1000, 0, 
         False, True, 0.05, True, False, False, 0, 0, str(output))                 
 
 
-def read_tpm(file, colname, tpm_col):
-    import pandas as pd
-
+def read_tpm(file, colname="sample", tpm_col=4):
     quant_df = pd.read_csv(file, sep = "\t")
     tpm_df = pd.DataFrame({colname: quant_df.iloc[:, tpm_col-1]})
     tpm_df.index = quant_df.iloc[:, 0]
     return tpm_df
 
 
 def calculate_psi(ioe, tpm_files, tpm_th, tpm_col, tx_col):
-    import pandas as pd
     ioe_df = pd.read_csv(ioe, sep="\t")
-
     psi_dic = {}
     tpm_ls = []
     for tf in tpm_files:
         sf_name = Path(tf).parent.name  # only consider salmon output, now
         tpm_df = read_tpm(tf, sf_name, tpm_col)
         psi_dic[sf_name] = get_ioe_psi(ioe_df, tpm_df, tpm_th=tpm_th)
         tpm_ls.append(tpm_df)
     tpm_df = pd.concat(tpm_ls, axis=1)
     psi_df = pd.DataFrame(psi_dic)
     psi_df.index = ioe_df["event_id"]
     return psi_df, tpm_df
 
 
 def parse_meta(meta_file: FilePath) -> Dict:
-
     tpm_dic = {}
     with open(meta_file, "r") as f:
         try:
             meta_dic = json.load(f)
         except json.decoder.JSONDecodeError:
             print("ERROR: JSON file is excepted!")
             sys.exit()
@@ -104,51 +100,47 @@
     etypes: Sequence[str],
     outdir: FilePath, 
     method: str,
     id_type: str,
     pval: float,
     abs_dpsi: float,
     tpm_threshold: float,
-    event_pos: str
+    event_pos: str,
+    tpm_col: int
     ):
-    import pandas as pd
-
     Path(outdir).mkdir(exist_ok=True)
     tpm_dic = parse_meta(meta)
     genome = construct_genome(gtf)
     ref_dir = Path(outdir) / "ref"
     ref_dir.mkdir(exist_ok=True)
     make_events(ref_dir / "annotation", genome, etypes, id_type, event_pos)
-    
+
     tpm_dir =  Path(outdir) / "tpm"
     psi_dir =  Path(outdir) / "psi"
     dpsi_dir =  Path(outdir) / "dpsi"
     sig_dir =  Path(outdir) / ("sig" + str(abs_dpsi).replace(".", ''))
     tpm_dir.mkdir(exist_ok=True)
     psi_dir.mkdir(exist_ok=True)
     dpsi_dir.mkdir(exist_ok=True)
     sig_dir.mkdir(exist_ok=True)
     sig_psi_dir = sig_dir / "psi"
     sig_psi_dir.mkdir(exist_ok=True)
 
     for gn, gn_dic in tpm_dic.items():
         for et in etypes:
-            if event_pos is None:
-                es = ""
-            else:
-                es = f"_{event_pos}"
+            es = "" if event_pos is None else f"_{event_pos}"
             ioe = ref_dir / f"annotation{es}_{et}_strict.ioe"
             ioe_df = pd.read_csv(ioe, sep="\t")
             ctrl_tpm_ls = []
             case_tpm_ls = []
             ctrl_psi_ls = []
             case_psi_ls = []
             for (cf, cn), (tf, tn) in zip(gn_dic["ctrl"], gn_dic["case"]):
-                cdf = read_tpm(cf, cn, 4)
-                tdf = read_tpm(tf, tn, 4)
+                cdf = read_tpm(cf, cn, tpm_col)
+                tdf = read_tpm(tf, tn, tpm_col)
                 ctrl_tpm_ls.append(cdf)
                 case_tpm_ls.append(tdf)
 
                 cpsi_df = pd.DataFrame(get_ioe_psi(ioe_df, cdf, tpm_th=tpm_threshold), 
                         columns=cdf.columns, index=ioe_df["event_id"])
                 tpsi_df = pd.DataFrame(get_ioe_psi(ioe_df, tdf, tpm_th=tpm_threshold), 
                         columns=tdf.columns, index=ioe_df["event_id"])
@@ -169,28 +161,27 @@
             ctrl_psi.to_csv(ctrl_psi_file, sep="\t")
             case_psi.to_csv(case_psi_file, sep="\t")
             psi_files = [ctrl_psi_file, case_psi_file]
             exp_files = [ctrl_tpm_file, case_tpm_file]
             dpsi_out = dpsi_dir / f"{gn}_{et}"
             mca(method, psi_files, exp_files, ioe, 1000, 0, 
                 False, True, 0.05, True, False, False, tpm_threshold, 0, str(dpsi_out))
-            
             sig_dpsi_out = (sig_dir / dpsi_out.name).with_suffix(".sig.dpsi")
             sig_pos_dpsi_out = (sig_dir / dpsi_out.name).with_suffix(".sig+.dpsi")
             sig_neg_dpsi_out = (sig_dir / dpsi_out.name).with_suffix(".sig-.dpsi")
             kwargs = {"abs_dpsi": abs_dpsi, "pval": pval, "app": "SUPPA2"}
             dpsi_df = pd.read_csv(dpsi_out.with_suffix(".dpsi"), sep="\t", index_col=0).dropna()
             old_col = dpsi_df.columns
             dpsi_df.columns = ["dpsi", "pval"]
             df_fil = sl.sig_filter(dpsi_df, **kwargs)
-            df_fil.columns = old_col      
+            df_fil.columns = old_col
             df_fil.to_csv(sig_dpsi_out, sep="\t")
 
             pos_df = df_fil.loc[df_fil[old_col[0]] > 0, ]
             neg_df = df_fil.loc[df_fil[old_col[0]] < 0, ]
             pos_df.to_csv(sig_pos_dpsi_out, sep="\t")
             neg_df.to_csv(sig_neg_dpsi_out, sep="\t")
 
             ctrl_psi_file = sig_psi_dir / f"{gn}_{et}_c1.sig.psi"
             case_psi_file = sig_psi_dir / f"{gn}_{et}_c2.sig.psi"
-            ctrl_psi.loc[df_fil.index, ].to_csv(ctrl_psi_file, sep="\t")
-            case_psi.loc[df_fil.index, ].to_csv(case_psi_file, sep="\t")
+            ctrl_psi.loc[df_fil.index, ].to_csv(ctrl_psi_file, sep="\t", index_label=False)
+            case_psi.loc[df_fil.index, ].to_csv(case_psi_file, sep="\t", index_label=False)
```

### Comparing `astk-0.1.2/astk/suppa/event_psi.py` & `astk-0.1.2b0/astk/suppa/event_psi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 
 
 def cal_psi(alter_tx, total_tx, tpm_df, tpm_th=1):
     alter_tx = [i for i in alter_tx if i in tpm_df.index]
     total_tx = [i for i in total_tx if i in tpm_df.index]
-    if len(total_tx) == 0 or len(alter_tx) == 0:
+    if not total_tx or not alter_tx:
         psi = "nan"
     else:
-        alter_tx_tpm = sum([tpm_df.at[i, tpm_df.columns[0]] for i in alter_tx])
+        alter_tx_tpm = sum(tpm_df.at[i, tpm_df.columns[0]] for i in alter_tx)
         total_tx_tpms = [tpm_df.at[i, tpm_df.columns[0]] for i in total_tx]
         if sum(total_tx_tpms) / len(total_tx_tpms) < tpm_th:
             psi = "nan"
         elif alter_tx_tpm <= 0.0001:
             psi = 0
         else:
             try:
@@ -22,16 +22,15 @@
 
 
 def ioe_df_row(row, tpm_df, tpm_th):
     """Get the PSI value of the event for the row in the ioe df
     """
     alternative_txs = row["alternative_transcripts"].split(",")
     total_txs = row["total_transcripts"].split(",")
-    psi = cal_psi(alternative_txs, total_txs, tpm_df, tpm_th=tpm_th)
-    return psi
+    return cal_psi(alternative_txs, total_txs, tpm_df, tpm_th=tpm_th)
 
 
 def get_ioe_psi(ioe_df, tpm_df, tpm_th=1):
     """Get the PSI value of the event for each row in the ioe df
     """
     psi_ls = ioe_df.apply(ioe_df_row, axis=1, args=(tpm_df, tpm_th))
     return psi_ls.tolist()
```

### Comparing `astk-0.1.2/astk/suppa/gtf_parse.py` & `astk-0.1.2b0/astk/suppa/gtf_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,24 +93,24 @@
 Exon = namedtuple('Exon',('id, chr, start, end, strand, attr'))
 
 
 def parse_gtf_line(line, feature=["gene", "exon", "transcript"]):
     line = line.strip().split('\t')
     if len(line) != 9:
         print('Missmatch in number of Fields. skipping line')
-        return 
+        return
     if line[2] not in feature:
-        return   
-    info_dic = {k:v for k, v in zip(GTF_COLUMNS[:8], line[:8])}
+        return
+    info_dic = dict(zip(GTF_COLUMNS[:8], line[:8]))
     attributes_str = line[-1][:-1].replace('"', "")
     att_dic = {}
     for att in attributes_str.split('; '):
         k, *v = att.split()
         att_dic[k] = " ".join(v)
-    info_dic.update(att_dic)
+    info_dic |= att_dic
     return info_dic
 
 
 def construct_genome(gtf):
     from tqdm import tqdm
 
     genome = Genome()
```

### Comparing `astk-0.1.2/astk/suppa/lib/diff_tools.py` & `astk-0.1.2b0/astk/suppa/lib/diff_tools.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/suppa/lib/event.py` & `astk-0.1.2b0/astk/suppa/lib/event.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/suppa/lib/gtf_store.py` & `astk-0.1.2b0/astk/suppa/lib/gtf_store.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/suppa/lib/optics.py` & `astk-0.1.2b0/astk/suppa/lib/optics.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/suppa/lib/tools.py` & `astk-0.1.2b0/astk/suppa/lib/tools.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/suppa/lib/var_event.py` & `astk-0.1.2b0/astk/suppa/lib/var_event.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.2/astk/utils/_cli_func.py` & `astk-0.1.2b0/astk/utils/_cli_func.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import os
 import sys
 import shutil
 import subprocess
 from pathlib import Path
-from typing import Sequence, Union, Tuple
+from typing import Sequence
 
-
-import astk.ChromHMM as ch
 from astk.constant import *
 from . import func as ulf
 from astk.utils.meta_template import Template
 
 
-def meta(output, replicate, groupname, ctrl, case, replicate1, replicate2, **kwargs):
-
-    if not (pdir:= Path(output).parent).exists():
-        print(f"{pdir} doest not exist")
-        exit() 
-    if replicate:
-        repN1 = [int(i) for i in replicate]
-        repN2 = [int(i) for i in replicate]
-    elif all([replicate1, replicate1]):
-        repN1 = [int(i) for i in replicate1]
-        repN2 = [int(i) for i in replicate2]
-    else:
-        print("repN1 and repN2 must be set!")    
-        sys.exit()
+def meta(
+    output: str,
+    ctrl_file: Sequence[str], 
+    case_file: Sequence[str], 
+    ctrl_rep: Sequence[int], 
+    case_rep: Sequence[int], 
+    groupname: Sequence[str], 
+    **kwargs
+):
+    app = kwargs.pop("app")
     try:
         tp = Template(kwargs.pop("condition", None))
-        tp.complete_df(groupname, ctrl, case, repN1, repN2, **kwargs)
-        tp.to_csv(output)
-        tp.to_json(output)
+        tp.complete_df(groupname, ctrl_file, case_file, ctrl_rep, case_rep, **kwargs)
     except BaseException as e:
         print(e)
+        sys.exit()
+
+    if app == "SUPPA2":        
+        tp.to_csv(output)
+        tp.to_json(output)
+    elif app == "rMATS":
+        for gn, gdf in tp.df.groupby("group"):
+            for cn, cdf in gdf.groupby("condition"):
+                path_str = ",".join(cdf["path"].tolist())
+                out = Path(output).with_suffix(f".{gn}.{cn}.txt")
+                with open(out, "w") as f:
+                    f.write(path_str)
 
 
 def install(requirement, OrgDb, cran, bioconductor, java, mirror, conda):
 
     pdir = BASE_DIR
     rscript = pdir / "R" / "install.R"
     if conda:
@@ -48,18 +52,18 @@
             os.system(f"conda install -y -c bioconda {bioc_pkg}")
     if java:
         print("install ChromHMM")
         ch.install(pdir)
         shutil.copyfile(pdir/"ChromHMM.jar", pdir/"ChromHMM/ChromHMM.jar")
     param_dic = {
         "requirement": requirement,
-        "OrgDb": OrgDb if OrgDb else False,
-        "CRAN": cran if cran else False, 
-        "bioconductor": bioconductor if bioconductor else False, 
-        "mirror": mirror
+        "OrgDb": OrgDb or False,
+        "CRAN": cran or False,
+        "bioconductor": bioconductor or False,
+        "mirror": mirror,
     }
     param_ls = ulf.parse_cmd_r(**param_dic)
     subprocess.run([ulf.Rscript_bin(), rscript, *param_ls])
 
 
 def getmeme(motifid, meme, database, organism, output):
 
@@ -90,42 +94,14 @@
 def anchor(file, output, index, sideindex, offset5, offset3, strand_sp):
     try:
         ulf.gen_anchor_bed(file, output, index, sideindex, offset5, offset3, strand_sp)
     except BaseException as e:
         print(e)
  
 
-def getcoor(
-    file: Union[str, Path],
-    output: Union[str, Path],
-    anchor: Sequence[int], 
-    upstream_w: int, 
-    downstream_w: int, 
-    interval: Tuple[int, int],
-    strand_sp: bool,
-    fasta: Union[str, Path]
-    ):
-    start, end = interval
-    if not any([start, end, anchor]):
-        etype = ulf.sniff_AS_type(file)
-        anchors = list(range(1, SSN[etype]+1))
-    else:
-        anchors = anchor
-
-    for  a in anchors:
-        try:
-            coor_df = ulf.get_coor_bed(file, start, end, strand_sp, a, upstream_w, downstream_w)
-            out_bed = Path(output).with_suffix(f".a{a}.bed")
-            coor_df.to_csv(out_bed, index=False, header=False, sep="\t")
-            if fasta:
-                ulf.get_coor_fa(coor_df, fasta, Path(output).with_suffix(f".a{a}.fa"))
-        except BaseException as e:
-            print(e)
-
-
 def mkTxDb(gtf, organism, output):
     sp = RBP_sp_dic.get(organism, None)
     sp = sp.replace("_", " ")
     rscript = BASE_DIR / "R" / "makeTxDb.R"
     if not output:
         output = Path(gtf).with_suffix(".txdb")
     param_dic = {
```

### Comparing `astk-0.1.2/astk/utils/_coord.py` & `astk-0.1.2b0/astk/utils/_coord.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from astk.event import SuppaEventID
-from astk.constant import SS_SCORE_LEN, rMATS_POS_COLS
-from astk.types import FilePath
+from astk.constant import SS_SCORE_LEN, rMATS_POS_COLS, ALT_IDX
+from astk.ctypes import *
 from astk.utils import detect_file_info
+from astk.lazy_loader import LazyLoader
+
+pd = LazyLoader("pd", globals(), "pandas")
 
 
 class EventCoord:
 
     def __init__(self, file) -> None:
         self.set_metadata(file)
 
@@ -63,21 +66,28 @@
     def get_all_flank_bed(
         self,
         ups_w: int = 150,
         dws_w: int = 150,
         sss: bool = False,
         based0 = True,
         **kwargs
-    ):  
+    ):
         """get all splice site flank coordination bed and return a dict
         """
         dic = {}
         slens = SS_SCORE_LEN[self.app][self.etype]
         site_dic = {23: "3SS", 9: "5SS", -23: "pse_3SS", -9: "pse_5SS"}
+        sites = kwargs.get("ss_idx", False)
+        if not sites:
+            sites = list(range(len(slens)))
+        if kwargs.get("altidx", False):
+            sites = ALT_IDX[self.app][self.etype]
         for idx, slen in enumerate(slens):
+            if idx not in sites:
+                continue
             sn = site_dic[slen]
             key = f"A{idx+1}_{sn}"
             dic[key] = self.get_ss_flank_bed(idx, ups_w, dws_w, sss, based0, **kwargs)
         return dic
 
     def _5ss_width(self, ups_w, dws_w, exon_w, intron_w, sss):
         if exon_w and intron_w:
@@ -98,92 +108,79 @@
             ups_w, dws_w = self._3ss_width(ups_w, dws_w, exon_w, intron_w, sss)
         elif abs(site) == 9:
             ups_w, dws_w = self._5ss_width(ups_w, dws_w, exon_w, intron_w, sss)
         return ups_w, dws_w
     
     def _exclude_region(self, site, **kwargs):
         if kwargs.get("excludeSS", False):
-            if site == 23:
+            if abs(site) == 23:
                 ex_ups_w, ex_dws_w = 20, 3
-            elif site == 9:
+            elif abs(site) == 9:
                 ex_ups_w, ex_dws_w = 3, 6
-            else:
-                ex_ups_w, ex_dws_w = 0, 0
         else:
             ex_ups_w, ex_dws_w = 0, 0
         return ex_ups_w, ex_dws_w
     
-    def _ns_adaptor(self):
-        pass
-
     def set_metadata(self, file):
         pass
 
 
 class SuppaEventCoord(EventCoord):
 
     def __init__(self, file) -> None:
         super().__init__(file)
 
     def set_metadata(self, file):
-        from pandas import DataFrame, read_csv
-
         fileinfo = detect_file_info(file)
         self.etype = fileinfo["etype"]
         self.app = fileinfo["app"]
 
-        dpsi_df = read_csv(file, sep="\t", index_col=0)
+        dpsi_df = pd.read_csv(file, sep="\t", index_col=0)
+        dpsi_df["event_id"] = dpsi_df.index
         dpsi_df.drop_duplicates(inplace=True)
         dpsi_df.dropna(inplace=True)
-        dpsi_df["event_id"] = dpsi_df.index
 
         def _get_coor(event_id):
             ei = SuppaEventID(event_id)
-            if ei.strand == "-":
-                coords = reversed(ei.coordinates)
-            else:
-                coords = ei.coordinates
-            row = ei.Chr, ei.event_id, ei.strand, *coords
-            return row
-        event_df = DataFrame(dpsi_df["event_id"].apply(_get_coor).tolist(),
-                             index=dpsi_df.index)
+            coords = reversed(ei.coordinates) if ei.strand == "-" else ei.coordinates
+            return  pd.Series((ei.Chr, ei.event_id, ei.strand, *coords))
+        
+        event_df = dpsi_df["event_id"].apply(_get_coor)
         self.df_ss = event_df.iloc[:, 3:]
         self.df_ss.columns = range(self.df_ss.shape[1])
         self.ps_idx = event_df.loc[event_df.iloc[:, 2] == "+", ].index
         self.ns_idx = event_df.loc[event_df.iloc[:, 2] == "-", ].index
 
         cols = ["seqname", "start", "end", "name", "score", "strand"]
-        df_temp = DataFrame(columns=cols, index=dpsi_df.index)
+        df_temp = pd.DataFrame(columns=cols, index=dpsi_df.index)
         df_temp["seqname"] = event_df[0]
         df_temp["strand"] = event_df[2]
         df_temp["score"] = 0
         df_temp["name"] = event_df[1]
         self.df_temp = df_temp
 
         
 class rMATSEventCoord(EventCoord):
 
     def __init__(self, file) -> None:
         super().__init__(file)
 
     def set_metadata(self, file):
-        from pandas import DataFrame, read_csv, concat
-
-        dpsi_df = read_csv(file, sep="\t", index_col=0)
+        dpsi_df = pd.read_csv(file, sep="\t", index_col=0)
         dpsi_df.drop_duplicates(inplace=True)
         dpsi_df.dropna(inplace=True)
         fileinfo = detect_file_info(file)
         self.etype = fileinfo["etype"]
         self.app = fileinfo["app"]
 
         self.ps_idx = dpsi_df.loc[dpsi_df["strand"] == "+", ].index
         self.ns_idx = dpsi_df.loc[dpsi_df["strand"] == "-", ].index
 
         cols = ["seqname", "start", "end", "name", "score", "strand"]
-        df_temp = DataFrame(columns=cols, index=dpsi_df.index)
+        df_temp = pd.DataFrame(columns=cols, index=dpsi_df.index)
         df_temp["seqname"] = dpsi_df["chr"]
         df_temp["strand"] = dpsi_df["strand"]
         df_temp["score"] = 0
         df_temp["name"] = dpsi_df["geneSymbol"]
         self.df_temp = df_temp
 
         # tansform 1-based index for unified management
@@ -197,15 +194,15 @@
             start_col = ["upstreamES", "downstreamES"]
         dpsi_df.loc[:, start_col] += 1
 
         ps_df = dpsi_df.loc[self.ps_idx, rMATS_POS_COLS[self.etype]["+"]]
         ns_df = dpsi_df.loc[self.ns_idx, rMATS_POS_COLS[self.etype]["-"]]
         ps_df.columns = range(len(rMATS_POS_COLS[self.etype]["+"]))
         ns_df.columns = range(len(rMATS_POS_COLS[self.etype]["-"]))
-        self.df_ss = concat([ps_df, ns_df]).loc[dpsi_df.index, :]
+        self.df_ss = pd.concat([ps_df, ns_df]).loc[dpsi_df.index, :]
 
 
 def get_event_coord(event, app):
     if app == "auto":
         app = detect_file_info(event)["app"]
     if app == "SUPPA2":
         coori = SuppaEventCoord(event)
@@ -214,27 +211,60 @@
     return coori
 
 
 def get_ss_bed(
     event_file: FilePath, 
     ups_width: int = 150, 
     dws_width: int = 150,
-    strand_sp: bool = False,
     sss: bool = False,
     app: str = "auto",
     **kwargs
-    ):
+) -> Dict:
+    if app == "auto":
+        app = detect_file_info(event_file)["app"]
     coori = get_event_coord(event_file, app)
-    df_dic = coori.get_all_flank_bed(ups_w=ups_width,dws_w=dws_width,sss=sss, **kwargs)
-    return df_dic
+    return coori.get_all_flank_bed(
+        ups_w=ups_width, dws_w=dws_width, sss=sss, **kwargs
+    )
 
 
-def get_ss_range(event_file, app):
-    from pandas import DataFrame
-    
+def get_all_ss_distance(event_file, mode, app):
+    einfo = detect_file_info(event_file)
+    app, etype = einfo["app"], einfo["etype"]
     coori = get_event_coord(event_file, app)
     df_ss = coori.df_ss
     ncol = df_ss.shape[1] - 1
-    df_len = DataFrame(index=df_ss.index, columns=range(ncol))
-    for idx in range(ncol):
-        df_len.iloc[:, idx] = abs(df_ss.iloc[:, idx+1] - df_ss.iloc[:, idx])
+    df_len = pd.DataFrame(index=df_ss.index)
+    if mode == "junction" and etype in ("MX", "MXE"):
+        if app == "SUPPA2":
+            cols1 = [0, 1, 2, 5]
+            cols2 = [0, 3, 4, 5]
+        elif app == "rMATS":
+            cols1 = [0, 1, 2, 3, 6, 7]
+            cols2 = [1, 4, 5, 6]
+        for i in range(len(cols1)-1):   
+            df_len[i] = abs(df_ss.iloc[:, cols1[i+1]] - df_ss.iloc[:, cols1[i]])
+        for i in range(len(cols2)-1):
+            df_len[len(cols1)+i] = abs(df_ss.iloc[:, cols2[i+1]] - df_ss.iloc[:, cols2[i]])
+    else:
+        for idx in range(ncol):
+            df_len[idx] = abs(df_ss.iloc[:, idx+1] - df_ss.iloc[:, idx])
     return df_len
+
+
+def get_ss_range(
+    event_file: FilePath,
+    start: int,
+    end: int,
+    app: str = "auto",
+    **kwargs
+):
+    coori = get_event_coord(event_file, app)
+    df_ss = coori.df_ss
+    coord = sorted([start, end])
+    df = coori.df_temp
+    ps_df = df_ss.loc[coori.ps_idx, coord]
+    ns_df = df_ss.loc[coori.ns_idx, reversed(coord)]
+    df.loc[coori.ps_idx, ["start", "end"]] = ps_df.values
+    df.loc[coori.ns_idx, ["start", "end"]] = ns_df.values
+    df["start"] -= 1
+    return df
```

### Comparing `astk-0.1.2/astk/utils/func.py` & `astk-0.1.2b0/astk/utils/func.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import sys
 import mmap
 import json
 from pathlib import Path
 from functools import partial
 
-from astk.types import FilePath
+from astk.ctypes import FilePath
 from astk.event import SuppaEventID
+from astk.lazy_loader import LazyLoader
 from astk.constant import OrgDb_dic, BASE_DIR, SSN, RBP_sp_dic
 
 
+np = LazyLoader("np", globals(), "numpy")
+pd = LazyLoader("pd", globals(), "pandas")
+
+
 class RunConfigure:
     def __init__(self) -> None:
         self.path = Path.home() / ".astkrc"
         self.rc_dic = self.read()
     
     def read(self, path=None):
         if path is None:
@@ -53,25 +58,21 @@
     if abs_dpsi > 0:
         keep = (abs(dpsi_df.loc[:, "dpsi"]) > abs_dpsi) & keep
     fdf = dpsi_df.loc[keep, ]
     return fdf
 
 
 def compute_feature_len(df):
-    import pandas as pd
-
     AS_len = lambda x: SuppaEventID(x).alter_element_len
     lens = df["event_id"].apply(AS_len)
     len_df = pd.DataFrame(lens.tolist())
     return len_df
 
 
 def extract_info(df):
-    import pandas as pd
-
     AS_len = lambda x: SuppaEventID(x).alter_element_len
     chrs = df["event_id"].apply(lambda x: x.split(":")[1])
     genes = df["event_id"].apply(lambda x: x.split(";")[0].strip())
     lens = df["event_id"].apply(AS_len)
     len_df = pd.DataFrame(lens.tolist(), columns=["len"])
     data = {
         "geneId": genes,
@@ -80,16 +81,14 @@
     new_df = pd.DataFrame(data)
     len_df.index = new_df.index
     new_df = pd.concat([new_df, len_df], axis=1)
     return new_df
 
 
 def len_hist(len_counts, width, max_len):
-    import numpy as np
-
     offset = (width - max_len % width) if max_len % width else 0
     bins =  (max_len + offset) // width
     counts, bin_edges = np.histogram(len_counts, bins=bins, range=(1, max_len+offset+1))
     return counts, bin_edges
 
 
 def plot_hist_cluster(out, cluster_ls, bins):
@@ -99,16 +98,14 @@
     for i, subset in enumerate(cluster_ls, 1):
         ax.hist(subset, bins=bins, alpha=0.5, label=f"Cluster {i}")
     ax.legend()
     plt.savefig(out)
 
                                                          
 def custome_cluster_len(df, out, lens, width=10, max_len=500):
-    import pandas as pd
-
     len_count = df["len"]
     counts, bin_edges = len_hist(len_count, width, max_len)
     cluster_ls = []
     start = 0
     for idx, item in enumerate(lens):
         tmp = len_count[start < len_count]
         subset = tmp[tmp <= item]
@@ -130,16 +127,14 @@
 
     plot_hist_cluster(out, cluster_ls, bin_edges)
     return df
 
 
 def cluster_len(df, out, n_cls=5, width=10, max_len=500, len_weight=5):
     from sklearn.cluster import KMeans
-    import pandas as pd
-    import numpy as np
 
     len_count = df["len"]
     counts, bin_edges = len_hist(df["len"], width, max_len)
     lens = [(bin_edges[i] + bin_edges[i+1])/2-1  for i,v in enumerate(bin_edges[:-1])]
     lens = np.array(lens).reshape(-1,1) * len_weight
     counts = counts.reshape(-1,1)
     data = np.concatenate([counts, lens], axis = 1)
@@ -221,16 +216,14 @@
         print("param error")
         sys.exit()
     return eid.Chr, s, e, event_id, 0, eid.strand
 
 
 #TODO re-code it
 def get_coor_bed(dpsi_file, start, end, strand_sp, anchor, upstream_w, downstream_w):
-    import pandas as pd
-
     wget_coor_coor = partial(get_coor, start=start, end=end, strand_sp=strand_sp,
                     anchor=anchor, upstream_w=upstream_w, downstream_w=downstream_w)
     dpsi_df = pd.read_csv(dpsi_file, sep="\t", index_col=0)
     dpsi_df.drop_duplicates(inplace=True)
     dpsi_df["event_id"] = dpsi_df.index
     coors = dpsi_df["event_id"].apply(wget_coor_coor)
     coor_df = pd.DataFrame(coors.tolist())
@@ -259,15 +252,14 @@
     else:
         new_anchor = anchor - offset5 + offset3
 
     return eid.Chr, new_anchor, eid.strand
 
 
 def gen_anchor_bed(dpsi_file, out, index, sideindex, offset5, offset3, strand_sp):
-    import pandas as pd
     from functools import partial
 
     wget_anchor_coor = partial(get_anchor_coor, index=index, 
             sideindex=sideindex, offset5=offset5, offset3=offset3, 
             strand_sp=strand_sp)
     dpsi_df = pd.read_csv(dpsi_file, sep="\t", index_col=0)
     dpsi_df.drop_duplicates(inplace=True)
@@ -278,23 +270,22 @@
 
 
 def get_evnet_ss_bed(
     event_file: FilePath, 
     ups_width: int, 
     dws_width: int
     ):
-    from pandas import concat
     dic = {}
     etype = sniff_AS_type(event_file)
     for i in range(1, SSN[etype]+1):
         ps_coor_df = get_coor_bed(event_file, None, None, False, 
                         i, ups_width, dws_width)
         ns_coor_df = get_coor_bed(event_file, None, None, False, 
                         SSN[etype]+1-i, dws_width, ups_width)
-        ai_coor_df = concat([
+        ai_coor_df = pd.concat([
                         ps_coor_df.loc[ps_coor_df[5] == "+", ],
                         ns_coor_df.loc[ns_coor_df[5] == "-", ]])
         dic[f"A{i}"] = ai_coor_df
     return dic
 
 
 def parse_cmd_r(**param_dic):
@@ -331,16 +322,14 @@
 def sep_name(name, sep, *idx):
     str_ls = name.split(sep)
     name_ls = [str_ls[int(i)-1] for i in idx]
     return ".".join(name_ls)
 
 
 def df_len_select(infile, outfile, s, e):
-    import pandas as pd
-
     AS_len = lambda x: SuppaEventID(x).alter_element_len
     sep = sniff_file_sep(infile)
     df = pd.read_csv(infile, sep=sep, index_col=0)
     cols = df.columns
     df["event_id"] = df.index
     df["len"] = df["event_id"].apply(AS_len)
     pdf = df.loc[(s <= df["len"]) & ( df["len"] < e), cols]
@@ -400,73 +389,70 @@
             seq_ls.append(line)
     else:
         yield descr, ''.join(seq_ls)
 
 
 def detect_file_info(file):
     info_dic = {}
-    with open(file, "r") as f:
-        line1_ls = f.readline().split()
-        ## just simple judgment
-        if line1_ls[:5] == ["ID","GeneID","geneSymbol","chr","strand"]:
-            info_dic["app"] = "rMATS"
-
-            if "riExonStart_0base" in line1_ls:
-                info_dic["etype"] = "RI"
-            elif "2ndExonStart_0base" in line1_ls:
-                info_dic["etype"] = "MXE"
-            elif "exonStart_0base" in line1_ls:
-                info_dic["etype"] = "SE"
-            else:
-                line2_ls = f.readline().split()
-                if line2_ls[4] == "+":
-                    if line2_ls[5] == line2_ls[7]:
-                        info_dic["etype"] = "A5SS"
-                    else:
-                        info_dic["etype"] = "A3SS"
-                else:
-                    if line2_ls[5] == line2_ls[7]:
-                        info_dic["etype"] = "A3SS"
-                    else:
-                        info_dic["etype"] = "A5SS"
+    sep = sniff_file_sep(file)
+    if sep == " ":
+        raise ValueError("The input file separator should not be a single space")
+    df = pd.read_csv(file, sep=sep, index_col=0).dropna()
+    cols = list(df.columns)
+    if cols[:4] == ["GeneID","geneSymbol","chr","strand"]:
+        info_dic["app"] = "rMATS"
+        if "riExonStart_0base" in cols:
+            info_dic["etype"] = "RI"
+        elif "2ndExonStart_0base" in cols:
+            info_dic["etype"] = "MXE"
+        elif "exonStart_0base" in cols:
+            info_dic["etype"] = "SE"
+        elif df.iat[0, 3] == "+":
+            info_dic["etype"] = "A5SS" if df.iat[0, 4] == df.iat[0, 6] else "A3SS"
         else:
-            info_dic["app"] = "SUPPA2"
-            lines = f.readlines()
-            events = [SuppaEventID(line.split()[0]) for line in lines]
-            if len(set([e.AS_type for e in events])) != 1:
-                raise ValueError("input SUPPA2 must contain one AS type!")
-            info_dic["etype"] = events[0].AS_type
-
+            info_dic["etype"] = "A3SS" if df.iat[0, 4] == df.iat[0, 6] else "A5SS"
+    elif cols == ['Gene', 'Event_Type', 'Position', 'Pvalue', 'Zvalue', 'Delta PSI']:
+        info_dic["app"] = "EventPointer"
+        ets = set(df["Event_Type"])
+        info_dic["etype"] = None if len(ets) > 1 else list(ets)[0]
+    else:
+        info_dic["app"] = "SUPPA2"
+        events = [SuppaEventID(eid) for eid in df.index]
+        if len({e.AS_type for e in events}) != 1:
+            raise ValueError("input SUPPA2 must contain one AS type!")
+        info_dic["etype"] = events[0].AS_type
     return info_dic                        
 
 
 def sniff_file_sep(file):
-    """simply check the sep of file
+    """simply check the separator of file
     """
     sep_dic = {}
     with open(file, "r") as f:
         line = f.readline()        
         sep_dic[","] = line.split(",")
         sep_dic["\t"] = line.split("\t")
+        sep_dic[" "] = line.split(" ")
     sep = sorted(sep_dic, key=lambda x: len(sep_dic[x]), reverse=True)[0]
     return sep
 
 
-def merge_files(files, output, axis, rmdup, rmna):
-    from pandas import read_csv, concat
-
+def merge_files(files, output, axis, rmdup, rmna, grouplabel):
     sep = sniff_file_sep(files[0])
     df_ls = []
-    for file in files:
-        df = read_csv(file, sep=sep, index_col=0)
+    for idx, file in enumerate(files):
+        df = pd.read_csv(file, sep=sep, index_col=0)
         if axis == 0:
             df.columns = [f"c{i}" for i in range(df.shape[1])]
+        if axis == 1 and grouplabel:
+            lp = grouplabel[idx]
+            df.columns = [f"{lp}_{i}" for i in df.columns]
         df_ls.append(df)
-    df = concat(df_ls, axis=axis)
-    if rmdup == "all":        
+    df = pd.concat(df_ls, axis=axis)
+    if rmdup == "all":    
         df["event_id"] = df.index
         df = df.drop_duplicates()
         del df["event_id"]
     elif  rmdup == "index":
         df["event_id"] = df.index
         df = df.drop_duplicates(subset=["event_id"])
         del df["event_id"]
@@ -474,16 +460,14 @@
         df = df.drop_duplicates()
     if rmna:
         df.dropna(inplace=True)
     df.to_csv(output, index=True, sep=sep, na_rep="nan")
 
 
 def shift2nease(file):
-    import pandas as pd
-
     get_geneid = lambda x: SuppaEventID(x).gene_id.split(".")[0]
     get_start = lambda x: SuppaEventID(x).alter_element_coor[0]
     get_end = lambda x: SuppaEventID(x).alter_element_coor[1]
 
     df = pd.read_csv(file, sep="\t", index_col=0)
     df["event_id"] = df.index
```

### Comparing `astk-0.1.2/astk/utils/meta_template.py` & `astk-0.1.2b0/astk/utils/meta_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,30 +11,29 @@
 from pathlib import Path
 
 from pandas import DataFrame, concat
 
 
 class Template:
     def __init__(self, condition):
-        self.condition = condition if condition else ["ctrl", "case"]
+        self.condition = condition or ["ctrl", "case"]
 
     def infer_file(self, path, rep):
         rep_num = len(rep)
         path_num = len(path)
 
         if rep_num == 1:
             if isinstance(fold := path_num // int(rep[0]), int):
                 group_num = fold
             else:
                 raise ValueError("path file number or replicate number is wrong!")
+        elif path_num == sum(rep):
+            group_num = rep_num
         else:
-            if path_num == sum(rep):
-                group_num = rep_num
-            else:
-                raise ValueError("path file number or replicate number is wrong!")
+            raise ValueError("path file number or replicate number is wrong!")
         return group_num
 
     def df_generate(self, group_name, rep, path, **kwargs):
         group_num = len(group_name)
 
         if len(rep) == 1:
             replicates = [int(rep[0])] * group_num
@@ -76,41 +75,38 @@
                 raise ValueError("path1 dismatched path2!")
             if len(group) == group_num:
                 group_name = group
             elif len(group) == 0:
                 group_name = list(range(1, group_num+1))
             else:
                 raise ValueError("dismatched path files!")
-
             df1 = self.df_generate(group_name, repN1, path1, **kwargs)
             df2 = self.df_generate(group_name, repN2, path2, **kwargs)
             df1.insert(1, "condition", self.condition[0])
             df2.insert(1, "condition", self.condition[1])
-            df = concat([df1, df2]).sort_values(by=["group"])
-  
+            df = concat([df1, df2]).sort_values(by=["group", "condition", "replicate"])
         else:
             if path1:
-                cdname = self.condition[0]
                 path = path1
                 repN = repN1
             else:
-                cdname = self.condition[0]
                 path = path2
-                repN = repN2            
+                repN = repN2
+            cdname = self.condition[0]
             group_num = self.infer_file(path, repN)
             if len(group) == group_num:
                 group_name = group
             elif len(group) == 0:
                 group_name = list(range(1, group_num+1))
             else:
-                raise ValueError("group names dismatched path files!")                
+                raise ValueError("group names dismatched path files!")
             df = self.df_generate(group_name, repN, path, **kwargs)
-            
+
             df.insert(1, "condition", cdname) 
-        
+
         self.df = df
     
     def to_json(self, out):
         df = self.df
         meta_dic = {} 
         for gn, gdf in df.groupby("group"):
             meta_dic[gn] = {cd:{"samples": []} for cd in df["condition"].unique()}
```

### Comparing `astk-0.1.2/astk/utils/select.py` & `astk-0.1.2b0/astk/utils/select.py`

 * *Files 16% similar despite different names*

```diff
@@ -109,47 +109,7 @@
         if abs(self.dpsi) >= 0:
             for i in sig_psi:
                 self.sig_psi.append(i.with_suffix(".sig.psi"))
                 
     def run(self):
         self.filter_dpsi()
         self.filter_psi()
-
-
-class PsiFilter:
-
-    def __init__(self, file, output, threshold, quantile) -> None:
-        self.file = file
-        self.output = output
-        self.threshold = threshold
-        self.quantile = quantile
-        self.psi_df = read_csv(file, sep="\t", index_col=0).dropna()
-        self.mean_psi = self.psi_df.apply(lambda row: sum(row)/len(row), axis=1)   
-
-    def value_filter(self):
-        th = self.threshold
-        mp = self.mean_psi
-        if th >= 0:
-            filter_idx = mp[mp > th].index
-        else:
-            filter_idx = mp[mp < abs(th)].index
-        return self.psi_df.loc[filter_idx, ]
-    
-    def quantile_filter(self):
-        qt = self.quantile
-        mp = self.mean_psi
-        th = mp.quantile(abs(qt))
-        if qt >= 0:
-            filter_idx = mp[mp > th].index
-        else:
-            filter_idx = mp[mp <th].index
-        return self.psi_df.loc[filter_idx, ]
-    
-    def run(self):
-        if self.threshold:
-            psi_df = self.value_filter()
-        elif self.quantile:
-            psi_df = self.quantile_filter()
-        else:
-            psi_df = self.psi_df    
-        psi_df.to_csv(self.output, sep="\t", index_label=False)
-
```

### Comparing `astk-0.1.2/astk.egg-info/SOURCES.txt` & `astk-0.1.2b0/astk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,43 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-astk/ChromHMM.jar
-astk/ChromHMM.py
 astk/__init__.py
 astk/constant.py
-astk/types.py
+astk/ctypes.py
+astk/lazy_loader.py
 astk.egg-info/PKG-INFO
 astk.egg-info/SOURCES.txt
 astk.egg-info/dependency_links.txt
 astk.egg-info/entry_points.txt
 astk.egg-info/requires.txt
 astk.egg-info/top_level.txt
-astk/R/ChromHMM_hm.R
 astk/R/CoSpliceNet.R
-astk/R/barplot.R
 astk/R/dl_keggdata.R
 astk/R/enrich.R
 astk/R/enrichCompare.R
-astk/R/epiFeature.R
-astk/R/epiProfile.R
 astk/R/gsea.R
 astk/R/gseaPlot.R
-astk/R/heatmap.R
 astk/R/install.R
 astk/R/makeTxDb.R
-astk/R/motifEnrich.R
-astk/R/motifFind.R
 astk/R/motifMap.R
 astk/R/motifPlot.R
-astk/R/pca.R
 astk/R/seqLogo.R
-astk/R/signalCompare.R
-astk/R/signalHeatmap.R
-astk/R/signalProfile.R
 astk/R/upset.R
 astk/R/utils.R
-astk/R/volcano.R
 astk/cli/__init__.py
+astk/cli/aliases.ini
 astk/cli/as_event.py
 astk/cli/config.py
 astk/cli/draw.py
 astk/cli/epi.py
+astk/cli/experiment.py
 astk/cli/gsea.py
+astk/cli/ml.py
 astk/cli/motif.py
 astk/cli/net.py
 astk/cli/seqfeature.py
 astk/cli/suppa.py
 astk/cli/utils.py
 astk/data/maxent/ss3_score.json
 astk/data/maxent/ss5seq_score.json
@@ -366,14 +356,18 @@
 astk/epi/__init__.py
 astk/epi/_func.py
 astk/event/__init__.py
 astk/event/_cli_func.py
 astk/event/eid.py
 astk/gsea/__init__.py
 astk/gsea/_func.py
+astk/ml/__init__.py
+astk/ml/_chunk_permutation_importance.py
+astk/ml/_metric.py
+astk/ml/_tools.py
 astk/motif/__init__.py
 astk/motif/_func.py
 astk/motif/elm.py
 astk/network/__init__.py
 astk/network/_func.py
 astk/seqfeature/__init__.py
 astk/seqfeature/_compare.py
```

