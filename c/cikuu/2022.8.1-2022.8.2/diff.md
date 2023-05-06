# Comparing `tmp/cikuu-2022.8.1.tar.gz` & `tmp/cikuu-2022.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cikuu-2022.8.1.tar", last modified: Tue May  2 04:03:48 2023, max compression
+gzip compressed data, was "cikuu-2022.8.2.tar", last modified: Sat May  6 09:49:02 2023, max compression
```

## Comparing `cikuu-2022.8.1.tar` & `cikuu-2022.8.2.tar`

### file list

```diff
@@ -1,374 +1,373 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.133234 cikuu-2022.8.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-03-04 12:51:34.000000 cikuu-2022.8.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-05-02 04:03:48.133234 cikuu-2022.8.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:47.857233 cikuu-2022.8.1/api/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-03-04 12:49:43.000000 cikuu-2022.8.1/api/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-03-04 12:49:43.000000 cikuu-2022.8.1/api/c4.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1236 2023-03-04 12:49:46.000000 cikuu-2022.8.1/api/chunk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-03-04 12:49:49.000000 cikuu-2022.8.1/api/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-03-04 12:49:43.000000 cikuu-2022.8.1/api/dm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21647 2023-03-04 12:49:44.000000 cikuu-2022.8.1/api/es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-03-04 12:49:46.000000 cikuu-2022.8.1/api/feishu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-03-04 12:49:49.000000 cikuu-2022.8.1/api/mynac.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-03-04 12:49:44.000000 cikuu-2022.8.1/api/sntjson-es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-03-04 12:49:44.000000 cikuu-2022.8.1/api/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1333 2023-03-04 12:49:46.000000 cikuu-2022.8.1/api/wget.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:47.857233 cikuu-2022.8.1/app/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:49:46.000000 cikuu-2022.8.1/app/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:47.877233 cikuu-2022.8.1/app/dmdsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2097 2023-03-04 12:49:46.000000 cikuu-2022.8.1/app/dmdsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2298 2023-03-04 12:49:46.000000 cikuu-2022.8.1/app/dmdsk/app_navbar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:47.885233 cikuu-2022.8.1/app/dmdsk/func/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:49:49.000000 cikuu-2022.8.1/app/dmdsk/func/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-03-04 12:49:44.000000 cikuu-2022.8.1/app/dmdsk/func/dim-awl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-03-04 12:49:44.000000 cikuu-2022.8.1/app/dmdsk/func/dims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2023-03-04 12:49:46.000000 cikuu-2022.8.1/app/dmdsk/func/eidv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-03-04 12:49:49.000000 cikuu-2022.8.1/app/dmdsk/func/feedback.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-03-04 12:49:44.000000 cikuu-2022.8.1/app/dmdsk/func/info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-03-04 12:49:44.000000 cikuu-2022.8.1/app/dmdsk/func/lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-03-04 12:49:46.000000 cikuu-2022.8.1/app/dmdsk/func/scores.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-03-04 12:49:49.000000 cikuu-2022.8.1/app/dmdsk/func/sent.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-03-04 12:49:44.000000 cikuu-2022.8.1/app/dmdsk/func/trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      708 2023-03-04 12:49:49.000000 cikuu-2022.8.1/app/dmdsk/index.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:47.889233 cikuu-2022.8.1/cikuu.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-05-02 04:03:47.000000 cikuu-2022.8.1/cikuu.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6223 2023-05-02 04:03:47.000000 cikuu-2022.8.1/cikuu.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 04:03:47.000000 cikuu-2022.8.1/cikuu.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-02 04:03:47.000000 cikuu-2022.8.1/cikuu.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-05-02 04:03:47.000000 cikuu-2022.8.1/cikuu.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.089234 cikuu-2022.8.1/dic/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6977 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-03-04 12:49:46.000000 cikuu-2022.8.1/dic/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72703 2023-03-04 12:49:46.000000 cikuu-2022.8.1/dic/adjlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15209 2023-03-04 12:49:48.000000 cikuu-2022.8.1/dic/advlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2036435 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/bnc_wordlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   742662 2023-03-04 12:49:49.000000 cikuu-2022.8.1/dic/confu_set.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1423371 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/ecdic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8101 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/errants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   716825 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/essays.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   479692 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/frame.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1966581 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/lemma_lex.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   446749 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/lemma_mf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182701 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/lemma_scale.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1724920 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/lex_lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4088 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/mwe_disconj.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10043 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/mwe_pv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173703 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/n_is_sb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173515 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/nounlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3696547 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/nyt_wc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/oneself.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41916 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/orals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/poslist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2786732 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/propbank.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1350 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/stoplist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/to_redislite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    90499 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/verbform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9125 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/verblist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   147209 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/verbtag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   357010 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/vocab.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42948 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/word_awl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   825665 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/word_bits.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   518752 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/word_grade.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46473 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/word_gsl1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42152 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/word_gsl2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2765429 2023-03-04 12:51:15.000000 cikuu-2022.8.1/dic/word_idf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2717304 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/word_oov.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3086978 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/word_pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182843 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/word_scale.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4370200 2023-03-04 12:51:15.000000 cikuu-2022.8.1/dic/wordattr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   300932 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/wordcnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   353846 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/wordlist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   957421 2023-03-04 12:50:25.000000 cikuu-2022.8.1/dic/wordlist_ed1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   100665 2023-03-04 12:51:15.000000 cikuu-2022.8.1/dic/wordnet_verb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1150605 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/wordpos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53593 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dic/words.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.097234 cikuu-2022.8.1/dsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7973 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    94356 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5471 2023-03-04 12:51:16.000000 cikuu-2022.8.1/dsk/dm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2874 2023-03-06 07:28:15.000000 cikuu-2022.8.1/dsk/dsk-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-03-06 07:28:15.000000 cikuu-2022.8.1/dsk/dsk-req.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/dsk-to-dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9144 2023-05-01 01:51:11.000000 cikuu-2022.8.1/dsk/dsk2023.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-03-04 12:51:16.000000 cikuu-2022.8.1/dsk/dskapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/dskes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/dskmkf_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2465 2023-03-04 12:51:16.000000 cikuu-2022.8.1/dsk/dsktrain.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/essaydm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/gears-xdsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4284 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/gecv1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7911 2023-03-04 12:51:16.000000 cikuu-2022.8.1/dsk/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6162 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/innersim.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6946 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/json-to-dskmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9243 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/kvrdsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-03-04 12:51:16.000000 cikuu-2022.8.1/dsk/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8998 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/mkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/mqconsume.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83132 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/pingyu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3416 2023-03-04 12:51:16.000000 cikuu-2022.8.1/dsk/score.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6150 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/sntsdims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-03-04 12:51:16.000000 cikuu-2022.8.1/dsk/tok-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3629 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/uvidsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6616 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/wps-gec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-23 13:45:01.000000 cikuu-2022.8.1/dsk/wps-xgec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11219 2023-04-23 13:45:08.000000 cikuu-2022.8.1/dsk/wps7000.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9689 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/xessay.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10368 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/xgecv1-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-04-23 13:45:57.000000 cikuu-2022.8.1/dsk/xgecv1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4396 2023-03-04 12:51:16.000000 cikuu-2022.8.1/dsk/xmkf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2902 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/xsnt-gec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2186 2023-03-04 12:50:48.000000 cikuu-2022.8.1/dsk/xsnt-spacy.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.109234 cikuu-2022.8.1/en/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80279 2023-03-20 11:54:15.000000 cikuu-2022.8.1/en/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/annotate.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.109234 cikuu-2022.8.1/en/arc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    74716 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/arc/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/arc/sntjson-innodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15868 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/arc/sntjson-naclite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6901 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/arc/sntjson-naclite0.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23369 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/arc/sntjson-nacp-20230206.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26784 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/arc/sntjson-nacp-20230207.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4-cl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3675 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4-fts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/c4-gram-upload.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4-gram.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      875 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4-grams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4-np.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/c4-postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4-trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2039 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4cl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4down.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1884 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/c4gram-mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2812 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4gram-upsert.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1731 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4gram.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4gramcl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/c4matcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1401 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4np.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3683 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4skenp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/c4tree.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4trp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/c4vp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/clause.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6120 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/dims.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16963 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/docfts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8115 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/docjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-03-16 03:10:14.000000 cikuu-2022.8.1/en/en-hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8717 2023-03-25 07:35:03.000000 cikuu-2022.8.1/en/es-index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/esbulk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3777 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/esfile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6311 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3506 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/exchunk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1159 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/exphrase.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1387 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/extrp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4656 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/havc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18434 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/kpsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4234 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/lempostag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2023-03-16 12:13:36.000000 cikuu-2022.8.1/en/nacp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/nlp-lit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4581 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/nlp-lmdb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1900 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/postag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/shav.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/silite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1506 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/snt-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4786 2023-03-16 12:13:36.000000 cikuu-2022.8.1/en/sntjson-fts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-03-16 12:13:36.000000 cikuu-2022.8.1/en/sntjson-kpsnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8237 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/sntjson-mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13520 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/sntjson-nacp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      963 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/sntjson-parse-snt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/sntjson-si.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/sntjson-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2023-03-18 08:29:48.000000 cikuu-2022.8.1/en/sntjson-topk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-30 03:58:22.000000 cikuu-2022.8.1/en/sntjson-tosnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3888 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/sntjson-trpx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/sntjson-vp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/spacybs-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30937 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/spacybs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2733 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/spider-esjson.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6730 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/sqlsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30005 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/terms.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/verbnet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1874 2023-03-04 12:50:48.000000 cikuu-2022.8.1/en/xsnt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-03-04 12:51:16.000000 cikuu-2022.8.1/en/zset-load.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.109234 cikuu-2022.8.1/gecdsk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9190 2023-05-01 01:51:11.000000 cikuu-2022.8.1/gecdsk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.113234 cikuu-2022.8.1/lit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16540 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1467 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.113234 cikuu-2022.8.1/lit/es/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5386 2023-03-04 12:50:48.000000 cikuu-2022.8.1/lit/es/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:15.000000 cikuu-2022.8.1/lit/es/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:27.000000 cikuu-2022.8.1/lit/essay.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/filling.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1905 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/fillmul.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      778 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/hello-pages.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-03-04 12:51:27.000000 cikuu-2022.8.1/lit/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/mock-scoring.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.113234 cikuu-2022.8.1/lit/penly/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/penly/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/penly/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/penly-resend.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1827 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/redis-dump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-03-04 12:51:27.000000 cikuu-2022.8.1/lit/reorder.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/restore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/scoring.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/single.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-03-04 12:51:27.000000 cikuu-2022.8.1/lit/sntspolish.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1091 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/sntupgrade.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/student-input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/teacher-admin.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.113234 cikuu-2022.8.1/lit/yulk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      668 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/yulk/YULK.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/yulk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/yulk/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.117234 cikuu-2022.8.1/lit/yulk/func/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/bipos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/cola.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      666 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/corpuslist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      549 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      501 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/eshyb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/given-expect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/gramx-single.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/lemma.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1912 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/lemvs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/pos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/posvs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1925 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/style-in-mul.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/style.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      353 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/wcloud.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1547 2023-03-04 12:51:16.000000 cikuu-2022.8.1/lit/yulk/func/wordrank.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-03-04 12:51:27.000000 cikuu-2022.8.1/lit/yulk/index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1255 2023-03-04 12:51:18.000000 cikuu-2022.8.1/lit/yulk/lemma.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.117234 cikuu-2022.8.1/pipe/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4906 2023-03-04 12:51:27.000000 cikuu-2022.8.1/pipe/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2622 2023-03-04 12:51:18.000000 cikuu-2022.8.1/pipe/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4039 2023-03-04 12:51:18.000000 cikuu-2022.8.1/pipe/redisgec8180.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6514 2023-03-04 12:51:27.000000 cikuu-2022.8.1/pipe/xgecv1.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.117234 cikuu-2022.8.1/rabbitmq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3075 2023-04-30 03:58:22.000000 cikuu-2022.8.1/rabbitmq/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.117234 cikuu-2022.8.1/redisr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      746 2023-04-30 03:58:22.000000 cikuu-2022.8.1/redisr/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.117234 cikuu-2022.8.1/sbert/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      255 2023-03-04 12:51:18.000000 cikuu-2022.8.1/sbert/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1316 2023-03-04 12:51:18.000000 cikuu-2022.8.1/sbert/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      613 2023-03-04 12:51:27.000000 cikuu-2022.8.1/sbert/hello.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13086 2023-03-04 12:51:18.000000 cikuu-2022.8.1/sbert/sntvec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-02 04:03:48.133234 cikuu-2022.8.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      799 2023-05-02 04:03:44.000000 cikuu-2022.8.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.121234 cikuu-2022.8.1/so/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27535 2023-05-02 04:03:44.000000 cikuu-2022.8.1/so/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-05-02 04:03:44.000000 cikuu-2022.8.1/so/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13741 2023-03-04 12:51:28.000000 cikuu-2022.8.1/so/corpusly.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9475 2023-03-04 12:51:18.000000 cikuu-2022.8.1/so/cos.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2283 2023-05-02 04:03:44.000000 cikuu-2022.8.1/so/dsk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17434 2023-03-04 12:51:18.000000 cikuu-2022.8.1/so/esapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2427 2023-03-04 12:51:18.000000 cikuu-2022.8.1/so/eslite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1317 2023-03-04 12:51:18.000000 cikuu-2022.8.1/so/kps-si.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1559 2023-03-04 12:51:18.000000 cikuu-2022.8.1/so/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-03-04 12:51:29.000000 cikuu-2022.8.1/so/loadc4.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1746 2023-03-04 12:51:18.000000 cikuu-2022.8.1/so/loades.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1294 2023-03-04 12:51:18.000000 cikuu-2022.8.1/so/sikps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1744 2023-05-02 04:03:44.000000 cikuu-2022.8.1/so/sntbr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21465 2023-03-04 12:51:29.000000 cikuu-2022.8.1/so/sntvec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1333 2023-05-02 04:03:44.000000 cikuu-2022.8.1/so/spacytok.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27099 2023-03-26 10:23:51.000000 cikuu-2022.8.1/so/test-lowercase.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18777 2023-05-01 14:50:34.000000 cikuu-2022.8.1/so/tocos.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.121234 cikuu-2022.8.1/sqlite/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6138 2023-05-01 13:24:28.000000 cikuu-2022.8.1/sqlite/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      500 2023-05-01 14:50:34.000000 cikuu-2022.8.1/sqlite/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.125234 cikuu-2022.8.1/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4840 2023-04-04 03:49:41.000000 cikuu-2022.8.1/util/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/annotate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3455 2023-03-04 12:51:34.000000 cikuu-2022.8.1/util/bcp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2820 2023-03-04 12:51:30.000000 cikuu-2022.8.1/util/c4data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/client-blpop.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/client-xwps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-03-04 12:51:34.000000 cikuu-2022.8.1/util/clientx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9342 2023-03-04 12:51:30.000000 cikuu-2022.8.1/util/dsk-util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/fire-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-03-04 12:51:34.000000 cikuu-2022.8.1/util/frame.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4097 2023-03-04 12:51:30.000000 cikuu-2022.8.1/util/kvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/mq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      713 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/nldp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      796 2023-03-04 12:51:34.000000 cikuu-2022.8.1/util/pubsub-sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-03-04 12:51:30.000000 cikuu-2022.8.1/util/pubsub2api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/sent-diff.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3123 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/spider.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-03-04 12:51:34.000000 cikuu-2022.8.1/util/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-04 12:51:30.000000 cikuu-2022.8.1/util/sqlitedict-load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4749 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/wps-blpop.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36149 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/wps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-03-04 12:51:34.000000 cikuu-2022.8.1/util/xfile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-03-04 12:51:30.000000 cikuu-2022.8.1/util/xgec-blpop120.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      371 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/xrange.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/xsnt-spacy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-03-04 12:51:34.000000 cikuu-2022.8.1/util/xstream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-03-04 12:51:30.000000 cikuu-2022.8.1/util/xtest-params.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-03-04 12:51:33.000000 cikuu-2022.8.1/util/xtest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.125234 cikuu-2022.8.1/uviapp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-05-01 14:50:34.000000 cikuu-2022.8.1/uviapp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.133234 cikuu-2022.8.1/uvirun/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-03-04 12:51:44.000000 cikuu-2022.8.1/uvirun/Jinja2-test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2151 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3034 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6573 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/c4es.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2023-03-04 12:51:44.000000 cikuu-2022.8.1/uvirun/c4gramsi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4734 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/cos_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-04-30 03:58:22.000000 cikuu-2022.8.1/uvirun/demo_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22269 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/dsk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-03-04 12:51:44.000000 cikuu-2022.8.1/uvirun/echart_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4778 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/elastic_fastapi.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.133234 cikuu-2022.8.1/uvirun/errant/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-03-04 12:51:33.000000 cikuu-2022.8.1/uvirun/errant/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7269 2023-03-04 12:51:33.000000 cikuu-2022.8.1/uvirun/errant/alignment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/errant/annotator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.133234 cikuu-2022.8.1/uvirun/errant/commands/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.1/uvirun/errant/commands/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16344 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/errant/commands/compare_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-03-04 12:51:30.000000 cikuu-2022.8.1/uvirun/errant/commands/m2_to_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3801 2023-03-04 12:51:33.000000 cikuu-2022.8.1/uvirun/errant/commands/parallel_to_m2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2352 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/errant/edit.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 04:03:48.133234 cikuu-2022.8.1/uvirun/errant/en/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.1/uvirun/errant/en/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16879 2023-03-04 12:51:33.000000 cikuu-2022.8.1/uvirun/errant/en/classifier.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12340 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/errant/en/lancaster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5602 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/errant/en/merger.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10943 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/errant_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14040 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/es1_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25631 2023-03-20 01:06:12.000000 cikuu-2022.8.1/uvirun/es_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4806 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/essay_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18163 2023-04-30 03:58:22.000000 cikuu-2022.8.1/uvirun/exchunk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18525 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/feishu_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3892 2023-03-04 12:51:44.000000 cikuu-2022.8.1/uvirun/flair_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1809 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1010 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/fusion_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/gec_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-03-04 12:51:44.000000 cikuu-2022.8.1/uvirun/gec_fastapi_33000.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13116 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/gensim_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6638 2023-04-12 02:56:55.000000 cikuu-2022.8.1/uvirun/gramx_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2562 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/hnswlib_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-03-04 12:51:44.000000 cikuu-2022.8.1/uvirun/kenlm_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6264 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/kpsi_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/kvr_dskdm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/kvr_dskdm1230.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19126 2023-03-04 12:51:44.000000 cikuu-2022.8.1/uvirun/nldp_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/nltk_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/nsp_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10222 2023-03-16 03:10:15.000000 cikuu-2022.8.1/uvirun/penlykvr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4343 2023-03-04 12:51:44.000000 cikuu-2022.8.1/uvirun/sbert_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/single_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32687 2023-04-30 03:58:22.000000 cikuu-2022.8.1/uvirun/spacy_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4320 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/textacy_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2089 2023-03-04 12:51:44.000000 cikuu-2022.8.1/uvirun/trans_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4113 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/unmasker_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8742 2023-03-04 12:51:34.000000 cikuu-2022.8.1/uvirun/util_fastapi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45795 2023-03-04 12:51:41.000000 cikuu-2022.8.1/uvirun/uviredis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37415 2023-04-13 09:21:47.000000 cikuu-2022.8.1/uvirun/yulk-nac.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.152003 cikuu-2022.8.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-03-04 12:51:34.000000 cikuu-2022.8.2/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-05-06 09:49:02.152003 cikuu-2022.8.2/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.431992 cikuu-2022.8.2/api/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-03-04 12:49:43.000000 cikuu-2022.8.2/api/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2086 2023-03-04 12:49:43.000000 cikuu-2022.8.2/api/c4.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1236 2023-03-04 12:49:46.000000 cikuu-2022.8.2/api/chunk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1399 2023-03-04 12:49:49.000000 cikuu-2022.8.2/api/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2023-03-04 12:49:43.000000 cikuu-2022.8.2/api/dm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21647 2023-03-04 12:49:44.000000 cikuu-2022.8.2/api/es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-03-04 12:49:46.000000 cikuu-2022.8.2/api/feishu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-03-04 12:49:49.000000 cikuu-2022.8.2/api/mynac.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-03-04 12:49:44.000000 cikuu-2022.8.2/api/sntjson-es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-03-04 12:49:44.000000 cikuu-2022.8.2/api/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1333 2023-03-04 12:49:46.000000 cikuu-2022.8.2/api/wget.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.431992 cikuu-2022.8.2/app/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.451992 cikuu-2022.8.2/app/dmdsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2097 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/dmdsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2298 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/dmdsk/app_navbar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.487993 cikuu-2022.8.2/app/dmdsk/func/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:49:49.000000 cikuu-2022.8.2/app/dmdsk/func/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/dim-awl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/dims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/dmdsk/func/eidv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-03-04 12:49:49.000000 cikuu-2022.8.2/app/dmdsk/func/feedback.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2023-03-04 12:49:46.000000 cikuu-2022.8.2/app/dmdsk/func/scores.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-03-04 12:49:49.000000 cikuu-2022.8.2/app/dmdsk/func/sent.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-03-04 12:49:44.000000 cikuu-2022.8.2/app/dmdsk/func/trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      708 2023-03-04 12:49:49.000000 cikuu-2022.8.2/app/dmdsk/index.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:48:59.487993 cikuu-2022.8.2/cikuu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6254 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-05-06 09:48:58.000000 cikuu-2022.8.2/cikuu.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:00.999999 cikuu-2022.8.2/dic/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6977 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-03-04 12:49:46.000000 cikuu-2022.8.2/dic/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    72703 2023-03-04 12:49:46.000000 cikuu-2022.8.2/dic/adjlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15209 2023-03-04 12:49:48.000000 cikuu-2022.8.2/dic/advlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2036481 2023-05-04 07:44:16.000000 cikuu-2022.8.2/dic/bnc_wordlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   742662 2023-03-04 12:49:49.000000 cikuu-2022.8.2/dic/confu_set.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1423371 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/ecdic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8101 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/errants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   716825 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   479692 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/frame.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1966581 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/lemma_lex.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   446749 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/lemma_mf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182701 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/lemma_scale.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1724920 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/lex_lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4088 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/mwe_disconj.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10043 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/mwe_pv.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173703 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/n_is_sb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   173515 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/nounlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3696547 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/nyt_wc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/oneself.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41916 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/orals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/poslist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2786732 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/propbank.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1350 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/stoplist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/to_redislite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    90499 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/verbform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9125 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/verblist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   147209 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/verbtag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   357010 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/vocab.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42948 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_awl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   825665 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/word_bits.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   518752 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_grade.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46473 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_gsl1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42152 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_gsl2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2765429 2023-03-04 12:51:15.000000 cikuu-2022.8.2/dic/word_idf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2717304 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/word_oov.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  3086978 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/word_pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   182843 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/word_scale.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  4370200 2023-03-04 12:51:15.000000 cikuu-2022.8.2/dic/wordattr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   300932 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/wordcnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   353846 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/wordlist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   957421 2023-03-04 12:50:25.000000 cikuu-2022.8.2/dic/wordlist_ed1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   100665 2023-03-04 12:51:15.000000 cikuu-2022.8.2/dic/wordnet_verb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1150605 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/wordpos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53593 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dic/words.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.231999 cikuu-2022.8.2/dsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7973 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    94356 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5471 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/dm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2874 2023-03-06 07:28:15.000000 cikuu-2022.8.2/dsk/dsk-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-03-06 07:28:15.000000 cikuu-2022.8.2/dsk/dsk-req.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4928 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/dsk-to-dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9144 2023-05-01 01:51:11.000000 cikuu-2022.8.2/dsk/dsk2023.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3970 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/dskapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/dskes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5532 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/dskmkf_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2465 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/dsktrain.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/essaydm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/gears-xdsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4284 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/gecv1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7911 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6162 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/innersim.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6946 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/json-to-dskmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9243 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/kvrdsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8998 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/mkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/mqconsume.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83132 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/pingyu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3416 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/score.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6150 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/sntsdims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/tok-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3629 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/uvidsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6616 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/wps-gec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-23 13:45:01.000000 cikuu-2022.8.2/dsk/wps-xgec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11219 2023-04-23 13:45:08.000000 cikuu-2022.8.2/dsk/wps7000.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9689 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/xessay.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10368 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/xgecv1-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-04-23 13:45:57.000000 cikuu-2022.8.2/dsk/xgecv1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4396 2023-03-04 12:51:16.000000 cikuu-2022.8.2/dsk/xmkf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2902 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/xsnt-gec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2186 2023-03-04 12:50:48.000000 cikuu-2022.8.2/dsk/xsnt-spacy.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.500001 cikuu-2022.8.2/en/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80279 2023-03-20 11:54:15.000000 cikuu-2022.8.2/en/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/annotate.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.512001 cikuu-2022.8.2/en/arc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    74716 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1257 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/sntjson-innodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15868 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/sntjson-naclite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6901 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/arc/sntjson-naclite0.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23369 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/sntjson-nacp-20230206.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26784 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/arc/sntjson-nacp-20230207.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-cl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3675 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-fts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4-gram-upload.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-gram.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      875 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-grams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-np.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4-postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      589 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4-trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2039 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4cl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4down.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1884 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4gram-mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2812 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4gram-upsert.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1731 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4gram.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5885 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4gramcl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3602 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4matcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1401 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4np.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3683 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4skenp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/c4tree.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4trp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/c4vp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/clause.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6120 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/dims.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16963 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/docfts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8115 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/docjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-03-16 03:10:14.000000 cikuu-2022.8.2/en/en-hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8717 2023-03-25 07:35:03.000000 cikuu-2022.8.2/en/es-index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/esbulk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3777 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/esfile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6311 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3506 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/exchunk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1159 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/exphrase.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1387 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/extrp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4656 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/havc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18434 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/kpsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4234 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/lempostag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2023-03-16 12:13:36.000000 cikuu-2022.8.2/en/nacp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/nlp-lit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4581 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/nlp-lmdb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1900 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/postag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/shav.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/silite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1506 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/snt-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4786 2023-03-16 12:13:36.000000 cikuu-2022.8.2/en/sntjson-fts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-03-16 12:13:36.000000 cikuu-2022.8.2/en/sntjson-kpsnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8237 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13520 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-nacp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      963 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-parse-snt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2031 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/sntjson-si.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      569 2023-03-18 08:29:48.000000 cikuu-2022.8.2/en/sntjson-topk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-30 03:58:22.000000 cikuu-2022.8.2/en/sntjson-tosnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3888 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/sntjson-trpx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/sntjson-vp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/spacybs-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30937 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/spacybs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2733 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/spider-esjson.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6730 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/sqlsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30005 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/terms.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/verbnet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1874 2023-03-04 12:50:48.000000 cikuu-2022.8.2/en/xsnt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1093 2023-03-04 12:51:16.000000 cikuu-2022.8.2/en/zset-load.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.532001 cikuu-2022.8.2/gecdsk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9234 2023-05-03 03:14:08.000000 cikuu-2022.8.2/gecdsk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      704 2023-05-03 03:19:37.000000 cikuu-2022.8.2/gecdsk/essays.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.580001 cikuu-2022.8.2/lit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16540 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1467 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/common.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.588001 cikuu-2022.8.2/lit/es/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5386 2023-03-04 12:50:48.000000 cikuu-2022.8.2/lit/es/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:15.000000 cikuu-2022.8.2/lit/es/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/essay.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/filling.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1905 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/fillmul.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      778 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/hello-pages.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/mock-scoring.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.588001 cikuu-2022.8.2/lit/penly/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/penly/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/penly/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/penly-resend.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1827 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/redis-dump.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/reorder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/restore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/scoring.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/single.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/sntspolish.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1091 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/sntupgrade.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/student-input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/teacher-admin.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.608001 cikuu-2022.8.2/lit/yulk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      668 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/yulk/YULK.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/yulk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/yulk/common.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.636001 cikuu-2022.8.2/lit/yulk/func/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/bipos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/cola.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16942 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      666 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/corpuslist.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      549 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      501 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/eshyb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/given-expect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/gramx-single.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/lemma.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1912 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/lemvs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/pos.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/posvs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1925 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/style-in-mul.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/style.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      353 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/wcloud.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1547 2023-03-04 12:51:16.000000 cikuu-2022.8.2/lit/yulk/func/wordrank.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-03-04 12:51:27.000000 cikuu-2022.8.2/lit/yulk/index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1255 2023-03-04 12:51:18.000000 cikuu-2022.8.2/lit/yulk/lemma.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.640001 cikuu-2022.8.2/pipe/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4906 2023-03-04 12:51:27.000000 cikuu-2022.8.2/pipe/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2622 2023-03-04 12:51:18.000000 cikuu-2022.8.2/pipe/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4039 2023-03-04 12:51:18.000000 cikuu-2022.8.2/pipe/redisgec8180.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6514 2023-03-04 12:51:27.000000 cikuu-2022.8.2/pipe/xgecv1.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.640001 cikuu-2022.8.2/rabbitmq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3075 2023-04-30 03:58:22.000000 cikuu-2022.8.2/rabbitmq/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.660001 cikuu-2022.8.2/redisr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      746 2023-04-30 03:58:22.000000 cikuu-2022.8.2/redisr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8210 2023-05-04 00:09:32.000000 cikuu-2022.8.2/redisr/glove-get.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-05-03 09:15:53.000000 cikuu-2022.8.2/redisr/glove.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8249 2023-05-04 11:54:55.000000 cikuu-2022.8.2/redisr/sntvec-get.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.664001 cikuu-2022.8.2/sbert/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-04 10:29:10.000000 cikuu-2022.8.2/sbert/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1316 2023-03-04 12:51:18.000000 cikuu-2022.8.2/sbert/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-03 08:06:44.000000 cikuu-2022.8.2/sbert/hello.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2023-05-04 13:39:29.000000 cikuu-2022.8.2/sbert/redis-sntvec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2379 2023-05-05 09:11:12.000000 cikuu-2022.8.2/sbert/sntvec-so.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13086 2023-03-04 12:51:18.000000 cikuu-2022.8.2/sbert/sntvec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-06 09:49:02.152003 cikuu-2022.8.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      799 2023-05-06 09:48:53.000000 cikuu-2022.8.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.692001 cikuu-2022.8.2/so/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32697 2023-05-06 03:47:46.000000 cikuu-2022.8.2/so/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2177 2023-05-02 11:43:44.000000 cikuu-2022.8.2/so/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1116 2023-05-06 09:45:29.000000 cikuu-2022.8.2/so/dis-eev.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2040 2023-05-05 09:11:12.000000 cikuu-2022.8.2/so/dis-essays.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-05 09:11:12.000000 cikuu-2022.8.2/so/dis-folder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-03 03:14:08.000000 cikuu-2022.8.2/so/dsk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-05-03 03:14:08.000000 cikuu-2022.8.2/so/folder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1707 2023-05-06 09:45:29.000000 cikuu-2022.8.2/so/index-dis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1559 2023-03-04 12:51:18.000000 cikuu-2022.8.2/so/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1746 2023-03-04 12:51:18.000000 cikuu-2022.8.2/so/loades.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.716001 cikuu-2022.8.2/sqlite/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6138 2023-05-01 13:24:28.000000 cikuu-2022.8.2/sqlite/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      500 2023-05-01 14:50:34.000000 cikuu-2022.8.2/sqlite/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.888002 cikuu-2022.8.2/util/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5596 2023-05-05 02:24:34.000000 cikuu-2022.8.2/util/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/annotate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3455 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/bcp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2820 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/c4data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/client-blpop.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/client-xwps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/clientx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9342 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/dsk-util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      506 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/fire-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/frame.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4097 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/kvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/mq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      713 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/nldp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      796 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/pubsub-sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/pubsub2api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/sent-diff.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3123 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/spider.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/sqlitedict-load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4749 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/wps-blpop.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36149 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/wps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/xfile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/xgec-blpop120.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      371 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/xrange.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/xsnt-spacy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1521 2023-03-04 12:51:34.000000 cikuu-2022.8.2/util/xstream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-03-04 12:51:30.000000 cikuu-2022.8.2/util/xtest-params.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1404 2023-03-04 12:51:33.000000 cikuu-2022.8.2/util/xtest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:01.896002 cikuu-2022.8.2/uviapp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-05-01 14:50:34.000000 cikuu-2022.8.2/uviapp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.112003 cikuu-2022.8.2/uvirun/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/Jinja2-test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2151 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3034 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6573 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/c4es.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/c4gramsi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4734 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/cos_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-04-30 03:58:22.000000 cikuu-2022.8.2/uvirun/demo_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22269 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/dsk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5335 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/echart_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4778 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/elastic_fastapi.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.128003 cikuu-2022.8.2/uvirun/errant/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7269 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/alignment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/errant/annotator.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.144003 cikuu-2022.8.2/uvirun/errant/commands/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/commands/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16344 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/errant/commands/compare_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-03-04 12:51:30.000000 cikuu-2022.8.2/uvirun/errant/commands/m2_to_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3801 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/commands/parallel_to_m2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2352 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/errant/edit.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-06 09:49:02.152003 cikuu-2022.8.2/uvirun/errant/en/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/en/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16879 2023-03-04 12:51:33.000000 cikuu-2022.8.2/uvirun/errant/en/classifier.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12340 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/errant/en/lancaster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5602 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/errant/en/merger.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10943 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/errant_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14040 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/es1_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25631 2023-03-20 01:06:12.000000 cikuu-2022.8.2/uvirun/es_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4806 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/essay_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18163 2023-04-30 03:58:22.000000 cikuu-2022.8.2/uvirun/exchunk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18525 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/feishu_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3892 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/flair_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1809 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1010 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/fusion_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3717 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/gec_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/gec_fastapi_33000.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13116 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/gensim_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6638 2023-04-12 02:56:55.000000 cikuu-2022.8.2/uvirun/gramx_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2562 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/hnswlib_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/kenlm_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6264 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/kpsi_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/kvr_dskdm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13096 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/kvr_dskdm1230.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19126 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/nldp_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/nltk_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/nsp_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10222 2023-03-16 03:10:15.000000 cikuu-2022.8.2/uvirun/penlykvr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6558 2023-05-04 10:29:10.000000 cikuu-2022.8.2/uvirun/sbert_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/single_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32687 2023-04-30 03:58:22.000000 cikuu-2022.8.2/uvirun/spacy_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4320 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/textacy_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2089 2023-03-04 12:51:44.000000 cikuu-2022.8.2/uvirun/trans_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4113 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/unmasker_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8742 2023-03-04 12:51:34.000000 cikuu-2022.8.2/uvirun/util_fastapi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45795 2023-03-04 12:51:41.000000 cikuu-2022.8.2/uvirun/uviredis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37415 2023-04-13 09:21:47.000000 cikuu-2022.8.2/uvirun/yulk-nac.py
```

### Comparing `cikuu-2022.8.1/api/c4.py` & `cikuu-2022.8.2/api/c4.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/api/chunk.py` & `cikuu-2022.8.2/api/chunk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/api/common.py` & `cikuu-2022.8.2/api/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/api/dm.py` & `cikuu-2022.8.2/api/dm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/api/es.py` & `cikuu-2022.8.2/api/es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/api/feishu.py` & `cikuu-2022.8.2/api/feishu.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/api/mynac.py` & `cikuu-2022.8.2/api/mynac.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/api/sntjson-es.py` & `cikuu-2022.8.2/api/sntjson-es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/api/wget.py` & `cikuu-2022.8.2/api/wget.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/app/dmdsk/__init__.py` & `cikuu-2022.8.2/app/dmdsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/app/dmdsk/app_navbar.py` & `cikuu-2022.8.2/app/dmdsk/app_navbar.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/app/dmdsk/func/lemma.py` & `cikuu-2022.8.2/app/dmdsk/func/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/app/dmdsk/func/trp.py` & `cikuu-2022.8.2/app/dmdsk/func/trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/app/dmdsk/index.py` & `cikuu-2022.8.2/app/dmdsk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/cikuu.egg-info/SOURCES.txt` & `cikuu-2022.8.2/cikuu.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -182,14 +182,15 @@
 en/arc/__init__.py
 en/arc/sntjson-innodb.py
 en/arc/sntjson-naclite.py
 en/arc/sntjson-naclite0.py
 en/arc/sntjson-nacp-20230206.py
 en/arc/sntjson-nacp-20230207.py
 gecdsk/__init__.py
