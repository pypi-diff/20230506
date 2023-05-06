# Comparing `tmp/not1mm-23.5.5.tar.gz` & `tmp/not1mm-23.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.5.5.tar", last modified: Fri May  5 20:09:14 2023, max compression
+gzip compressed data, was "not1mm-23.5.6.tar", last modified: Sat May  6 21:00:03 2023, max compression
```

## Comparing `not1mm-23.5.5.tar` & `not1mm-23.5.6.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.606593 not1mm-23.5.5/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.5/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23536 2023-05-05 20:09:14.605593 not1mm-23.5.5/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22791 2023-05-05 20:07:53.000000 not1mm-23.5.5/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.507595 not1mm-23.5.5/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.5/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77867 2023-05-05 16:13:26.000000 not1mm-23.5.5/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    18606 2023-05-03 01:46:35.000000 not1mm-23.5.5/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.528594 not1mm-23.5.5/not1mm/data/
--rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.5/not1mm/data/Combinear.qss
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.5/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.5/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.5/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.5/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.5/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.5/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39001 2023-05-01 19:49:53.000000 not1mm-23.5.5/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.5/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.5/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.5/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.5/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.5/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.5/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.5/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.5/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.5/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.5/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.5/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43663 2023-05-04 21:24:02.000000 not1mm-23.5.5/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.5/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.5/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.595593 not1mm-23.5.5/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.5/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.5/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.5/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.5/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.5/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.5/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.5/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.5/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.5/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.5/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.5/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.5/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.5/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.5/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.5/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.5/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.5/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.5/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.5/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.5/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.5/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.5/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.5/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.5/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.5/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.5/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.5/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.5/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.5/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.5/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.5/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.5/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.5/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.5/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.5/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.5/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.5/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.5/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.5/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.5/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.5/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.5/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.5/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.5/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.5/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.5/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.5/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.5/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.5/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.5/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.5/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.5/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.602593 not1mm-23.5.5/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.5/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.5/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.5/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.5/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.5/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.5/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.5/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.5/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.5/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.5/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.5/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.5/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.5/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.5/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.5/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5781 2023-05-01 19:29:49.000000 not1mm-23.5.5/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-05 20:06:58.000000 not1mm-23.5.5/not1mm/lib/version.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30050 2023-05-05 15:32:10.000000 not1mm-23.5.5/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.605593 not1mm-23.5.5/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.5/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.5/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.5/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.5/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.5/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.5/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.5/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.5/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.5/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.5/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.5/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15022 2023-05-05 16:10:06.000000 not1mm-23.5.5/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.5/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.5/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.5/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.5/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.5/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.5/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.5/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.5/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.605593 not1mm-23.5.5/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.5/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.509595 not1mm-23.5.5/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23536 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-05 20:06:54.000000 not1mm-23.5.5/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-05 20:09:14.606593 not1mm-23.5.5/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.605593 not1mm-23.5.5/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.5/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.640622 not1mm-23.5.6/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.6/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23714 2023-05-06 21:00:03.639622 not1mm-23.5.6/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22969 2023-05-06 20:55:00.000000 not1mm-23.5.6/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.540621 not1mm-23.5.6/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.6/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77957 2023-05-06 20:37:05.000000 not1mm-23.5.6/not1mm/__main__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    18633 2023-05-06 20:41:34.000000 not1mm-23.5.6/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.567621 not1mm-23.5.6/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.6/not1mm/data/Combinear.qss
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.6/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.6/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.6/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.6/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.6/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.6/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40156 2023-05-06 20:10:52.000000 not1mm-23.5.6/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.6/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.6/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.6/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.6/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.6/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.6/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.6/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.6/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.6/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.6/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.6/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43767 2023-05-05 23:13:09.000000 not1mm-23.5.6/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.6/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.6/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.599622 not1mm-23.5.6/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.6/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.6/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.6/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.6/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.6/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.6/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.6/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.6/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.6/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.6/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.6/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.6/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.6/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.6/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.6/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.6/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.6/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.6/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.6/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.6/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.6/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.6/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.6/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.6/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.6/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.6/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.6/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.6/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.6/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.6/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.6/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.6/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.6/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.6/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.6/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.6/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.6/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.6/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.6/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.6/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.6/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.6/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.6/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.6/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.6/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.6/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.6/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.6/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.6/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.6/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.6/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.6/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.630622 not1mm-23.5.6/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.6/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.6/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.6/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.6/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.6/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.6/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.6/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.6/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.6/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.6/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.6/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.6/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.6/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.6/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.6/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6188 2023-05-06 20:36:00.000000 not1mm-23.5.6/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-06 20:59:18.000000 not1mm-23.5.6/not1mm/lib/version.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30050 2023-05-05 15:32:10.000000 not1mm-23.5.6/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.638622 not1mm-23.5.6/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.6/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.6/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.6/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.6/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.6/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.6/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.6/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.6/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.6/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.6/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.6/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15022 2023-05-05 16:10:06.000000 not1mm-23.5.6/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.6/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.6/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.6/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.6/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.6/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.6/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.6/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.6/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.638622 not1mm-23.5.6/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.6/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.544621 not1mm-23.5.6/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23714 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-06 20:59:08.000000 not1mm-23.5.6/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-06 21:00:03.640622 not1mm-23.5.6/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.639622 not1mm-23.5.6/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.6/testing/test.py
```

### Comparing `not1mm-23.5.5/LICENSE` & `not1mm-23.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/PKG-INFO` & `not1mm-23.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.5
+Version: 23.5.6
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -119,14 +119,15 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-5-6] Added AR Cluster filter options for the bandmap.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
@@ -330,15 +331,17 @@
 
 ### CW Keyer interface
 
 Under the `CW` TAB, There are three options. `cwdaemon`, which normally uses IP `127.0.0.1` and port `6789`. `pywinkeyer` which normally uses IP `127.0.0.1` and port `8000`. Or `None`, if you want to Morse it like it's 1899.
 
 ### Cluster
 