+gecdsk/essays.py
 lit/__init__.py
 lit/common.py
 lit/essay.py
 lit/filling.py
 lit/fillmul.py
 lit/hello-pages.py
 lit/index.py
@@ -232,35 +233,33 @@
 lit/yulk/func/wordrank.py
 pipe/__init__.py
 pipe/__main__.py
 pipe/redisgec8180.py
 pipe/xgecv1.py
 rabbitmq/__init__.py
 redisr/__init__.py
+redisr/glove-get.py
+redisr/glove.py
+redisr/sntvec-get.py
 sbert/__init__.py
 sbert/__main__.py
 sbert/hello.py
+sbert/redis-sntvec.py
+sbert/sntvec-so.py
 sbert/sntvec.py
 so/__init__.py
 so/__main__.py
-so/corpusly.py
-so/cos.py
+so/dis-eev.py
+so/dis-essays.py
+so/dis-folder.py
 so/dsk.py
-so/esapi.py
-so/eslite.py
-so/kps-si.py
+so/folder.py
+so/index-dis.py
 so/load.py
-so/loadc4.py
 so/loades.py
-so/sikps.py
-so/sntbr.py
-so/sntvec.py
-so/spacytok.py
-so/test-lowercase.py
-so/tocos.py
 sqlite/__init__.py
 sqlite/__main__.py
 util/__init__.py
 util/__main__.py
 util/annotate.py
 util/bcp.py
 util/c4data.py