-  Under the `Cluster` TAB you can change the default AR Cluster server and port settings used for the bandmap window.
+![Configuration Settings screen](https://github.com/mbridak/not1mm/raw/master/pic/configuration_cluster.png)
+
+  Under the `Cluster` TAB you can change the default AR Cluster server, port and filter settings used for the bandmap window.
 
 ## Hiding screen elements
 
 You can show or hide certain buttons/indicators by checking and unchecking their boxes under the view menu. You can then resize the screen to make it more compact.
 
 ![View Menu](https://github.com/mbridak/not1mm/raw/master/pic/view_menu.png)
```

### Comparing `not1mm-23.5.5/README.md` & `not1mm-23.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-5-6] Added AR Cluster filter options for the bandmap.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
@@ -311,15 +312,17 @@
 
 ### CW Keyer interface
 
 Under the `CW` TAB, There are three options. `cwdaemon`, which normally uses IP `127.0.0.1` and port `6789`. `pywinkeyer` which normally uses IP `127.0.0.1` and port `8000`. Or `None`, if you want to Morse it like it's 1899.
 
 ### Cluster
 
-  Under the `Cluster` TAB you can change the default AR Cluster server and port settings used for the bandmap window.
+![Configuration Settings screen](https://github.com/mbridak/not1mm/raw/master/pic/configuration_cluster.png)
+
+  Under the `Cluster` TAB you can change the default AR Cluster server, port and filter settings used for the bandmap window.
 
 ## Hiding screen elements
 
 You can show or hide certain buttons/indicators by checking and unchecking their boxes under the view menu. You can then resize the screen to make it more compact.
 
 ![View Menu](https://github.com/mbridak/not1mm/raw/master/pic/view_menu.png)
```

### Comparing `not1mm-23.5.5/not1mm/__main__.py` & `not1mm-23.5.6/not1mm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,16 @@
         "cwip": "127.0.0.1",
         "cwport": 6789,
         "cwtype": 1,
         "useserver": False,
         "CAT_port": 4532,
         "cluster_server": "dxc.nc7j.com",
         "cluster_port": 7373,
+        "cluster_filter": "Set DX Filter SpotterCont=NA",
+        "cluster_mode": "OPEN",
     }
     appstarted = False
     contact = {}
     contest = None
     contest_settings = {}
     pref = None
     station = {}
```

### Comparing `not1mm-23.5.5/not1mm/bandmap.py` & `not1mm-23.5.6/not1mm/bandmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -481,16 +481,16 @@
 
     def receive(self):
         """doc"""
         data = self.socket.readAll()
         data = str(data, "utf-8").strip()
         if "login:" in data:
             self.send_command(self.callsignField.text())
-            # self.send_command("Set DX Filter SpotterCont=NA")
-            self.send_command("set dx mode filter")
+            self.send_command(PREF.get("cluster_filter", ""))
+            self.send_command("set dx mode " + PREF.get("cluster_mode", "OPEN"))
             return
         if "DX de" in data:
             parts = data.split()
             spotter = parts[2]
             freq = parts[3]
             dx = parts[4]
             _time = parts[-1]
```

### Comparing `not1mm-23.5.5/not1mm/data/Combinear.qss` & `not1mm-23.5.6/not1mm/data/Combinear.qss`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.5.6/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/MASTER.SCP` & `not1mm-23.5.6/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/about.ui` & `not1mm-23.5.6/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/bandmap.ui` & `not1mm-23.5.6/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/configuration.ui` & `not1mm-23.5.6/not1mm/data/configuration.ui`

 * *Files 4% similar despite different names*

#### Comparing `not1mm-23.5.5/not1mm/data/configuration.ui` & `not1mm-23.5.6/not1mm/data/configuration.ui`

```diff
@@ -18,14 +18,43 @@
     <property name="windowTitle">
       <string>Configuration Settings</string>
     </property>
     <property name="styleSheet">
       <string notr="true"/>
     </property>
     <layout class="QGridLayout" name="gridLayout">
+      <item row="1" column="1" alignment="Qt::AlignHCenter">
+        <widget class="QDialogButtonBox" name="buttonBox">
+          <property name="sizePolicy">
+            <sizepolicy hsizetype="Maximum" vsizetype="Fixed">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
+          </property>
+          <property name="font">
+            <font>
+              <family>JetBrains Mono</family>
+              <pointsize>12</pointsize>
+              <bold>false</bold>
+            </font>
+          </property>
+          <property name="layoutDirection">
+            <enum>Qt::LeftToRight</enum>
+          </property>
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+          <property name="standardButtons">
+            <set>QDialogButtonBox::Cancel|QDialogButtonBox::Save</set>
+          </property>
+          <property name="centerButtons">
+            <bool>true</bool>
+          </property>
+        </widget>
+      </item>
       <item row="0" column="1">
         <widget class="QTabWidget" name="tabWidget">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="font">
             <font>
@@ -37,15 +66,15 @@
           <property name="tabPosition">
             <enum>QTabWidget::North</enum>
           </property>
           <property name="tabShape">
             <enum>QTabWidget::Rounded</enum>
           </property>
           <property name="currentIndex">
-            <number>4</number>
+            <number>0</number>
           </property>
           <property name="elideMode">
             <enum>Qt::ElideNone</enum>
           </property>
           <property name="documentMode">
             <bool>true</bool>
           </property>
@@ -681,72 +710,88 @@
             </layout>
           </widget>
           <widget class="QWidget" name="cluster_tab">
             <attribute name="title">
               <string>Cluster</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_5">
-              <item row="3" column="3">
-                <spacer name="horizontalSpacer_9">
+              <item row="5" column="0">
+                <spacer name="horizontalSpacer_7">
                   <property name="orientation">
                     <enum>Qt::Horizontal</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
                     <size>
                       <width>40</width>
                       <height>20</height>
                     </size>
                   </property>
                 </spacer>
               </item>
-              <item row="3" column="5">
-                <spacer name="horizontalSpacer_10">
+              <item row="6" column="1">
+                <spacer name="verticalSpacer_7">
+                  <property name="orientation">
+                    <enum>Qt::Vertical</enum>
+                  </property>
+                  <property name="sizeHint" stdset="0">
+                    <size>
+                      <width>20</width>
+                      <height>40</height>
+                    </size>
+                  </property>
+                </spacer>
+              </item>
+              <item row="5" column="4">
+                <spacer name="horizontalSpacer_11">
                   <property name="orientation">
                     <enum>Qt::Horizontal</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
                     <size>
                       <width>40</width>
                       <height>20</height>
                     </size>
                   </property>
                 </spacer>
               </item>
-              <item row="3" column="0">
-                <spacer name="horizontalSpacer_7">
+              <item row="5" column="3">
+                <spacer name="horizontalSpacer_9">
                   <property name="orientation">
                     <enum>Qt::Horizontal</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
                     <size>
                       <width>40</width>
                       <height>20</height>
                     </size>
                   </property>
                 </spacer>
               </item>
-              <item row="2" column="1">
-                <widget class="QLabel" name="label_8">
-                  <property name="text">
-                    <string>Port:</string>
+              <item row="5" column="5">
+                <spacer name="horizontalSpacer_10">
+                  <property name="orientation">
+                    <enum>Qt::Horizontal</enum>
                   </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                  <property name="sizeHint" stdset="0">
+                    <size>
+                      <width>40</width>
+                      <height>20</height>
+                    </size>
                   </property>
-                </widget>
+                </spacer>
               </item>
-              <item row="4" column="1">
-                <spacer name="verticalSpacer_7">
+              <item row="5" column="1">
+                <spacer name="horizontalSpacer_8">
                   <property name="orientation">
-                    <enum>Qt::Vertical</enum>
+                    <enum>Qt::Horizontal</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
                     <size>
-                      <width>20</width>
-                      <height>40</height>
+                      <width>40</width>
+                      <height>20</height>
                     </size>
                   </property>
                 </spacer>
               </item>
               <item row="0" column="1">
                 <spacer name="verticalSpacer_6">
                   <property name="orientation">
@@ -756,56 +801,77 @@
                     <size>
                       <width>20</width>
                       <height>40</height>
                     </size>
                   </property>
                 </spacer>
               </item>
-              <item row="3" column="1">
-                <spacer name="horizontalSpacer_8">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
+              <item row="4" column="0">
+                <widget class="QLabel" name="label_21">
+                  <property name="text">
+                    <string>Mode:</string>
                   </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>40</width>
-                      <height>20</height>
-                    </size>
+                  <property name="alignment">
+                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
-                </spacer>
+                </widget>
               </item>
-              <item row="1" column="1">
-                <widget class="QLabel" name="label_5">
+              <item row="3" column="0">
+                <widget class="QLabel" name="label_20">
                   <property name="text">
-                    <string>Server:</string>
+                    <string>Filter:</string>
                   </property>
                   <property name="alignment">
                     <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
                 </widget>
               </item>
-              <item row="3" column="4">
-                <spacer name="horizontalSpacer_11">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
+              <item row="2" column="0">
+                <widget class="QLabel" name="label_8">
+                  <property name="text">
+                    <string>Port:</string>
                   </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>40</width>
-                      <height>20</height>
-                    </size>
+                  <property name="alignment">
+                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
-                </spacer>
+                </widget>
               </item>
-              <item row="2" column="3" colspan="2">
-                <widget class="QLineEdit" name="cluster_port_field"/>
+              <item row="1" column="0">
+                <widget class="QLabel" name="label_5">
+                  <property name="text">
+                    <string>Server:</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                  </property>
+                </widget>
               </item>
-              <item row="1" column="3" colspan="2">
+              <item row="1" column="1" colspan="5">
                 <widget class="QLineEdit" name="cluster_server_field"/>
               </item>
+              <item row="3" column="1" colspan="5">
+                <widget class="QLineEdit" name="cluster_filter"/>
+              </item>
+              <item row="4" column="1" colspan="2">
+                <widget class="QComboBox" name="cluster_mode">
+                  <item>
+                    <property name="text">
+                      <string>OPEN</string>
+                    </property>
+                  </item>
+                  <item>
+                    <property name="text">
+                      <string>FILTER</string>
+                    </property>
+                  </item>
+                </widget>
+              </item>
+              <item row="2" column="1" colspan="2">
+                <widget class="QLineEdit" name="cluster_port_field"/>
+              </item>
             </layout>
           </widget>
           <widget class="QWidget" name="group_tab">
             <property name="enabled">
               <bool>false</bool>
             </property>
             <property name="font">
@@ -1186,43 +1252,14 @@
                   </property>
                 </widget>
               </item>
             </layout>
           </widget>
         </widget>
       </item>
-      <item row="1" column="1" alignment="Qt::AlignHCenter">
-        <widget class="QDialogButtonBox" name="buttonBox">
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="Maximum" vsizetype="Fixed">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
-          <property name="font">
-            <font>
-              <family>JetBrains Mono</family>
-              <pointsize>12</pointsize>
-              <bold>false</bold>
-            </font>
-          </property>
-          <property name="layoutDirection">
-            <enum>Qt::LeftToRight</enum>
-          </property>
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="standardButtons">
-            <set>QDialogButtonBox::Cancel|QDialogButtonBox::Save</set>
-          </property>
-          <property name="centerButtons">
-            <bool>true</bool>
-          </property>
-        </widget>
-      </item>
     </layout>
   </widget>
   <tabstops>
     <tabstop>tabWidget</tabstop>
     <tabstop>usehamqth_radioButton</tabstop>
     <tabstop>useqrz_radioButton</tabstop>
     <tabstop>radioButton_3</tabstop>
@@ -1285,11 +1322,11 @@
           <x>286</x>
           <y>274</y>
         </hint>
       </hints>
     </connection>
   </connections>
   <buttongroups>
-    <buttongroup name="buttonGroup_2"/>
     <buttongroup name="buttonGroup"/>
+    <buttongroup name="buttonGroup_2"/>
   </buttongroups>
 </ui>
```

### Comparing `not1mm-23.5.5/not1mm/data/contests.sql` & `not1mm-23.5.6/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/cty.json` & `not1mm-23.5.6/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/editcontact.ui` & `not1mm-23.5.6/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/editmacro.ui` & `not1mm-23.5.6/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.5.6/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.5.6/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.5.6/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/logwindow.ui` & `not1mm-23.5.6/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/main.ui` & `not1mm-23.5.6/not1mm/data/main.ui`

 * *Files 1% similar despite different names*

#### Comparing `not1mm-23.5.5/not1mm/data/main.ui` & `not1mm-23.5.6/not1mm/data/main.ui`

```diff
@@ -641,14 +641,15 @@
                             <property name="enabled">
                               <bool>true</bool>
                             </property>
                             <property name="font">
                               <font>
                                 <family>JetBrains Mono</family>
                                 <pointsize>20</pointsize>
+                                <weight>75</weight>
                                 <bold>true</bold>
                               </font>
                             </property>
                             <property name="styleSheet">
                               <string notr="true">color: rgb(246, 10, 10);</string>
                             </property>
                             <property name="text">
@@ -1015,15 +1016,15 @@
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>1975</width>
-          <height>30</height>
+          <height>23</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>File</string>
         </property>
         <addaction name="actionNew_Database"/>
@@ -1100,15 +1101,18 @@
       </property>
     </action>
     <action name="actionCommand_Buttons">
       <property name="checkable">
         <bool>true</bool>
       </property>
       <property name="checked">
-        <bool>true</bool>
+        <bool>false</bool>
+      </property>
+      <property name="enabled">
+        <bool>false</bool>
       </property>
       <property name="text">
         <string>Command Buttons</string>
       </property>
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
```

### Comparing `not1mm-23.5.5/not1mm/data/new_contest.ui` & `not1mm-23.5.6/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/opon.ui` & `not1mm-23.5.6/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/0.wav` & `not1mm-23.5.6/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/1.wav` & `not1mm-23.5.6/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/2.wav` & `not1mm-23.5.6/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/3.wav` & `not1mm-23.5.6/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/4.wav` & `not1mm-23.5.6/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/5.wav` & `not1mm-23.5.6/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/6.wav` & `not1mm-23.5.6/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/7.wav` & `not1mm-23.5.6/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/73.wav` & `not1mm-23.5.6/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/8.wav` & `not1mm-23.5.6/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/9.wav` & `not1mm-23.5.6/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/a.wav` & `not1mm-23.5.6/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/again.wav` & `not1mm-23.5.6/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/b.wav` & `not1mm-23.5.6/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/c.wav` & `not1mm-23.5.6/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/contest.wav` & `not1mm-23.5.6/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/cq.wav` & `not1mm-23.5.6/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/d.wav` & `not1mm-23.5.6/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/e.wav` & `not1mm-23.5.6/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/f.wav` & `not1mm-23.5.6/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/g.wav` & `not1mm-23.5.6/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/h.wav` & `not1mm-23.5.6/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/i.wav` & `not1mm-23.5.6/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/j.wav` & `not1mm-23.5.6/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/k.wav` & `not1mm-23.5.6/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.5.6/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/l.wav` & `not1mm-23.5.6/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/m.wav` & `not1mm-23.5.6/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.5.6/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/n.wav` & `not1mm-23.5.6/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/nil.wav` & `not1mm-23.5.6/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/o.wav` & `not1mm-23.5.6/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/p.wav` & `not1mm-23.5.6/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/q.wav` & `not1mm-23.5.6/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/r.wav` & `not1mm-23.5.6/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/roger.wav` & `not1mm-23.5.6/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/s.wav` & `not1mm-23.5.6/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/space.wav` & `not1mm-23.5.6/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/t.wav` & `not1mm-23.5.6/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.5.6/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.5.6/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/u.wav` & `not1mm-23.5.6/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/v.wav` & `not1mm-23.5.6/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/w.wav` & `not1mm-23.5.6/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/x.wav` & `not1mm-23.5.6/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/y.wav` & `not1mm-23.5.6/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.5.6/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/phonetics/z.wav` & `not1mm-23.5.6/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/pickcontest.ui` & `not1mm-23.5.6/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/reddot.png` & `not1mm-23.5.6/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/data/settings.ui` & `not1mm-23.5.6/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/cat_interface.py` & `not1mm-23.5.6/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/cwinterface.py` & `not1mm-23.5.6/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/database.py` & `not1mm-23.5.6/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/edit_macro.py` & `not1mm-23.5.6/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/edit_station.py` & `not1mm-23.5.6/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/ham_utility.py` & `not1mm-23.5.6/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/lookup.py` & `not1mm-23.5.6/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/multicast.py` & `not1mm-23.5.6/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/n1mm.py` & `not1mm-23.5.6/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/lib/settings.py` & `not1mm-23.5.6/not1mm/lib/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,14 +67,19 @@
         self.n1mm_contactport.setText(str(self.preference.get("n1mm_contactport", "")))
         self.n1mm_lookupport.setText(str(self.preference.get("n1mm_lookupport", "")))
         self.n1mm_scoreport.setText(str(self.preference.get("n1mm_scoreport", "")))
         self.cluster_server_field.setText(
             str(self.preference.get("cluster_server", "dxc.nc7j.com"))
         )
         self.cluster_port_field.setText(str(self.preference.get("cluster_port", 7373)))
+        self.cluster_filter.setText(self.preference.get("cluster_filter", ""))
+        value = self.preference.get("cluster_mode", "")
+        index = self.cluster_mode.findText(value)
+        if index != -1:
+            self.cluster_mode.setCurrentIndex(index)
 
     def save_changes(self):
         """
         Write preferences to json file.
         """
         self.preference["sounddevice"] = self.sounddevice.currentText()
         self.preference["useqrz"] = self.useqrz_radioButton.isChecked()
@@ -110,7 +115,9 @@
         self.preference["n1mm_ip"] = self.n1mm_ip.text()
         self.preference["n1mm_radioport"] = self.n1mm_radioport.text()
         self.preference["n1mm_contactport"] = self.n1mm_contactport.text()
         self.preference["n1mm_lookupport"] = self.n1mm_lookupport.text()
         self.preference["n1mm_scoreport"] = self.n1mm_scoreport.text()
         self.preference["cluster_server"] = self.cluster_server_field.text()
         self.preference["cluster_port"] = int(self.cluster_port_field.text())
+        self.preference["cluster_filter"] = self.cluster_filter.text()
+        self.preference["cluster_mode"] = self.cluster_mode.currentText()
```

### Comparing `not1mm-23.5.5/not1mm/logwindow.py` & `not1mm-23.5.6/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.5.6/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.5.6/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.5.6/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.5.6/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.5.6/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.5.6/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/arrl_field_day.py` & `not1mm-23.5.6/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.5.6/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.5.6/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.5.6/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.5.6/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.5.6/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.5.6/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.5.6/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/cwt.py` & `not1mm-23.5.6/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/general_logging.py` & `not1mm-23.5.6/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/jidx_cw.py` & `not1mm-23.5.6/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/jidx_ph.py` & `not1mm-23.5.6/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/plugins/winter_field_day.py` & `not1mm-23.5.6/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm/testing/test.py` & `not1mm-23.5.6/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/not1mm.egg-info/PKG-INFO` & `not1mm-23.5.6/not1mm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.5
+Version: 23.5.6
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -119,14 +119,15 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-5-6] Added AR Cluster filter options for the bandmap.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
@@ -330,15 +331,17 @@
 
 ### CW Keyer interface
 
 Under the `CW` TAB, There are three options. `cwdaemon`, which normally uses IP `127.0.0.1` and port `6789`. `pywinkeyer` which normally uses IP `127.0.0.1` and port `8000`. Or `None`, if you want to Morse it like it's 1899.
 
 ### Cluster
 
-  Under the `Cluster` TAB you can change the default AR Cluster server and port settings used for the bandmap window.
+![Configuration Settings screen](https://github.com/mbridak/not1mm/raw/master/pic/configuration_cluster.png)
+
+  Under the `Cluster` TAB you can change the default AR Cluster server, port and filter settings used for the bandmap window.
 
 ## Hiding screen elements
 
 You can show or hide certain buttons/indicators by checking and unchecking their boxes under the view menu. You can then resize the screen to make it more compact.
 
 ![View Menu](https://github.com/mbridak/not1mm/raw/master/pic/view_menu.png)
```

### Comparing `not1mm-23.5.5/not1mm.egg-info/SOURCES.txt` & `not1mm-23.5.6/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.5/pyproject.toml` & `not1mm-23.5.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.5.5"
+version = "23.5.6"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `not1mm-23.5.5/testing/test.py` & `not1mm-23.5.6/testing/test.py`

 * *Files identical despite different names*