```

### Comparing `cikuu-2022.8.1/dic/__init__.py` & `cikuu-2022.8.2/dic/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/adjlist.py` & `cikuu-2022.8.2/dic/adjlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/advlist.py` & `cikuu-2022.8.2/dic/advlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/bnc_wordlist.py` & `cikuu-2022.8.2/dic/bnc_wordlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -127263,16 +127263,19 @@
 001f11e0: 6b65 6c69 686f 6f64 2869 2c62 6e63 5f77  kelihood(i,bnc_w
 001f11f0: 6f72 646c 6973 742e 6765 7428 732c 3029  ordlist.get(s,0)
 001f1200: 202c 7369 5f73 756d 2c62 6e63 5f73 756d   ,si_sum,bnc_sum
 001f1210: 2920 2920 666f 7220 732c 6920 696e 2073  ) ) for s,i in s
 001f1220: 692e 6974 656d 7328 295d 0a0a 6465 6620  i.items()]..def 
 001f1230: 7361 7665 2829 3a0a 0969 6d70 6f72 7420  save():..import 
 001f1240: 6a73 6f6e 0a09 7769 7468 206f 7065 6e28  json..with open(
-001f1250: 2762 6e63 5f77 6f72 646c 6973 7427 2c27  'bnc_wordlist','
-001f1260: 7727 2920 6173 2066 773a 200a 0909 6677  w') as fw: ...fw
-001f1270: 2e77 7269 7465 286a 736f 6e2e 6475 6d70  .write(json.dump
-001f1280: 7328 5b20 2877 2c20 6629 2066 6f72 2077  s([ (w, f) for w
-001f1290: 2c66 2069 6e20 626e 635f 776f 7264 6c69  ,f in bnc_wordli
-001f12a0: 7374 2e69 7465 6d73 2829 5d29 290a 0a69  st.items()]))..i
-001f12b0: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
-001f12c0: 5f6d 6169 6e5f 5f22 3a20 200a 0973 6176  _main__":  ..sav
-001f12d0: 6528 29                                  e()
+001f1250: 2762 6e63 5f77 6f72 646c 6973 742e 6a73  'bnc_wordlist.js
+001f1260: 6f6e 272c 2777 2729 2061 7320 6677 3a20  on','w') as fw: 
+001f1270: 0a09 0966 772e 7772 6974 6528 206a 736f  ...fw.write( jso
+001f1280: 6e2e 6475 6d70 7328 626e 635f 776f 7264  n.dumps(bnc_word
+001f1290: 6c69 7374 2920 2920 0a09 0923 6677 2e77  list) ) ...#fw.w
+001f12a0: 7269 7465 286a 736f 6e2e 6475 6d70 7328  rite(json.dumps(
+001f12b0: 5b20 2877 2c20 6629 2066 6f72 2077 2c66  [ (w, f) for w,f
+001f12c0: 2069 6e20 626e 635f 776f 7264 6c69 7374   in bnc_wordlist
+001f12d0: 2e69 7465 6d73 2829 5d29 290a 0a69 6620  .items()]))..if 
+001f12e0: 5f5f 6e61 6d65 5f5f 203d 3d20 225f 5f6d  __name__ == "__m
+001f12f0: 6169 6e5f 5f22 3a20 200a 0973 6176 6528  ain__":  ..save(
+001f1300: 29                                       )
```

### Comparing `cikuu-2022.8.1/dic/confu_set.py` & `cikuu-2022.8.2/dic/confu_set.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/ecdic.py` & `cikuu-2022.8.2/dic/ecdic.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/errants.py` & `cikuu-2022.8.2/dic/errants.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/essays.py` & `cikuu-2022.8.2/dic/essays.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/frame.py` & `cikuu-2022.8.2/dic/frame.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/lemma_lex.py` & `cikuu-2022.8.2/dic/lemma_lex.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/lemma_mf.py` & `cikuu-2022.8.2/dic/lemma_mf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/lemma_scale.py` & `cikuu-2022.8.2/dic/lemma_scale.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/lex_lemma.py` & `cikuu-2022.8.2/dic/lex_lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/mwe_disconj.py` & `cikuu-2022.8.2/dic/mwe_disconj.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/mwe_pv.py` & `cikuu-2022.8.2/dic/mwe_pv.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/n_is_sb.py` & `cikuu-2022.8.2/dic/n_is_sb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/nounlist.py` & `cikuu-2022.8.2/dic/nounlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/nyt_wc.py` & `cikuu-2022.8.2/dic/nyt_wc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/orals.py` & `cikuu-2022.8.2/dic/orals.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/propbank.py` & `cikuu-2022.8.2/dic/propbank.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/stoplist.py` & `cikuu-2022.8.2/dic/stoplist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/to_redislite.py` & `cikuu-2022.8.2/dic/to_redislite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/verbform.py` & `cikuu-2022.8.2/dic/verbform.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/verblist.py` & `cikuu-2022.8.2/dic/verblist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/verbtag.py` & `cikuu-2022.8.2/dic/verbtag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/vocab.py` & `cikuu-2022.8.2/dic/vocab.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/word_awl.py` & `cikuu-2022.8.2/dic/word_awl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/word_bits.py` & `cikuu-2022.8.2/dic/word_bits.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/word_grade.py` & `cikuu-2022.8.2/dic/word_grade.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/word_gsl1.py` & `cikuu-2022.8.2/dic/word_gsl1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/word_gsl2.py` & `cikuu-2022.8.2/dic/word_gsl2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/word_idf.py` & `cikuu-2022.8.2/dic/word_idf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/word_oov.py` & `cikuu-2022.8.2/dic/word_oov.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/word_pos.py` & `cikuu-2022.8.2/dic/word_pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/word_scale.py` & `cikuu-2022.8.2/dic/word_scale.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/wordattr.py` & `cikuu-2022.8.2/dic/wordattr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/wordcnt.py` & `cikuu-2022.8.2/dic/wordcnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/wordlist.py` & `cikuu-2022.8.2/dic/wordlist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/wordlist_ed1.py` & `cikuu-2022.8.2/dic/wordlist_ed1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/wordnet_verb.py` & `cikuu-2022.8.2/dic/wordnet_verb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/wordpos.py` & `cikuu-2022.8.2/dic/wordpos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dic/words.py` & `cikuu-2022.8.2/dic/words.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/__init__.py` & `cikuu-2022.8.2/dsk/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/__main__.py` & `cikuu-2022.8.2/dsk/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/common.py` & `cikuu-2022.8.2/dsk/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/dm.py` & `cikuu-2022.8.2/dsk/dm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/dsk-hello.py` & `cikuu-2022.8.2/dsk/dsk-hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/dsk-to-dskmkf.py` & `cikuu-2022.8.2/dsk/dsk-to-dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/dsk2023.py` & `cikuu-2022.8.2/dsk/dsk2023.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/dskapi.py` & `cikuu-2022.8.2/dsk/dskapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/dskes.py` & `cikuu-2022.8.2/dsk/dskes.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/dskmkf.py` & `cikuu-2022.8.2/dsk/dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/dskmkf_fastapi.py` & `cikuu-2022.8.2/dsk/dskmkf_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/dsktrain.py` & `cikuu-2022.8.2/dsk/dsktrain.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/essaydm.py` & `cikuu-2022.8.2/dsk/essaydm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/gears-xdsk.py` & `cikuu-2022.8.2/dsk/gears-xdsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/gecv1.py` & `cikuu-2022.8.2/dsk/gecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/index.py` & `cikuu-2022.8.2/dsk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/innersim.py` & `cikuu-2022.8.2/dsk/innersim.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/json-to-dskmkf.py` & `cikuu-2022.8.2/dsk/json-to-dskmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/kvrdsk.py` & `cikuu-2022.8.2/dsk/kvrdsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/load.py` & `cikuu-2022.8.2/dsk/load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/mkf.py` & `cikuu-2022.8.2/dsk/mkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/mqconsume.py` & `cikuu-2022.8.2/dsk/mqconsume.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/pingyu.py` & `cikuu-2022.8.2/dsk/pingyu.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/score.py` & `cikuu-2022.8.2/dsk/score.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/sntsdims.py` & `cikuu-2022.8.2/dsk/sntsdims.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/test.py` & `cikuu-2022.8.2/dsk/test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/tok-hello.py` & `cikuu-2022.8.2/dsk/tok-hello.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/uvidsk.py` & `cikuu-2022.8.2/dsk/uvidsk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/wps-gec.py` & `cikuu-2022.8.2/dsk/wps-gec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/wps-xgec.py` & `cikuu-2022.8.2/dsk/wps-xgec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/wps7000.py` & `cikuu-2022.8.2/dsk/wps7000.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/xessay.py` & `cikuu-2022.8.2/dsk/xessay.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/xgecv1-test.py` & `cikuu-2022.8.2/dsk/xgecv1-test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/xgecv1.py` & `cikuu-2022.8.2/dsk/xgecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/xmkf.py` & `cikuu-2022.8.2/dsk/xmkf.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/xsnt-gec.py` & `cikuu-2022.8.2/dsk/xsnt-gec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/dsk/xsnt-spacy.py` & `cikuu-2022.8.2/dsk/xsnt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/__init__.py` & `cikuu-2022.8.2/en/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/__main__.py` & `cikuu-2022.8.2/en/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/annotate.py` & `cikuu-2022.8.2/en/annotate.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/arc/__init__.py` & `cikuu-2022.8.2/en/arc/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/arc/sntjson-innodb.py` & `cikuu-2022.8.2/en/arc/sntjson-innodb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/arc/sntjson-naclite.py` & `cikuu-2022.8.2/en/arc/sntjson-naclite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/arc/sntjson-naclite0.py` & `cikuu-2022.8.2/en/arc/sntjson-naclite0.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/arc/sntjson-nacp-20230206.py` & `cikuu-2022.8.2/en/arc/sntjson-nacp-20230206.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/arc/sntjson-nacp-20230207.py` & `cikuu-2022.8.2/en/arc/sntjson-nacp-20230207.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4-cl.py` & `cikuu-2022.8.2/en/c4-cl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4-fts.py` & `cikuu-2022.8.2/en/c4-fts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4-gram-upload.py` & `cikuu-2022.8.2/en/c4-gram-upload.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4-gram.py` & `cikuu-2022.8.2/en/c4-gram.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4-grams.py` & `cikuu-2022.8.2/en/c4-grams.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4-np.py` & `cikuu-2022.8.2/en/c4-np.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4-trp.py` & `cikuu-2022.8.2/en/c4-trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4cl.py` & `cikuu-2022.8.2/en/c4cl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4gram-mysql.py` & `cikuu-2022.8.2/en/c4gram-mysql.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4gram-upsert.py` & `cikuu-2022.8.2/en/c4gram-upsert.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4gram.py` & `cikuu-2022.8.2/en/c4gram.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4gramcl.py` & `cikuu-2022.8.2/en/c4gramcl.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4matcher.py` & `cikuu-2022.8.2/en/c4matcher.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4np.py` & `cikuu-2022.8.2/en/c4np.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4postag.py` & `cikuu-2022.8.2/en/c4postag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4skenp.py` & `cikuu-2022.8.2/en/c4skenp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4tree.py` & `cikuu-2022.8.2/en/c4tree.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4trp.py` & `cikuu-2022.8.2/en/c4trp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/c4vp.py` & `cikuu-2022.8.2/en/c4vp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/clause.py` & `cikuu-2022.8.2/en/clause.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/dims.py` & `cikuu-2022.8.2/en/dims.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/docfts.py` & `cikuu-2022.8.2/en/docfts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/docjson.py` & `cikuu-2022.8.2/en/docjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/es-index.py` & `cikuu-2022.8.2/en/es-index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/esbulk.py` & `cikuu-2022.8.2/en/esbulk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/esfile.py` & `cikuu-2022.8.2/en/esfile.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/esjson.py` & `cikuu-2022.8.2/en/esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/exchunk.py` & `cikuu-2022.8.2/en/exchunk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/exphrase.py` & `cikuu-2022.8.2/en/exphrase.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/extrp.py` & `cikuu-2022.8.2/en/extrp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/havc.py` & `cikuu-2022.8.2/en/havc.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/kpsi.py` & `cikuu-2022.8.2/en/kpsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/lempostag.py` & `cikuu-2022.8.2/en/lempostag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/nacp.py` & `cikuu-2022.8.2/en/nacp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/nlp-lit.py` & `cikuu-2022.8.2/en/nlp-lit.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/nlp-lmdb.py` & `cikuu-2022.8.2/en/nlp-lmdb.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/postag.py` & `cikuu-2022.8.2/en/postag.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/shav.py` & `cikuu-2022.8.2/en/shav.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/silite.py` & `cikuu-2022.8.2/en/silite.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/snt-esjson.py` & `cikuu-2022.8.2/en/snt-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-fts.py` & `cikuu-2022.8.2/en/sntjson-fts.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-kpsnt.py` & `cikuu-2022.8.2/en/sntjson-kpsnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-mysql.py` & `cikuu-2022.8.2/en/sntjson-mysql.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-nacp.py` & `cikuu-2022.8.2/en/sntjson-nacp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-parse-snt.py` & `cikuu-2022.8.2/en/sntjson-parse-snt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-si.py` & `cikuu-2022.8.2/en/sntjson-si.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-spacy.py` & `cikuu-2022.8.2/en/sntjson-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-topk.py` & `cikuu-2022.8.2/en/sntjson-topk.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-tosnt.py` & `cikuu-2022.8.2/en/sntjson-tosnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-trpx.py` & `cikuu-2022.8.2/en/sntjson-trpx.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sntjson-vp.py` & `cikuu-2022.8.2/en/sntjson-vp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/spacybs-esjson.py` & `cikuu-2022.8.2/en/spacybs-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/spacybs.py` & `cikuu-2022.8.2/en/spacybs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/spider-esjson.py` & `cikuu-2022.8.2/en/spider-esjson.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/sqlsi.py` & `cikuu-2022.8.2/en/sqlsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/terms.py` & `cikuu-2022.8.2/en/terms.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/verbnet.py` & `cikuu-2022.8.2/en/verbnet.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/xsnt.py` & `cikuu-2022.8.2/en/xsnt.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/en/zset-load.py` & `cikuu-2022.8.2/en/zset-load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/gecdsk/__init__.py` & `cikuu-2022.8.2/gecdsk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 if not hasattr(spacy, 'nlp'):
 	from spacy.lang import en
 	spacy.sntbr		= (inst := en.English(), inst.add_pipe("sentencizer"))[0]
 	spacy.sntpid	= lambda essay: (pid:=0, [ ( pid := pid + 1 if "\n" in snt.text else pid,  (snt.text, pid))[-1] for snt in  spacy.sntbr(essay).sents] )[-1]
 	spacy.nlp		= spacy.load('en_core_web_sm')
 
 def parse(arr:dict={"essay":"English is a internationaly language which becomes importantly for modern world. In China, English is took to be a foreigh language which many student choosed to learn. They begin to studying English at a early age. They use at least one hour to learn English knowledges a day. Even kids in kindergarten have begun learning simple words. That's a good phenomenan, for English is essential nowadays. In addition to, some people think English is superior than Chinese. In me opinion, though English is for great significance, but English is after all a foreign language. it is hard for people to see eye to eye. English do help us read English original works, but Chinese helps us learn a true China. Only by characters Chinese literature can send off its brilliance. Learning a country's culture, especial its classic culture, the first thing is learn its language. Because of we are Chinese, why do we give up our mother tongue and learn our owne culture through a foreign language?"}
-		, asdsk:bool=True, gec_local:bool=False, topk_gec:int=64, diffmerge:bool=False,  timeout:int=9, ttl:int=79200):  
+		, asdsk:bool=True, use_gec:bool=True, topk_gec:int=64, diffmerge:bool=False,  timeout:int=9, ttl:int=79200):  
 	''' # 依赖 dskhost 和 gechost	'''
 	try:
-		essay	= arr.get("essay", arr.get('doc','')).strip()
+		essay	= arr.get("essay", arr.get('doc','')).strip() if isinstance(arr, dict) else arr # arr is dict/str 
 		if not essay: return {"failed":"empty essay"}
 		sntpids = spacy.sntpid(essay)  # [(snt,pid) ]
 		snts	= [snt.strip() for snt,pid in sntpids ] 	
 		if hasattr(redis, 'r') : [redis.r.xadd('xsnt-spacy', {'snt':snt}, maxlen=30000) for snt in snts if snt]  # notify:  spacy/gec , added maxlen 2022.10.15
 
-		sntdic	= requests.post(f"http://{gechost}/xgec-snts?name=xsnts&timeout={timeout}&ttl={ttl}", json=snts).json() if not gec_local else {}
+		sntdic	= requests.post(f"http://{gechost}/xgec-snts?name=xsnts&timeout={timeout}&ttl={ttl}", json=snts).json() if use_gec else {}
 		docs	= getdocs(snts, ttl) 
 		input	= [ mkf_input(i,snts[i],sntdic[snts[i]], [t.text for t in doc], [t.text for t in (doc if snts[i] == sntdic.get(snts[i],snts[i]) else getdoc(sntdic.get(snts[i],snts[i])) ) ], doc, diffmerge)  for i, doc in enumerate(docs)]
 		dsk		= requests.post(f"http://{dskhost}/parser", data={"q":json.dumps({"snts":input, "rid":"10"} if asdsk else input).encode("utf-8")}).json()
 		return dsk
 	except Exception as ex:
 		print(">>parse_dsk Ex:", ex, "\t|", arr)
```

### Comparing `cikuu-2022.8.1/lit/__init__.py` & `cikuu-2022.8.2/lit/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/common.py` & `cikuu-2022.8.2/lit/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/es/__init__.py` & `cikuu-2022.8.2/lit/es/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/es/index.py` & `cikuu-2022.8.2/lit/es/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/essay.py` & `cikuu-2022.8.2/lit/essay.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/fillmul.py` & `cikuu-2022.8.2/lit/fillmul.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/hello-pages.py` & `cikuu-2022.8.2/lit/hello-pages.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/index.py` & `cikuu-2022.8.2/lit/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/mock-scoring.py` & `cikuu-2022.8.2/lit/mock-scoring.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/penly/index.py` & `cikuu-2022.8.2/lit/penly/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/penly-resend.py` & `cikuu-2022.8.2/lit/penly-resend.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/redis-dump.py` & `cikuu-2022.8.2/lit/redis-dump.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/reorder.py` & `cikuu-2022.8.2/lit/reorder.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/restore.py` & `cikuu-2022.8.2/lit/restore.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/scoring.py` & `cikuu-2022.8.2/lit/scoring.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/single.py` & `cikuu-2022.8.2/lit/single.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/sntspolish.py` & `cikuu-2022.8.2/lit/sntspolish.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/sntupgrade.py` & `cikuu-2022.8.2/lit/sntupgrade.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/student-input.py` & `cikuu-2022.8.2/lit/student-input.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/teacher-admin.py` & `cikuu-2022.8.2/lit/teacher-admin.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/YULK.py` & `cikuu-2022.8.2/lit/yulk/YULK.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/common.py` & `cikuu-2022.8.2/lit/yulk/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/bipos.py` & `cikuu-2022.8.2/lit/yulk/func/bipos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/cola.py` & `cikuu-2022.8.2/lit/yulk/func/cola.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/common.py` & `cikuu-2022.8.2/lit/yulk/func/common.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/corpuslist.py` & `cikuu-2022.8.2/lit/yulk/func/corpuslist.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/es.py` & `cikuu-2022.8.2/lit/yulk/func/es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/given-expect.py` & `cikuu-2022.8.2/lit/yulk/func/given-expect.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/gramx-single.py` & `cikuu-2022.8.2/lit/yulk/func/gramx-single.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/lemma.py` & `cikuu-2022.8.2/lit/yulk/func/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/lemvs.py` & `cikuu-2022.8.2/lit/yulk/func/lemvs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/pos.py` & `cikuu-2022.8.2/lit/yulk/func/pos.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/posvs.py` & `cikuu-2022.8.2/lit/yulk/func/posvs.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/style-in-mul.py` & `cikuu-2022.8.2/lit/yulk/func/style-in-mul.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/func/wordrank.py` & `cikuu-2022.8.2/lit/yulk/func/wordrank.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/index.py` & `cikuu-2022.8.2/lit/yulk/index.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/lit/yulk/lemma.py` & `cikuu-2022.8.2/lit/yulk/lemma.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/pipe/__init__.py` & `cikuu-2022.8.2/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/pipe/__main__.py` & `cikuu-2022.8.2/pipe/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/pipe/redisgec8180.py` & `cikuu-2022.8.2/pipe/redisgec8180.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/pipe/xgecv1.py` & `cikuu-2022.8.2/pipe/xgecv1.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/rabbitmq/__init__.py` & `cikuu-2022.8.2/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/redisr/__init__.py` & `cikuu-2022.8.2/redisr/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/sbert/__main__.py` & `cikuu-2022.8.2/sbert/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/sbert/hello.py` & `cikuu-2022.8.2/sbert/hello.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 #Sentences are encoded by calling model.encode()
 embeddings = model.encode(sentences)
 
 #Print the embeddings
 for sentence, embedding in zip(sentences, embeddings):
     print("Sentence:", sentence)
-    print("Embedding:", embedding)
+    print("Embedding:", len(embedding)) # 384
     print("")
```

### Comparing `cikuu-2022.8.1/sbert/sntvec.py` & `cikuu-2022.8.2/sbert/sntvec.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/setup.py` & `cikuu-2022.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time: 2022-2-13
 #############################################
  
 from setuptools import setup, find_packages
  
 setup(
   name = "cikuu",
-  version = "2022.8.1",
+  version = "2022.8.2",
   keywords = ("pip"),
   description = "cikuu tools",
   long_description = "add replace into soinit",
   license = "MIT Licence",
  
   url = "http://www.cikuu.com",
   author = "cikuu",
```

### Comparing `cikuu-2022.8.1/so/__main__.py` & `cikuu-2022.8.2/so/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 # 2023.5.1  .# 2022-2-13  cp from cikuu/bin/es.py 
-import so, requests,time
-
-def addfolder(self, folder:str, pattern=".txt", idxname=None): 
-	''' folder -> docbase, 2022.1.23 '''
-	if idxname is None : idxname=  folder
-	print("addfolder started:", folder, idxname, self.es, flush=True)
-	if not self.es.indices.exists(index=idxname): self.es.indices.create(index=idxname, body=config)
-	for root, dirs, files in os.walk(folder):
-		for file in files: 
-			if file.endswith(pattern):
-				self.add(f"{folder}/{file}", idxname = idxname) 
-				print (f"{folder}/{file}", flush=True)
-	print("addfolder finished:", folder, idxname, self.es, flush=True)
+import so, requests,time,os
 
 def add(infile, idxname="testdoc", taglist:str=None):
 	''' add doc only , 2023.5.1 '''
-	import hashlib
-	if not requests.es.indices.exists(index=idxname): requests.es.indices.create(index=idxname, body=so.config)
+	so.check(idxname)
 	start = time.time()
 	text = open(infile, 'r').read().strip() 
-	did	 = hashlib.md5(text.encode("utf8")).hexdigest()
+	did	 = so.md5(text)
 	requests.es.index(index=idxname, body={"did": f"doc-{did}", "doc":text,  "filename": infile, 'type':'doc', 'tags':[] if taglist is None else taglist.strip().split(',') if isinstance(taglist, str) else taglist }, id = f"doc-{did}")
 	print(f"{infile} is finished, \t| using: ", time.time() - start) 
 
+def addfolder(folder:str, idxname:str=None, pattern:str=".txt"): 
+	''' folder -> esindex '''
+	if idxname is None : idxname=  folder
+	print("addfolder started:", folder, idxname, requests.es, flush=True)
+	for root, dirs, files in os.walk(folder):
+		for file in files: 
+			if file.endswith(pattern):
+				add(f"{folder}/{file}", idxname = idxname, taglist=folder) 
+				print (f"{folder}/{file}", flush=True)
+	print("addfolder finished:", folder, idxname, requests.es, flush=True)
+
 def init(idxname):
 	''' init a new index '''
 	if requests.es.indices.exists(index=idxname):requests.es.indices.delete(index=idxname)
 	requests.es.indices.create(index=idxname, body=so.config) #, body=snt_mapping
 	print(">>finished " + idxname )
 
+def drop(idxname): 
+	''' drop a index ''' 
+	print ( requests.es.indices.delete(index=idxname) )
+
 if __name__ == '__main__':
-	#print( requests.eshost)
 	import fire
 	fire.Fire()
 
 '''
+
+1. ubuntu@dicvec-scivec-jukuu-com-flair-64-245:~/cikuu/pypi/so$ python __main__.py addfolder inaugural
+2. ubuntu@dicvec-scivec-jukuu-com-flair-64-245:~/cikuu/pypi/so$ python sntbr.py inaugural
+58
+sntbr indexing finished: inaugural, 	| using:  54.86855387687683
+
+python sntbr.py inaugural --debug true --postag true
+
 POST /policy_document/policy_document/222/_update
 {
   "doc": {
     "tags":["VIP"]
   }
 }
```

### Comparing `cikuu-2022.8.1/so/corpusly.py` & `cikuu-2022.8.2/uvirun/es1_fastapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,236 +1,248 @@
-# 2022.3.20 cp from corpusly-es.py ,  for  python -m so.corpusly uvirun ,   load , ..  support both cmd and restapi 
-# 2022.2.6  cp from corpusly.py ,  only ES, no redis  | uvicorn corpusly-es:app --host 0.0.0.0 --port 19200 --reload
-import json,os,re, requests,traceback,fire, time,math,collections , hashlib
-from collections import	defaultdict, Counter
-
-from fastapi import FastAPI, File, UploadFile,Form, Body
-from uvirun import * 
-app.title = "corpusly-ES"
-app.tm = "2022.2.26"
-
-os.environ['eshost'] = 'es.corpusly.com' # tmp , to be removed later 
-from so import * 
-import en  #from en import * #import en # need 3.1.1
-from en import terms,verbnet
-from en.dims import essay_to_dims
-attach = lambda doc: ( terms.attach(doc), verbnet.attach(doc), doc.user_data )[-1]  # return ssv, defaultdict(dict)
-
-@app.get("/corpus/warmup")
-def corpus_warmup():
-	return requests.put(f"http://{eshost}:{esport}/_cluster/settings", json={"persistent": {"search.max_buckets": 1000000}}).text
+# 2022.6.30 cp from uvicorn corpusly-19200:app --host 0.0.0.0 --port 19200 --reload
+from uvirun import *
+from util import likelihood
+
+requests.eshost		= os.getenv('eshost', 'es.corpusly.com:9200')
+# to be removed later, when cikuu is updated
+kwic	= lambda cp, w, topk=3 : [ re.sub(rf"\b({w})\b", f"<b>{w}</b>", row[0]) for row in rows(f"select snt from {cp} where type = 'snt' and match (snt, '{w}') limit {topk}")]
+
+@app.get('/es/typesum', tags=["es"])
+def typesum(type:str='snt', cp:str='clec'):
+	return requests.post(f"http://{requests.eshost}/_sql", json={"query":f"select count(*) from {cp} where type='{type}'"}).json()['rows'][0][0]
+
+@app.get('/es/kpsum', tags=["es"])
+def kpsum(kp:str="dobj:open_VERB:NOUN_door", cp:str='clec'):
+	arr = requests.post(f"http://{requests.eshost}/{cp}/_search", json={
+"query": {
+  "bool":{
+      "filter": [ 
+      {"term":{"type":"snt"}},
+      {"term":{"kps": kp}} #"dobj:open_VERB:NOUN_door"
+        ]
+  }
+},   
+"track_total_hits": True
+}).json()
+	return arr.get('hits',{}).get('total',{}).get("value",0) 
+
+@app.get('/es/kpcnt', tags=["es"])
+def kp_cnt(kps:str="ccomp:consider_VERB|dobj:consider_VERB|vtov:consider_VERB|vvbg:consider_VERB", cp:str='clec'):
+	arr =  requests.post(f"http://{requests.eshost}/{cp}/_search", json={
+	  "query": { "match": {"type": "snt"}   }, 
+	  "track_total_hits": True,
+	  "size":0,
+	  "aggs": {
+		"myagg": {
+		  "terms": {
+			"field": "kps",
+			 "include": kps
+		  }
+		}
+	  }
+	}).json() 
+	return [ (row['key'], row['doc_count']) for row in arr["aggregations"]["myagg"]["buckets"] ]
+	#[('ccomp:consider_VERB', 114), ('dobj:consider_VERB', 81), ('vvbg:consider_VERB', 5), ('vtov:consider_VERB', 2)]
+
+@app.get('/es/kpsnt', tags=["es"])
+def kp_snt(kp:str="dobj:open_VERB:NOUN_door", cp:str='clec', topk:int=5):
+	arr =  requests.post(f"http://{requests.eshost}/{cp}/_search", json={
+"query": {
+  "bool":{
+      "filter": [ 
+      {"term":{"type":"snt"}},
+      {"term":{"kps":"dobj:open_VERB:NOUN_door"}}
+        ]
+  }
+}
+}).json()
+	return [ row['_source']['snt'] for row in arr['hits']['hits'] ]
+
+@app.get('/es/kpcntsnt', tags=["es"])
+def kp_cnt_snt(kp:str="dobj:open_VERB:NOUN_door", cp:str='clec', topk:int=5):
+	return requests.post(f"http://{requests.eshost}/{cp}/_search", json={
+  "query": { "match": {"type": "snt"}   }, 
+  "size":0,
+  "aggs": {
+    "myagg": {
+      "terms": {
+        "field": "kps",
+         "include": kp  #"dobj:have_VERB:NOUN_dream"
+      },
+    "aggs" : {
+                "snt" : {
+                    "top_hits": { "_source": {"includes":"snt" }, "size": topk
+                    }
+                }
+            }
+
+    }
+  }
+}).json()["aggregations"]["myagg"]["buckets"][0]
+# {'key': 'dobj:open_VERB:NOUN_door', 'doc_count': 28, 'snt': {'hits': {'total': {'value': 28, 'relation': 'eq'}, 'max_score': 2.5384653, 'hits': [{'_index': 'clec', '_type': '_doc', '_id': '5657', '_score': 2.5384653, '_source': {'snt': 'And I ran to the bus quickly, asked the driver open the door.'}}, {'_index': 'clec', '_type': '_doc', '_id': '47892', '_score': 2.5384653, '_source': {'snt': 'When you open the door you can see that on each side of the room there is a double-layer bed .Between the two book shelves there are two desks and two benches, at which I usually read and write .At one up coner of the room ,there is a TV set that by watching it I can known all the news of our country and the others of the world .'}}, {'_index': 'clec', '_type': '_doc', '_id': '58153', '_score': 2.5384653, '_source': {'snt': 'He had to get out of bed, get his canes, walk 12 feet, open the bedroom door, walk 43 feet, and open the front door -- all in 15 seconds.'}}, {'_index': 'clec', '_type': '_doc', '_id': '34992', '_score': 2.5384653, '_source': {'snt': 'It reformed the past economic system in our country and opened the door of our courtry to bring into anvanced sciente and technology.'}}, {'_index': 'clec', '_type': '_doc', '_id': '71183', '_score': 2.5384653, '_source': {'snt': 'Then television is introduced to us and opens the door for us to travel in those places and enables us to see what happens there, to hear what those people say, and to feel what they experience only on that little screen.'}}]}}}
+
+@app.get('/es/trpcntsnt', tags=["es"])
+def trp_cnt_snt(trp:str="dobj:open_VERB:NOUN_.*", cp:str='clec', term_size:int=1000, topk:int=1):
+	arr = requests.post(f"http://{requests.eshost}/{cp}/_search", json={
+  "query": { "match": {"type": "snt"}   }, 
+  "track_total_hits": True, 
+  "size":0,
+  "aggs": {
+    "myagg": {
+      "terms": {
+        "field": "kps",
+         "include": trp, #"dobj:open_VERB:NOUN_.*"
+		 "size":term_size 
+      },
+    "aggs" : {
+                "snt" : {
+                    "top_hits": { "_source": {"includes":"snt" }, "size":topk
+                    }
+                }
+            }
+
+    }
+  }
+}).json()
+	return [ (row['key'], row['doc_count'], row['snt']['hits']['hits'][0]['_source']['snt']) for row in arr["aggregations"]["myagg"]["buckets"] ]
+
+
+@app.get('/es/xcnt/{cp}/{type}/{column}')
+def es_xcnt( column:str='lex', cp:str='dic', type:str='tok', where:str="", order:str="order by cnt desc limit 10",  name:str="es.corpusly.com:9200" ):
+	''' where:  and lem='book'  | JSONCompactColumns
+	* select lex,count(*) cnt from dic where type = 'tok' and lem= 'book' group by lex '''
+	query  = f"select {column}, count(*) cnt from {cp} where type = '{type}' {where} group by {column} {order}"
+	res = requests.post(f"http://{name}/_sql",json={"query": query}).json() 
+	return [  { column: ar[0], "cnt": ar[1]} for ar in res['rows'] ] 
+
+@app.get('/es/sqlrows')
+def sqlrows(query="select lem, count(*) cnt  from gzjc where type = 'tok' and pos != 'PUNCT' group by lem order by cnt desc limit 10", perc_column:str=None):
+	''' perc_column: cnt  
+	# select gov, count(*) cnt from gzjc where type = 'tok' and lem='door' and pos='NOUN' and dep='dobj' group by gov
+	# select lem, count(*) cnt from gzjc where type = 'tok' and gov='open_VERB' and pos='NOUN' and dep='dobj' group by lem
+	'''
+	res = requests.post(f"http://{requests.eshost}:{requests.esport}/_sql",json={"query": query}).json() 
+	arr = [  dict(zip([ ar['name'] for ar in res['columns'] ] , ar)) for ar in res['rows'] ] 
+	if perc_column:  
+		sump = sum([ ar[perc_column] for ar in arr]) + 0.0001
+		[ ar.update({'perc': round(ar[perc_column] / sump, 4) }) for ar in arr]
+	return arr
+
+@app.post('/es/sqlrows')
+def es_sqlrows_post(querys:list=["show tables","select lem, count(*) cnt  from gzjc where type = 'tok' and pos != 'PUNCT' group by lem order by cnt desc limit 10"], asdic:bool=True):
+	return {query: sqlrows(query) for query in querys} if asdic else [ sqlrows(query) for query in querys ]
+
+@app.post('/es/rows')
+def named_rows(arr:dict={'query':"select lem, count(*) cnt from dic where type='tok' and  tag='VBG' group by lem order by cnt desc ", 'columns':["lem", "tagcnt"]}):
+	''' 2022.6.21 '''
+	return [  dict(zip(arr['columns'], ar)) for ar in rows( arr.get('query', "") ) ] 
+
+@app.get('/es/termcnt')
+def es_query_termcnt(cps:str="clec,gzjc", query:str="select gov, count(*) cnt from __0__ where type = 'tok' and lem='door' and pos='NOUN' and dep='dobj' group by gov", topk:int=10 ):
+	''' added 2022.6.19 '''
+	map = defaultdict(dict)
+	for cp in cps.strip().split(','): 
+		sql = query.replace("__0__", cp ) 
+		for row in rows(sql): # assume the first one is the key 
+			for i in range(1, len(row)): 
+				map[ row[0]][ f"{cp}_{i}" if i > 1 else cp] = row[i]
+	df = pd.DataFrame(map).fillna(0).transpose()
+	for col in df.columns:
+		df[f"{col}_perc"] = round((df[col] / df[col].sum()) * 100, 2)
+	if topk > 0 : df = df.sort_values(df.columns[0], ascending=False)
+	arr = [ dict(dict(row), **{"term": index} ) for index, row in df.iterrows()] 
+	return arr[0:topk] if topk > 0  else arr 
 
-@app.get("/corpus/indexlist/")
+@app.get("/es/indexlist/")
 def corpus_indexlist(verbose:bool=False):
-	''' added 2022.2.7 '''
-	names =  [name for name, type, kind in sql("show tables") if not name.startswith(".") and type == 'TABLE' and kind == 'INDEX']
-	return {name: dict(sql(f"select type, count(*) cnt from {name} group by type")) for name in names} if verbose else names
-
-@app.post('/corpus/indexdoc')
-def indexdoc(arr:dict={"body":"The quick fox jumped over the lazy dog. Justice delayed is justice denied.", "filename":"a.txt"}, idxname:str='testidx', essay_field:str='body', tags_commalist:str='', refresh_index:bool = False):  
-	''' arr:  { 'body':, 'filename':  }, optional:  title/tag, ...  updated 2021.11.5 ''' 
-	if refresh_index: es.indices.delete(index=idxname)
-	if not es.indices.exists(index=idxname): es.indices.create(index=idxname, body=config) 
-	filename = arr.get('filename', hashlib.md5(arr.get(essay_field,'').encode(encoding='UTF-8')).hexdigest()) 
-	body = arr.get(essay_field,'')
-	if not body : return f"empty, on '{essay_field}' found"
-
-	docsnts = spacy.snts(body) 
-	for idx, snt in enumerate(docsnts):
-		doc = spacy.nlp(snt)
-		es.index(index=idxname, id = f"{filename}-{idx}", body= {'type':'snt', 'snt':snt,
-				'postag':' '.join([f"{t.text}_{t.lemma_}_{t.pos_}_{t.tag_}" if t.text == t.text.lower() else f"{t.text}_{t.text.lower()}_{t.lemma_}_{t.pos_}_{t.tag_}" for t in doc]),
-				'src': f"{filename}-{idx}",  'tc': len(doc)})
-		ssv = attach(doc) 
-		for id, sour in ssv.items():
-			sour.update({"src":f"{filename}-{idx}", "filename": filename}) # sid
-			es.index(index=idxname, id = f"{filename}-{idx}-{id}", body= sour)
-
-	arr.update( essay_to_dims(body)) # duplicated computing doc 
-	arr.update({'type':'doc', "sntnum":len(docsnts), "wordnum": sum([ len(snt) for snt in docsnts]), 'tag': tags_commalist.split(','), 'tm': time.time()})
-	es.index(index = idxname,  id = filename, body = arr)
-	return docsnts 
-
-@app.post("/corpus/uploadfile/")
-async def create_upload_file(index:str="testidx", file: UploadFile = File(...), refresh_index:bool = False):
-	''' folder is the index name '''
-	content = await file.read()
-	return indexdoc({'body':content.decode().strip(), 'index':index, 'filename':file.filename}, idxname=index, refresh_index=refresh_index)  
-
-@app.get("/corpus/sql")
-def corpus_sql(query:str="select lem, count(*) cnt  from gzjc where type = 'tok' and pos != 'PUNCT' group by lem order by cnt desc limit 10"):
-	return sql(query)
-
-@app.post('/corpus/es_search') 
-def es_search(query:dict, type:str='doc', index:str="testidx", size:int=10):  
-	''' "query" =  {"match": { "type":"trp"} } , updated 2021.11.5 '''
-	return es.search(index=index,  query=query if query else {"match": { "type":type} } if type  else {"match_all": {}}, size=size)
-
-@app.post("/corpus/trp/dep/govs")
-def corpus_dep_govs(corpus_list:list, w:str="door", rel:str="dobj_VERB_NOUN"):
-	''' ["clec","gzjc"] 
-	* door/dobj_VERB_NOUN -> open, close , ...,  2022.2.7	'''
-	return { cp: sql(f"select gov, count(*) cnt from {cp} where type ='trp' and rel='{rel}' and dep='{w}' group by gov order by cnt desc") for cp in corpus_list }
-@app.post("/corpus/trp/gov/deps")
-def corpus_gov_deps(corpus_list:list, w:str="open", rel:str="dobj_VERB_NOUN"):
-	''' ["clec","gzjc"] '''
-	return {cp: sql(f"select dep, count(*) cnt from {cp} where type ='trp' and rel='{rel}' and gov='{w}' group by dep order by cnt desc") for cp in corpus_list }
-
-@app.get("/corpus/chunk")
-def corpus_chunk(lem:str="book", segtype:str='np', cp:str="clec", topk:int=10):
-	''' segtype: np/vp/adjp/advp/vtov/vvbg '''
-	return sql(f"select chunk, count(*) cnt from {cp} where type = '{segtype}' and lem = '{lem}' group by chunk order by cnt desc limit {topk}")
-
-@app.post("/corpus/lemma/pos")
-def corpus_lemma_pos(corpus_list:list, lem:str="book"):
-	''' ["clec","gzjc"] '''
-	return {cp: sql(f"select pos, count(*) cnt from {cp} where type = 'tok' and lem ='{lem}' and pos != 'PROPN' group by pos") for cp in corpus_list }
-@app.post("/corpus/lemma/lex")
-def corpus_lemma_lex(corpus_list:list, lem:str="book"):
-	''' ["clec","gzjc"] '''
-	return {cp: sql(f"select low, count(*) cnt from {cp} where type = 'tok' and low ='{lem}' group by low") for cp in corpus_list }
-
-@app.get("/corpus/tok_head/by_dep")
-def corpus_tok_by_dep(cp:str="gzjc", dep:str="dative", topk:int=10):
-	''' 'dative' head '''
-	return sql(f"select head, count(*) cnt  from {cp} where type = 'tok' and dep = '{dep}' group by head order by cnt desc limit {topk}")
-
-@app.get("/corpus/sum/by_dep")
-def corpus_sntsum_by_dep(cp:str="gzjc", dep:str="dative"):
-	''' how many 'dative' in current corpus? 
-	dep:  dative/xcomp/ccomp/relcl/vprd/csubj/nsubjpass
-	'''
-	return sql(f"select count(*)  from {cp} where type = 'tok' and dep = '{dep}'" )
+	names =  [ar['name'] for ar in sqlrows("show tables")  if not ar['name'].startswith(".") and ar['type'] == 'TABLE' and ar['kind'] == 'INDEX'] # {"catalog":"elasticsearch","name": ".apm-custom-link", "type": "TABLE",    "kind": "INDEX"  },
+	return [ dict( dict(rows(f"select type, count(*) cnt from {name} group by type")), **{"name":name} ) for name in names] if verbose else names
 
-@app.get("/corpus/pos/rank")
-def corpus_pos_rank(cp:str='clec', pos:str="VERB", topk:int=50):
-	''' set pos=None when return all lemmas , POS:VERB/NOUN/ADJ/ADV/None '''
-	return sql(f"select lem, count(*) cnt from {cp} where type = 'tok' and pos = '{pos}' group by lem order by cnt desc limit {topk}" ) if pos else sql(f"select lem, count(*) cnt from {cp} where type = 'tok' and pos != 'PUNCT' group by lem order by cnt desc limit {topk}")
-@app.post("/corpus/lemmas/cnt")
-def corpus_lemmas_cnt(lemmas:list, cp:str='clec', pos:str="VERB"):
-	''' ["be","have","get"] '''
-	words = ",".join([f"'{lem}'" for lem in lemmas] )
-	return sql(f"select lem, count(*) cnt from {cp} where type = 'tok' and pos = 'VERB' and lem in ({words}) group by lem") if pos else sql(f"select lem, count(*) cnt from {cp} where type = 'tok' and lem in ({words}) group by lem")
- 
-@app.get("/corpus/word/rank")
-def corpus_word_rank(cp:str='clec', topk:int=50): return sql(f"select low, count(*) cnt from {cp} where type = 'tok' group by low order by cnt desc limit {topk}" )
-@app.get("/corpus/trp/rank")
-def corpus_trp_rank(cp:str='clec', rel:str="dobj_VERB_NOUN", topk:int=10): return sql(f"select gov, dep, count(*) cnt from {cp} where type = 'trp' and rel= '{rel}' group by gov,dep order by cnt desc limit {topk}" )
-@app.get("/corpus/kwic")
-def corpus_kwic(cp:str='clec', w:str="opened", topk:int=10): return sql(f"select snt, postag from {cp} where type = 'snt' and match (snt, '{w}') limit {topk}" )
-
-@app.post("/{cp}/ids")
-def corpus_ids(_ids:list, cp:str='gzjc'):  return ids(_ids, cp),
-
-@app.get("/corpus/trp/snts")
-def corpus_trp_snts(gov:str='open', rel:str='dobj_VERB_NOUN', dep:str='door', cp:str='clec', topk:int=10): 
-	''' snts of trp '''
-	rows = sql(f"select src from {cp} where type = 'trp' and gov='{gov}' and rel='{rel}' and dep='{dep}' limit {topk}")
-	sql	= {
-    "query": {
-        "ids" : {
-            "type" : "_doc",
-            "values" : [row[0] for row in rows] #clec:snt-34993,  clec:snt-32678
-			}
-		}
-	}
-	return requests.post(f"http://{eshost}:{esport}/{cp}/_search/", json=sql).json()
+@app.get("/es/stats")
+def corpus_stats(names:str=None, types:str="doc,snt,np,tok,trp,vp"):
+	''' doc,snt,np,tok,simple_sent,vtov,vvbg,vp, added 2022.5.21 '''
+	names = name.strip().split(',') if names else [ar['name'] for ar in sqlrows("show tables")  if not ar['name'].startswith(".") and ar['type'] == 'TABLE' and ar['kind'] == 'INDEX']
+	types = types.replace(",", "','")
+	return [ dict( dict(rows(f"select type, count(*) cnt from {name} where type in ('{types}') group by type")), **{"name":name} ) for name in names]
+
+@app.get("/es/kwic")
+def corpus_kwic(cp:str='dic', w:str="opened", topk:int=10, left_tag:str="<b>", right_tag:str="</b>"): # expected_tc:int=15,
+	''' search snt using word,  | select snt,postag, tc from gzjc where type = 'snt' and match(snt, 'books') | 2022.6.19 '''
+	return [ {"snt": re.sub(rf"\b({w})\b", f"{left_tag}{w}{right_tag}", snt), "tc": tc } for snt, postag, tc in rows(f"select snt, postag, tc from {cp.strip().split(',')[0]} where type = 'snt' and match (snt, '{w}') limit {topk}")]
+
+@app.get("/es/mf")
+def corpus_mf(cps:str="gzjc,clec", w:str="considered", topk:int=3, with_snt:bool=False):
+	dic =  {cp: round(1000000 * phrase_num(w, cp) / (sntnum(cp)+0.1), 2 ) for cp in cps.strip().split(',') }
+	return [ {"cp":cp, "mf":mf, "snts": json.dumps(kwic(cp, w, topk)) } for cp,mf in dic.items()] if with_snt else [ {"cp":cp, "mf":mf } for cp,mf in dic.items()]
+
+@app.get("/es/srcsnts")
+def corpus_srcsnts(query:str="select src from gzjc where type='tok' and lem='book' and pos='NOUN' limit 10",highlight:str='book', left_tag:str="<b>", right_tag:str="</b>"):  #, cp:str='gzjc'
+	''' '''
+	cp = query.split("where")[0].strip().split('from')[-1].strip()
+	srclist = "','".join([ src for src, in rows(query)])
+	return [{'snt':re.sub(rf"\b({highlight})\b", f"{left_tag}{highlight}{right_tag}", snt)} for snt, in rows(f"select snt from {cp} where type='snt' and src in ('{srclist}')")]
+
+@app.get("/es/lempos/snts")
+def lempos_snts(cp:str='gzjc', lem:str='book', pos:str='VERB', topk:int=3, left_tag:str="<b>", right_tag:str="</b>"): 
+	''' "select snt from gzjc where type = 'snt' and kp = 'book_VERB' limit 2" , added 2022.6.24 '''
+	query = f"select snt from {cp} where type = 'snt' and kp = '{lem}_{pos}' limit {topk}"
+	return [{'snt':re.sub(rf"\b({lem})\b", f"{left_tag}{lem}{right_tag}", snt)} for snt, in rows(query)]	
+
+@app.get("/es/trp/snts")
+def trp_snts(cp:str='gzjc', word:str='door', rel:str='~dobj_VERB_NOUN', cur:str='open',  topk:int=3): 
+	query = f"select snt from {cp} where type = 'snt' and kp = '{rel[1:]}/{cur} {word}' limit {topk}" if rel.startswith('~') else f"select snt from {cp} where type = 'snt' and kp = '{rel}/{word} {cur}' limit {topk}"
+	print (query, flush=True)
+	return [{'snt':snt} for snt, in rows(query)]
 
-@app.get("/corpus/match_phrase")
+@app.get("/es/match_phrase")
 def corpus_match_phrase(phrase:str='opened the box', cp:str='clec', topk:int=10):  return match_phrase(phrase, cp, topk)
-@app.get("/corpus/match_phrase_num")
+@app.get("/es/match_phrase_num")
 def corpus_phrase_num(phrase:str='opened the box', cp:str='clec', topk:int=10): return phrase_num(phrase, cp, topk)["hits"]["total"]["value"]
 
-@app.post("/corpus/mf")
-def corpus_mf(corpus_list:list, input:str="consider", type:str='lemma'):
-	''' ["gzjc","clec"] ,  type:lemma/phrase '''
-	return {cp: round(1000000 * es.lemnum(input, cp) / (es.sntnum(cp)+0.1), 2 ) for cp in corpus_list} if type =='lemma' else {cp: round(1000000 * es.phrase_num(input, cp) / (es.sntnum(cp)+0.1), 2 ) for cp in corpus_list}
-
-@app.get("/corpus/nearby")
+@app.get("/es/nearby")
 def corpus_nearby(lem:str="environment", corpus:str='spin', poslist:str="'NOUN','ADJ','VERB'", topk:int=20):
 	''' words nearby '''
-	rows = requests.post(f"http://{eshost}:{esport}/_sql",json={"query": f"select src from {corpus} where type = 'tok' and lem = '{lem}'"}).json()['rows']
+	rows = requests.post(f"http://{requests.eshost}:{requests.esport}/_sql",json={"query": f"select src from {corpus} where type = 'tok' and lem = '{lem}'"}).json()['rows']
 	snts = "','".join([row[0] for row in rows])
-	res = requests.post(f"http://{eshost}:{esport}/_sql",json={"query": f"select lem from {corpus} where type = 'tok'  and pos in ({poslist}) and src in ('{snts}')" }).json()['rows']
+	res = requests.post(f"http://{requests.eshost}:{requests.esport}/_sql",json={"query": f"select lem from {corpus} where type = 'tok'  and pos in ({poslist}) and src in ('{snts}')" }).json()['rows']
 	si = Counter() 
 	[si.update({row[0]:1}) for row in res if row[0] != lem and not row[0] in spacy.stoplist ]
 	return Counter({ s:i * spacy.wordidf.get(s, 0) for s,i in si.items()}).most_common(topk)
 
-@app.get("/corpus/wordlevel")
-def corpus_wordlevel(index:str='gzjc', tag:str=None, topk:int=10): 
-	''' wordlevel:  awl/gsl1/gsl2/others , added 2021.11.5 '''
-	import dic 
-	if not hasattr(corpus_wordlevel, 'wordlevel'): corpus_wordlevel.word_level = dic.word_level() 
-	rows = sql(f"select low, count(*) from {index} where type = 'tok' group by low")
-	return [ (s,i, word_level.get(s.lower(), "others"))  for s,i in rows] if not tag else Counter(dict([ (s,i) for s,i in rows if tag == corpus_wordlevel.word_level.get(s.lower(), "others")])).most_common(topk)
-
-@app.get('/corpus/hybchunk')
-def corpus_hybchunk(hyb:str='the _NNS of', index:str='gzjc', size:int=-1, topk:int=10):
-	''' the _NNS of -> {the books of: 13, the doors of: 7} , added 2021.10.13 '''
-	return hybchunk(hyb, index, size, topk)
-
-@app.get('/corpus/truncate_index')
-def truncate_index(index:str='testidx'):
-	return requests.post(f"http://{eshost}:{esport}/{index}/_delete_by_query?conflicts=proceed", json={"query": { "match_all": {} }}).json()
-@app.get('/corpus/delete_file')
-def delete_file(filename:str, index:str='testidx'):
-	return requests.post(f"http://{eshost}:{esport}/{index}/_delete_by_query?conflicts=proceed", json={"query": { "match": { "filename": filename} }}).json()
-
-@app.post('/corpus/dualarr_keyness')
-def dualarr_keyness(src:dict, tgt:dict, sum1:float=None, sum2:float=None, threshold:float=0.0, leftonly:bool=False): 
-	'''  "src": {"one":2, "two":12}, "tgt": {"three":3, "one":1}, added 2021.10.24  '''
-	if not sum1: sum1 = sum([i for s,i in src.items()])
-	if not sum2: sum2 = sum([i for s,i in tgt.items()])
-	words = set(src.keys()) | set(tgt.keys()) if not leftonly else set(src.keys())
-	res  = [(w, src.get(w,0), tgt.get(w,0), sum1, sum2, likelihood(src.get(w,0.01), tgt.get(w,0.01), sum1, sum2))  for w in words]
-	res.sort(key=lambda a:a[-1], reverse=True)
-	return [ar for ar in res if abs(ar[-1]) > threshold ]
-
-@app.post('/corpus/txtkeyness')
-def text_keyness(txt:str= Form(...), pos:str='VERB', corpus:str='inau', skip_NNP:bool=True, threshold:float=0.0): 
-	''' keyness of (txt, corpus), pos:LEX/VERB/NOUN, added 2021.10.16  '''
-	src = dict(requests.post(f"http://spacy.wrask.com/nlp/lexcnt", json={'txt':txt, 'pos':pos,'skip_NNP':skip_NNP}).json())
-	tgt = dict(requests.post(f"http://{eshost}:{esport}/_sql",json={"query": f"select lem, count(*) from {corpus} where type = 'tok' and pos='{pos}' group by lem"}).json()['rows'])
-	return dualarr_keyness(src, tgt, threshold) 
-
-@app.get('/corpus/dualsql_keyness')
-def text_keyness(sql1:str= "select lem,  count(*) from inau where type = 'tok' and pos='VERB' and filename in ('1989-Bush.txt')  group by lem", sql2:str="select lem,  count(*) from inau where type = 'tok' and pos='VERB' group by lem", threshold:float=0.0): 
-	''' keyness of sql1, sql2, added 2021.10.24  '''
-	src = dict(requests.post(f"http://{eshost}:{esport}/_sql",json={"query": sql1}).json()['rows'])
-	tgt = dict(requests.post(f"http://{eshost}:{esport}/_sql",json={"query": sql2}).json()['rows'])
-	return dualarr_keyness(src, tgt, threshold) 
-
-@app.get('/sqles/count_of_item')
-def sqles_si_group(q:str="SELECT triple.gov FROM sentnest where corpus='gzjc' and triple.rel = 'dobj_VERB_NOUN' and triple.dep='door'", es_host:str="127.0.0.1:{esport}", topk:int=None):
-	''' SELECT tok.pos FROM sentnest where tok.lem = 'sound' ,2021.10.18 '''
-	si = Counter()
-	res = requests.post(f"http://{es_host}:{esport}/_sql", json={"query":q}).json()
-	[ si.update({word:1}) for word, in res['rows'] ]
-	return si.most_common(topk)
-
-@app.get('/corpus/init_index')
-def init_index(idxname:str='testidx'):  newindex(idxname)
-
-class util(object): 
-	def __init__(self): pass
-
-	def hello(self):  
-		''' show corpuslist '''
-		print (  corpus_indexlist() )
-
-	def init(self, idxname):  
-		''' init an index '''
-		newindex(idxname) 
-
-	def uvirun(self, port) : 
-		''' python -m so.corpusly uvirun 80 '''
-		uvicorn.run(app, host='0.0.0.0', port=port)
-
-	def load(self, infile, idxname) : 
-		''' load text file into index, 
-		find . -name "*.txt" -exec python -m so.corpusly load {} inau \;   '''
-		with open(infile, 'r',encoding='utf-8') as fp:
-			indexdoc({"body": fp.read(), 'filename': infile}, idxname = idxname) 
-		print ("finished:", infile ) 
 
-if __name__ == "__main__":  
-	fire.Fire(util) 
+@app.get('/es/attach_dsk')
+def attach_dsk(idxname:str='essay'):  
+	dsk		= requests.post(f"http://{gecdskhost}/gecdsk", json=arr).json()
+	snts	= [mkf.get('meta',{}).get('snt','') for mkf in dsk.get('snt',[])]
+	arr.update({"type":"doc", "did": did, "sntnum":len(snts), "score":float(dsk.get('info',{}).get("final_score",0)), "snts": json.dumps(snts) })
+	newdoc.es.index(index = index,  id = did, body = arr)
+	newdoc.es.index(index = index,  id = f"{did}-dims", body = dict(dsk.get('doc',{}), **{"type":"dims", "did":did}) )
+
+if __name__ == "__main__":   #uvicorn.run(app, host='0.0.0.0', port=80)
+	#print (trp_cnt_snt())	
+	#print (cursor_rows("select rid,uid, essay from essay")) 
+
+	requests.post(f"http://{requests.eshost}/essay/_delete_by_query?conflicts=proceed", json={"query": { "match": {"type": "dsk"} }}).text
+	for rid,uid, essay in cursor_rows("select rid,uid, essay from essay where rid='230537' "):
+		dsk		= requests.post(f"http://gpu120.wrask.com:8180/gecdsk", json={"essay_or_snts":essay, "rid":rid, "uid":uid}).json()
+		snts	= [mkf.get('meta',{}).get('snt','') for mkf in dsk.get('snt',[])]
+		requests.put(f"http://{requests.eshost}/essay/_doc/rid-{rid}:uid-{uid}:dsk", json={"type":"dsk", "did":f"rid-{rid}:uid-{uid}", "sntnum":len(snts), "score":float(dsk.get('info',{}).get("final_score",0)), "snts": json.dumps(snts) })
+		requests.put(f"http://{requests.eshost}/essay/_doc/rid-{rid}:uid-{uid}:dims", json=dict(dsk.get('doc',{}), **{"type":"dims", "did":f"rid-{rid}:uid-{uid}"}) 
+
+'''
+GET /gzjc/_search
+{
+  "query": {
+    "match": {"type":"frame"}
+  },
+  	"track_total_hits": true,
+	  "size":0,
+	  "aggs": {
+		"myagg": {
+		  "terms": {
+			"field": "frame",
+			 "include": "return.*"
+		  }
+		}
+	  }
+}
+'''
```

### Comparing `cikuu-2022.8.1/so/dsk.py` & `cikuu-2022.8.2/so/dsk.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,8 +47,19 @@
             index=log['_index'],
             doc_type='_doc',
             id=log['_id'],
             body={'doc':log['_source']} # 
         )
 
 ubuntu@dicvec-scivec-jukuu-com-flair-64-245:~/cikuu/pypi/so/inaugural$ find . -name "*.txt" -exec python ../__main__.py add {} --taglist inau \;
+
+{
+    "query": {
+        "bool": {
+            "must": [
+                {"match": {"one_field" : "one_value"}},
+                {"match": {"another_field" : "another_value"}},
+            ]
+        }
+    }
+}
 '''
```

### Comparing `cikuu-2022.8.1/so/load.py` & `cikuu-2022.8.2/so/load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/so/loades.py` & `cikuu-2022.8.2/so/loades.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/so/sntbr.py` & `cikuu-2022.8.2/so/folder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,61 @@
-# 2023.5.2,  dsk including  sntbr, if not dsk, start standalone sntbr  
-import so, requests,time, fire,json, spacy
-
-if not hasattr(spacy, 'nlp'):
-	from spacy.lang import en
-	spacy.sntbr		= (inst := en.English(), inst.add_pipe("sentencizer"))[0]
-	#spacy.nlp		= spacy.load('en_core_web_sm')
-
-def run(idxname, debug:bool=False):
-	''' testdoc, 2023.5.2 '''
-	so.check(idxname) 
-	start = time.time()
-	rows = so.cursor_rows(f"select did, doc from {idxname} where type ='doc' and did is not null")
+# 2023.5.2,  loading inau 
+import requests,time, fire,json, spacy # so 
+from __init__ import *  # for debug , change to : from so import * 
+nlp = spacy.load('en_core_web_sm')
+
+def run(folder:str, idxname:str=None, pattern:str=".txt", debug:bool=False, reset:bool=False): 
+	''' inau, 2023.5.2 '''
+	if idxname is None: idxname = folder 
+	if reset: drop(idxname)
+	check(idxname) 
+	addfolder(folder, idxname, pattern)
+	
+	rows = cursor_rows(f"select did, doc from {idxname} where type ='doc' and did is not null ")
 	print (len(rows), flush=True)
-	for did, essay in rows: 
-		if debug: print ( did, essay[0:20], flush=True) 
-		doc = spacy.sntbr(essay) 
-
-		snts = [ sp.text.strip() for sp in doc.sents ]
-		if not requests.es.exists(index=idxname, id=f"snts-{did}"):
-			requests.es.index(index=idxname, body={"did": f"snts-{did}", 'pid': did, 'type':'snts', 'snts': snts, 'sntnum':len(snts) }, id = f"snts-{did}")
-
-		for sp in doc.sents
-			snt = sp.text.strip()
-			sntmd5 = so.md5(snt)
-			if not requests.es.exists(index=idxname, id=f"snt-{sntmd5}"): # sntbr 
-				requests.es.index(index=idxname, body={"did": f"snt-{sntmd5}",'pid': did, 'type':'snt', 'sent': snt, 'tc': len(sp)}, id = f"snt-{sntmd5}")
+	for did, doc in rows: 
+		if debug : print ( did, doc[0:20], flush=True) 
+		tdoc = sntbr(doc) 
+		for i, sp in enumerate(tdoc.sents): 
+			snt = sp.text.strip() 
+			sntid = f"{did}:snt-{i}"
+			doc = nlp(snt) 
+			arr = skenp(doc)
+			arr.update({"did":did, "sntid":sntid, "type":"snt", "tc": len(sp),"snt":snt}) #			update(idxname, sntid, skenp(doc)) #requests.es.update(index=idxname, id =sid, body= skenp(doc))  #partial update 
+			esindex(idxname, sntid, arr ) 
+			for t in doc: 
+				esindex(idxname, f"{sntid}:tok-{t.i}", {"did": did, 'sntid': sntid, 'i': t.i, 'type':'tok', 'lex': t.text, 'lem':t.lemma_, 'pos':t.pos_, 'tag':t.tag_, 'dep':t.dep_, 'govlem': t.head.lemma_, 'govpos': t.head.pos_ })
 
-	print(f"sntbr indexing finished: {idxname}, \t| using: ", time.time() - start) 
+	print(f"tok indexing finished: {idxname}") 
 
-if __name__ == '__main__':
-	run('testdoc', debug=True)
+if __name__ == '__main__': 	#run('testdoc', debug=True)
+	#run('inau') 
 	fire.Fire(run)
 
 '''
+fire.es.delete_by_query(index=fire.index, conflicts='proceed', body={"query":{"match":{"eid":eid}}})
+
 POST /policy_document/policy_document/222/_update
 {
   "doc": {
     "tags":["VIP"]
   }
+
+GET /inau/_search
+{
+    "query": {
+        "bool": {
+            "must": [
+                {"match": {"type" : "tok"}},
+                {"match": {"tag" : "VBD"}}
+            ]
+        }
+    }
+}
+
 }
 
   es.update( # excpetion here 
             index=log['_index'],
             doc_type='_doc',
             id=log['_id'],
             body={'doc':log['_source']} #
```

### Comparing `cikuu-2022.8.1/so/test-lowercase.py` & `cikuu-2022.8.2/so/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # 2022.5.11 updated , add sqlrow for EachRowJson
 # 2022.2.13 created 
-import requests,json, os, math,re,traceback,fire,time
+import requests,json, os, math,re,traceback,fire,time,sys,hashlib
 from elasticsearch import Elasticsearch,helpers
 from collections import	defaultdict, Counter
-import pandas as pd 
-import warnings
+import warnings #import pandas as pd # remove dependency 2023.4.7
 warnings.filterwarnings("ignore")
 
-if not hasattr(requests, 'eshost'):
-	requests.eshost	= os.getenv("eshost", "172.17.0.1:9200") 
+if not hasattr(requests, 'eshost'): # or use: so.eshost ?
+	requests.eshost	= os.getenv("eshost", "172.17.0.1:9200" if 'linux' in sys.platform else 'sntvec.wrask.com:9200') 
 	requests.es		= Elasticsearch([ f"http://{requests.eshost}" ])  
 
 config = {  
 		"settings" : {
 			"refresh_interval": "1s",
 			"number_of_shards": "3",
 			"max_result_window":"2147483647",
@@ -22,15 +21,14 @@
 			  "filter": {
 				"postag_filter": {
 				  "type": "pattern_capture",   # add _contact_VERB as a term , => _contact_VERB with  ( _([a-z]+)_(VERB|NOUN|ADJ|ADV)
 				  "preserve_original": "false",
 				  "patterns": [
 					#"(^([^_]+)_[a-z]+[,\\.$]?)",  
 					"(^[^_]+)",   # first lex
-					"(^[^_]+_)",   # first lex to lower 
 					"(_[a-z]+_[VERB|NOUN|ADJ|ADV]+)", # lex_tag_lem_pos , _contact_VERB (VERB|NOUN|ADJ|ADV)
 					"(_[a-z]+_VERB_[VBD|VBP|VBG|VBZ|VB]+_)",  # except VBN, 2023.3.20
 					"(_[a-z]+_VERB_VBN_)", 
 					#"(_[a-zA-Z\\-\\.\\'\\$0-9]+)$",  # remove _NP5,  _NP5 => _NP 
 					"(_[a-zA-Z,\\-\\.\\'\\$\\*]+)",  # _^ _ADJ _, _NOUN _VERB , _open/VERB 
 					#"(_[^\\w]+)_",
 					#"([^\\w])_"
@@ -38,20 +36,14 @@
 				},
 				"postag_filter1": {
 					  "type": "pattern_replace",
 					  "pattern": "(^_([a-z]+)_([VERB|NOUN|ADJ|ADV]))",
 					  "replacement": "$2/$3",  # _open_VERB => open/VERB
 					  "all": False
 					},
-				"postag_filter_headlow": {
-					  "type": "pattern_replace",
-					  "pattern": "(^([^_]+)_)",
-					  "replacement": "$2", #  "replacement": "$1|lowercase"
-					  "all": False
-					},
 				"postag_filterV": {
 					  "type": "pattern_replace",
 					  "pattern": "(^_([a-z]+)(_VERB_[VBD|VBP|VBG|VBZ|VB]+)_)",
 					  "replacement": "$2/V",  # _open_VERB_VBD => open/V
 					  "all": False
 					},
 				"postag_filterVBN": {
@@ -88,15 +80,15 @@
 				},
 				"unique_filter": {
 				  "type": "unique",
 				  "only_on_same_position": "true"
 				}
 			  },
 			  "analyzer": {
-				"postag_ana": {"filter": ["postag_filter", "postag_filter_headlow", "postag_filterV", "postag_filterVBN", "postag_filter1",  "postag_filter2", "unique_filter"], "type": "custom", "tokenizer": "whitespace" }, #"lowercase",
+				"postag_ana": {"filter": ["postag_filter", "postag_filterV", "postag_filterVBN", "postag_filter1",  "postag_filter2", "unique_filter"], "type": "custom", "tokenizer": "whitespace" }, #"lowercase",
 				"path_ana": {"type": "custom", "tokenizer": "path-tokenizer"},
 				"path_ana3": {"type": "custom", "tokenizer": "path-tokenizer3"},
 				"feedback_ana": {"type": "custom", "tokenizer": "feedback-tokenizer"},
 				"err_ana": {"type": "custom",  "tokenizer": "path-tokenizer1"  },
 				"chunk_ana": {"type": "custom", "tokenizer": "path-tokenizer2" },
 				"kp_ana": { "filter": ["lowercase"], "type": "custom", "tokenizer": "keyword"}
 			  },
@@ -133,17 +125,20 @@
 			"ratio": { "type": "float", "index": "false"},
 			"memo": { "type": "keyword", "index": "false"}, # to store some memo info, for show only
 			"sent": { "type": "keyword", "index": "false"},
 			"offset": { "type": "float"},
 			"final_score": { "type": "float"},
 			"sid": { "type": "keyword"},
 			"sntid": { "type": "keyword"},
+			"pid": { "type": "keyword"}, # parentid 
+			"paraid": { "type": "keyword"}, # paragraph
 			"id": { "type": "keyword"},
 			"rid": { "type": "keyword"},
 			"did": { "type": "keyword"},
+			"vpat": { "type": "keyword"},
 			"ibeg": { "type": "integer"},
 			"iend": { "type": "integer"},
 			"len": { "type": "integer"}, # [start, start + len) 
 			"docid": { "type": "keyword"},
 			"uid": { "type": "keyword"},
 			"eid": { "type": "keyword"},
 			"sntnum": { "type": "integer"},
@@ -153,17 +148,19 @@
 			"vers": { "type": "integer"},
 			"ver": { "type": "integer"},
 			"ct": { "type": "integer"},
 			"lem": { "type": "keyword"},
 			"frame": { "type": "keyword"}, # flair/frame 
 			"lempos": { "type": "keyword"}, # for wordattr , ie: open/VERB 
 			"lex": { "type": "keyword"},
+			"word": { "type": "keyword"},
 			"low": { "type": "keyword"},
 			"pos": { "type": "keyword"},
 			"tag": { "type": "keyword"},
+			"tags": { "type": "keyword"},
 			"ctag": { "type": "keyword"}, # chunk tag
 			"stag": { "type": "keyword"}, # snt tag
 			"term": { "type": "keyword"},
 			"gpos": { "type": "keyword"},  "glem": { "type": "keyword"}, "gtag": { "type": "keyword"},
 			"lem1": { "type": "keyword"},  "lem2": { "type": "keyword"}, "tag1": { "type": "keyword"}, "tag2": { "type": "keyword"},
 			"VERB": { "type": "keyword"},  "NOUN": { "type": "keyword"}, "ADV": { "type": "keyword"},  "ADJ": { "type": "keyword"},
 			"advcl": { "type": "keyword"},  "acomp": { "type": "keyword"}, "dobj": { "type": "keyword"},  "nsubj": { "type": "keyword"},"xcomp": { "type": "keyword"},  "amod": { "type": "keyword"},  "advmod": { "type": "keyword"},
@@ -248,18 +245,23 @@
 					  "pos": {"type": "keyword"},
 					  "tag": {"type": "keyword"},
 					  "dep": {"type": "keyword"},
 					  "gpos": {"type": "keyword"},
 					  "glem": {"type": "keyword"}
 				   }
 				},
-
+			 "wordvec": {
+			   "type": "dense_vector",
+			   "dims": 300,  # gpu55:/home/cikuu/gensim-data/glove-wiki-gigaword-300
+			   "index": True,
+			   "similarity": "l2_norm"
+			 },
 			 "sntvec": {
 			   "type": "dense_vector",
-			   "dims": 384,
+			   "dims": 384,  # sbert, all-MiniLM-L6-v2
 			   "index": True,
 			   "similarity": "l2_norm"
 			 },
 			 "skevec": {  # _NP jumped over _NP
 			   "type": "dense_vector",
 			   "dims": 384,
 			   "index": True,
@@ -283,24 +285,26 @@
 			"dims": { "type": "keyword", "index": "false" , "ignore_above": 50},
 			"meta": { "type": "keyword", "index": "false", "ignore_above": 50},
 			"mkf": { "type": "keyword", "index": "false", "ignore_above": 50 },
 			"tc": {"type": "integer" , "index": "false"},
 			"sc": {"type": "integer" , "index": "false"},
 			"isum": {"type": "integer" , "index": "false"},
 			"md5": { "type": "text", "store": "false", "norms":"false"},
+			"md5snt": { "type": "keyword", "index": "false"},
+			"sntmd5": { "type": "keyword", "index": "false"}, # added 2023.4.4
 			"toks": { "type": "keyword", "index": "false" ,"store": "false"},
 			"snts": { "type": "keyword", "index": "false" },
 			"blob": { "type": "binary", "store": "false"},
 			"zlib": { "type": "binary", "store": "false"},
 			"title": { "type": "text", "analyzer": "standard"},
 			"essay": { "type": "text", "analyzer": "standard"},
 			"body": { "type": "text", "index": "false" },
 			"spacy": { "type": "text", "index": "false" }, # spacy json result 
 			"doc": { "type": "text", "index": "false" },#"doc": { "type": "keyword", "index": "false" ,"store": "false"}, # dim arr of dsk
-			"tm": { "type": "date"}, #"format": "yyyy-MM-dd HH:mm:ss || yyyy-MM-dd || yyyy/MM/dd HH:mm:ss|| yyyy/MM/dd ||epoch_millis"
+			"tm": {"type": "date", "format": "strict_date_optional_time||yyyy-MM-dd HH:mm:ss||epoch_millis"}, #"format": "yyyy-MM-dd HH:mm:ss || yyyy-MM-dd || yyyy/MM/dd HH:mm:ss|| yyyy/MM/dd ||epoch_millis"
 			"timestamp": { "type": "date"},
 			"pubdate": { "type": "date"},
 			"sdate": { "type": "date",  "format": "yyyy-MM-dd"},
 			"csv": { "type": "keyword",  "index": "false"},
 			"tsv": { "type": "keyword",  "index": "false"},
 			"pair": { "type": "keyword",  "index": "false"},
 			"json": { "type": "keyword",  "index": "false"},
@@ -321,35 +325,44 @@
 sntsum	= lambda cp: sql(f"select count(*) cnt from {cp} where type = 'snt'" )[0][0] # added 2022.6.29
 lexsum	= lambda cp: sql(f"select count(*) cnt from {cp} where type = 'tok'" )[0][0] 
 lexnum	= lambda w,cp: sql(f"select count(*) cnt from {cp} where low = '{w}' and type = 'tok'")[0][0] # opened = 70
 lemnum	= lambda w,cp: sql(f"select count(*) cnt from {cp} where lem = '{w}' and type = 'tok'")[0][0] 
 sqlsi	= lambda query: (si:=Counter(), [si.update({row[0]:1}) for row in sql(query)])[0]
 warmup  = lambda : requests.put(f"http://{requests.eshost}/_cluster/settings", json={"persistent": {"search.max_buckets": 1000000}}).text
 kwic	= lambda cp, w, topk=3 : [ re.sub(rf"\b({w})\b", f"<b>{w}</b>", row[0]) for row in rows(f"select snt from {cp} where type = 'snt' and match (snt, '{w}') limit {topk}")]
+check	= lambda idxname : requests.es.indices.create(index=idxname, body=config) if not requests.es.indices.exists(index=idxname) else None
+md5		= lambda text: hashlib.md5(text.encode("utf8")).hexdigest()
 
 def sqlrow(query="select lem, count(*) cnt  from gzjc where type = 'tok' and pos != 'PUNCT' group by lem order by cnt desc limit 10"):
 	''' {'columns': [{'name': 'lem', 'type': 'keyword'}, {'name': 'cnt', 'type': 'long'}], 'rows': [['the', 7552], ['be', 5640], ['and', 3604], ['to', 3561], ['of', 3127], ['a', 2902], ['in', 2687], ['I', 2063], ['have', 1562], ['it', 1311]]} '''
 	res = requests.post(f"http://{requests.eshost}/_sql",json={"query": query}).json() 
 	columns = [ ar['name'] for ar in res['columns'] ]
 	return  [  dict(zip(columns, ar)) for ar in res['rows'] ] #[{'lem': 'the', 'cnt': 7552}, {'lem': 'be', 'cnt': 5640}, {'lem': 'and', 'cnt': 3604}, {'lem': 'to', 'cnt': 3561}, {'lem': 'of', 'cnt': 3127}, {'lem': 'a', 'cnt': 2902}, {'lem': 'in', 'cnt': 2687}, {'lem': 'I', 'cnt': 2063}, {'lem': 'have', 'cnt': 1562}, {'lem': 'it', 'cnt': 1311}]
 
 ## added 2022.7.3
-requests.eshost	= os.getenv('eshost', 'es.corpusly.com:9200') #requests.esname = os.getenv("esname", "es.corpusly.com:9200")
-cursor_sql = lambda query, cursor: requests.post(f"http://{requests.esname}/_sql", json={"query":query, "cursor":cursor}).json() 
-
-def cursor_rows(query="select dep, gov, lem, pos, count(*) cnt from gzjc where type='tok' group by dep, gov, lem, pos"):
+cursor_sql = lambda query, cursor: requests.post(f"http://{requests.eshost}/_sql", json={"query":query, "cursor":cursor}).json() 
+def cursor_rows(query="select did, doc from testdoc where type ='doc' and did is not null"): #select dep, gov, lem, pos, count(*) cnt from gzjc where type='tok' group by dep, gov, lem, pos
 	rows = []				
 	cursor=''
 	while True : 
 		res = cursor_sql(query, cursor)  
 		rows.extend(res['rows'])
 		cursor = res.get('cursor','') 
 		if not cursor: break
 	return rows 
 
+def esindex(idxname, id , source): 
+	''' source = {"did": sid,'pid': did, 'type':'snt', 'snt': sp.text.strip(), 'tc': len(sp)} '''
+	try:
+		requests.es.index(index=idxname, body=source, id = id)
+	except Exception as e:
+		print ("esindex ex:",e, idxname, source, id)
+		exc_type, exc_value, exc_traceback_obj = sys.exc_info()
+		traceback.print_tb(exc_traceback_obj)
+
 def walk(query): 
 	cursor=''
 	while True : 
 		res = cursor_sql(query, cursor)  
 		yield res['rows']
 		cursor = res.get('cursor','') 
 		if not cursor: break
@@ -397,32 +410,24 @@
 		G2 = round(2 * ((a * math.log(a / E1)) + (b * math.log(b / E2))), 2)
 		if minus or  (minus is None and a/c < b/d): G2 = 0 - G2
 		return G2
 	except Exception as e:
 		print ("likelihood ex:",e, a,b,c,d)
 		return 0
 
-#PUT twitter/_mapping {  "properties": {  "email": { "type": "keyword"  }  }}
-#"stroke": { "type": "keyword", "index": "false"},
-def delete_index(cp:str='testidx'): 
-	return requests.delete(f"http://{requests.eshost}:{requests.esport}/{cp}").text #DELETE /twitter
+#PUT twitter/_mapping {  "properties": {  "email": { "type": "keyword"  }  }}#"stroke": { "type": "keyword", "index": "false"},
+def delete_index(cp:str='testidx'): 	return requests.delete(f"http://{requests.eshost}:{requests.esport}/{cp}").text #DELETE /twitter
 def new_empty_index(cp:str='testidx', delete:bool=True): 
 	if delete: requests.delete(f"http://{requests.eshost}:{requests.esport}/{cp}").text
 	return requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}", data={}).text #PUT twitter  {}
-def add_mapping_keyword(kws:list, cp:str='testidx'): 
-	return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{kw}": { "type": "keyword"  }  }}).text for kw in kws]
-def add_mapping_keyword_noindex(kws:list, cp:str='testidx'): 
-	return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{kw}": { "type": "keyword", "index": "false"} }}).text for kw in kws]
-def add_mapping_float(kws:list, cp:str='testidx'): 
-	return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{kw}": { "type": "float"  }  }}).text for kw in kws]
-def add_mapping_integer(kws:list, cp:str='testidx'): 
-	return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{kw}": { "type": "integer"  }  }}).text for kw in kws]
-def add_mapping(dic:dict, cp:str='testidx'): 
-	''' {"num":"integer", "awl":"float", "tag":"keyword"} '''
-	return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{k}": { "type": "{v}"  }  }}).text for k,v in dic.items()]
+def add_mapping_keyword(kws:list, cp:str='testidx'): 		return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{kw}": { "type": "keyword"  }  }}).text for kw in kws]
+def add_mapping_keyword_noindex(kws:list, cp:str='test'):	return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{kw}": { "type": "keyword", "index": "false"} }}).text for kw in kws]
+def add_mapping_float(kws:list, cp:str='testidx'): 			return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{kw}": { "type": "float"  }  }}).text for kw in kws]
+def add_mapping_integer(kws:list, cp:str='testidx'): 		return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{kw}": { "type": "integer"  }  }}).text for kw in kws]
+def add_mapping(dic:dict, cp:str='testidx'):				return [requests.put(f"http://{requests.eshost}:{requests.esport}/{cp}/_mapping/", data={"properties": {  f"{k}": { "type": "{v}"  }  }}).text for k,v in dic.items()] #''' {"num":"integer", "awl":"float", "tag":"keyword"} '''
 
 def bulk(arr, batch=100000, debug=False):
 	''' bulk submit , added 2022.3.27, not tested yet '''
 	if not hasattr(bulk, 'actions'):	bulk.actions=[]
 	bulk.actions.append(arr)  #{'_op_type':'index', '_index':idxname, '_id': did, '_source': arr}
 	if len(bulk.actions) > batch : 
 		try:
@@ -436,48 +441,42 @@
 		print ("bulk submit is called, un-submiited actions len: ", len(bulk.actions)) 
 		if len(bulk.actions) >0 : 
 			helpers.bulk(client=es,actions=bulk.actions, raise_on_error=False)
 			bulk.actions = []	
 
 def ids(_ids:list, cp:str='inau'): 
 	''' ["one","two"] '''
-	sql	= { 
-    "query": {
-        "ids" : {
-            "type" : "_doc",
-            "values" : _ids
-			}
-		}
-	}
+	sql	= { "query": {  "ids" : {    "type" : "_doc",   "values" : _ids }		}	}
 	return requests.post(f"http://{requests.eshost}/{cp}/_search/", json=sql).json()
 
 def term_to_snts(sql): 
 	rows = requests.es.sql(sql) #f"select src from {cp} where type = 'trp' and gov='{gov}' and rel='{rel}' and dep='{dep}' limit {topk}"
-	sql	= {
-    "query": {
-        "ids" : {
-            "type" : "_doc",
+	sql	= { "query": {   "ids" : {   "type" : "_doc",
             "values" : [row[0] for row in rows] #clec:snt-34993,  clec:snt-32678
-			}
-		}
-	}
+			}}	}
 	return requests.post(f"http://{requests.eshost}/{cp}/_search/", json=sql).json()
 
 def match_phrase(phrase:str='opened the box', cp:str='clec', topk:int=10): 
 	''' '''
-	sql	= {
-  "query": {
-    "match_phrase": {
-      "snt": phrase
-    }
-  }
-  , "size": topk
-}
+	sql	= {  "query": { "match_phrase": { "snt": phrase    } }  , "size": topk}
 	return requests.post(f"http://{requests.eshost}/{cp}/_search/", json=sql).json()
 
+def alltrue(must_match:dict={"rid" : 230537,"type" : "sntfd","cate" : "e_snt.nv_agree" }, index:str='essay', topk:int=10): 
+	''' 2023.5.2 '''
+	sql	= { "query": {
+        "bool": {"must": [ {"match": {k:v}} for k,v in must_match.items() ]  }
+    }, "size": topk }
+	return requests.post(f"http://{requests.eshost}/{index}/_search/", json=sql).json()
+
+def lemlist(index:str='essay', pos:str='VERB', topk:int=1000): 
+	''' "aggregations" : { "buckets" : [  {   "key" : "have",   "doc_count" : 70 '''
+	sql = {  "query": {    "match": {"pos":pos}  },  "size" : 0,
+    "aggs" : { "termrank" : { "terms" : { "field" : "lem", "size":1000  }  }    }  }
+	return requests.post(f"http://{requests.eshost}/{index}/_search/", json=sql).json()
+
 phrase_num = lambda phrase, cp='clec', topk=10: match_phrase(phrase, cp, topk)["hits"]["total"]["value"]
 
 addpat	= lambda s : f"{s}_[^ ]*" if not s.startswith('_') else f"[^ ]*{s}[^ ]*"   # if the last one, add $ 
 rehyb   = lambda hyb: ' '.join([ addpat(s) for s in hyb.split()])  #'the_[^ ]* [^ ]*_NNS_[^ ]* of_[^ ]*'
 heads   = lambda chunk:  ' '.join([s.split('_')[0].lower() for s in chunk.split()])		#the_the_DT_DET adventures_adventure_NNS_NOUN of_of_IN_ADP
 def hybchunk(hyb:str='the _NNS of', index:str='dic', size:int= -1, topk:int=10):
 	''' the _NNS of -> {the books of: 13, the doors of: 7} , added 2021.10.13 '''
@@ -493,28 +492,103 @@
 
 def init(idxname):
 	''' init a new index '''
 	if requests.es.indices.exists(index=idxname):requests.es.indices.delete(index=idxname)
 	requests.es.indices.create(index=idxname, body=config) #, body=snt_mapping
 	print(">>finished " + idxname )
 
+def skenp(doc): # added 2023.5.2
+	import en 
+	#doc = spacy.nlp(snt)
+	return {"postag": en.es_postag(doc), 'skenp': en.es_skenp(doc)}
+
+def sntbr(essay): # added 2023.5.2
+	import spacy
+	from spacy.lang import en
+	if not hasattr(sntbr, 'inst'): 
+		sntbr.inst = (inst := en.English(), inst.add_pipe("sentencizer"))[0]
+	return sntbr.inst(essay) 
+
+def dskindex(idxname, did, dsk_or_essay):
+	''' (sntid, did, snt, ... ) , 2023.5.2 '''
+	import gecdsk 
+	dsk = gecdsk.parse({"essay":dsk_or_essay}) if isinstance(dsk_or_essay, str) else dsk_or_essay
+	info = dsk['info'] 
+
+	if not requests.es.exists(index=idxname, id=f"{did}:snts" ):  # return  # already exists 
+		snts = [ mkf['meta']['snt'].strip() for mkf in dsk['snt'] ]
+		esindex(idxname, f"{did}:snts", {"id": f"{did}:snts", 'did': did, 'type':'snts', 'snts': snts, 'sntnum':len(snts) })
+	
+	if not requests.es.exists(index=idxname, id=f"{did}:dims"):
+		esindex(idxname, f"{did}:dims", {"id": f"{did}:dims", 'did': did, 'type':'dims', 'dims': json.dumps(dsk['doc'] ) })
+	
+	for i,mkf in enumerate(dsk['snt']): 
+		snt = mkf['meta']['snt'].strip() 	
+		sid = f"{did}:snt-{i}"
+		esindex(idxname, sid, {"did": did,'sntid': sid, 'type':'snt', 'snt': snt, 'rid': info.get('rid',0), 'uid': info.get('uid',0), 'tc': mkf['meta'].get('tc',0)} )
+		for k, item in mkf['feedback'].items():
+			cate = item.get('cate','')
+			if cate.startswith("e_") or cate.startswith("w_"):
+				esindex(idxname, f"{sid}:{k}", {"did": did, 'sntid': sid, 'rid': info.get('rid',0), 'uid': info.get('uid',0), 'type':'sntfd', 'kp': item['kp'], 'cate': cate, 'short_msg':item.get('short_msg',''), 'sent':snt})
+
+def update(idxname, id, arr): # arr = {"tags":"VIP"}
+	try:
+		return requests.post(f"http://{requests.eshost}/{idxname}/_doc/{id}/_update", json={"doc":arr }).json() 
+	except Exception as ex:
+		print(">>update ex:", ex)
+
+def drop(idxname): 
+	try:
+		requests.es.indices.delete(index=idxname)
+	except Exception as ex:
+		print(">>drop index ex:", ex)
+
+def addfile(infile, idxname="testdoc", taglist:str=None):
+	''' add doc only , 2023.5.1 '''
+	check(idxname)
+	start = time.time()
+	text = open(infile, 'r').read().strip() 
+	did	 = md5(text)
+	esindex(idxname, f"doc-{did}", {"did": f"doc-{did}", "doc":text,  "filename": infile, 'type':'doc', 'tags':[] if taglist is None else taglist.strip().split(',') if isinstance(taglist, str) else taglist })
+	print(f"{infile} is finished, \t| using: ", time.time() - start) 
+
+def addfolder(folder:str, idxname:str=None, pattern:str=".txt"): 
+	''' folder -> esindex '''
+	if idxname is None : idxname=  folder
+	print("addfolder started:", folder, idxname, requests.es, flush=True)
+	for root, dirs, files in os.walk(folder):
+		for file in files: 
+			if file.endswith(pattern):
+				addfile(f"{folder}/{file}", idxname = idxname, taglist=folder) 
+				print (f"{folder}/{file}", flush=True)
+	print("addfolder finished:", folder, idxname, requests.es, flush=True)
+
+def walkfolder(folder:str, pattern:str=".txt"): 
+	''' 2023.5.5 '''
+	for root, dirs, files in os.walk(folder):
+		for file in files: 
+			if file.endswith(pattern):
+				text = open(f"{folder}/{file}", 'r').read().strip() 
+				yield (file, text)  #{"folder":folder, "filename":file, "content":text}
+
 def testana(index:str='test'):
 	requests.eshost	= os.getenv("eshost", "sntvec.wrask.com:9200") 
 	requests.es		= Elasticsearch([ f"http://{requests.eshost}" ])  
 	init( index ) 
 	arr = requests.post(f"http://sntvec.wrask.com:9200/{index}/_analyze", json={
   "analyzer": "postag_ana",
-  "text": "Booked_book_VERB_VBN_NP5"
+  "text": "booked_book_VERB_VBN_NP5"
 }).json()
 	for t in arr['tokens']:
 		print (t) 
 
 if __name__ == "__main__": 
 	import platform
-	testana() if platform.system() in ('Windows') else fire.Fire({"init":init,"test":testana}) 
+	#testana()
+	print( lemlist()) if platform.system() in ('Windows') else fire.Fire({"init":init,"test":testana}) 
 	
 '''
 {'tokens': [{'token': 'booked', 'start_offset': 0, 'end_offset': 22, 'type': 'word', 'position': 0}, 
 {'token': 'd', 'start_offset': 0, 'end_offset': 22, 'type': 'word', 'position': 0}, 
 {'token': '_book', 'start_offset': 0, 'end_offset': 22, 'type': 'word', 'position': 0}, 
 {'token': '_,', 'start_offset': 0, 'end_offset': 22, 'type': 'word', 'position': 0}]}
 the_[^ ]* [^ ]*_NNS_[^ ]* of_[^ ]* 
@@ -524,28 +598,34 @@
   "properties": {
     "email": {
       "type": "keyword"
     }
   }
 }
 
+POST /essay/_doc/doc-1819783:snt-23/_update
+{
+  "doc": {
+    "tags":"VIP"
+  }
+}
+
+
 	sql= {
   "query": { 
     "bool": { 
       "must": [
         { "match_phrase": { "postag":  hyb}},
         { "match": { "type":"snt" }}
       ]
     }
   },
   "size":  size
 }
 
-
-
 PUT my_index
 {
   "mappings": {
     "properties": {
       "my_vector": {
         "type": "dense_vector",
         "dims": 4
@@ -570,15 +650,14 @@
           "query_vector": [ 1,2,3]
         }
       }
     }
   }
 }
 
-
 PUT my_index/_doc/1
 {
   "my_text" : "text1",
   "my_vector" : [0.5, 10, 6, 3]
 }
 
 PUT my_index/_doc/2
@@ -652,15 +731,14 @@
 }
 
 GET /gzjc/_analyze
 {
   "analyzer": "postag_ana", 
   "text": "foxes jumped_jump_VERB_VBD lazy dogs"
 }
-
 GET /_analyze
 {
   "tokenizer": "whitespace",
   "filter": [
     {
       "type": "pattern_replace",
       "pattern": "((^[^_]+)_([a-z]+)_([VERB|NOUN|ADJ|ADV]+)_.*)",
@@ -676,8 +754,52 @@
 ubuntu@dicvec-scivec-jukuu-com-flair-64-245:~/cikuu/pypi/so$ python __init__.py test
 {'token': 'booked', 'start_offset': 0, 'end_offset': 24, 'type': 'word', 'position': 0}
 {'token': 'book/VERB', 'start_offset': 0, 'end_offset': 24, 'type': 'word', 'position': 0}
 {'token': '_book', 'start_offset': 0, 'end_offset': 24, 'type': 'word', 'position': 0}
 {'token': '_VERB', 'start_offset': 0, 'end_offset': 24, 'type': 'word', 'position': 0}
 {'token': '_VBD', 'start_offset': 0, 'end_offset': 24, 'type': 'word', 'position': 0}
 {'token': '_NP', 'start_offset': 0, 'end_offset': 24, 'type': 'word', 'position': 0}
+
+GET /self_essay/_search
+{
+  "query": {
+    "bool": {
+      "must": [
+        {"term": {
+          "tag":  "VBD"
+        }},
+        {"term": {
+          "pos":  "VERB"
+        }}
+      ]
+    }
+  }
+}
+
+GET /essay/_search
+{
+    "query": {
+        "bool": {
+            "must": [
+                {"match": {"rid" : 230537}},
+                {"match": {"type" : "sntfd"}},
+                {"match": {"cate" : "e_snt.nv_agree"}}
+            ]
+        }
+    }, "size": topk
+}
+
+POST /essay/_search
+{
+  "query": {
+    "match": {"pos":"VERB"}
+  },
+  "size" : 0,
+    "aggs" : {
+        "termrank" : {
+            "terms" : { "field" : "lem", "size":1000  } 
+            
+        }
+    }
+}
+
 '''
```

### Comparing `cikuu-2022.8.1/sqlite/__init__.py` & `cikuu-2022.8.2/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/__init__.py` & `cikuu-2022.8.2/util/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,41 @@
 # 2022.3.10
-import requests,re,time,sqlite3,itertools
+import requests,re,time,sqlite3,itertools,sys,traceback,os
 from collections import	Counter, defaultdict
 now	= lambda: time.strftime('%Y.%m.%d %H:%M:%S',time.localtime(time.time()))
 
 import hashlib
 sntmd5	= lambda sntarr: " ".join([hashlib.md5(snt.strip().lower().encode("utf-8")).hexdigest() for snt in sntarr if len(snt) > 1])
 md5text	= lambda text: hashlib.md5(text.strip().encode("utf-8")).hexdigest()
+md5		= lambda text: hashlib.md5(text.strip().encode("utf-8")).hexdigest()
+
+from functools import wraps 
+def tried(func):
+	@wraps(func)
+	def get_except(*args,**kw):
+		try:
+			return func(*args,**kw)
+		except Exception as e:
+			print(f'{func.__name__} exception:{e}')
+			exc_type, exc_value, exc_traceback_obj = sys.exc_info()
+			traceback.print_tb(exc_traceback_obj)
+	return get_except
+    
+#test_demo
+@tried
+def tried_demo(num):
+	return num/0
+
+def walkfolder(folder:str, pattern:str=".txt"): 
+	''' 2023.5.5 '''
+	for root, dirs, files in os.walk(folder):
+		for file in files: 
+			if file.endswith(pattern):
+				text = open(f"{folder}/{file}", 'r').read().strip() 
+				yield (file, text)  #{"folder":folder, "filename":file, "content":text}
 
 def sqlite_conn(sql:str="create table nac( name varchar(64) not null , attr varchar(64) not null, count int not null default 0, primary key(name, attr) ) without rowid") :
 	conn  =	sqlite3.connect(outfile, check_same_thread=False) 
 	conn.execute(sql)
 	conn.execute('PRAGMA synchronous=OFF')
 	conn.execute('PRAGMA case_sensitive_like = 1')
 	conn.commit()
```

### Comparing `cikuu-2022.8.1/util/__main__.py` & `cikuu-2022.8.2/util/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/annotate.py` & `cikuu-2022.8.2/util/annotate.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/bcp.py` & `cikuu-2022.8.2/util/bcp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/c4data.py` & `cikuu-2022.8.2/util/c4data.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/client-blpop.py` & `cikuu-2022.8.2/util/client-blpop.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/client-xwps.py` & `cikuu-2022.8.2/util/client-xwps.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/clientx.py` & `cikuu-2022.8.2/util/clientx.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/dsk-util.py` & `cikuu-2022.8.2/util/dsk-util.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/kvr.py` & `cikuu-2022.8.2/util/kvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/mq.py` & `cikuu-2022.8.2/util/mq.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/nldp.py` & `cikuu-2022.8.2/util/nldp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/pubsub-sync.py` & `cikuu-2022.8.2/util/pubsub-sync.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/pubsub2api.py` & `cikuu-2022.8.2/util/pubsub2api.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/spider.py` & `cikuu-2022.8.2/util/spider.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/sqlitedict-load.py` & `cikuu-2022.8.2/util/sqlitedict-load.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/wps-blpop.py` & `cikuu-2022.8.2/util/wps-blpop.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/wps.py` & `cikuu-2022.8.2/util/wps.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/xsnt-spacy.py` & `cikuu-2022.8.2/util/xsnt-spacy.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/xstream.py` & `cikuu-2022.8.2/util/xstream.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/xtest-params.py` & `cikuu-2022.8.2/util/xtest-params.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/util/xtest.py` & `cikuu-2022.8.2/util/xtest.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uviapp/__init__.py` & `cikuu-2022.8.2/uviapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/Jinja2-test.py` & `cikuu-2022.8.2/uvirun/Jinja2-test.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/__init__.py` & `cikuu-2022.8.2/uvirun/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/__main__.py` & `cikuu-2022.8.2/uvirun/__main__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/c4es.py` & `cikuu-2022.8.2/uvirun/c4es.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/c4gramsi.py` & `cikuu-2022.8.2/uvirun/c4gramsi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/cos_fastapi.py` & `cikuu-2022.8.2/uvirun/cos_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/demo_fastapi.py` & `cikuu-2022.8.2/uvirun/demo_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/dsk_fastapi.py` & `cikuu-2022.8.2/uvirun/dsk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/echart_fastapi.py` & `cikuu-2022.8.2/uvirun/echart_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/elastic_fastapi.py` & `cikuu-2022.8.2/uvirun/elastic_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/__init__.py` & `cikuu-2022.8.2/uvirun/errant/__init__.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/alignment.py` & `cikuu-2022.8.2/uvirun/errant/alignment.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/annotator.py` & `cikuu-2022.8.2/uvirun/errant/annotator.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/commands/compare_m2.py` & `cikuu-2022.8.2/uvirun/errant/commands/compare_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/commands/m2_to_m2.py` & `cikuu-2022.8.2/uvirun/errant/commands/m2_to_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/commands/parallel_to_m2.py` & `cikuu-2022.8.2/uvirun/errant/commands/parallel_to_m2.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/edit.py` & `cikuu-2022.8.2/uvirun/errant/edit.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/en/classifier.py` & `cikuu-2022.8.2/uvirun/errant/en/classifier.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/en/lancaster.py` & `cikuu-2022.8.2/uvirun/errant/en/lancaster.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant/en/merger.py` & `cikuu-2022.8.2/uvirun/errant/en/merger.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/errant_fastapi.py` & `cikuu-2022.8.2/uvirun/errant_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/es_fastapi.py` & `cikuu-2022.8.2/uvirun/es_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/essay_fastapi.py` & `cikuu-2022.8.2/uvirun/essay_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/exchunk_fastapi.py` & `cikuu-2022.8.2/uvirun/exchunk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/feishu_fastapi.py` & `cikuu-2022.8.2/uvirun/feishu_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/flair_fastapi.py` & `cikuu-2022.8.2/uvirun/flair_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/ftp.py` & `cikuu-2022.8.2/uvirun/ftp.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/fusion_fastapi.py` & `cikuu-2022.8.2/uvirun/fusion_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/gec_fastapi.py` & `cikuu-2022.8.2/uvirun/gec_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/gec_fastapi_33000.py` & `cikuu-2022.8.2/uvirun/gec_fastapi_33000.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/gensim_fastapi.py` & `cikuu-2022.8.2/uvirun/gensim_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/gramx_fastapi.py` & `cikuu-2022.8.2/uvirun/gramx_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/hnswlib_fastapi.py` & `cikuu-2022.8.2/uvirun/hnswlib_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/kenlm_fastapi.py` & `cikuu-2022.8.2/uvirun/kenlm_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/kpsi_fastapi.py` & `cikuu-2022.8.2/uvirun/kpsi_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/kvr_dskdm.py` & `cikuu-2022.8.2/uvirun/kvr_dskdm.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/kvr_dskdm1230.py` & `cikuu-2022.8.2/uvirun/kvr_dskdm1230.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/nldp_fastapi.py` & `cikuu-2022.8.2/uvirun/nldp_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/nltk_fastapi.py` & `cikuu-2022.8.2/uvirun/nltk_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/nsp_fastapi.py` & `cikuu-2022.8.2/uvirun/nsp_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/penlykvr.py` & `cikuu-2022.8.2/uvirun/penlykvr.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/spacy_fastapi.py` & `cikuu-2022.8.2/uvirun/spacy_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/textacy_fastapi.py` & `cikuu-2022.8.2/uvirun/textacy_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/trans_fastapi.py` & `cikuu-2022.8.2/uvirun/trans_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/unmasker_fastapi.py` & `cikuu-2022.8.2/uvirun/unmasker_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/util_fastapi.py` & `cikuu-2022.8.2/uvirun/util_fastapi.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/uviredis.py` & `cikuu-2022.8.2/uvirun/uviredis.py`

 * *Files identical despite different names*

### Comparing `cikuu-2022.8.1/uvirun/yulk-nac.py` & `cikuu-2022.8.2/uvirun/yulk-nac.py`

 * *Files identical despite different names*

