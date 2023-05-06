# Comparing `tmp/maptasker-1.3.3.tar.gz` & `tmp/maptasker-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maptasker-1.3.3.tar", max compression
+gzip compressed data, was "maptasker-1.3.4.tar", max compression
```

## Comparing `maptasker-1.3.3.tar` & `maptasker-1.3.4.tar`

### file list

```diff
@@ -1,98 +1,99 @@
--rw-r--r--   0        0        0    35149 2023-02-10 17:49:08.224000 maptasker-1.3.3/LICENSE.txt
--rw-r--r--   0        0        0      296 2023-03-16 14:54:53.454155 maptasker-1.3.3/README_PyPl.md
--rw-r--r--   0        0        0     8196 2023-02-27 17:44:14.167143 maptasker-1.3.3/maptasker/.DS_Store
--rw-r--r--   0        0        0      220 2023-04-12 16:31:10.132958 maptasker-1.3.3/maptasker/.MapTasker_arguments.json
--rw-r--r--   0        0        0        0 2023-02-15 21:09:13.241439 maptasker-1.3.3/maptasker/__init__.py
--rw-r--r--   0        0        0      169 2023-03-11 17:11:25.837533 maptasker-1.3.3/maptasker/main.py
--rw-r--r--   0        0        0     6148 2023-02-27 16:37:40.000000 maptasker-1.3.3/maptasker/src/.DS_Store
--rw-r--r--   0        0        0        0 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/__init__.py
--rw-r--r--   0        0        0      212 2023-03-23 17:49:08.090530 maptasker-1.3.3/maptasker/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3135 2023-04-09 16:37:37.154363 maptasker-1.3.3/maptasker/src/__pycache__/actargs.cpython-310.pyc
--rw-r--r--   0        0        0     5461 2023-04-13 17:51:08.803769 maptasker-1.3.3/maptasker/src/__pycache__/action.cpython-310.pyc
--rw-r--r--   0        0        0   107715 2023-03-23 17:49:08.156251 maptasker-1.3.3/maptasker/src/__pycache__/actionc.cpython-310.pyc
--rw-r--r--   0        0        0     2565 2023-04-09 16:37:37.155274 maptasker-1.3.3/maptasker/src/__pycache__/actiond.cpython-310.pyc
--rw-r--r--   0        0        0     4096 2023-04-14 13:57:38.116885 maptasker-1.3.3/maptasker/src/__pycache__/actione.cpython-310.pyc
--rw-r--r--   0        0        0     2992 2023-04-13 17:32:39.155638 maptasker-1.3.3/maptasker/src/__pycache__/actionr.cpython-310.pyc
--rw-r--r--   0        0        0    14483 2023-03-23 17:49:08.400678 maptasker-1.3.3/maptasker/src/__pycache__/actiont.cpython-310.pyc
--rw-r--r--   0        0        0     1005 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/__pycache__/argsdict.cpython-310.pyc
--rw-r--r--   0        0        0     1885 2023-04-16 16:38:35.415407 maptasker-1.3.3/maptasker/src/__pycache__/caveats.cpython-310.pyc
--rw-r--r--   0        0        0     4400 2023-03-23 17:49:08.182225 maptasker-1.3.3/maptasker/src/__pycache__/colors.cpython-310.pyc
--rw-r--r--   0        0        0     1717 2023-04-16 15:45:05.862632 maptasker-1.3.3/maptasker/src/__pycache__/colrmode.cpython-310.pyc
--rw-r--r--   0        0        0     3848 2023-03-23 17:49:08.203819 maptasker-1.3.3/maptasker/src/__pycache__/condition.cpython-310.pyc
--rw-r--r--   0        0        0      290 2023-04-13 16:13:11.506371 maptasker-1.3.3/maptasker/src/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     1135 2023-04-11 19:03:07.815707 maptasker-1.3.3/maptasker/src/__pycache__/debug.cpython-310.pyc
--rw-r--r--   0        0        0      351 2023-03-23 17:49:08.397467 maptasker-1.3.3/maptasker/src/__pycache__/depricated.cpython-310.pyc
--rw-r--r--   0        0        0     1232 2023-04-13 16:38:33.007320 maptasker-1.3.3/maptasker/src/__pycache__/frmthtml.cpython-310.pyc
--rw-r--r--   0        0        0     1348 2023-04-10 14:44:42.113922 maptasker-1.3.3/maptasker/src/__pycache__/getids.cpython-310.pyc
--rw-r--r--   0        0        0     1636 2023-04-10 14:52:10.413906 maptasker-1.3.3/maptasker/src/__pycache__/getputarg.cpython-310.pyc
--rw-r--r--   0        0        0      754 2023-03-23 17:49:08.190511 maptasker-1.3.3/maptasker/src/__pycache__/initparg.cpython-310.pyc
--rw-r--r--   0        0        0     1267 2023-04-09 16:33:30.097241 maptasker-1.3.3/maptasker/src/__pycache__/kidapp.cpython-310.pyc
--rw-r--r--   0        0        0     5236 2023-04-17 15:14:53.838375 maptasker-1.3.3/maptasker/src/__pycache__/mapit.cpython-310.pyc
--rw-r--r--   0        0        0     1727 2023-04-10 14:52:10.410513 maptasker-1.3.3/maptasker/src/__pycache__/migrate.cpython-310.pyc
--rw-r--r--   0        0        0     4219 2023-04-17 15:38:49.141755 maptasker-1.3.3/maptasker/src/__pycache__/outputl.cpython-310.pyc
--rw-r--r--   0        0        0     4396 2023-03-23 17:49:08.186264 maptasker-1.3.3/maptasker/src/__pycache__/parsearg.cpython-310.pyc
--rw-r--r--   0        0        0     3872 2023-04-11 16:27:41.747208 maptasker-1.3.3/maptasker/src/__pycache__/prefers.cpython-310.pyc
--rw-r--r--   0        0        0      811 2023-04-11 19:20:37.385389 maptasker-1.3.3/maptasker/src/__pycache__/priority.cpython-310.pyc
--rw-r--r--   0        0        0     2104 2023-04-09 16:37:37.296644 maptasker-1.3.3/maptasker/src/__pycache__/proclist.cpython-310.pyc
--rw-r--r--   0        0        0     4733 2023-04-17 14:57:19.160832 maptasker-1.3.3/maptasker/src/__pycache__/profiles.cpython-310.pyc
--rw-r--r--   0        0        0      678 2023-03-23 17:49:08.179364 maptasker-1.3.3/maptasker/src/__pycache__/progargs.cpython-310.pyc
--rw-r--r--   0        0        0     5827 2023-04-12 16:13:37.277181 maptasker-1.3.3/maptasker/src/__pycache__/proginit.cpython-310.pyc
--rw-r--r--   0        0        0     7211 2023-04-16 16:33:54.842749 maptasker-1.3.3/maptasker/src/__pycache__/projects.cpython-310.pyc
--rw-r--r--   0        0        0     4273 2023-03-23 17:49:08.181004 maptasker-1.3.3/maptasker/src/__pycache__/runcli.cpython-310.pyc
--rw-r--r--   0        0        0     1578 2023-04-10 15:06:22.084248 maptasker-1.3.3/maptasker/src/__pycache__/rungui.cpython-310.pyc
--rw-r--r--   0        0        0     4362 2023-04-11 16:47:22.438398 maptasker-1.3.3/maptasker/src/__pycache__/scenes.cpython-310.pyc
--rw-r--r--   0        0        0     8098 2023-03-23 17:49:08.215471 maptasker-1.3.3/maptasker/src/__pycache__/servicec.cpython-310.pyc
--rw-r--r--   0        0        0     1976 2023-04-16 19:09:38.125947 maptasker-1.3.3/maptasker/src/__pycache__/share.cpython-310.pyc
--rw-r--r--   0        0        0      998 2023-03-23 17:49:08.120911 maptasker-1.3.3/maptasker/src/__pycache__/shellsort.cpython-310.pyc
--rw-r--r--   0        0        0     2362 2023-04-13 16:19:33.935300 maptasker-1.3.3/maptasker/src/__pycache__/sysconst.cpython-310.pyc
--rw-r--r--   0        0        0     2471 2023-04-13 17:22:06.645489 maptasker-1.3.3/maptasker/src/__pycache__/taskactn.cpython-310.pyc
--rw-r--r--   0        0        0     1329 2023-04-10 15:03:06.565941 maptasker-1.3.3/maptasker/src/__pycache__/taskerd.cpython-310.pyc
--rw-r--r--   0        0        0     8012 2023-04-17 14:57:19.157983 maptasker-1.3.3/maptasker/src/__pycache__/tasks.cpython-310.pyc
--rw-r--r--   0        0        0     3387 2023-04-16 16:28:05.704058 maptasker-1.3.3/maptasker/src/__pycache__/taskuniq.cpython-310.pyc
--rw-r--r--   0        0        0    14185 2023-04-10 14:44:20.491744 maptasker-1.3.3/maptasker/src/__pycache__/userintr.cpython-310.pyc
--rw-r--r--   0        0        0     2538 2023-04-10 19:05:04.241243 maptasker-1.3.3/maptasker/src/__pycache__/xmldata.cpython-310.pyc
--rw-r--r--   0        0        0     6363 2023-04-09 16:37:34.662793 maptasker-1.3.3/maptasker/src/actargs.py
--rw-r--r--   0        0        0    14351 2023-04-13 17:51:08.762301 maptasker-1.3.3/maptasker/src/action.py
--rw-r--r--   0        0        0   150799 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/actionc.py
--rw-r--r--   0        0        0     6754 2023-04-09 16:37:34.640363 maptasker-1.3.3/maptasker/src/actiond.py
--rw-r--r--   0        0        0     9805 2023-04-13 19:15:57.876035 maptasker-1.3.3/maptasker/src/actione.py
--rw-r--r--   0        0        0     7252 2023-04-13 17:32:39.100785 maptasker-1.3.3/maptasker/src/actionr.py
--rw-r--r--   0        0        0    17381 2023-03-23 17:42:41.413000 maptasker-1.3.3/maptasker/src/actiont.py
--rw-r--r--   0        0        0     3397 2023-04-16 16:35:22.994038 maptasker-1.3.3/maptasker/src/caveats.py
--rw-r--r--   0        0        0     8220 2023-03-23 17:42:41.450000 maptasker-1.3.3/maptasker/src/colors.py
--rw-r--r--   0        0        0     3276 2023-04-14 15:43:15.116427 maptasker-1.3.3/maptasker/src/colrmode.py
--rw-r--r--   0        0        0     9131 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/condition.py
--rw-r--r--   0        0        0     2303 2023-04-13 16:10:32.286658 maptasker-1.3.3/maptasker/src/config.py
--rw-r--r--   0        0        0     2527 2023-04-11 18:04:19.248727 maptasker-1.3.3/maptasker/src/debug.py
--rw-r--r--   0        0        0      342 2023-03-23 17:42:41.413000 maptasker-1.3.3/maptasker/src/depricated.py
--rw-r--r--   0        0        0     2017 2023-04-13 16:38:32.954840 maptasker-1.3.3/maptasker/src/frmthtml.py
--rw-r--r--   0        0        0     2441 2023-04-10 14:44:41.937204 maptasker-1.3.3/maptasker/src/getids.py
--rw-r--r--   0        0        0     3042 2023-04-10 14:52:10.334081 maptasker-1.3.3/maptasker/src/getputarg.py
--rw-r--r--   0        0        0     2366 2023-03-23 17:42:41.413000 maptasker-1.3.3/maptasker/src/initparg.py
--rw-r--r--   0        0        0     2463 2023-04-09 16:33:24.154727 maptasker-1.3.3/maptasker/src/kidapp.py
--rw-r--r--   0        0        0    15473 2023-04-17 15:14:53.760673 maptasker-1.3.3/maptasker/src/mapit.py
--rw-r--r--   0        0        0     3459 2023-04-10 14:52:10.335844 maptasker-1.3.3/maptasker/src/migrate.py
--rw-r--r--   0        0        0     9892 2023-04-17 15:38:49.066257 maptasker-1.3.3/maptasker/src/outputl.py
--rw-r--r--   0        0        0     8092 2023-03-23 17:42:41.413000 maptasker-1.3.3/maptasker/src/parsearg.py
--rw-r--r--   0        0        0     7786 2023-04-11 16:25:21.280491 maptasker-1.3.3/maptasker/src/prefers.py
--rw-r--r--   0        0        0     1684 2023-04-11 19:20:37.207118 maptasker-1.3.3/maptasker/src/priority.py
--rw-r--r--   0        0        0     4706 2023-04-09 16:37:34.668518 maptasker-1.3.3/maptasker/src/proclist.py
--rw-r--r--   0        0        0    10653 2023-04-16 19:14:51.915412 maptasker-1.3.3/maptasker/src/profiles.py
--rw-r--r--   0        0        0     1947 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/progargs.py
--rw-r--r--   0        0        0    10342 2023-04-12 16:13:37.228970 maptasker-1.3.3/maptasker/src/proginit.py
--rw-r--r--   0        0        0    15066 2023-04-16 16:33:54.739972 maptasker-1.3.3/maptasker/src/projects.py
--rw-r--r--   0        0        0     8999 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/runcli.py
--rw-r--r--   0        0        0     4149 2023-04-10 15:06:22.010146 maptasker-1.3.3/maptasker/src/rungui.py
--rw-r--r--   0        0        0     7934 2023-04-11 16:43:39.790321 maptasker-1.3.3/maptasker/src/scenes.py
--rw-r--r--   0        0        0    14219 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/servicec.py
--rw-r--r--   0        0        0     4290 2023-04-16 19:08:14.858448 maptasker-1.3.3/maptasker/src/share.py
--rw-r--r--   0        0        0     3354 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/shellsort.py
--rw-r--r--   0        0        0     4056 2023-04-17 15:44:26.479132 maptasker-1.3.3/maptasker/src/sysconst.py
--rw-r--r--   0        0        0     5820 2023-04-13 17:20:50.341670 maptasker-1.3.3/maptasker/src/taskactn.py
--rw-r--r--   0        0        0     3100 2023-04-10 15:03:06.364934 maptasker-1.3.3/maptasker/src/taskerd.py
--rw-r--r--   0        0        0    15369 2023-04-16 19:14:51.911035 maptasker-1.3.3/maptasker/src/tasks.py
--rw-r--r--   0        0        0     9713 2023-04-16 16:23:58.449719 maptasker-1.3.3/maptasker/src/taskuniq.py
--rw-r--r--   0        0        0    30601 2023-04-10 14:44:20.412620 maptasker-1.3.3/maptasker/src/userintr.py
--rw-r--r--   0        0        0     6769 2023-04-10 19:04:43.346454 maptasker-1.3.3/maptasker/src/xmldata.py
--rw-r--r--   0        0        0     1179 2023-04-09 16:07:12.762776 maptasker-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 maptasker-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-10 17:49:08.224000 maptasker-1.3.4/LICENSE.txt
+-rw-r--r--   0        0        0      296 2023-03-16 14:54:53.454155 maptasker-1.3.4/README_PyPl.md
+-rw-r--r--   0        0        0     8196 2023-02-27 17:44:14.167143 maptasker-1.3.4/maptasker/.DS_Store
+-rw-r--r--   0        0        0        0 2023-02-15 21:09:13.241439 maptasker-1.3.4/maptasker/__init__.py
+-rw-r--r--   0        0        0     1298 2023-04-21 18:13:43.143443 maptasker-1.3.4/maptasker/main.py
+-rw-r--r--   0        0        0     6148 2023-02-27 16:37:40.000000 maptasker-1.3.4/maptasker/src/.DS_Store
+-rw-r--r--   0        0        0        0 2023-03-23 17:42:41.454000 maptasker-1.3.4/maptasker/src/__init__.py
+-rw-r--r--   0        0        0      212 2023-03-23 17:49:08.090530 maptasker-1.3.4/maptasker/src/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3287 2023-04-26 16:35:54.917982 maptasker-1.3.4/maptasker/src/__pycache__/actargs.cpython-310.pyc
+-rw-r--r--   0        0        0     7042 2023-04-27 17:42:35.449508 maptasker-1.3.4/maptasker/src/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0   107715 2023-03-23 17:49:08.156251 maptasker-1.3.4/maptasker/src/__pycache__/actionc.cpython-310.pyc
+-rw-r--r--   0        0        0     2565 2023-04-09 16:37:37.155274 maptasker-1.3.4/maptasker/src/__pycache__/actiond.cpython-310.pyc
+-rw-r--r--   0        0        0     4205 2023-04-26 15:31:01.037168 maptasker-1.3.4/maptasker/src/__pycache__/actione.cpython-310.pyc
+-rw-r--r--   0        0        0     3086 2023-04-27 17:02:44.779364 maptasker-1.3.4/maptasker/src/__pycache__/actionr.cpython-310.pyc
+-rw-r--r--   0        0        0    14483 2023-03-23 17:49:08.400678 maptasker-1.3.4/maptasker/src/__pycache__/actiont.cpython-310.pyc
+-rw-r--r--   0        0        0     1005 2023-03-23 17:42:41.454000 maptasker-1.3.4/maptasker/src/__pycache__/argsdict.cpython-310.pyc
+-rw-r--r--   0        0        0     1885 2023-04-16 16:38:35.415407 maptasker-1.3.4/maptasker/src/__pycache__/caveats.cpython-310.pyc
+-rw-r--r--   0        0        0     4031 2023-04-22 19:12:32.658784 maptasker-1.3.4/maptasker/src/__pycache__/colors.cpython-310.pyc
+-rw-r--r--   0        0        0     1717 2023-04-16 15:45:05.862632 maptasker-1.3.4/maptasker/src/__pycache__/colrmode.cpython-310.pyc
+-rw-r--r--   0        0        0     3848 2023-03-23 17:49:08.203819 maptasker-1.3.4/maptasker/src/__pycache__/condition.cpython-310.pyc
+-rw-r--r--   0        0        0      290 2023-04-23 15:52:23.640032 maptasker-1.3.4/maptasker/src/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     1135 2023-04-11 19:03:07.815707 maptasker-1.3.4/maptasker/src/__pycache__/debug.cpython-310.pyc
+-rw-r--r--   0        0        0      351 2023-03-23 17:49:08.397467 maptasker-1.3.4/maptasker/src/__pycache__/depricated.cpython-310.pyc
+-rw-r--r--   0        0        0      701 2023-04-22 19:12:32.622013 maptasker-1.3.4/maptasker/src/__pycache__/error.cpython-310.pyc
+-rw-r--r--   0        0        0     1232 2023-04-27 16:01:42.023971 maptasker-1.3.4/maptasker/src/__pycache__/frmthtml.cpython-310.pyc
+-rw-r--r--   0        0        0     1348 2023-04-10 14:44:42.113922 maptasker-1.3.4/maptasker/src/__pycache__/getids.cpython-310.pyc
+-rw-r--r--   0        0        0     1732 2023-04-22 19:12:32.655380 maptasker-1.3.4/maptasker/src/__pycache__/getputarg.cpython-310.pyc
+-rw-r--r--   0        0        0      754 2023-03-23 17:49:08.190511 maptasker-1.3.4/maptasker/src/__pycache__/initparg.cpython-310.pyc
+-rw-r--r--   0        0        0     1267 2023-04-09 16:33:30.097241 maptasker-1.3.4/maptasker/src/__pycache__/kidapp.cpython-310.pyc
+-rw-r--r--   0        0        0     5810 2023-04-27 16:10:16.442192 maptasker-1.3.4/maptasker/src/__pycache__/mapit.cpython-310.pyc
+-rw-r--r--   0        0        0     2390 2023-04-22 19:12:32.652164 maptasker-1.3.4/maptasker/src/__pycache__/migrate.cpython-310.pyc
+-rw-r--r--   0        0        0     4241 2023-04-25 17:23:38.355120 maptasker-1.3.4/maptasker/src/__pycache__/outputl.cpython-310.pyc
+-rw-r--r--   0        0        0     4396 2023-03-23 17:49:08.186264 maptasker-1.3.4/maptasker/src/__pycache__/parsearg.cpython-310.pyc
+-rw-r--r--   0        0        0     3872 2023-04-11 16:27:41.747208 maptasker-1.3.4/maptasker/src/__pycache__/prefers.cpython-310.pyc
+-rw-r--r--   0        0        0      807 2023-04-21 17:53:58.807545 maptasker-1.3.4/maptasker/src/__pycache__/priority.cpython-310.pyc
+-rw-r--r--   0        0        0     2104 2023-04-09 16:37:37.296644 maptasker-1.3.4/maptasker/src/__pycache__/proclist.cpython-310.pyc
+-rw-r--r--   0        0        0     4733 2023-04-17 14:57:19.160832 maptasker-1.3.4/maptasker/src/__pycache__/profiles.cpython-310.pyc
+-rw-r--r--   0        0        0      678 2023-03-23 17:49:08.179364 maptasker-1.3.4/maptasker/src/__pycache__/progargs.cpython-310.pyc
+-rw-r--r--   0        0        0     6715 2023-04-27 16:02:27.485899 maptasker-1.3.4/maptasker/src/__pycache__/proginit.cpython-310.pyc
+-rw-r--r--   0        0        0     7239 2023-04-25 16:27:06.769722 maptasker-1.3.4/maptasker/src/__pycache__/projects.cpython-310.pyc
+-rw-r--r--   0        0        0     4291 2023-04-22 19:12:32.657451 maptasker-1.3.4/maptasker/src/__pycache__/runcli.cpython-310.pyc
+-rw-r--r--   0        0        0     1500 2023-04-20 19:18:26.030952 maptasker-1.3.4/maptasker/src/__pycache__/rungui.cpython-310.pyc
+-rw-r--r--   0        0        0     4362 2023-04-11 16:47:22.438398 maptasker-1.3.4/maptasker/src/__pycache__/scenes.cpython-310.pyc
+-rw-r--r--   0        0        0     8098 2023-03-23 17:49:08.215471 maptasker-1.3.4/maptasker/src/__pycache__/servicec.cpython-310.pyc
+-rw-r--r--   0        0        0     2527 2023-04-25 15:13:53.384912 maptasker-1.3.4/maptasker/src/__pycache__/share.cpython-310.pyc
+-rw-r--r--   0        0        0      998 2023-03-23 17:49:08.120911 maptasker-1.3.4/maptasker/src/__pycache__/shellsort.cpython-310.pyc
+-rw-r--r--   0        0        0     2361 2023-04-26 13:49:33.906022 maptasker-1.3.4/maptasker/src/__pycache__/sysconst.cpython-310.pyc
+-rw-r--r--   0        0        0     2457 2023-04-27 16:10:16.481520 maptasker-1.3.4/maptasker/src/__pycache__/taskactn.cpython-310.pyc
+-rw-r--r--   0        0        0     1335 2023-04-22 19:12:32.671777 maptasker-1.3.4/maptasker/src/__pycache__/taskerd.cpython-310.pyc
+-rw-r--r--   0        0        0     8115 2023-04-27 17:38:32.664128 maptasker-1.3.4/maptasker/src/__pycache__/tasks.cpython-310.pyc
+-rw-r--r--   0        0        0     3353 2023-04-20 16:52:34.126874 maptasker-1.3.4/maptasker/src/__pycache__/taskuniq.cpython-310.pyc
+-rw-r--r--   0        0        0    14966 2023-04-20 19:21:07.842095 maptasker-1.3.4/maptasker/src/__pycache__/userintr.cpython-310.pyc
+-rw-r--r--   0        0        0     2538 2023-04-27 16:03:47.812281 maptasker-1.3.4/maptasker/src/__pycache__/xmldata.cpython-310.pyc
+-rw-r--r--   0        0        0     6515 2023-04-26 16:28:52.677548 maptasker-1.3.4/maptasker/src/actargs.py
+-rw-r--r--   0        0        0    16528 2023-04-27 17:42:19.415894 maptasker-1.3.4/maptasker/src/action.py
+-rw-r--r--   0        0        0   150799 2023-03-23 17:42:41.454000 maptasker-1.3.4/maptasker/src/actionc.py
+-rw-r--r--   0        0        0     6754 2023-04-09 16:37:34.640363 maptasker-1.3.4/maptasker/src/actiond.py
+-rw-r--r--   0        0        0     9949 2023-04-26 15:31:00.964051 maptasker-1.3.4/maptasker/src/actione.py
+-rw-r--r--   0        0        0     7419 2023-04-27 16:31:28.982832 maptasker-1.3.4/maptasker/src/actionr.py
+-rw-r--r--   0        0        0    17381 2023-03-23 17:42:41.413000 maptasker-1.3.4/maptasker/src/actiont.py
+-rw-r--r--   0        0        0     3397 2023-04-16 16:35:22.994038 maptasker-1.3.4/maptasker/src/caveats.py
+-rw-r--r--   0        0        0     7930 2023-04-21 19:22:49.218968 maptasker-1.3.4/maptasker/src/colors.py
+-rw-r--r--   0        0        0     3276 2023-04-14 15:43:15.116427 maptasker-1.3.4/maptasker/src/colrmode.py
+-rw-r--r--   0        0        0     9131 2023-03-23 17:42:41.454000 maptasker-1.3.4/maptasker/src/condition.py
+-rw-r--r--   0        0        0     2303 2023-04-23 15:52:23.542415 maptasker-1.3.4/maptasker/src/config.py
+-rw-r--r--   0        0        0     2527 2023-04-11 18:04:19.248727 maptasker-1.3.4/maptasker/src/debug.py
+-rw-r--r--   0        0        0      342 2023-03-23 17:42:41.413000 maptasker-1.3.4/maptasker/src/depricated.py
+-rw-r--r--   0        0        0     1616 2023-04-22 17:40:12.983468 maptasker-1.3.4/maptasker/src/error.py
+-rw-r--r--   0        0        0     2017 2023-04-27 16:01:38.179160 maptasker-1.3.4/maptasker/src/frmthtml.py
+-rw-r--r--   0        0        0     2441 2023-04-10 14:44:41.937204 maptasker-1.3.4/maptasker/src/getids.py
+-rw-r--r--   0        0        0     3256 2023-04-22 17:40:12.971409 maptasker-1.3.4/maptasker/src/getputarg.py
+-rw-r--r--   0        0        0     2366 2023-03-23 17:42:41.413000 maptasker-1.3.4/maptasker/src/initparg.py
+-rw-r--r--   0        0        0     2463 2023-04-09 16:33:24.154727 maptasker-1.3.4/maptasker/src/kidapp.py
+-rw-r--r--   0        0        0    16425 2023-04-27 16:06:27.079020 maptasker-1.3.4/maptasker/src/mapit.py
+-rw-r--r--   0        0        0     4268 2023-04-22 18:26:38.533858 maptasker-1.3.4/maptasker/src/migrate.py
+-rw-r--r--   0        0        0     9688 2023-04-25 17:23:38.282515 maptasker-1.3.4/maptasker/src/outputl.py
+-rw-r--r--   0        0        0     8092 2023-03-23 17:42:41.413000 maptasker-1.3.4/maptasker/src/parsearg.py
+-rw-r--r--   0        0        0     7786 2023-04-11 16:25:21.280491 maptasker-1.3.4/maptasker/src/prefers.py
+-rw-r--r--   0        0        0     1680 2023-04-21 17:53:58.730134 maptasker-1.3.4/maptasker/src/priority.py
+-rw-r--r--   0        0        0     4706 2023-04-09 16:37:34.668518 maptasker-1.3.4/maptasker/src/proclist.py
+-rw-r--r--   0        0        0    10653 2023-04-16 19:14:51.915412 maptasker-1.3.4/maptasker/src/profiles.py
+-rw-r--r--   0        0        0     1947 2023-03-23 17:42:41.454000 maptasker-1.3.4/maptasker/src/progargs.py
+-rw-r--r--   0        0        0    11332 2023-04-27 16:02:27.391980 maptasker-1.3.4/maptasker/src/proginit.py
+-rw-r--r--   0        0        0    15224 2023-04-25 16:18:47.286005 maptasker-1.3.4/maptasker/src/projects.py
+-rw-r--r--   0        0        0     8961 2023-04-22 17:50:43.782568 maptasker-1.3.4/maptasker/src/runcli.py
+-rw-r--r--   0        0        0     4132 2023-04-20 19:17:22.314634 maptasker-1.3.4/maptasker/src/rungui.py
+-rw-r--r--   0        0        0     7934 2023-04-11 16:43:39.790321 maptasker-1.3.4/maptasker/src/scenes.py
+-rw-r--r--   0        0        0    14219 2023-03-23 17:42:41.454000 maptasker-1.3.4/maptasker/src/servicec.py
+-rw-r--r--   0        0        0     5187 2023-04-25 15:13:53.284259 maptasker-1.3.4/maptasker/src/share.py
+-rw-r--r--   0        0        0     3354 2023-03-23 17:42:41.454000 maptasker-1.3.4/maptasker/src/shellsort.py
+-rw-r--r--   0        0        0     4056 2023-04-25 19:28:11.948593 maptasker-1.3.4/maptasker/src/sysconst.py
+-rw-r--r--   0        0        0     5661 2023-04-27 16:10:16.374769 maptasker-1.3.4/maptasker/src/taskactn.py
+-rw-r--r--   0        0        0     3101 2023-04-22 17:50:43.803273 maptasker-1.3.4/maptasker/src/taskerd.py
+-rw-r--r--   0        0        0    15554 2023-04-27 17:38:32.563768 maptasker-1.3.4/maptasker/src/tasks.py
+-rw-r--r--   0        0        0     9666 2023-04-20 15:30:13.440537 maptasker-1.3.4/maptasker/src/taskuniq.py
+-rw-r--r--   0        0        0    31748 2023-04-20 19:21:07.760276 maptasker-1.3.4/maptasker/src/userintr.py
+-rw-r--r--   0        0        0     6769 2023-04-27 16:02:41.759417 maptasker-1.3.4/maptasker/src/xmldata.py
+-rw-r--r--   0        0        0     1179 2023-04-17 16:57:35.862398 maptasker-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 maptasker-1.3.4/PKG-INFO
```

### Comparing `maptasker-1.3.3/LICENSE.txt` & `maptasker-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/.DS_Store` & `maptasker-1.3.4/maptasker/.DS_Store`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/.DS_Store` & `maptasker-1.3.4/maptasker/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/actargs.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/actargs.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr  9 16:37:34 2023 UTC, .py size: 6363 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cee9 3264 db18 0000  o.........2d....
+00000000: 6f0d 0d0a 0000 0000 4451 4964 7319 0000  o.......DQIds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0012 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a05 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c06 6d07 0200 0100 6d08 5a09 0100  d.l.m.....m.Z...
 00000060: 6404 650a 6405 650b 6406 650c 6407 650c  d.e.d.e.d.e.d.e.
 00000070: 6408 6505 6a0d 6a0e 6409 6505 6a0d 6a0e  d.e.j.j.d.e.j.j.
@@ -62,135 +62,145 @@
 000003d0: a101 7d16 7c16 6418 7501 9001 726b 7c16  ..}.|.d.u...rk|.
 000003e0: 6a08 6418 7501 9001 726b 7c16 6a08 a009  j.d.u...rk|.j...
 000003f0: 6420 6421 a102 7d17 7c17 a009 6422 6423  d d!..}.|...d"d#
 00000400: a102 7d17 7c17 a009 6424 6425 a102 7d17  ..}.|...d$d%..}.
 00000410: 7c00 6426 1900 a000 7c17 a101 0100 6402  |.d&....|.....d.
 00000420: 7c00 6407 3c00 7c00 5300 0900 740a a00b  |.d.<.|.S...t...
 00000430: 6427 7c03 1700 6428 1700 a101 0100 7c00  d'|...d(......|.
-00000440: 5300 2929 6199 0100 000a 0a20 2020 203a  S.))a......    :
-00000450: 7061 7261 6d20 6576 616c 7561 7465 645f  param evaluated_
-00000460: 7265 7375 6c74 733a 2061 6c6c 2074 6865  results: all the
-00000470: 2041 6374 696f 6e20 6172 6775 6d65 6e74   Action argument
-00000480: 2022 7479 7065 7322 2061 6e64 2022 6172   "types" and "ar
-00000490: 6775 6d65 6e74 7322 0a20 2020 203a 7061  guments".    :pa
-000004a0: 7261 6d20 6172 673a 2074 6865 2069 6e63  ram arg: the inc
-000004b0: 6f6d 696e 6720 6172 6775 6d65 6e74 0a20  oming argument. 
-000004c0: 2020 203a 7061 7261 6d20 6172 6765 7661     :param argeva
-000004d0: 6c3a 2074 6865 2065 7661 6c75 6174 696f  l: the evaluatio
-000004e0: 6e20 6172 6775 6d65 6e74 0a20 2020 203a  n argument.    :
-000004f0: 7061 7261 6d20 6172 6774 7970 653a 2074  param argtype: t
-00000500: 6865 2061 7267 756d 656e 7420 2274 7970  he argument "typ
-00000510: 6522 0a20 2020 203a 7061 7261 6d20 636f  e".    :param co
-00000520: 6465 5f61 6374 696f 6e3a 2074 6865 2041  de_action: the A
-00000530: 6374 696f 6e20 636f 6465 0a20 2020 203a  ction code.    :
-00000540: 7061 7261 6d20 6163 7469 6f6e 5f74 7970  param action_typ
-00000550: 653a 2074 6865 2041 6374 696f 6e20 7479  e: the Action ty
-00000560: 7065 0a20 2020 203a 7061 7261 6d20 636f  pe.    :param co
-00000570: 6c6f 726d 6170 3a20 636f 6c6f 7273 2074  lormap: colors t
-00000580: 6f20 7573 6520 696e 206f 7574 7075 740a  o use in output.
-00000590: 2020 2020 3a70 6172 616d 2070 726f 6772      :param progr
-000005a0: 616d 5f61 7267 733a 2072 756e 7469 6d65  am_args: runtime
-000005b0: 2061 7267 756d 656e 7473 0a20 2020 203a   arguments.    :
-000005c0: 7265 7475 726e 3a20 6469 6374 696f 6e61  return: dictiona
-000005d0: 7279 206f 6620 7265 7375 6c74 730a 2020  ry of results.  
-000005e0: 2020 da03 5374 7254 da0c 6765 745f 786d    ..StrT..get_xm
-000005f0: 6c5f 666c 6167 da07 7374 7261 7267 7372  l_flag..strargsr
-00000600: 0500 0000 da07 7374 7265 7661 6cda 1372  ......streval..r
-00000610: 6574 7572 6e69 6e67 5f73 6f6d 6574 6869  eturning_somethi
-00000620: 6e67 da03 496e 74da 0769 6e74 6172 6773  ng..Int..intargs
-00000630: da07 696e 7465 7661 6cda 0341 7070 da0a  ..inteval..App..
-00000640: 7265 7375 6c74 5f61 7070 7a02 2c20 da0d  result_appz., ..
-00000650: 436f 6e64 6974 696f 6e4c 6973 74da 00fa  ConditionList...
-00000660: 0120 7201 0000 00e9 0100 0000 e902 0000  . r.............
-00000670: 00da 0a72 6573 756c 745f 636f 6eda 0349  ...result_con..I
-00000680: 6d67 2902 7218 0000 0072 1800 0000 5a03  mg).r....r....Z.
-00000690: 6e6d 654e 5a03 706b 677a 0a2c 2050 6163  nmeNZ.pkgz., Pac
-000006a0: 6b61 6765 3ada 0376 6172 da0a 7265 7375  kage:..var..resu
-000006b0: 6c74 5f69 6d67 da06 4275 6e64 6c65 5a04  lt_img..BundleZ.
-000006c0: 5661 6c73 7a2c 636f 6d2e 7477 6f66 6f72  Valsz,com.twofor
-000006d0: 7479 666f 7572 616d 2e6c 6f63 616c 652e  tyfouram.locale.
-000006e0: 696e 7465 6e74 2e65 7874 7261 2e42 4c55  intent.extra.BLU
-000006f0: 5242 7a0f 3c2f 666f 6e74 3e3c 6272 3e3c  RBz.</font><br><
-00000700: 6272 3e7a 083c 6272 3e3c 6272 3e7a 0426  br>z.<br><br>z.&
-00000710: 6c74 3bfa 013c 7a04 2667 743b fa01 3eda  lt;..<z.&gt;..>.
-00000720: 0a72 6573 756c 745f 6275 6e7a 2467 6574  .result_bunz$get
-00000730: 5f61 6374 696f 6e5f 7265 7375 6c74 733a  _action_results:
-00000740: 2075 6e6b 6e6f 776e 2061 7267 7479 7065   unknown argtype
-00000750: 3a7a 0521 2121 2121 290c da06 6170 7065  :z.!!!!!)...appe
-00000760: 6e64 da03 7374 72da 0a67 6574 5f61 6374  nd..str..get_act
-00000770: 696f 6eda 0f67 6574 5f61 7070 5f64 6574  ion..get_app_det
-00000780: 6169 6c73 7202 0000 00da 0965 6e75 6d65  ailsr......enume
-00000790: 7261 7465 da03 6c65 6eda 0466 696e 64da  rate..len..find.
-000007a0: 0474 6578 74da 0772 6570 6c61 6365 7203  .text..replacer.
-000007b0: 0000 00da 0564 6562 7567 2918 7204 0000  .....debug).r...
-000007c0: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
-000007d0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-000007e0: 0b00 0000 da09 6170 705f 636c 6173 73da  ......app_class.
-000007f0: 0761 7070 5f70 6b67 da03 6170 70da 0565  .app_pkg..app..e
-00000800: 7874 7261 5a10 6669 6e61 6c5f 636f 6e64  xtraZ.final_cond
-00000810: 6974 696f 6e73 5a0e 636f 6e64 6974 696f  itionsZ.conditio
-00000820: 6e5f 6c69 7374 5a0c 626f 6f6c 6561 6e5f  n_listZ.boolean_
-00000830: 6c69 7374 5a04 6e75 6d78 5a09 636f 6e64  listZ.numxZ.cond
-00000840: 6974 696f 6e5a 0569 6d61 6765 da07 7061  itionZ.image..pa
-00000850: 636b 6167 65da 0563 6869 6c64 5a06 6368  ckage..childZ.ch
-00000860: 696c 6431 5a06 6368 696c 6432 5a06 6368  ild1Z.child2Z.ch
-00000870: 696c 6433 5a0c 636c 6561 6e5f 7374 7269  ild3Z.clean_stri
-00000880: 6e67 a900 7234 0000 00fa 762f 5573 6572  ng..r4....v/User
-00000890: 732f 6d69 6b72 7562 696e 2f4c 6962 7261  s/mikrubin/Libra
-000008a0: 7279 2f43 6c6f 7564 5374 6f72 6167 652f  ry/CloudStorage/
-000008b0: 476f 6f67 6c65 4472 6976 652d 6d69 6b72  GoogleDrive-mikr
-000008c0: 7562 696e 4067 6d61 696c 2e63 6f6d 2f4d  ubin@gmail.com/M
-000008d0: 7920 4472 6976 652f 5079 7468 6f6e 2f6d  y Drive/Python/m
-000008e0: 6170 7461 736b 6572 2f6d 6170 7461 736b  aptasker/maptask
-000008f0: 6572 2f73 7263 2f61 6374 6172 6773 2e70  er/src/actargs.p
-00000900: 79da 1467 6574 5f61 6374 696f 6e5f 6172  y..get_action_ar
-00000910: 6775 6d65 6e74 7313 0000 0073 8a00 0000  guments....s....
-00000920: 0216 0a01 0801 1801 0e01 0801 043b 0ac6  .............;..
-00000930: 0801 1801 0e01 0801 0436 0acb 1801 0e01  .........6......
-00000940: 0401 0801 0cff 1e03 0801 042e 0ad3 1801  ................
-00000950: 0e01 0401 0c01 1002 2002 02ff 1003 1401  ........ .......
-00000960: 0280 0e01 0801 0420 0ce1 0801 0a01 0e01  ....... ........
-00000970: 0c01 1001 1201 1001 0c01 0601 1601 0801  ................
-00000980: 0414 0eee 0412 08ef 0a01 0a01 0401 0201  ................
-00000990: 04ff 1603 0e02 0c01 0c01 0e01 0801 0405  ................
-000009a0: 02fc 0401 0a01 04ff 0403 7236 0000 0063  ..........r6...c
-000009b0: 0900 0000 0000 0000 0000 0000 0e00 0000  ................
-000009c0: 0a00 0000 4300 0000 7370 0000 0074 007c  ....C...sp...t.|
-000009d0: 0083 0144 005d 315c 027d 097d 0a7c 0a64  ...D.]1\.}.}.|.d
-000009e0: 016b 0272 0e7c 096e 087c 027c 0119 0064  .k.r.|.n.|.|...d
-000009f0: 0219 00a0 017c 0aa1 017d 0b7c 037c 0919  .....|...}.|.|..
-00000a00: 007d 0c7c 027c 0119 0064 0319 007c 0b19  .}.|.|...d...|..
-00000a10: 007d 0d7c 0864 0419 00a0 027c 0da1 0101  .}.|.d.....|....
-00000a20: 0074 037c 087c 0a7c 0c7c 0d7c 047c 057c  .t.|.|.|.|.|.|.|
-00000a30: 067c 0783 087d 0871 047c 0853 0029 054e  .|...}.q.|.S.).N
-00000a40: da02 6966 da04 6172 6773 da05 7479 7065  ..if..args..type
-00000a50: 73da 1170 6f73 6974 696f 6e5f 6172 675f  s..position_arg_
-00000a60: 7479 7065 2904 7228 0000 00da 0569 6e64  type).r(.....ind
-00000a70: 6578 7224 0000 0072 3600 0000 290e da08  exr$...r6...)...
-00000a80: 6172 675f 6c69 7374 da09 6469 6374 5f63  arg_list..dict_c
-00000a90: 6f64 65da 116c 6f6f 6b75 705f 636f 6465  ode..lookup_code
-00000aa0: 5f65 6e74 7279 da0d 6576 616c 7561 7465  _entry..evaluate
-00000ab0: 5f6c 6973 7472 0800 0000 7209 0000 0072  _listr....r....r
-00000ac0: 0a00 0000 720b 0000 0072 0400 0000 5a03  ....r....r....Z.
-00000ad0: 6e75 6d72 0500 0000 723b 0000 0072 0600  numr....r;...r..
-00000ae0: 0000 7207 0000 0072 3400 0000 7234 0000  ..r....r4...r4..
-00000af0: 0072 3500 0000 da0b 6163 7469 6f6e 5f61  .r5.....action_a
-00000b00: 7267 736f 0000 0073 2000 0000 100b 1e02  rgso...s .......
-00000b10: 0802 1001 0e01 0201 0201 0201 0201 0201  ................
-00000b20: 0201 0201 0201 0201 06f8 040b 7240 0000  ............r@..
-00000b30: 0029 115a 156d 6170 7461 736b 6572 2e73  .).Z.maptasker.s
-00000b40: 7263 2e61 6374 696f 6e64 7202 0000 00da  rc.actiondr.....
-00000b50: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
-00000b60: 7973 636f 6e73 7472 0300 0000 da16 6465  ysconstr......de
-00000b70: 6675 7365 6478 6d6c 2e45 6c65 6d65 6e74  fusedxml.Element
-00000b80: 5472 6565 da0a 6465 6675 7365 6478 6d6c  Tree..defusedxml
-00000b90: da14 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
-00000ba0: 6163 7469 6f6e da03 7372 63da 0661 6374  action..src..act
-00000bb0: 696f 6e72 2600 0000 da04 6469 6374 da06  ionr&.....dict..
-00000bc0: 6f62 6a65 6374 da04 6c69 7374 da0b 456c  object..list..El
-00000bd0: 656d 656e 7454 7265 65da 0358 4d4c 7236  ementTree..XMLr6
-00000be0: 0000 0072 4000 0000 7234 0000 0072 3400  ...r@...r4...r4.
-00000bf0: 0000 7234 0000 0072 3500 0000 da08 3c6d  ..r4...r5.....<m
-00000c00: 6f64 756c 653e 0100 0000 7330 0000 000c  odule>....s0....
-00000c10: 0c0c 0108 0112 0102 0302 0102 ff02 0202  ................
-00000c20: fe02 0302 fd02 0402 fc06 0502 fb06 0602  ................
-00000c30: fa02 0702 f902 0802 f802 090a f70c 5c    ..............\
+00000440: 5300 2929 6131 0200 000a 2020 2020 4769  S.))a1....    Gi
+00000450: 7665 6e20 616e 203c 6172 676e 3e20 656c  ven an <argn> el
+00000460: 656d 656e 742c 2065 7661 6c75 6174 6520  ement, evaluate 
+00000470: 6974 2773 2063 6f6e 7465 6e74 7320 6261  it's contents ba
+00000480: 7365 6420 6f6e 206f 7572 2041 6374 696f  sed on our Actio
+00000490: 6e20 636f 6465 2064 6963 7469 6f6e 6172  n code dictionar
+000004a0: 7920 2861 6374 696f 6e63 2e70 7929 0a20  y (actionc.py). 
+000004b0: 2020 2020 2020 203a 7061 7261 6d20 6576         :param ev
+000004c0: 616c 7561 7465 645f 7265 7375 6c74 733a  aluated_results:
+000004d0: 2061 6c6c 2074 6865 2041 6374 696f 6e20   all the Action 
+000004e0: 6172 6775 6d65 6e74 2022 7479 7065 7322  argument "types"
+000004f0: 2061 6e64 2022 6172 6775 6d65 6e74 7322   and "arguments"
+00000500: 2061 7320 6120 6469 6369 746f 6e61 7279   as a dicitonary
+00000510: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000520: 6172 673a 2074 6865 2069 6e63 6f6d 696e  arg: the incomin
+00000530: 6720 6172 6775 6d65 6e74 0a20 2020 2020  g argument.     
+00000540: 2020 203a 7061 7261 6d20 6172 6765 7661     :param argeva
+00000550: 6c3a 2074 6865 2065 7661 6c75 6174 696f  l: the evaluatio
+00000560: 6e20 6172 6775 6d65 6e74 0a20 2020 2020  n argument.     
+00000570: 2020 203a 7061 7261 6d20 6172 6774 7970     :param argtyp
+00000580: 653a 2074 6865 2061 7267 756d 656e 7420  e: the argument 
+00000590: 2274 7970 6522 0a20 2020 2020 2020 203a  "type".        :
+000005a0: 7061 7261 6d20 636f 6465 5f61 6374 696f  param code_actio
+000005b0: 6e3a 2074 6865 2041 6374 696f 6e20 636f  n: the Action co
+000005c0: 6465 0a20 2020 2020 2020 203a 7061 7261  de.        :para
+000005d0: 6d20 6163 7469 6f6e 5f74 7970 653a 2074  m action_type: t
+000005e0: 6865 2041 6374 696f 6e20 7479 7065 0a20  he Action type. 
+000005f0: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+00000600: 6c6f 726d 6170 3a20 636f 6c6f 7273 2074  lormap: colors t
+00000610: 6f20 7573 6520 696e 206f 7574 7075 740a  o use in output.
+00000620: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+00000630: 726f 6772 616d 5f61 7267 733a 2072 756e  rogram_args: run
+00000640: 7469 6d65 2061 7267 756d 656e 7473 0a20  time arguments. 
+00000650: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00000660: 6469 6374 696f 6e61 7279 206f 6620 7265  dictionary of re
+00000670: 7375 6c74 730a 2020 2020 da03 5374 7254  sults.    ..StrT
+00000680: da0c 6765 745f 786d 6c5f 666c 6167 da07  ..get_xml_flag..
+00000690: 7374 7261 7267 7372 0500 0000 da07 7374  strargsr......st
+000006a0: 7265 7661 6cda 1372 6574 7572 6e69 6e67  reval..returning
+000006b0: 5f73 6f6d 6574 6869 6e67 da03 496e 74da  _something..Int.
+000006c0: 0769 6e74 6172 6773 da07 696e 7465 7661  .intargs..inteva
+000006d0: 6cda 0341 7070 da0a 7265 7375 6c74 5f61  l..App..result_a
+000006e0: 7070 7a02 2c20 da0d 436f 6e64 6974 696f  ppz., ..Conditio
+000006f0: 6e4c 6973 74da 00da 0120 7201 0000 00e9  nList.... r.....
+00000700: 0100 0000 e902 0000 00da 0a72 6573 756c  ...........resul
+00000710: 745f 636f 6eda 0349 6d67 2902 7218 0000  t_con..Img).r...
+00000720: 0072 1800 0000 5a03 6e6d 654e 5a03 706b  .r....Z.nmeNZ.pk
+00000730: 677a 0a2c 2050 6163 6b61 6765 3ada 0376  gz., Package:..v
+00000740: 6172 da0a 7265 7375 6c74 5f69 6d67 da06  ar..result_img..
+00000750: 4275 6e64 6c65 5a04 5661 6c73 7a2c 636f  BundleZ.Valsz,co
+00000760: 6d2e 7477 6f66 6f72 7479 666f 7572 616d  m.twofortyfouram
+00000770: 2e6c 6f63 616c 652e 696e 7465 6e74 2e65  .locale.intent.e
+00000780: 7874 7261 2e42 4c55 5242 7a0f 3c2f 666f  xtra.BLURBz.</fo
+00000790: 6e74 3e3c 6272 3e3c 6272 3e7a 083c 6272  nt><br><br>z.<br
+000007a0: 3e3c 6272 3e7a 0426 6c74 3bfa 013c 7a04  ><br>z.&lt;..<z.
+000007b0: 2667 743b fa01 3eda 0a72 6573 756c 745f  &gt;..>..result_
+000007c0: 6275 6e7a 2467 6574 5f61 6374 696f 6e5f  bunz$get_action_
+000007d0: 7265 7375 6c74 733a 2075 6e6b 6e6f 776e  results: unknown
+000007e0: 2061 7267 7479 7065 3a7a 0521 2121 2121   argtype:z.!!!!!
+000007f0: 290c da06 6170 7065 6e64 da03 7374 72da  )...append..str.
+00000800: 0a67 6574 5f61 6374 696f 6eda 0f67 6574  .get_action..get
+00000810: 5f61 7070 5f64 6574 6169 6c73 7202 0000  _app_detailsr...
+00000820: 00da 0965 6e75 6d65 7261 7465 da03 6c65  ...enumerate..le
+00000830: 6eda 0466 696e 64da 0474 6578 74da 0772  n..find..text..r
+00000840: 6570 6c61 6365 7203 0000 00da 0564 6562  eplacer......deb
+00000850: 7567 2918 7204 0000 0072 0500 0000 7206  ug).r....r....r.
+00000860: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
+00000870: 0000 720a 0000 0072 0b00 0000 da09 6170  ..r....r......ap
+00000880: 705f 636c 6173 73da 0761 7070 5f70 6b67  p_class..app_pkg
+00000890: da03 6170 70da 0565 7874 7261 5a10 6669  ..app..extraZ.fi
+000008a0: 6e61 6c5f 636f 6e64 6974 696f 6e73 5a0e  nal_conditionsZ.
+000008b0: 636f 6e64 6974 696f 6e5f 6c69 7374 5a0c  condition_listZ.
+000008c0: 626f 6f6c 6561 6e5f 6c69 7374 5a04 6e75  boolean_listZ.nu
+000008d0: 6d78 da09 636f 6e64 6974 696f 6e5a 0569  mx..conditionZ.i
+000008e0: 6d61 6765 da07 7061 636b 6167 65da 0563  mage..package..c
+000008f0: 6869 6c64 5a06 6368 696c 6431 5a06 6368  hildZ.child1Z.ch
+00000900: 696c 6432 5a06 6368 696c 6433 5a0c 636c  ild2Z.child3Z.cl
+00000910: 6561 6e5f 7374 7269 6e67 a900 7235 0000  ean_string..r5..
+00000920: 00fa 762f 5573 6572 732f 6d69 6b72 7562  ..v/Users/mikrub
+00000930: 696e 2f4c 6962 7261 7279 2f43 6c6f 7564  in/Library/Cloud
+00000940: 5374 6f72 6167 652f 476f 6f67 6c65 4472  Storage/GoogleDr
+00000950: 6976 652d 6d69 6b72 7562 696e 4067 6d61  ive-mikrubin@gma
+00000960: 696c 2e63 6f6d 2f4d 7920 4472 6976 652f  il.com/My Drive/
+00000970: 5079 7468 6f6e 2f6d 6170 7461 736b 6572  Python/maptasker
+00000980: 2f6d 6170 7461 736b 6572 2f73 7263 2f61  /maptasker/src/a
+00000990: 6374 6172 6773 2e70 79da 1467 6574 5f61  ctargs.py..get_a
+000009a0: 6374 696f 6e5f 6172 6775 6d65 6e74 7313  ction_arguments.
+000009b0: 0000 0073 8a00 0000 0216 0a01 0801 1801  ...s............
+000009c0: 0e01 0801 043b 0ac6 0801 1801 0e01 0801  .....;..........
+000009d0: 0436 0acb 1801 0e01 0401 0801 0cff 1e03  .6..............
+000009e0: 0801 042e 0ad3 1801 0e01 0401 0c01 1002  ................
+000009f0: 2002 02ff 1003 1401 0280 0e01 0801 0420   .............. 
+00000a00: 0ce1 0801 0a01 0e01 0c01 1001 1201 1001  ................
+00000a10: 0c01 0601 1601 0801 0414 0eee 0412 08ef  ................
+00000a20: 0a01 0a01 0401 0201 04ff 1603 0e02 0c01  ................
+00000a30: 0c01 0e01 0801 0405 02fc 0401 0a01 04ff  ................
+00000a40: 0403 7237 0000 0063 0900 0000 0000 0000  ..r7...c........
+00000a50: 0000 0000 0e00 0000 0a00 0000 4300 0000  ............C...
+00000a60: 7370 0000 0074 007c 0083 0144 005d 315c  sp...t.|...D.]1\
+00000a70: 027d 097d 0a7c 0a64 016b 0272 0e7c 096e  .}.}.|.d.k.r.|.n
+00000a80: 087c 027c 0119 0064 0219 00a0 017c 0aa1  .|.|...d.....|..
+00000a90: 017d 0b7c 037c 0919 007d 0c7c 027c 0119  .}.|.|...}.|.|..
+00000aa0: 0064 0319 007c 0b19 007d 0d7c 0864 0419  .d...|...}.|.d..
+00000ab0: 00a0 027c 0da1 0101 0074 037c 087c 0a7c  ...|.....t.|.|.|
+00000ac0: 0c7c 0d7c 047c 057c 067c 0783 087d 0871  .|.|.|.|.|...}.q
+00000ad0: 047c 0853 0029 054e da02 6966 da04 6172  .|.S.).N..if..ar
+00000ae0: 6773 da05 7479 7065 73da 1170 6f73 6974  gs..types..posit
+00000af0: 696f 6e5f 6172 675f 7479 7065 2904 7228  ion_arg_type).r(
+00000b00: 0000 00da 0569 6e64 6578 7224 0000 0072  .....indexr$...r
+00000b10: 3700 0000 290e da08 6172 675f 6c69 7374  7...)...arg_list
+00000b20: da09 6469 6374 5f63 6f64 65da 116c 6f6f  ..dict_code..loo
+00000b30: 6b75 705f 636f 6465 5f65 6e74 7279 da0d  kup_code_entry..
+00000b40: 6576 616c 7561 7465 5f6c 6973 7472 0800  evaluate_listr..
+00000b50: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000b60: 0072 0400 0000 da03 6e75 6d72 0500 0000  .r......numr....
+00000b70: 723c 0000 0072 0600 0000 7207 0000 0072  r<...r....r....r
+00000b80: 3500 0000 7235 0000 0072 3600 0000 da0b  5...r5...r6.....
+00000b90: 6163 7469 6f6e 5f61 7267 736f 0000 0073  action_argso...s
+00000ba0: 2000 0000 100b 1e02 0802 1001 0e01 0201   ...............
+00000bb0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000bc0: 06f8 040b 7242 0000 0029 115a 156d 6170  ....rB...).Z.map
+00000bd0: 7461 736b 6572 2e73 7263 2e61 6374 696f  tasker.src.actio
+00000be0: 6e64 7202 0000 00da 166d 6170 7461 736b  ndr......maptask
+00000bf0: 6572 2e73 7263 2e73 7973 636f 6e73 7472  er.src.sysconstr
+00000c00: 0300 0000 da16 6465 6675 7365 6478 6d6c  ......defusedxml
+00000c10: 2e45 6c65 6d65 6e74 5472 6565 da0a 6465  .ElementTree..de
+00000c20: 6675 7365 6478 6d6c da14 6d61 7074 6173  fusedxml..maptas
+00000c30: 6b65 722e 7372 632e 6163 7469 6f6e da03  ker.src.action..
+00000c40: 7372 63da 0661 6374 696f 6e72 2600 0000  src..actionr&...
+00000c50: da04 6469 6374 da06 6f62 6a65 6374 da04  ..dict..object..
+00000c60: 6c69 7374 da0b 456c 656d 656e 7454 7265  list..ElementTre
+00000c70: 65da 0358 4d4c 7237 0000 0072 4200 0000  e..XMLr7...rB...
+00000c80: 7235 0000 0072 3500 0000 7235 0000 0072  r5...r5...r5...r
+00000c90: 3600 0000 da08 3c6d 6f64 756c 653e 0100  6.....<module>..
+00000ca0: 0000 7330 0000 000c 0c0c 0108 0112 0102  ..s0............
+00000cb0: 0302 0102 ff02 0202 fe02 0302 fd02 0402  ................
+00000cc0: fc06 0502 fb06 0602 fa02 0702 f902 0802  ................
+00000cd0: f802 090a f70c 5c                        ......\
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/actionc.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/actionc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/actiond.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/actiond.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/actione.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/actione.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 19:15:57 2023 UTC, .py size: 9805 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,256 +1,263 @@
-00000000: 6f0d 0d0a 0000 0000 ed54 3864 4d26 0000  o........T8dM&..
+00000000: 6f0d 0d0a 0000 0000 b443 4964 dd26 0000  o........CId.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000e 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
+00000020: 000e 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 6d05 0200  d.l.Z.d.d.l.m...
 00000050: 0100 6d06 5a07 0100 6400 6402 6c08 6d09  ..m.Z...d.d.l.m.
 00000060: 5a09 0100 6400 6403 6c0a 6d0b 5a0b 0100  Z...d.d.l.m.Z...
 00000070: 6400 6404 6c0c 6d0d 5a0d 0100 6400 6405  d.d.l.m.Z...d.d.
-00000080: 6c0e 6d0f 5a0f 0100 6400 6406 6c0e 6d10  l.m.Z...d.d.l.m.
-00000090: 5a10 0100 6501 a011 6407 a101 5a12 6408  Z...e...d...Z.d.
-000000a0: 6409 8400 5a13 640a 640b 8400 5a14 640c  d...Z.d.d...Z.d.
-000000b0: 640d 8400 5a15 640e 6503 6a16 6a17 640f  d...Z.d.e.j.j.d.
-000000c0: 6503 6a16 6a17 6410 6518 6411 6519 6412  e.j.j.d.e.d.e.d.
-000000d0: 651a 6413 6519 6414 651a 660e 6415 6416  e.d.e.d.e.f.d.d.
-000000e0: 8404 5a1b 6417 6418 8400 5a1c 6401 5300  ..Z.d.d...Z.d.S.
-000000f0: 2919 e900 0000 004e 2901 da0f 6765 745f  )......N)...get_
-00000100: 6578 7472 615f 7374 7566 6629 01da 0b66  extra_stuff)...f
-00000110: 6f72 6d61 745f 6874 6d6c 2901 da0c 6163  ormat_html)...ac
-00000120: 7469 6f6e 5f63 6f64 6573 2901 da06 6c6f  tion_codes)...lo
-00000130: 6767 6572 2901 da0b 464f 4e54 5f54 4f5f  gger)...FONT_TO_
-00000140: 5553 457a 062c 5b2c 205d 2b63 0100 0000  USEz.,[, ]+c....
-00000150: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00000160: 4300 0000 7394 0000 007c 00a0 0064 0164  C...s....|...d.d
-00000170: 02a1 027d 007c 00a0 0064 0364 04a1 027d  ...}.|...d.d...}
-00000180: 0074 01a0 0264 057c 00a1 027d 007c 00a0  .t...d.|...}.|..
-00000190: 0064 0664 07a1 027d 007c 00a0 0064 0864  .d.d...}.|...d.d
-000001a0: 09a1 027d 007c 00a0 0064 0a64 04a1 027d  ...}.|...d.d...}
-000001b0: 007c 00a0 0064 0b64 04a1 027d 007c 00a0  .|...d.d...}.|..
-000001c0: 0064 0c64 04a1 027d 007c 00a0 0064 0d64  .d.d...}.|...d.d
-000001d0: 04a1 027d 007c 00a0 0064 0e64 04a1 027d  ...}.|...d.d...}
-000001e0: 007c 00a0 0064 0f64 04a1 027d 007c 00a0  .|...d.d...}.|..
-000001f0: 0064 1064 11a1 027d 007c 0053 0029 124e  .d.d...}.|.S.).N
-00000200: 7a09 2c20 203c 666f 6e74 3e7a 063c 666f  z.,  <font>z.<fo
-00000210: 6e74 3e7a 032c 2028 da00 7a02 2c20 7a07  nt>z., (..z., z.
-00000220: 2c20 3c73 7061 6e7a 053c 7370 616e 7a08  , <spanz.<spanz.
-00000230: 2c20 203c 7370 616e 7a07 2020 3c73 7061  ,  <spanz.  <spa
-00000240: 6e7a 072c 2063 6f64 653a 7a05 3c62 6967  nz., code:z.<big
-00000250: 3e7a 073c 736d 616c 6c3e 7a04 3c74 743e  >z.<small>z.<tt>
-00000260: 7a03 3c69 3e7a 033c 753e 7a07 2c20 3c66  z.<i>z.<u>z., <f
-00000270: 6f6e 747a 053c 666f 6e74 2903 da07 7265  ontz.<font)...re
-00000280: 706c 6163 65da 0770 6174 7465 726e da03  place..pattern..
-00000290: 7375 6229 01da 0772 6573 756c 7473 a900  sub)...results..
-000002a0: 720c 0000 00fa 762f 5573 6572 732f 6d69  r.....v/Users/mi
-000002b0: 6b72 7562 696e 2f4c 6962 7261 7279 2f43  krubin/Library/C
-000002c0: 6c6f 7564 5374 6f72 6167 652f 476f 6f67  loudStorage/Goog
-000002d0: 6c65 4472 6976 652d 6d69 6b72 7562 696e  leDrive-mikrubin
-000002e0: 4067 6d61 696c 2e63 6f6d 2f4d 7920 4472  @gmail.com/My Dr
-000002f0: 6976 652f 5079 7468 6f6e 2f6d 6170 7461  ive/Python/mapta
-00000300: 736b 6572 2f6d 6170 7461 736b 6572 2f73  sker/maptasker/s
-00000310: 7263 2f61 6374 696f 6e65 2e70 79da 1263  rc/actione.py..c
-00000320: 6c65 616e 7570 5f74 6865 5f72 6573 756c  leanup_the_resul
-00000330: 7422 0000 0073 1e00 0000 0403 0401 04ff  t"...s..........
-00000340: 0c03 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00000350: 0c01 0c01 0c01 0401 720e 0000 0063 0000  ........r....c..
-00000360: 0000 0000 0000 0000 0000 0500 0000 0500  ................
-00000370: 0000 4300 0000 739c 0000 0064 017d 0074  ..C...s....d.}.t
-00000380: 0044 005d 3f7d 0174 007c 0119 007d 027c  .D.]?}.t.|...}.|
-00000390: 0264 0219 007d 037c 0364 036b 0472 2a64  .d...}.|.d.k.r*d
-000003a0: 047c 0276 0172 2a64 057c 019b 0064 067c  .|.v.r*d.|...d.|
-000003b0: 039b 009d 047d 0474 017c 0483 0101 0074  .....}.t.|.....t
-000003c0: 02a0 037c 049b 00a1 0101 0064 077d 0064  ...|.......d.}.d
-000003d0: 087c 0276 0172 4364 057c 019b 0064 099d  .|.v.rCd.|...d..
-000003e0: 037d 0474 017c 0483 0101 0074 02a0 037c  .}.t.|.....t...|
-000003f0: 04a1 0101 0064 0a7c 0264 083c 0064 077d  .....d.|.d.<.d.}
-00000400: 0071 047c 0072 4c74 0464 0b83 0101 0064  .q.|.rLt.d.....d
-00000410: 0053 0064 0053 0029 0c4e 46da 076e 756d  .S.d.S.).NF..num
-00000420: 6172 6773 7201 0000 00da 0772 6571 6172  argsr......reqar
-00000430: 6773 7a11 4572 726f 723a 2064 6963 745f  gsz.Error: dict_
-00000440: 636f 6465 207a 1b20 6d69 7373 696e 6720  code z. missing 
-00000450: 7265 7161 7267 7321 2020 6e75 6d61 7267  reqargs!  numarg
-00000460: 733a 54da 0764 6973 706c 6179 7a13 206d  s:T..displayz. m
-00000470: 6973 7369 6e67 2022 6469 7370 6c61 7922  issing "display"
-00000480: 215a 0875 6e6d 6170 7065 64e9 6300 0000  !Z.unmapped.c...
-00000490: 2905 7204 0000 00da 0570 7269 6e74 7205  ).r......printr.
-000004a0: 0000 00da 0564 6562 7567 da04 6578 6974  .....debug..exit
-000004b0: 2905 da04 666c 6167 da04 6974 656d da05  )...flag..item..
-000004c0: 656e 7472 7972 0f00 0000 da09 6572 726f  entryr......erro
-000004d0: 725f 6d73 6772 0c00 0000 720c 0000 0072  r_msgr....r....r
-000004e0: 0d00 0000 da14 6c6f 6f6b 5f66 6f72 5f6d  ......look_for_m
-000004f0: 6973 7369 6e67 5f72 6571 3900 0000 7326  issing_req9...s&
-00000500: 0000 0004 0108 0108 0108 0110 0110 0108  ................
-00000510: 010c 0104 0108 010c 0108 010a 0108 0104  ................
-00000520: 0102 8004 010c 0104 ff72 1a00 0000 6301  .........r....c.
-00000530: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00000540: 0000 0043 0000 0073 4400 0000 6401 6402  ...C...sD...d.d.
-00000550: 6c00 6d01 7d01 0100 7c00 6400 6403 8502  l.m.}...|.d.d...
-00000560: 1900 7d02 7c02 7c01 7600 7220 7c00 7402  ..}.|.|.v.r |.t.
-00000570: 7600 7220 6404 7402 7c00 1900 6404 1900  v.r d.t.|...d...
-00000580: 6405 1700 6901 7402 7c00 3c00 6400 5300  d...i.t.|.<.d.S.
-00000590: 2906 4e72 0100 0000 2901 da0a 6465 7072  ).Nr....)...depr
-000005a0: 6963 6174 6564 e9ff ffff ff72 1100 0000  icated.....r....
-000005b0: 7a1a 3c65 6d3e 2028 4973 2044 6570 7265  z.<em> (Is Depre
-000005c0: 6361 7465 6429 3c2f 656d 3e20 2903 5a18  cated)</em> ).Z.
-000005d0: 6d61 7074 6173 6b65 722e 7372 632e 6465  maptasker.src.de
-000005e0: 7072 6963 6174 6564 721b 0000 0072 0400  pricatedr....r..
-000005f0: 0000 2903 da09 6469 6374 5f63 6f64 6572  ..)...dict_coder
-00000600: 1b00 0000 da06 6c6f 6f6b 7570 720c 0000  ......lookupr...
-00000610: 0072 0c00 0000 720d 0000 00da 1563 6865  .r....r......che
-00000620: 636b 5f66 6f72 5f64 6570 7265 6361 7469  ck_for_deprecati
-00000630: 6f6e 5000 0000 730c 0000 000c 010c 0210  onP...s.........
-00000640: 0110 0208 ff04 0372 1f00 0000 da0a 636f  .......r......co
-00000650: 6465 5f63 6869 6c64 da0b 636f 6465 5f61  de_child..code_a
-00000660: 6374 696f 6eda 0b61 6374 696f 6e5f 7479  ction..action_ty
-00000670: 7065 da08 636f 6c6f 726d 6170 da09 636f  pe..colormap..co
-00000680: 6465 5f74 7970 65da 0c70 726f 6772 616d  de_type..program
-00000690: 5f61 7267 73da 0672 6574 7572 6e63 0600  _args..returnc..
-000006a0: 0000 0000 0000 0000 0000 0c00 0000 0a00  ................
-000006b0: 0000 4300 0000 7358 0100 0074 00a0 0164  ..C...sX...t...d
-000006c0: 017c 006a 029b 007c 049b 009d 03a1 0101  .|.j...|........
-000006d0: 007c 006a 027c 0417 007d 0674 037c 0683  .|.j.|...}.t.|..
-000006e0: 0101 007c 0674 0476 0173 1e64 0274 047c  ...|.t.v.s.d.t.|
-000006f0: 0619 0076 0172 3564 037c 069b 0064 0474  ...v.r5d.|...d.t
-00000700: 057c 017c 027c 037c 0583 049b 009d 047d  .|.|.|.|.......}
-00000710: 0774 00a0 0164 057c 069b 0064 069d 03a1  .t...d.|...d....
-00000720: 0101 006e 7174 067c 0364 0764 0874 047c  ...nqt.|.d.d.t.|
-00000730: 0619 0064 0219 0064 0983 057d 0764 0a74  ...d...d...}.d.t
-00000740: 047c 0619 0076 0072 4e74 047c 0619 0064  .|...v.rNt.|...d
-00000750: 0a19 007d 086e 0264 0b7d 087c 0864 0b6b  ...}.n.d.}.|.d.k
-00000760: 0372 6e64 0c74 047c 0619 0076 0072 6e74  .rnd.t.|...v.rnt
-00000770: 07a0 087c 0674 047c 017c 027c 0374 047c  ...|.t.|.|.|.t.|
-00000780: 0619 0064 0c19 0074 047c 0619 0064 0d19  ...d...t.|...d..
-00000790: 007c 05a1 087d 0764 0e74 047c 0619 0076  .|...}.d.t.|...v
-000007a0: 0072 a674 047c 0619 0064 0e19 0064 0b19  .r.t.|...d...d..
-000007b0: 007d 097c 0674 09a0 0a74 047c 0919 00a1  .}.|.t...t.|....
-000007c0: 0169 017d 0a74 047c 0619 0064 0219 007d  .i.}.t.|...d...}
-000007d0: 0b74 09a0 0a7c 0ba1 017c 0a64 023c 0074  .t...|...|.d.<.t
-000007e0: 07a0 087c 067c 0a7c 017c 027c 037c 0a7c  ...|.|.|.|.|.|.|
-000007f0: 0619 0064 0c19 007c 0a7c 0619 0064 0d19  ...d...|.|...d..
-00000800: 007c 05a1 087d 0774 0b7c 0783 017d 077c  .|...}.t.|...}.|
-00000810: 0753 0029 0f61 9501 0000 0a20 2020 2047  .S.).a.....    G
-00000820: 6976 656e 2061 6e20 6163 7469 6f6e 2063  iven an action c
-00000830: 6f64 652c 2065 7661 6c75 6174 6520 6974  ode, evaluate it
-00000840: 2066 6f72 2064 6973 706c 6179 0a20 2020   for display.   
-00000850: 2020 2020 203a 7061 7261 6d20 636f 6465       :param code
-00000860: 5f63 6869 6c64 3a20 786d 6c20 656c 656d  _child: xml elem
-00000870: 656e 7420 6f66 2074 6865 203c 636f 6465  ent of the <code
-00000880: 3e0a 2020 2020 2020 2020 3a70 6172 616d  >.        :param
-00000890: 2063 6f64 655f 6163 7469 6f6e 3a20 7661   code_action: va
-000008a0: 6c75 6520 6f66 203c 636f 6465 3e20 2865  lue of <code> (e
-000008b0: 2e67 2e20 2235 3439 2229 0a20 2020 2020  .g. "549").     
-000008c0: 2020 203a 7061 7261 6d20 6163 7469 6f6e     :param action
-000008d0: 5f74 7970 653a 0a20 2020 2020 2020 203a  _type:.        :
-000008e0: 7061 7261 6d20 636f 6c6f 726d 6170 3a20  param colormap: 
-000008f0: 636f 6c6f 7273 2074 6f20 7573 6520 696e  colors to use in
-00000900: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
-00000910: 3a70 6172 616d 2063 6f64 655f 7479 7065  :param code_type
-00000920: 3a20 2765 273d 6576 656e 742c 2027 7327  : 'e'=event, 's'
-00000930: 3d73 7461 7465 2c20 2774 273d 7461 736b  =state, 't'=task
-00000940: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000950: 7072 6f67 7261 6d5f 6172 6773 3a20 7275  program_args: ru
-00000960: 6e74 696d 6520 6172 6775 6d65 6e74 730a  ntime arguments.
-00000970: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00000980: 2066 6f72 6d61 7474 6564 206f 7574 7075   formatted outpu
-00000990: 7420 6c69 6e65 2077 6974 6820 6163 7469  t line with acti
-000009a0: 6f6e 2064 6574 6169 6c73 0a20 2020 207a  on details.    z
-000009b0: 0867 6574 636f 6465 3a72 1100 0000 7a05  .getcode:r....z.
-000009c0: 436f 6465 207a 0f20 6e6f 7420 7965 7420  Code z. not yet 
-000009d0: 6d61 7070 6564 7a14 756e 6d61 7070 6564  mappedz.unmapped
-000009e0: 2074 6173 6b20 636f 6465 3a20 fa01 205a   task code: .. Z
-000009f0: 1161 6374 696f 6e5f 6e61 6d65 5f63 6f6c  .action_name_col
-00000a00: 6f72 7207 0000 0054 720f 0000 0072 0100  orr....Tr....r..
-00000a10: 0000 7210 0000 005a 0865 7661 6c61 7267  ..r....Z.evalarg
-00000a20: 735a 0872 6564 6972 6563 7429 0c72 0500  sZ.redirect).r..
-00000a30: 0000 7214 0000 00da 0474 6578 7472 1f00  ..r......textr..
-00000a40: 0000 7204 0000 0072 0200 0000 7203 0000  ..r....r....r...
-00000a50: 00da 0e61 6374 696f 6e5f 7265 7375 6c74  ...action_result
-00000a60: 735a 1267 6574 5f61 6374 696f 6e5f 7265  sZ.get_action_re
-00000a70: 7375 6c74 73da 0463 6f70 79da 0864 6565  sults..copy..dee
-00000a80: 7063 6f70 7972 0e00 0000 290c 7220 0000  pcopyr....).r ..
-00000a90: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
-00000aa0: 7224 0000 0072 2500 0000 721d 0000 005a  r$...r%...r....Z
-00000ab0: 0a74 6865 5f72 6573 756c 7472 0f00 0000  .the_resultr....
-00000ac0: 5a08 7265 6665 7272 616c 5a11 7465 6d70  Z.referralZ.temp
-00000ad0: 5f6c 6f6f 6b75 705f 636f 6465 735a 0c64  _lookup_codesZ.d
-00000ae0: 6973 706c 6179 5f6e 616d 6572 0c00 0000  isplay_namer....
-00000af0: 720c 0000 0072 0d00 0000 da0f 6765 745f  r....r......get_
-00000b00: 6163 7469 6f6e 5f63 6f64 655e 0000 0073  action_code^...s
-00000b10: 5e00 0000 1612 0a01 0802 1402 0802 0c01  ^...............
-00000b20: 04ff 02ff 1404 0204 1201 04ff 0c04 0e01  ................
-00000b30: 0402 1402 0401 0201 0201 0201 0201 0201  ................
-00000b40: 0a01 0a01 0201 04f8 0c0c 0a01 0201 04ff  ................
-00000b50: 1203 0601 0201 04ff 0e03 0402 0201 0201  ................
-00000b60: 0201 0201 0201 0a01 0a01 0201 04f8 080b  ................
-00000b70: 0401 722c 0000 0063 0600 0000 0000 0000  ..r,...c........
-00000b80: 0000 0000 0c00 0000 0a00 0000 4300 0000  ............C...
-00000b90: 7312 0100 0064 0164 026c 006d 017d 0601  s....d.d.l.m.}..
-00000ba0: 007c 047d 077c 0764 016b 0372 1d7c 02a0  .|.}.|.d.k.r.|..
-00000bb0: 0274 039b 0064 039d 0274 039b 0064 037c  .t...d...t...d.|
-00000bc0: 059b 009d 0364 04a1 037d 0264 017d 077c  .....d...}.d.}.|
-00000bd0: 0764 016b 0072 257c 057c 0217 007d 027c  .d.k.r%|.|...}.|
-00000be0: 0264 056b 0372 7d7c 02a0 0464 06a1 017d  .d.k.r}|...d...}
-00000bf0: 0874 057c 0283 017d 097c 0864 076b 0272  .t.|...}.|.d.k.r
-00000c00: 417c 0964 086b 0472 417c 01a0 067c 02a1  A|.d.k.rA|...|..
-00000c10: 0101 0064 0053 007c 02a0 0764 06a1 017d  ...d.S.|...d...}
-00000c20: 0a64 017d 077c 0a44 005d 307d 0b7c 0764  .d.}.|.D.]0}.|.d
-00000c30: 016b 0272 567c 01a0 067c 0ba1 0101 006e  .k.rV|...|.....n
-00000c40: 087c 01a0 0664 097c 0b9b 009d 02a1 0101  .|...d.|........
-00000c50: 007c 0764 0437 007d 077c 077c 066b 0272  .|.d.7.}.|.|.k.r
-00000c60: 7a7c 01a0 0674 087c 0064 0a64 0564 0b74  z|...t.|.d.d.d.t
-00000c70: 097c 0683 019b 0064 0c9d 0364 0d83 05a1  .|.....d...d....
-00000c80: 0101 0001 0064 0053 0071 4a64 0053 007c  .....d.S.qJd.S.|
-00000c90: 01a0 0664 0e7c 036a 0a9b 0064 0f9d 03a1  ...d.|.j...d....
-00000ca0: 0101 0064 0053 0029 104e 7201 0000 0029  ...d.S.).Nr....)
-00000cb0: 01da 0e43 4f4e 5449 4e55 455f 4c49 4d49  ...CONTINUE_LIMI
-00000cc0: 547a 0222 3ee9 0100 0000 7207 0000 00da  Tz.">.....r.....
-00000cd0: 010a 721c 0000 00e9 5000 0000 7a03 2e2e  ..r.....P...z...
-00000ce0: 2e5a 0352 6564 7a17 202e 2e2e 2063 6f6e  .Z.Redz. ... con
-00000cf0: 7469 6e75 6520 6c69 6d69 7420 6f66 207a  tinue limit of z
-00000d00: 3a20 7265 6163 6865 642e 2020 5365 6520  : reached.  See 
-00000d10: 2243 4f4e 5449 4e55 455f 4c49 4d49 5420  "CONTINUE_LIMIT 
-00000d20: 3d22 2069 6e20 636f 6e66 6967 2e70 7920  =" in config.py 
-00000d30: 666f 7220 6465 7461 696c 7354 7a07 4163  for detailsTz.Ac
-00000d40: 7469 6f6e 207a 103a 206e 6f74 2079 6574  tion z.: not yet
-00000d50: 206d 6170 7065 6429 0b5a 146d 6170 7461   mapped).Z.mapta
-00000d60: 736b 6572 2e73 7263 2e63 6f6e 6669 6772  sker.src.configr
-00000d70: 2d00 0000 7208 0000 0072 0600 0000 da04  -...r....r......
-00000d80: 6669 6e64 da03 6c65 6eda 0661 7070 656e  find..len..appen
-00000d90: 64da 0573 706c 6974 7203 0000 00da 0373  d..splitr......s
-00000da0: 7472 7228 0000 0029 0c72 2300 0000 5a05  trr(...).r#...Z.
-00000db0: 616c 6973 745a 0574 636f 6465 5a0c 636f  alistZ.tcodeZ.co
-00000dc0: 6465 5f65 6c65 6d65 6e74 da06 696e 6465  de_element..inde
-00000dd0: 6e74 5a0a 696e 6465 6e74 5f61 6d74 722d  ntZ.indent_amtr-
-00000de0: 0000 00da 0563 6f75 6e74 da07 6e65 776c  .....count..newl
-00000df0: 696e 655a 0974 636f 6465 5f6c 656e 5a0e  ineZ.tcode_lenZ.
-00000e00: 6172 7261 795f 6f66 5f6c 696e 6573 7217  array_of_linesr.
-00000e10: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000e20: 0000 da0c 6275 696c 645f 6163 7469 6f6e  ....build_action
-00000e30: b000 0000 7348 0000 000c 0104 0308 011e  ....sH..........
-00000e40: 0104 0108 0108 0108 030a 0108 0110 030a  ................
-00000e50: 0104 1c0a e604 0108 0108 010c 0110 0208  ................
-00000e60: 0108 0204 0102 0102 0102 0102 010e 0202  ................
-00000e70: 0402 f704 ff02 0d04 0302 ef04 1114 ff04  ................
-00000e80: 0172 3900 0000 291d 722a 0000 00da 0272  .r9...).r*.....r
-00000e90: 65da 1664 6566 7573 6564 786d 6c2e 456c  e..defusedxml.El
-00000ea0: 656d 656e 7454 7265 65da 0a64 6566 7573  ementTree..defus
-00000eb0: 6564 786d 6c5a 156d 6170 7461 736b 6572  edxmlZ.maptasker
-00000ec0: 2e73 7263 2e61 6374 696f 6e72 da03 7372  .src.actionr..sr
-00000ed0: 635a 0761 6374 696f 6e72 7229 0000 005a  cZ.actionrr)...Z
-00000ee0: 146d 6170 7461 736b 6572 2e73 7263 2e61  .maptasker.src.a
-00000ef0: 6374 696f 6e72 0200 0000 5a16 6d61 7074  ctionr....Z.mapt
-00000f00: 6173 6b65 722e 7372 632e 6672 6d74 6874  asker.src.frmtht
-00000f10: 6d6c 7203 0000 005a 156d 6170 7461 736b  mlr....Z.maptask
-00000f20: 6572 2e73 7263 2e61 6374 696f 6e63 7204  er.src.actioncr.
-00000f30: 0000 00da 166d 6170 7461 736b 6572 2e73  .....maptasker.s
-00000f40: 7263 2e73 7973 636f 6e73 7472 0500 0000  rc.sysconstr....
-00000f50: 7206 0000 00da 0763 6f6d 7069 6c65 7209  r......compiler.
-00000f60: 0000 0072 0e00 0000 721a 0000 0072 1f00  ...r....r....r..
-00000f70: 0000 da0b 456c 656d 656e 7454 7265 65da  ....ElementTree.
-00000f80: 0358 4d4c da04 626f 6f6c da04 6469 6374  .XML..bool..dict
-00000f90: 7235 0000 0072 2c00 0000 7239 0000 0072  r5...r,...r9...r
-00000fa0: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000fb0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000fc0: 0073 3a00 0000 080c 0801 0801 1202 0c02  .s:.............
-00000fd0: 0c01 0c01 0c01 0c01 0a02 0809 0817 0817  ................
-00000fe0: 020e 0601 02ff 0602 02fe 0203 02fd 0204  ................
-00000ff0: 02fc 0205 02fb 0206 02fa 0207 0af9 0c52  ...............R
+00000080: 6c0e 6d0f 5a0f 0100 6400 6406 6c10 6d11  l.m.Z...d.d.l.m.
+00000090: 5a11 0100 6400 6407 6c10 6d12 5a12 0100  Z...d.d.l.m.Z...
+000000a0: 6501 a013 6408 a101 5a14 6409 640a 8400  e...d...Z.d.d...
+000000b0: 5a15 641a 640c 640d 8404 5a16 640e 640f  Z.d.d.d...Z.d.d.
+000000c0: 8400 5a17 6410 6503 6a18 6a19 6411 6503  ..Z.d.e.j.j.d.e.
+000000d0: 6a18 6a19 6412 651a 6413 651b 6414 651c  j.j.d.e.d.e.d.e.
+000000e0: 6415 651b 640b 651c 660e 6416 6417 8404  d.e.d.e.f.d.d...
+000000f0: 5a1d 6418 6419 8400 5a1e 6401 5300 291b  Z.d.d...Z.d.S.).
+00000100: e900 0000 004e 2901 da0f 6765 745f 6578  .....N)...get_ex
+00000110: 7472 615f 7374 7566 6629 01da 0b66 6f72  tra_stuff)...for
+00000120: 6d61 745f 6874 6d6c 2901 da0d 6572 726f  mat_html)...erro
+00000130: 725f 6861 6e64 6c65 7229 01da 0c61 6374  r_handler)...act
+00000140: 696f 6e5f 636f 6465 7329 01da 066c 6f67  ion_codes)...log
+00000150: 6765 7229 01da 0b46 4f4e 545f 544f 5f55  ger)...FONT_TO_U
+00000160: 5345 7a06 2c5b 2c20 5d2b 6301 0000 0000  SEz.,[, ]+c.....
+00000170: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+00000180: 0000 0073 9400 0000 7c00 a000 6401 6402  ...s....|...d.d.
+00000190: a102 7d00 7c00 a000 6403 6404 a102 7d00  ..}.|...d.d...}.
+000001a0: 7401 a002 6405 7c00 a102 7d00 7c00 a000  t...d.|...}.|...
+000001b0: 6406 6407 a102 7d00 7c00 a000 6408 6409  d.d...}.|...d.d.
+000001c0: a102 7d00 7c00 a000 640a 6404 a102 7d00  ..}.|...d.d...}.
+000001d0: 7c00 a000 640b 6404 a102 7d00 7c00 a000  |...d.d...}.|...
+000001e0: 640c 6404 a102 7d00 7c00 a000 640d 6404  d.d...}.|...d.d.
+000001f0: a102 7d00 7c00 a000 640e 6404 a102 7d00  ..}.|...d.d...}.
+00000200: 7c00 a000 640f 6404 a102 7d00 7c00 a000  |...d.d...}.|...
+00000210: 6410 6411 a102 7d00 7c00 5300 2912 4e7a  d.d...}.|.S.).Nz
+00000220: 092c 2020 3c66 6f6e 743e 7a06 3c66 6f6e  .,  <font>z.<fon
+00000230: 743e 7a03 2c20 28da 007a 022c 207a 072c  t>z., (..z., z.,
+00000240: 203c 7370 616e 7a05 3c73 7061 6e7a 082c   <spanz.<spanz.,
+00000250: 2020 3c73 7061 6e7a 0720 203c 7370 616e    <spanz.  <span
+00000260: 7a07 2c20 636f 6465 3a7a 053c 6269 673e  z., code:z.<big>
+00000270: 7a07 3c73 6d61 6c6c 3e7a 043c 7474 3e7a  z.<small>z.<tt>z
+00000280: 033c 693e 7a03 3c75 3e7a 072c 203c 666f  .<i>z.<u>z., <fo
+00000290: 6e74 7a05 3c66 6f6e 7429 03da 0772 6570  ntz.<font)...rep
+000002a0: 6c61 6365 da07 7061 7474 6572 6eda 0373  lace..pattern..s
+000002b0: 7562 2901 da07 7265 7375 6c74 73a9 0072  ub)...results..r
+000002c0: 0d00 0000 fa76 2f55 7365 7273 2f6d 696b  .....v/Users/mik
+000002d0: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
+000002e0: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
+000002f0: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
+00000300: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
+00000310: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
+00000320: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
+00000330: 632f 6163 7469 6f6e 652e 7079 da12 636c  c/actione.py..cl
+00000340: 6561 6e75 705f 7468 655f 7265 7375 6c74  eanup_the_result
+00000350: 2300 0000 731e 0000 0004 0304 0104 ff0c  #...s...........
+00000360: 030c 010c 010c 010c 010c 010c 010c 010c  ................
+00000370: 010c 010c 0104 0172 0f00 0000 da06 7265  .......r......re
+00000380: 7475 726e 6300 0000 0000 0000 0000 0000  turnc...........
+00000390: 0004 0000 0006 0000 0043 0000 0073 6200  .........C...sb.
+000003a0: 0000 6401 7d00 7400 4400 5d2a 7d01 7400  ..d.}.t.D.]*}.t.
+000003b0: 7c01 1900 7d02 7c02 6402 1900 7d03 7c03  |...}.|.d...}.|.
+000003c0: 6403 6b04 7221 6404 7c02 7601 7221 7401  d.k.r!d.|.v.r!t.
+000003d0: 6405 7c01 9b00 6406 7c03 9b00 9d04 6407  d.|...d.|.....d.
+000003e0: 8302 0100 6408 7c02 7601 722e 7401 6405  ....d.|.v.r.t.d.
+000003f0: 7c01 9b00 6409 9d03 6407 8302 0100 7104  |...d...d.....q.
+00000400: 640a 5300 290b 7a9d 0a20 2020 2046 6f72  d.S.).z..    For
+00000410: 2064 6562 7567 2070 7572 706f 7365 732c   debug purposes,
+00000420: 2074 6869 7320 7365 6172 6368 6573 2064   this searches d
+00000430: 6963 7469 6f6e 6172 7920 666f 7220 6d69  ictionary for mi
+00000440: 7373 696e 6720 6b65 7973 3a20 2772 6571  ssing keys: 'req
+00000450: 6172 6773 2720 616e 6420 2764 6973 706c  args' and 'displ
+00000460: 6179 270a 2020 2020 2020 2020 4966 2066  ay'.        If f
+00000470: 6f75 6e64 2c20 7468 6520 6572 726f 7220  ound, the error 
+00000480: 6973 2068 616e 646c 6564 2061 6e64 2074  is handled and t
+00000490: 6865 2070 726f 6772 616d 2065 7869 7473  he program exits
+000004a0: 0a20 2020 2046 da07 6e75 6d61 7267 7372  .    F..numargsr
+000004b0: 0100 0000 da07 7265 7161 7267 737a 0a64  ......reqargsz.d
+000004c0: 6963 745f 636f 6465 207a 1b20 6d69 7373  ict_code z. miss
+000004d0: 696e 6720 7265 7161 7267 7321 2020 6e75  ing reqargs!  nu
+000004e0: 6d61 7267 733a e901 0000 00da 0764 6973  margs:.......dis
+000004f0: 706c 6179 7a13 206d 6973 7369 6e67 2022  playz. missing "
+00000500: 6469 7370 6c61 7922 214e 2902 7205 0000  display"!N).r...
+00000510: 0072 0400 0000 2904 da04 666c 6167 da04  .r....)...flag..
+00000520: 6974 656d da05 656e 7472 7972 1100 0000  item..entryr....
+00000530: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+00000540: 146c 6f6f 6b5f 666f 725f 6d69 7373 696e  .look_for_missin
+00000550: 675f 7265 713a 0000 0073 1a00 0000 0405  g_req:...s......
+00000560: 0801 0801 0801 1002 0201 0e01 0201 04fe  ................
+00000570: 0805 1201 0280 0402 7218 0000 0063 0100  ........r....c..
+00000580: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00000590: 0000 4300 0000 7344 0000 0064 0164 026c  ..C...sD...d.d.l
+000005a0: 006d 017d 0101 007c 0064 0064 0385 0219  .m.}...|.d.d....
+000005b0: 007d 027c 027c 0176 0072 207c 0074 0276  .}.|.|.v.r |.t.v
+000005c0: 0072 2064 0474 027c 0019 0064 0419 0064  .r d.t.|...d...d
+000005d0: 0517 0069 0174 027c 003c 0064 0053 0029  ...i.t.|.<.d.S.)
+000005e0: 064e 7201 0000 0029 01da 0a64 6570 7269  .Nr....)...depri
+000005f0: 6361 7465 64e9 ffff ffff 7214 0000 007a  cated.....r....z
+00000600: 1a3c 656d 3e20 2849 7320 4465 7072 6563  .<em> (Is Deprec
+00000610: 6174 6564 293c 2f65 6d3e 2029 035a 186d  ated)</em> ).Z.m
+00000620: 6170 7461 736b 6572 2e73 7263 2e64 6570  aptasker.src.dep
+00000630: 7269 6361 7465 6472 1900 0000 7205 0000  ricatedr....r...
+00000640: 0029 03da 0964 6963 745f 636f 6465 7219  .)...dict_coder.
+00000650: 0000 00da 066c 6f6f 6b75 7072 0d00 0000  .....lookupr....
+00000660: 720d 0000 0072 0e00 0000 da15 6368 6563  r....r......chec
+00000670: 6b5f 666f 725f 6465 7072 6563 6174 696f  k_for_deprecatio
+00000680: 6e53 0000 0073 0c00 0000 0c01 0c02 1001  nS...s..........
+00000690: 1002 08ff 0403 721d 0000 00da 0a63 6f64  ......r......cod
+000006a0: 655f 6368 696c 64da 0b63 6f64 655f 6163  e_child..code_ac
+000006b0: 7469 6f6e da0b 6163 7469 6f6e 5f74 7970  tion..action_typ
+000006c0: 65da 0863 6f6c 6f72 6d61 70da 0963 6f64  e..colormap..cod
+000006d0: 655f 7479 7065 da0c 7072 6f67 7261 6d5f  e_type..program_
+000006e0: 6172 6773 6306 0000 0000 0000 0000 0000  argsc...........
+000006f0: 000c 0000 000a 0000 0043 0000 0073 5801  .........C...sX.
+00000700: 0000 7400 a001 6401 7c00 6a02 9b00 7c04  ..t...d.|.j...|.
+00000710: 9b00 9d03 a101 0100 7c00 6a02 7c04 1700  ........|.j.|...
+00000720: 7d06 7403 7c06 8301 0100 7c06 7404 7601  }.t.|.....|.t.v.
+00000730: 731e 6402 7404 7c06 1900 7601 7235 6403  s.d.t.|...v.r5d.
+00000740: 7c06 9b00 6404 7405 7c01 7c02 7c03 7c05  |...d.t.|.|.|.|.
+00000750: 8304 9b00 9d04 7d07 7400 a001 6405 7c06  ......}.t...d.|.
+00000760: 9b00 6406 9d03 a101 0100 6e71 7406 7c03  ..d.......nqt.|.
+00000770: 6407 6408 7404 7c06 1900 6402 1900 6409  d.d.t.|...d...d.
+00000780: 8305 7d07 640a 7404 7c06 1900 7600 724e  ..}.d.t.|...v.rN
+00000790: 7404 7c06 1900 640a 1900 7d08 6e02 640b  t.|...d...}.n.d.
+000007a0: 7d08 7c08 640b 6b03 726e 640c 7404 7c06  }.|.d.k.rnd.t.|.
+000007b0: 1900 7600 726e 7407 a008 7c06 7404 7c01  ..v.rnt...|.t.|.
+000007c0: 7c02 7c03 7404 7c06 1900 640c 1900 7404  |.|.t.|...d...t.
+000007d0: 7c06 1900 640d 1900 7c05 a108 7d07 640e  |...d...|...}.d.
+000007e0: 7404 7c06 1900 7600 72a6 7404 7c06 1900  t.|...v.r.t.|...
+000007f0: 640e 1900 640b 1900 7d09 7c06 7409 a00a  d...d...}.|.t...
+00000800: 7404 7c09 1900 a101 6901 7d0a 7404 7c06  t.|.....i.}.t.|.
+00000810: 1900 6402 1900 7d0b 7409 a00a 7c0b a101  ..d...}.t...|...
+00000820: 7c0a 6402 3c00 7407 a008 7c06 7c0a 7c01  |.d.<.t...|.|.|.
+00000830: 7c02 7c03 7c0a 7c06 1900 640c 1900 7c0a  |.|.|.|...d...|.
+00000840: 7c06 1900 640d 1900 7c05 a108 7d07 740b  |...d...|...}.t.
+00000850: 7c07 8301 7d07 7c07 5300 290f 6195 0100  |...}.|.S.).a...
+00000860: 000a 2020 2020 4769 7665 6e20 616e 2061  ..    Given an a
+00000870: 6374 696f 6e20 636f 6465 2c20 6576 616c  ction code, eval
+00000880: 7561 7465 2069 7420 666f 7220 6469 7370  uate it for disp
+00000890: 6c61 790a 2020 2020 2020 2020 3a70 6172  lay.        :par
+000008a0: 616d 2063 6f64 655f 6368 696c 643a 2078  am code_child: x
+000008b0: 6d6c 2065 6c65 6d65 6e74 206f 6620 7468  ml element of th
+000008c0: 6520 3c63 6f64 653e 0a20 2020 2020 2020  e <code>.       
+000008d0: 203a 7061 7261 6d20 636f 6465 5f61 6374   :param code_act
+000008e0: 696f 6e3a 2076 616c 7565 206f 6620 3c63  ion: value of <c
+000008f0: 6f64 653e 2028 652e 672e 2022 3534 3922  ode> (e.g. "549"
+00000900: 290a 2020 2020 2020 2020 3a70 6172 616d  ).        :param
+00000910: 2061 6374 696f 6e5f 7479 7065 3a0a 2020   action_type:.  
+00000920: 2020 2020 2020 3a70 6172 616d 2063 6f6c        :param col
+00000930: 6f72 6d61 703a 2063 6f6c 6f72 7320 746f  ormap: colors to
+00000940: 2075 7365 2069 6e20 6f75 7470 7574 0a20   use in output. 
+00000950: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+00000960: 6465 5f74 7970 653a 2027 6527 3d65 7665  de_type: 'e'=eve
+00000970: 6e74 2c20 2773 273d 7374 6174 652c 2027  nt, 's'=state, '
+00000980: 7427 3d74 6173 6b0a 2020 2020 2020 2020  t'=task.        
+00000990: 3a70 6172 616d 2070 726f 6772 616d 5f61  :param program_a
+000009a0: 7267 733a 2072 756e 7469 6d65 2061 7267  rgs: runtime arg
+000009b0: 756d 656e 7473 0a20 2020 2020 2020 203a  uments.        :
+000009c0: 7265 7475 726e 3a20 666f 726d 6174 7465  return: formatte
+000009d0: 6420 6f75 7470 7574 206c 696e 6520 7769  d output line wi
+000009e0: 7468 2061 6374 696f 6e20 6465 7461 696c  th action detail
+000009f0: 730a 2020 2020 7a08 6765 7463 6f64 653a  s.    z.getcode:
+00000a00: 7214 0000 007a 0543 6f64 6520 7a0f 206e  r....z.Code z. n
+00000a10: 6f74 2079 6574 206d 6170 7065 647a 1475  ot yet mappedz.u
+00000a20: 6e6d 6170 7065 6420 7461 736b 2063 6f64  nmapped task cod
+00000a30: 653a 20da 0120 5a11 6163 7469 6f6e 5f6e  e: .. Z.action_n
+00000a40: 616d 655f 636f 6c6f 7272 0800 0000 5472  ame_colorr....Tr
+00000a50: 1100 0000 7201 0000 0072 1200 0000 5a08  ....r....r....Z.
+00000a60: 6576 616c 6172 6773 5a08 7265 6469 7265  evalargsZ.redire
+00000a70: 6374 290c 7206 0000 00da 0564 6562 7567  ct).r......debug
+00000a80: da04 7465 7874 721d 0000 0072 0500 0000  ..textr....r....
+00000a90: 7202 0000 0072 0300 0000 da0e 6163 7469  r....r......acti
+00000aa0: 6f6e 5f72 6573 756c 7473 5a12 6765 745f  on_resultsZ.get_
+00000ab0: 6163 7469 6f6e 5f72 6573 756c 7473 da04  action_results..
+00000ac0: 636f 7079 da08 6465 6570 636f 7079 720f  copy..deepcopyr.
+00000ad0: 0000 0029 0c72 1e00 0000 721f 0000 0072  ...).r....r....r
+00000ae0: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
+00000af0: 0000 0072 1b00 0000 5a0a 7468 655f 7265  ...r....Z.the_re
+00000b00: 7375 6c74 7211 0000 005a 0872 6566 6572  sultr....Z.refer
+00000b10: 7261 6c5a 1174 656d 705f 6c6f 6f6b 7570  ralZ.temp_lookup
+00000b20: 5f63 6f64 6573 5a0c 6469 7370 6c61 795f  _codesZ.display_
+00000b30: 6e61 6d65 720d 0000 0072 0d00 0000 720e  namer....r....r.
+00000b40: 0000 00da 0f67 6574 5f61 6374 696f 6e5f  .....get_action_
+00000b50: 636f 6465 6100 0000 735e 0000 0016 120a  codea...s^......
+00000b60: 0108 0214 0208 020c 0104 ff02 ff14 0402  ................
+00000b70: 0412 0104 ff0c 040e 0104 0214 0204 0102  ................
+00000b80: 0102 0102 0102 0102 010a 010a 0102 0104  ................
+00000b90: f80c 0c0a 0102 0104 ff12 0306 0102 0104  ................
+00000ba0: ff0e 0304 0202 0102 0102 0102 0102 010a  ................
+00000bb0: 010a 0102 0104 f808 0b04 0172 2a00 0000  ...........r*...
+00000bc0: 6306 0000 0000 0000 0000 0000 000c 0000  c...............
+00000bd0: 000a 0000 0043 0000 0073 1201 0000 6401  .....C...s....d.
+00000be0: 6402 6c00 6d01 7d06 0100 7c04 7d07 7c07  d.l.m.}...|.}.|.
+00000bf0: 6401 6b03 721d 7c02 a002 7403 9b00 6403  d.k.r.|...t...d.
+00000c00: 9d02 7403 9b00 6403 7c05 9b00 9d03 6404  ..t...d.|.....d.
+00000c10: a103 7d02 6401 7d07 7c07 6401 6b00 7225  ..}.d.}.|.d.k.r%
+00000c20: 7c05 7c02 1700 7d02 7c02 6405 6b03 727d  |.|...}.|.d.k.r}
+00000c30: 7c02 a004 6406 a101 7d08 7405 7c02 8301  |...d...}.t.|...
+00000c40: 7d09 7c08 6407 6b02 7241 7c09 6408 6b04  }.|.d.k.rA|.d.k.
+00000c50: 7241 7c01 a006 7c02 a101 0100 7c01 5300  rA|...|.....|.S.
+00000c60: 7c02 a007 6406 a101 7d0a 6401 7d07 7c0a  |...d...}.d.}.|.
+00000c70: 4400 5d30 7d0b 7c07 6401 6b02 7256 7c01  D.]0}.|.d.k.rV|.
+00000c80: a006 7c0b a101 0100 6e08 7c01 a006 6409  ..|.....n.|...d.
+00000c90: 7c0b 9b00 9d02 a101 0100 7c07 6404 3700  |.........|.d.7.
+00000ca0: 7d07 7c07 7c06 6b02 727a 7c01 a006 7408  }.|.|.k.rz|...t.
+00000cb0: 7c00 640a 6405 640b 7409 7c06 8301 9b00  |.d.d.d.t.|.....
+00000cc0: 640c 9d03 640d 8305 a101 0100 0100 7c01  d...d.........|.
+00000cd0: 5300 714a 7c01 5300 7c01 a006 640e 7c03  S.qJ|.S.|...d.|.
+00000ce0: 6a0a 9b00 640f 9d03 a101 0100 7c01 5300  j...d.......|.S.
+00000cf0: 2910 4e72 0100 0000 2901 da0e 434f 4e54  ).Nr....)...CONT
+00000d00: 494e 5545 5f4c 494d 4954 7a02 223e 7213  INUE_LIMITz.">r.
+00000d10: 0000 0072 0800 0000 da01 0a72 1a00 0000  ...r.......r....
+00000d20: e950 0000 007a 032e 2e2e 5a03 5265 647a  .P...z....Z.Redz
+00000d30: 1720 2e2e 2e20 636f 6e74 696e 7565 206c  . ... continue l
+00000d40: 696d 6974 206f 6620 7a3a 2072 6561 6368  imit of z: reach
+00000d50: 6564 2e20 2053 6565 2022 434f 4e54 494e  ed.  See "CONTIN
+00000d60: 5545 5f4c 494d 4954 203d 2220 696e 2063  UE_LIMIT =" in c
+00000d70: 6f6e 6669 672e 7079 2066 6f72 2064 6574  onfig.py for det
+00000d80: 6169 6c73 547a 0741 6374 696f 6e20 7a10  ailsTz.Action z.
+00000d90: 3a20 6e6f 7420 7965 7420 6d61 7070 6564  : not yet mapped
+00000da0: 290b 5a14 6d61 7074 6173 6b65 722e 7372  ).Z.maptasker.sr
+00000db0: 632e 636f 6e66 6967 722b 0000 0072 0900  c.configr+...r..
+00000dc0: 0000 7207 0000 00da 0466 696e 64da 036c  ..r......find..l
+00000dd0: 656e da06 6170 7065 6e64 da05 7370 6c69  en..append..spli
+00000de0: 7472 0300 0000 da03 7374 7272 2600 0000  tr......strr&...
+00000df0: 290c 7221 0000 005a 0561 6c69 7374 5a05  ).r!...Z.alistZ.
+00000e00: 7463 6f64 655a 0c63 6f64 655f 656c 656d  tcodeZ.code_elem
+00000e10: 656e 74da 0669 6e64 656e 745a 0a69 6e64  ent..indentZ.ind
+00000e20: 656e 745f 616d 7472 2b00 0000 da05 636f  ent_amtr+.....co
+00000e30: 756e 74da 076e 6577 6c69 6e65 5a09 7463  unt..newlineZ.tc
+00000e40: 6f64 655f 6c65 6e5a 0e61 7272 6179 5f6f  ode_lenZ.array_o
+00000e50: 665f 6c69 6e65 7372 1600 0000 720d 0000  f_linesr....r...
+00000e60: 0072 0d00 0000 720e 0000 00da 0c62 7569  .r....r......bui
+00000e70: 6c64 5f61 6374 696f 6eb3 0000 0073 4800  ld_action....sH.
+00000e80: 0000 0c01 0403 0801 1e01 0401 0801 0801  ................
+00000e90: 0803 0a01 0801 1003 0a01 041c 0ae6 0401  ................
+00000ea0: 0801 0801 0c01 1002 0801 0802 0401 0201  ................
+00000eb0: 0201 0201 0201 0e02 0204 02f7 04ff 020d  ................
+00000ec0: 0403 02ef 0411 14ff 0401 7236 0000 0029  ..........r6...)
+00000ed0: 0272 1000 0000 4e29 1f72 2800 0000 da02  .r....N).r(.....
+00000ee0: 7265 da16 6465 6675 7365 6478 6d6c 2e45  re..defusedxml.E
+00000ef0: 6c65 6d65 6e74 5472 6565 da0a 6465 6675  lementTree..defu
+00000f00: 7365 6478 6d6c 5a15 6d61 7074 6173 6b65  sedxmlZ.maptaske
+00000f10: 722e 7372 632e 6163 7469 6f6e 72da 0373  r.src.actionr..s
+00000f20: 7263 5a07 6163 7469 6f6e 7272 2700 0000  rcZ.actionrr'...
+00000f30: 5a14 6d61 7074 6173 6b65 722e 7372 632e  Z.maptasker.src.
+00000f40: 6163 7469 6f6e 7202 0000 00da 166d 6170  actionr......map
+00000f50: 7461 736b 6572 2e73 7263 2e66 726d 7468  tasker.src.frmth
+00000f60: 746d 6c72 0300 0000 da13 6d61 7074 6173  tmlr......maptas
+00000f70: 6b65 722e 7372 632e 6572 726f 7272 0400  ker.src.errorr..
+00000f80: 0000 5a15 6d61 7074 6173 6b65 722e 7372  ..Z.maptasker.sr
+00000f90: 632e 6163 7469 6f6e 6372 0500 0000 da16  c.actioncr......
+00000fa0: 6d61 7074 6173 6b65 722e 7372 632e 7379  maptasker.src.sy
+00000fb0: 7363 6f6e 7374 7206 0000 0072 0700 0000  sconstr....r....
+00000fc0: da07 636f 6d70 696c 6572 0a00 0000 720f  ..compiler....r.
+00000fd0: 0000 0072 1800 0000 721d 0000 00da 0b45  ...r....r......E
+00000fe0: 6c65 6d65 6e74 5472 6565 da03 584d 4cda  lementTree..XML.
+00000ff0: 0462 6f6f 6cda 0464 6963 7472 3200 0000  .bool..dictr2...
+00001000: 722a 0000 0072 3600 0000 720d 0000 0072  r*...r6...r....r
+00001010: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
+00001020: 3c6d 6f64 756c 653e 0100 0000 733c 0000  <module>....s<..
+00001030: 0008 0c08 0108 0112 020c 020c 010c 010c  ................
+00001040: 010c 010c 010a 0208 090a 1708 1902 0e06  ................
+00001050: 0102 ff06 0202 fe02 0302 fd02 0402 fc02  ................
+00001060: 0502 fb02 0602 fa02 070a f90c 52         ............R
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/actionr.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/actionr.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 17:32:39 2023 UTC, .py size: 7252 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,187 +1,193 @@
-00000000: 6f0d 0d0a 0000 0000 b73c 3864 541c 0000  o........<8dT...
+00000000: 6f0d 0d0a 0000 0000 60a3 4a64 fb1c 0000  o.......`.Jd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0014 0000 0040 0000 0073 0c01 0000 6400  .....@...s....d.
+00000020: 0014 0000 0040 0000 0073 1801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a04 6400 6401 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 0200 0100 6d07 5a08 0100 6400 6403  m.....m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0d 6d0e 5a0e 0100  Z...d.d.l.m.Z...
 00000080: 6400 6406 6c0f 6d10 5a10 0100 6400 6407  d.d.l.m.Z...d.d.
 00000090: 6c11 6d12 5a12 0100 6400 6408 6c11 6d13  l.m.Z...d.d.l.m.
-000000a0: 5a13 0100 6409 6514 640a 6515 6604 640b  Z...d.e.d.e.f.d.
-000000b0: 640c 8404 5a16 640d 6504 6a17 6a18 640e  d...Z.d.e.j.j.d.
-000000c0: 6519 640f 6504 6a17 6a18 6410 651a 6411  e.d.e.j.j.d.e.d.
-000000d0: 6514 6412 6514 6413 6514 6414 6519 6409  e.d.e.d.e.d.e.d.
-000000e0: 6514 640a 651b 6614 6415 6416 8404 5a1c  e.d.e.f.d.d...Z.
-000000f0: 640d 6515 6413 6504 6a17 6a18 640f 6504  d.e.d.e.j.j.d.e.
-00000100: 6a17 6a18 6410 651a 6411 6504 6a17 6a18  j.j.d.e.d.e.j.j.
-00000110: 640e 6519 6515 1900 6414 6519 6515 1900  d.e.e...d.e.e...
-00000120: 6412 6504 6a17 6a18 640a 6515 6612 6417  d.e.j.j.d.e.f.d.
-00000130: 6418 8404 5a1d 6401 5300 2919 e900 0000  d...Z.d.S.).....
-00000140: 004e 2901 da0b 6465 6661 756c 7464 6963  .N)...defaultdic
-00000150: 7429 01da 0b61 6374 696f 6e5f 6172 6773  t)...action_args
-00000160: 2901 da0c 6163 7469 6f6e 5f63 6f64 6573  )...action_codes
-00000170: 2901 da0b 666f 726d 6174 5f68 746d 6c29  )...format_html)
-00000180: 01da 066c 6f67 6765 7229 01da 1d67 6574  ...logger)...get
-00000190: 5f78 6d6c 5f69 6e74 5f61 7267 756d 656e  _xml_int_argumen
-000001a0: 745f 746f 5f76 616c 7565 2901 da1d 6765  t_to_value)...ge
-000001b0: 745f 786d 6c5f 7374 725f 6172 6775 6d65  t_xml_str_argume
-000001c0: 6e74 5f74 6f5f 7661 6c75 65da 1165 7661  nt_to_value..eva
-000001d0: 6c75 6174 6564 5f72 6573 756c 7473 da06  luated_results..
-000001e0: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
-000001f0: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
-00000200: 5601 0000 6401 7d01 7c00 6402 1900 4400  V...d.}.|.d...D.
-00000210: 5da2 7d02 6401 7d03 7c02 0400 6403 6b02  ].}.d.}.|...d.k.
-00000220: 7222 0100 7c00 6404 1900 7221 7c00 6404  r"..|.d...r!|.d.
-00000230: 1900 6405 1900 7d03 7c00 6404 1900 a000  ..d...}.|.d.....
-00000240: 6405 a101 0100 6e7f 0400 6406 6b02 7239  d.....n...d.k.r9
-00000250: 0100 7c00 6407 1900 7238 7c00 6407 1900  ..|.d...r8|.d...
-00000260: 6405 1900 7d03 7c00 6407 1900 a000 6405  d...}.|.d.....d.
-00000270: a101 0100 6e68 0400 6408 6b02 7250 0100  ....nh..d.k.rP..
-00000280: 7c00 6409 1900 724f 7c00 6409 1900 6405  |.d...rO|.d...d.
-00000290: 1900 7d03 7c00 6409 1900 a000 6405 a101  ..}.|.d.....d...
-000002a0: 0100 6e51 0400 640a 6b02 7267 0100 7c00  ..nQ..d.k.rg..|.
-000002b0: 640b 1900 7266 7c00 640b 1900 6405 1900  d...rf|.d...d...
-000002c0: 7d03 7c00 640b 1900 a000 6405 a101 0100  }.|.d.....d.....
-000002d0: 6e3a 0400 640c 6b02 727e 0100 7c00 640d  n:..d.k.r~..|.d.
-000002e0: 1900 727d 7c00 640d 1900 6405 1900 7d03  ..r}|.d...d...}.
-000002f0: 7c00 640d 1900 a000 6405 a101 0100 6e23  |.d.....d.....n#
-00000300: 640e 6b02 7293 7c00 640f 1900 7292 7c00  d.k.r.|.d...r.|.
-00000310: 640f 1900 6405 1900 7d03 7c00 640f 1900  d...d...}.|.d...
-00000320: a000 6405 a101 0100 6e0e 0900 7401 a002  ..d.....n...t...
-00000330: 6410 7c02 9b00 9d02 a101 0100 7403 a004  d.|.........t...
-00000340: 6411 a101 0100 7c01 9b00 6412 7c03 9b00  d.....|...d.|...
-00000350: 9d03 7d01 7106 7c01 5300 2913 4eda 005a  ..}.q.|.S.).N..Z
-00000360: 1170 6f73 6974 696f 6e5f 6172 675f 7479  .position_arg_ty
-00000370: 7065 5a03 5374 72da 0a72 6573 756c 745f  peZ.Str..result_
-00000380: 7374 7272 0100 0000 5a03 496e 74da 0a72  strr....Z.Int..r
-00000390: 6573 756c 745f 696e 745a 0341 7070 5a0a  esult_intZ.AppZ.
-000003a0: 7265 7375 6c74 5f61 7070 5a0d 436f 6e64  result_appZ.Cond
-000003b0: 6974 696f 6e4c 6973 745a 0a72 6573 756c  itionListZ.resul
-000003c0: 745f 636f 6e5a 0349 6d67 5a0a 7265 7375  t_conZ.ImgZ.resu
-000003d0: 6c74 5f69 6d67 5a06 4275 6e64 6c65 5a0a  lt_imgZ.BundleZ.
-000003e0: 7265 7375 6c74 5f62 756e 7a36 4675 6e63  result_bunz6Func
-000003f0: 7469 6f6e 2067 6574 5f72 6573 756c 7473  tion get_results
-00000400: 5f69 6e5f 6172 675f 6f72 6465 723a 206e  _in_arg_order: n
-00000410: 6f20 6d61 7463 6820 666f 7220 2261 7267  o match for "arg
-00000420: 223a e908 0000 00fa 0120 2905 da03 706f  ":....... )...po
-00000430: 7072 0600 0000 da05 6465 6275 67da 0373  pr......debug..s
-00000440: 7973 da04 6578 6974 2904 7209 0000 005a  ys..exit).r....Z
-00000450: 0d72 6574 7572 6e5f 7265 7375 6c74 da03  .return_result..
-00000460: 6172 675a 0874 6865 5f69 7465 6da9 0072  argZ.the_item..r
-00000470: 1500 0000 fa76 2f55 7365 7273 2f6d 696b  .....v/Users/mik
-00000480: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
-00000490: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
-000004a0: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
-000004b0: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
-000004c0: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
-000004d0: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
-000004e0: 632f 6163 7469 6f6e 722e 7079 da18 6765  c/actionr.py..ge
-000004f0: 745f 7265 7375 6c74 735f 696e 5f61 7267  t_results_in_arg
-00000500: 5f6f 7264 6572 1e00 0000 7356 0000 0004  _order....sV....
-00000510: 010c 0104 0102 010a 0108 010c 0108 0102  ................
-00000520: 0104 ff02 800a 0308 010c 010e 0102 800a  ................
-00000530: 0108 010c 010e 0102 800a 0108 010c 010e  ................
-00000540: 0102 800a 0108 010c 010e 0102 8006 0108  ................
-00000550: 010c 010e 0102 8002 0104 0108 0104 ff0a  ................
-00000560: 0310 0104 0172 1700 0000 da09 6469 6374  .....r......dict
-00000570: 5f63 6f64 65da 0861 7267 5f6c 6973 74da  _code..arg_list.
-00000580: 0b63 6f64 655f 6163 7469 6f6e da0b 6163  .code_action..ac
-00000590: 7469 6f6e 5f74 7970 65da 0863 6f6c 6f72  tion_type..color
-000005a0: 6d61 70da 0c70 726f 6772 616d 5f61 7267  map..program_arg
-000005b0: 73da 116c 6f6f 6b75 705f 636f 6465 5f65  s..lookup_code_e
-000005c0: 6e74 7279 da0d 6576 616c 7561 7465 5f6c  ntry..evaluate_l
-000005d0: 6973 7463 0900 0000 0000 0000 0000 0000  istc............
-000005e0: 0900 0000 0a00 0000 4300 0000 7364 0000  ........C...sd..
-000005f0: 0074 007c 017c 007c 067c 077c 027c 037c  .t.|.|.|.|.|.|.|
-00000600: 047c 057c 0883 097d 087c 0864 0119 0072  .|.|...}.|.d...r
-00000610: 307c 0864 0219 0072 2074 017c 027c 0864  0|.d...r t.|.|.d
-00000620: 0219 007c 0864 0319 0083 037c 0864 043c  ...|.d.....|.d.<
-00000630: 007c 0864 0519 0072 3074 027c 027c 0864  .|.d...r0t.|.|.d
-00000640: 0519 007c 0864 0619 0083 037c 0864 073c  ...|.d.....|.d.<
-00000650: 007c 0853 0029 084e 5a0c 6765 745f 786d  .|.S.).NZ.get_xm
-00000660: 6c5f 666c 6167 5a07 7374 7261 7267 735a  l_flagZ.strargsZ
-00000670: 0773 7472 6576 616c 720c 0000 005a 0769  .strevalr....Z.i
-00000680: 6e74 6172 6773 5a07 696e 7465 7661 6c72  ntargsZ.intevalr
-00000690: 0d00 0000 2903 7203 0000 0072 0800 0000  ....).r....r....
-000006a0: 7207 0000 0029 0972 1800 0000 7219 0000  r....).r....r...
-000006b0: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-000006c0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-000006d0: 0900 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-000006e0: 0000 00da 1465 7661 6c75 6174 655f 6163  .....evaluate_ac
-000006f0: 7469 6f6e 5f61 7267 734a 0000 0073 2a00  tion_argsJ...s*.
-00000700: 0000 020c 0201 0201 0201 0201 0201 0201  ................
-00000710: 0201 0201 0201 04f7 080c 0801 0201 0e01  ................
-00000720: 08ff 0803 0201 0e01 08ff 0404 7220 0000  ............r ..
-00000730: 0063 0800 0000 0000 0000 0000 0000 0b00  .c..............
-00000740: 0000 0e00 0000 4300 0000 73a6 0000 0074  ......C...s....t
-00000750: 0064 0164 0284 0083 017d 0864 037d 0964  .d.d.....}.d.}.d
-00000760: 047d 0a7c 057c 017c 0019 0064 053c 007c  .}.|.|.|...d.<.|
-00000770: 067c 017c 0019 0064 063c 007c 0572 2a7c  .|.|...d.<.|.r*|
-00000780: 0764 0719 0064 086b 0372 2a74 017c 007c  .d...d.k.r*t.|.|
-00000790: 057c 027c 037c 047c 077c 017c 067c 0883  .|.|.|.|.|.|.|..
-000007a0: 097d 087c 0864 0919 0072 3274 027c 0883  .}.|.d...r2t.|..
-000007b0: 017d 0a74 037c 0464 0a64 0474 047c 0019  .}.t.|.d.d.t.|..
-000007c0: 0064 0b19 0064 0c83 0574 037c 0464 0d64  .d...d...t.|.d.d
-000007d0: 047c 099b 007c 0a9b 0064 0e74 05a0 067c  .|...|...d.t...|
-000007e0: 027c 037c 047c 07a1 049b 009d 0464 0f83  .|.|.|.......d..
-000007f0: 0517 0053 0029 104e 6300 0000 0000 0000  ...S.).Nc.......
-00000800: 0000 0000 0000 0000 0001 0000 0053 0000  .............S..
-00000810: 0073 0400 0000 6700 5300 2901 4e72 1500  .s....g.S.).Nr..
-00000820: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00000830: 0072 1600 0000 da08 3c6c 616d 6264 613e  .r......<lambda>
-00000840: 7e00 0000 7302 0000 0004 007a 2467 6574  ~...s......z$get
-00000850: 5f61 6374 696f 6e5f 7265 7375 6c74 732e  _action_results.
-00000860: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00000870: 3e7a 0c26 6e62 7370 3b26 6e62 7370 3b72  >z.&nbsp;&nbsp;r
-00000880: 0b00 0000 da07 7265 7161 7267 73da 0865  ......reqargs..e
-00000890: 7661 6c61 7267 735a 1464 6973 706c 6179  valargsZ.display
-000008a0: 5f64 6574 6169 6c5f 6c65 7665 6ce9 0200  _detail_level...
-000008b0: 0000 5a13 7265 7475 726e 696e 675f 736f  ..Z.returning_so
-000008c0: 6d65 7468 696e 67da 1161 6374 696f 6e5f  mething..action_
-000008d0: 6e61 6d65 5f63 6f6c 6f72 da07 6469 7370  name_color..disp
-000008e0: 6c61 7954 da0c 6163 7469 6f6e 5f63 6f6c  layT..action_col
-000008f0: 6f72 7a07 3c2f 7370 616e 3e46 2907 7202  orz.</span>F).r.
-00000900: 0000 0072 2000 0000 7217 0000 0072 0500  ...r ...r....r..
-00000910: 0000 7204 0000 00da 0a67 6574 5f61 6374  ..r......get_act
-00000920: 696f 6eda 0f67 6574 5f65 7874 7261 5f73  ion..get_extra_s
-00000930: 7475 6666 290b 7218 0000 0072 1e00 0000  tuff).r....r....
-00000940: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
-00000950: 1900 0000 721f 0000 0072 1d00 0000 7209  ....r....r....r.
-00000960: 0000 005a 0a74 776f 5f62 6c61 6e6b 73da  ...Z.two_blanks.
-00000970: 0672 6573 756c 7472 1500 0000 7215 0000  .resultr....r...
-00000980: 0072 1600 0000 da12 6765 745f 6163 7469  .r......get_acti
-00000990: 6f6e 5f72 6573 756c 7473 7300 0000 7344  on_resultss...sD
-000009a0: 0000 0002 0a06 0104 ff04 0304 010c 040c  ................
-000009b0: 0110 0202 0202 0102 0102 0102 0102 0102  ................
-000009c0: 0102 0102 0102 0104 f708 0d08 0102 0312  ................
-000009d0: 0102 ff02 0202 0102 0102 010a 020e 0104  ................
-000009e0: ff02 0302 f804 fe72 2b00 0000 291e 7212  .......r+...).r.
-000009f0: 0000 00da 0b63 6f6c 6c65 6374 696f 6e73  .....collections
-00000a00: 7202 0000 00da 1664 6566 7573 6564 786d  r......defusedxm
-00000a10: 6c2e 456c 656d 656e 7454 7265 65da 0a64  l.ElementTree..d
-00000a20: 6566 7573 6564 786d 6cda 146d 6170 7461  efusedxml..mapta
-00000a30: 736b 6572 2e73 7263 2e61 6374 696f 6eda  sker.src.action.
-00000a40: 0373 7263 da06 6163 7469 6f6e 7228 0000  .src..actionr(..
-00000a50: 005a 156d 6170 7461 736b 6572 2e73 7263  .Z.maptasker.src
-00000a60: 2e61 6374 6172 6773 7203 0000 00da 156d  .actargsr......m
-00000a70: 6170 7461 736b 6572 2e73 7263 2e61 6374  aptasker.src.act
-00000a80: 696f 6e63 7204 0000 00da 166d 6170 7461  ioncr......mapta
-00000a90: 736b 6572 2e73 7263 2e66 726d 7468 746d  sker.src.frmthtm
-00000aa0: 6c72 0500 0000 da16 6d61 7074 6173 6b65  lr......maptaske
-00000ab0: 722e 7372 632e 7379 7363 6f6e 7374 7206  r.src.sysconstr.
-00000ac0: 0000 005a 156d 6170 7461 736b 6572 2e73  ...Z.maptasker.s
-00000ad0: 7263 2e78 6d6c 6461 7461 7207 0000 0072  rc.xmldatar....r
-00000ae0: 0800 0000 da04 6469 6374 da03 7374 7272  ......dict..strr
-00000af0: 1700 0000 da0b 456c 656d 656e 7454 7265  ......ElementTre
-00000b00: 65da 0358 4d4c da04 6c69 7374 da04 626f  e..XML..list..bo
-00000b10: 6f6c da05 7475 706c 6572 2000 0000 722b  ol..tupler ...r+
-00000b20: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
-00000b30: 0000 7216 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000b40: 3e01 0000 0073 6600 0000 080c 0c01 0802  >....sf.........
-00000b50: 1202 0c01 0c01 0c01 0c01 0c01 0c01 1206  ................
-00000b60: 022c 0601 02ff 0202 02fe 0603 02fd 0204  .,..............
-00000b70: 02fc 0205 02fb 0206 02fa 0207 02f9 0208  ................
-00000b80: 02f8 0209 02f7 020a 0af6 0229 0201 02ff  ...........)....
-00000b90: 0602 02fe 0603 02fd 0204 02fc 0605 02fb  ................
-00000ba0: 0606 02fa 0607 02f9 0608 02f8 0209 0ef7  ................
+000000a0: 5a13 0100 6400 6409 6c11 6d14 5a14 0100  Z...d.d.l.m.Z...
+000000b0: 640a 6515 640b 6516 6604 640c 640d 8404  d.e.d.e.f.d.d...
+000000c0: 5a17 640e 6504 6a18 6a19 640f 651a 6410  Z.d.e.j.j.d.e.d.
+000000d0: 6504 6a18 6a19 6411 651b 6412 6515 6413  e.j.j.d.e.d.e.d.
+000000e0: 6515 6414 6515 6415 651a 640a 6515 640b  e.d.e.d.e.d.e.d.
+000000f0: 651c 6614 6416 6417 8404 5a1d 640e 6516  e.f.d.d...Z.d.e.
+00000100: 6414 6504 6a18 6a19 6410 6504 6a18 6a19  d.e.j.j.d.e.j.j.
+00000110: 6411 651b 6412 6504 6a18 6a19 640f 651a  d.e.d.e.j.j.d.e.
+00000120: 6516 1900 6415 651a 6516 1900 6413 6504  e...d.e.e...d.e.
+00000130: 6a18 6a19 640b 6516 6612 6418 6419 8404  j.j.d.e.f.d.d...
+00000140: 5a1e 6401 5300 291a e900 0000 004e 2901  Z.d.S.)......N).
+00000150: da0b 6465 6661 756c 7464 6963 7429 01da  ..defaultdict)..
+00000160: 0b61 6374 696f 6e5f 6172 6773 2901 da0c  .action_args)...
+00000170: 6163 7469 6f6e 5f63 6f64 6573 2901 da0b  action_codes)...
+00000180: 666f 726d 6174 5f68 746d 6c29 01da 066c  format_html)...l
+00000190: 6f67 6765 7229 01da 1d67 6574 5f78 6d6c  ogger)...get_xml
+000001a0: 5f69 6e74 5f61 7267 756d 656e 745f 746f  _int_argument_to
+000001b0: 5f76 616c 7565 2901 da1d 6765 745f 786d  _value)...get_xm
+000001c0: 6c5f 7374 725f 6172 6775 6d65 6e74 5f74  l_str_argument_t
+000001d0: 6f5f 7661 6c75 6529 01da 1072 656d 6f76  o_value)...remov
+000001e0: 655f 6874 6d6c 5f74 6167 73da 1165 7661  e_html_tags..eva
+000001f0: 6c75 6174 6564 5f72 6573 756c 7473 da06  luated_results..
+00000200: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+00000210: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
+00000220: 5601 0000 6401 7d01 7c00 6402 1900 4400  V...d.}.|.d...D.
+00000230: 5da2 7d02 6401 7d03 7c02 0400 6403 6b02  ].}.d.}.|...d.k.
+00000240: 7222 0100 7c00 6404 1900 7221 7c00 6404  r"..|.d...r!|.d.
+00000250: 1900 6405 1900 7d03 7c00 6404 1900 a000  ..d...}.|.d.....
+00000260: 6405 a101 0100 6e7f 0400 6406 6b02 7239  d.....n...d.k.r9
+00000270: 0100 7c00 6407 1900 7238 7c00 6407 1900  ..|.d...r8|.d...
+00000280: 6405 1900 7d03 7c00 6407 1900 a000 6405  d...}.|.d.....d.
+00000290: a101 0100 6e68 0400 6408 6b02 7250 0100  ....nh..d.k.rP..
+000002a0: 7c00 6409 1900 724f 7c00 6409 1900 6405  |.d...rO|.d...d.
+000002b0: 1900 7d03 7c00 6409 1900 a000 6405 a101  ..}.|.d.....d...
+000002c0: 0100 6e51 0400 640a 6b02 7267 0100 7c00  ..nQ..d.k.rg..|.
+000002d0: 640b 1900 7266 7c00 640b 1900 6405 1900  d...rf|.d...d...
+000002e0: 7d03 7c00 640b 1900 a000 6405 a101 0100  }.|.d.....d.....
+000002f0: 6e3a 0400 640c 6b02 727e 0100 7c00 640d  n:..d.k.r~..|.d.
+00000300: 1900 727d 7c00 640d 1900 6405 1900 7d03  ..r}|.d...d...}.
+00000310: 7c00 640d 1900 a000 6405 a101 0100 6e23  |.d.....d.....n#
+00000320: 640e 6b02 7293 7c00 640f 1900 7292 7c00  d.k.r.|.d...r.|.
+00000330: 640f 1900 6405 1900 7d03 7c00 640f 1900  d...d...}.|.d...
+00000340: a000 6405 a101 0100 6e0e 0900 7401 a002  ..d.....n...t...
+00000350: 6410 7c02 9b00 9d02 a101 0100 7403 a004  d.|.........t...
+00000360: 6411 a101 0100 7c01 9b00 6412 7c03 9b00  d.....|...d.|...
+00000370: 9d03 7d01 7106 7c01 5300 2913 4eda 005a  ..}.q.|.S.).N..Z
+00000380: 1170 6f73 6974 696f 6e5f 6172 675f 7479  .position_arg_ty
+00000390: 7065 da03 5374 72da 0a72 6573 756c 745f  pe..Str..result_
+000003a0: 7374 7272 0100 0000 5a03 496e 74da 0a72  strr....Z.Int..r
+000003b0: 6573 756c 745f 696e 745a 0341 7070 5a0a  esult_intZ.AppZ.
+000003c0: 7265 7375 6c74 5f61 7070 5a0d 436f 6e64  result_appZ.Cond
+000003d0: 6974 696f 6e4c 6973 745a 0a72 6573 756c  itionListZ.resul
+000003e0: 745f 636f 6e5a 0349 6d67 5a0a 7265 7375  t_conZ.ImgZ.resu
+000003f0: 6c74 5f69 6d67 5a06 4275 6e64 6c65 5a0a  lt_imgZ.BundleZ.
+00000400: 7265 7375 6c74 5f62 756e 7a36 4675 6e63  result_bunz6Func
+00000410: 7469 6f6e 2067 6574 5f72 6573 756c 7473  tion get_results
+00000420: 5f69 6e5f 6172 675f 6f72 6465 723a 206e  _in_arg_order: n
+00000430: 6f20 6d61 7463 6820 666f 7220 2261 7267  o match for "arg
+00000440: 223a e908 0000 00da 0120 2905 da03 706f  ":....... )...po
+00000450: 7072 0600 0000 da05 6465 6275 67da 0373  pr......debug..s
+00000460: 7973 da04 6578 6974 2904 720a 0000 005a  ys..exit).r....Z
+00000470: 0d72 6574 7572 6e5f 7265 7375 6c74 da03  .return_result..
+00000480: 6172 675a 0874 6865 5f69 7465 6da9 0072  argZ.the_item..r
+00000490: 1700 0000 fa76 2f55 7365 7273 2f6d 696b  .....v/Users/mik
+000004a0: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
+000004b0: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
+000004c0: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
+000004d0: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
+000004e0: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
+000004f0: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
+00000500: 632f 6163 7469 6f6e 722e 7079 da18 6765  c/actionr.py..ge
+00000510: 745f 7265 7375 6c74 735f 696e 5f61 7267  t_results_in_arg
+00000520: 5f6f 7264 6572 1f00 0000 7356 0000 0004  _order....sV....
+00000530: 010c 0104 0102 010a 0108 010c 0108 0102  ................
+00000540: 0104 ff02 800a 0308 010c 010e 0102 800a  ................
+00000550: 0108 010c 010e 0102 800a 0108 010c 010e  ................
+00000560: 0102 800a 0108 010c 010e 0102 8006 0108  ................
+00000570: 010c 010e 0102 8002 0104 0108 0104 ff0a  ................
+00000580: 0310 0104 0172 1900 0000 da09 6469 6374  .....r......dict
+00000590: 5f63 6f64 65da 0861 7267 5f6c 6973 74da  _code..arg_list.
+000005a0: 0b63 6f64 655f 6163 7469 6f6e da0b 6163  .code_action..ac
+000005b0: 7469 6f6e 5f74 7970 65da 0863 6f6c 6f72  tion_type..color
+000005c0: 6d61 70da 0c70 726f 6772 616d 5f61 7267  map..program_arg
+000005d0: 73da 116c 6f6f 6b75 705f 636f 6465 5f65  s..lookup_code_e
+000005e0: 6e74 7279 da0d 6576 616c 7561 7465 5f6c  ntry..evaluate_l
+000005f0: 6973 7463 0900 0000 0000 0000 0000 0000  istc............
+00000600: 0900 0000 0a00 0000 4300 0000 7364 0000  ........C...sd..
+00000610: 0074 007c 017c 007c 067c 077c 027c 037c  .t.|.|.|.|.|.|.|
+00000620: 047c 057c 0883 097d 087c 0864 0119 0072  .|.|...}.|.d...r
+00000630: 307c 0864 0219 0072 2074 017c 027c 0864  0|.d...r t.|.|.d
+00000640: 0219 007c 0864 0319 0083 037c 0864 043c  ...|.d.....|.d.<
+00000650: 007c 0864 0519 0072 3074 027c 027c 0864  .|.d...r0t.|.|.d
+00000660: 0519 007c 0864 0619 0083 037c 0864 073c  ...|.d.....|.d.<
+00000670: 007c 0853 0029 084e 5a0c 6765 745f 786d  .|.S.).NZ.get_xm
+00000680: 6c5f 666c 6167 5a07 7374 7261 7267 735a  l_flagZ.strargsZ
+00000690: 0773 7472 6576 616c 720e 0000 005a 0769  .strevalr....Z.i
+000006a0: 6e74 6172 6773 5a07 696e 7465 7661 6c72  ntargsZ.intevalr
+000006b0: 0f00 0000 2903 7203 0000 0072 0800 0000  ....).r....r....
+000006c0: 7207 0000 0029 0972 1a00 0000 721b 0000  r....).r....r...
+000006d0: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+000006e0: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+000006f0: 0a00 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+00000700: 0000 00da 1465 7661 6c75 6174 655f 6163  .....evaluate_ac
+00000710: 7469 6f6e 5f61 7267 734b 0000 0073 2a00  tion_argsK...s*.
+00000720: 0000 020c 0201 0201 0201 0201 0201 0201  ................
+00000730: 0201 0201 0201 04f7 080c 0801 0201 0e01  ................
+00000740: 08ff 0803 0201 0e01 08ff 0404 7222 0000  ............r"..
+00000750: 0063 0800 0000 0000 0000 0000 0000 0b00  .c..............
+00000760: 0000 0e00 0000 4300 0000 73be 0000 0074  ......C...s....t
+00000770: 0064 0164 0284 0083 017d 0864 037d 0964  .d.d.....}.d.}.d
+00000780: 047d 0a7c 057c 017c 0019 0064 053c 007c  .}.|.|.|...d.<.|
+00000790: 067c 017c 0019 0064 063c 007c 0572 2a7c  .|.|...d.<.|.r*|
+000007a0: 0764 0719 0064 086b 0372 2a74 017c 007c  .d...d.k.r*t.|.|
+000007b0: 057c 027c 037c 047c 077c 017c 067c 0883  .|.|.|.|.|.|.|..
+000007c0: 097d 087c 0864 0919 0072 3274 027c 0883  .}.|.d...r2t.|..
+000007d0: 017d 0a7c 0aa0 0364 0a64 0ba1 027d 0a7c  .}.|...d.d...}.|
+000007e0: 0aa0 0364 0c64 0da1 027d 0a74 047c 0464  ...d.d...}.t.|.d
+000007f0: 0e64 0474 057c 0019 0064 0f19 0064 1083  .d.t.|...d...d..
+00000800: 0574 047c 0464 1164 047c 099b 007c 0a9b  .t.|.d.d.|...|..
+00000810: 0064 1274 06a0 077c 027c 037c 047c 07a1  .d.t...|.|.|.|..
+00000820: 049b 009d 0464 1383 0517 0053 0029 144e  .....d.....S.).N
+00000830: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000840: 0001 0000 0053 0000 0073 0400 0000 6700  .....S...s....g.
+00000850: 5300 2901 4e72 1700 0000 7217 0000 0072  S.).Nr....r....r
+00000860: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
+00000870: 3c6c 616d 6264 613e 7f00 0000 7302 0000  <lambda>....s...
+00000880: 0004 007a 2467 6574 5f61 6374 696f 6e5f  ...z$get_action_
+00000890: 7265 7375 6c74 732e 3c6c 6f63 616c 733e  results.<locals>
+000008a0: 2e3c 6c61 6d62 6461 3e7a 0c26 6e62 7370  .<lambda>z.&nbsp
+000008b0: 3b26 6e62 7370 3b72 0c00 0000 da07 7265  ;&nbsp;r......re
+000008c0: 7161 7267 73da 0865 7661 6c61 7267 735a  qargs..evalargsZ
+000008d0: 1464 6973 706c 6179 5f64 6574 6169 6c5f  .display_detail_
+000008e0: 6c65 7665 6ce9 0200 0000 5a13 7265 7475  level.....Z.retu
+000008f0: 726e 696e 675f 736f 6d65 7468 696e 67fa  rning_something.
+00000900: 013c 7a04 266c 743b fa01 3e7a 0426 6774  .<z.&lt;..>z.&gt
+00000910: 3bda 1161 6374 696f 6e5f 6e61 6d65 5f63  ;..action_name_c
+00000920: 6f6c 6f72 da07 6469 7370 6c61 7954 5a0c  olor..displayTZ.
+00000930: 6163 7469 6f6e 5f63 6f6c 6f72 7a07 3c2f  action_colorz.</
+00000940: 7370 616e 3e46 2908 7202 0000 0072 2200  span>F).r....r".
+00000950: 0000 7219 0000 00da 0772 6570 6c61 6365  ..r......replace
+00000960: 7205 0000 0072 0400 0000 da0a 6765 745f  r....r......get_
+00000970: 6163 7469 6f6e da0f 6765 745f 6578 7472  action..get_extr
+00000980: 615f 7374 7566 6629 0b72 1a00 0000 7220  a_stuff).r....r 
+00000990: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+000009a0: 0000 721b 0000 0072 2100 0000 721f 0000  ..r....r!...r...
+000009b0: 0072 0a00 0000 5a0a 7477 6f5f 626c 616e  .r....Z.two_blan
+000009c0: 6b73 da06 7265 7375 6c74 7217 0000 0072  ks..resultr....r
+000009d0: 1700 0000 7218 0000 00da 1267 6574 5f61  ....r......get_a
+000009e0: 6374 696f 6e5f 7265 7375 6c74 7374 0000  ction_resultst..
+000009f0: 0073 4800 0000 020a 0601 04ff 0403 0401  .sH.............
+00000a00: 0c03 0c01 1002 0202 0201 0201 0201 0201  ................
+00000a10: 0201 0201 0201 0201 0201 04f7 080d 0801  ................
+00000a20: 0c03 0c01 0203 1201 02ff 0202 0201 0201  ................
+00000a30: 0201 0a02 0e01 04ff 0203 02f8 04fe 722f  ..............r/
+00000a40: 0000 0029 1f72 1400 0000 da0b 636f 6c6c  ...).r......coll
+00000a50: 6563 7469 6f6e 7372 0200 0000 da16 6465  ectionsr......de
+00000a60: 6675 7365 6478 6d6c 2e45 6c65 6d65 6e74  fusedxml.Element
+00000a70: 5472 6565 da0a 6465 6675 7365 6478 6d6c  Tree..defusedxml
+00000a80: da14 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
+00000a90: 6163 7469 6f6e da03 7372 63da 0661 6374  action..src..act
+00000aa0: 696f 6e72 2c00 0000 5a15 6d61 7074 6173  ionr,...Z.maptas
+00000ab0: 6b65 722e 7372 632e 6163 7461 7267 7372  ker.src.actargsr
+00000ac0: 0300 0000 da15 6d61 7074 6173 6b65 722e  ......maptasker.
+00000ad0: 7372 632e 6163 7469 6f6e 6372 0400 0000  src.actioncr....
+00000ae0: da16 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
+00000af0: 6672 6d74 6874 6d6c 7205 0000 00da 166d  frmthtmlr......m
+00000b00: 6170 7461 736b 6572 2e73 7263 2e73 7973  aptasker.src.sys
+00000b10: 636f 6e73 7472 0600 0000 5a15 6d61 7074  constr....Z.mapt
+00000b20: 6173 6b65 722e 7372 632e 786d 6c64 6174  asker.src.xmldat
+00000b30: 6172 0700 0000 7208 0000 0072 0900 0000  ar....r....r....
+00000b40: da04 6469 6374 da03 7374 7272 1900 0000  ..dict..strr....
+00000b50: da0b 456c 656d 656e 7454 7265 65da 0358  ..ElementTree..X
+00000b60: 4d4c da04 6c69 7374 da04 626f 6f6c da05  ML..list..bool..
+00000b70: 7475 706c 6572 2200 0000 722f 0000 0072  tupler"...r/...r
+00000b80: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+00000b90: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000ba0: 0073 6800 0000 080c 0c01 0802 1202 0c01  .sh.............
+00000bb0: 0c01 0c01 0c01 0c01 0c01 0c01 1206 022c  ...............,
+00000bc0: 0601 02ff 0202 02fe 0603 02fd 0204 02fc  ................
+00000bd0: 0205 02fb 0206 02fa 0207 02f9 0208 02f8  ................
+00000be0: 0209 02f7 020a 0af6 0229 0201 02ff 0602  .........)......
+00000bf0: 02fe 0603 02fd 0204 02fc 0605 02fb 0606  ................
+00000c00: 02fa 0607 02f9 0608 02f8 0209 0ef7       ..............
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/actiont.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/actiont.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/argsdict.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/argsdict.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/caveats.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/caveats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/colors.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/colors.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 23 17:42:41 2023 UTC, .py size: 8220 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,275 +1,252 @@
-00000000: 6f0d 0d0a 0000 0000 918f 1c64 1c20 0000  o..........d. ..
+00000000: 6f0d 0d0a 0000 0000 89e2 4264 fa1e 0000  o.........Bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
+00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c01 6d03 5a03 0100 6404  ..d.d.l.m.Z...d.
-00000050: 6405 8400 5a04 6406 6407 8400 5a05 6408  d...Z.d.d...Z.d.
-00000060: 6409 8400 5a06 640a 6507 640b 6507 640c  d...Z.d.e.d.e.d.
-00000070: 6508 640d 6401 6608 640e 640f 8404 5a09  e.d.d.f.d.d...Z.
-00000080: 6401 5300 2910 e900 0000 004e 2901 da14  d.S.)......N)...
-00000090: 5459 5045 535f 4f46 5f43 4f4c 4f52 5f4e  TYPES_OF_COLOR_N
-000000a0: 414d 4553 2901 da06 6c6f 6767 6572 6302  AMES)...loggerc.
-000000b0: 0000 0000 0000 0000 0000 0006 0000 0004  ................
-000000c0: 0000 0043 0000 0073 5400 0000 6401 7d02  ...C...sT...d.}.
-000000d0: 6402 7d03 7400 7c01 8301 6403 1800 7d04  d.}.t.|...d...}.
-000000e0: 7c00 7210 7401 7c00 8301 0100 7c01 4400  |.r.t.|.....|.D.
-000000f0: 5d11 7d05 7c01 a002 7c05 a101 7c04 6b02  ].}.|...|...|.k.
-00000100: 721d 6401 7d03 7c02 7c05 1700 7c03 1700  r.d.}.|.|...|...
-00000110: 7d02 7112 7401 7c02 8301 0100 6400 5300  }.q.t.|.....d.S.
-00000120: 2904 4eda 007a 022c 20e9 0100 0000 2903  ).N..z., .....).
-00000130: da03 6c65 6eda 0570 7269 6e74 da05 696e  ..len..print..in
-00000140: 6465 7829 065a 0a6c 6973 745f 7469 746c  dex).Z.list_titl
-00000150: 65da 0874 6865 5f6c 6973 745a 086c 696e  e..the_listZ.lin
-00000160: 655f 6f75 745a 0973 6570 6572 6174 6f72  e_outZ.seperator
-00000170: 5a0b 6c69 7374 5f6c 656e 6774 68da 0469  Z.list_length..i
-00000180: 7465 6da9 0072 0b00 0000 fa75 2f55 7365  tem..r.....u/Use
-00000190: 7273 2f6d 696b 7275 6269 6e2f 4c69 6272  rs/mikrubin/Libr
-000001a0: 6172 792f 436c 6f75 6453 746f 7261 6765  ary/CloudStorage
-000001b0: 2f47 6f6f 676c 6544 7269 7665 2d6d 696b  /GoogleDrive-mik
-000001c0: 7275 6269 6e40 676d 6169 6c2e 636f 6d2f  rubin@gmail.com/
-000001d0: 4d79 2044 7269 7665 2f50 7974 686f 6e2f  My Drive/Python/
-000001e0: 6d61 7074 6173 6b65 722f 6d61 7074 6173  maptasker/maptas
-000001f0: 6b65 722f 7372 632f 636f 6c6f 7273 2e70  ker/src/colors.p
-00000200: 79da 0a70 7269 6e74 5f6c 6973 7416 0000  y..print_list...
-00000210: 0073 1600 0000 0401 0401 0c01 0401 0801  .s..............
-00000220: 0801 0e01 0401 0e01 0801 0401 720d 0000  ............r...
-00000230: 0063 0100 0000 0000 0000 0000 0000 0d00  .c..............
-00000240: 0000 0400 0000 4300 0000 7330 0100 0067  ......C...s0...g
-00000250: 0064 01a2 017d 0167 0064 02a2 017d 0267  .d...}.g.d...}.g
-00000260: 0064 03a2 017d 0367 0064 04a2 017d 0467  .d...}.g.d...}.g
-00000270: 0064 05a2 017d 0567 0064 06a2 017d 0667  .d...}.g.d...}.g
-00000280: 0064 07a2 017d 0767 0064 08a2 017d 0867  .d...}.g.d...}.g
-00000290: 0064 09a2 017d 0967 0064 0aa2 017d 0a64  .d...}.g.d...}.d
-000002a0: 0b67 017d 0b7c 017c 0217 007c 0317 007c  .g.}.|.|...|...|
-000002b0: 0417 007c 0517 007c 0617 007c 0717 007c  ...|...|...|...|
-000002c0: 0817 007c 0917 007c 0a17 007c 0b17 007d  ...|...|...|...}
-000002d0: 0c7c 0064 0c6b 0372 5b74 00a0 017c 007c  .|.d.k.r[t...|.|
-000002e0: 0c76 00a1 0101 0074 0264 0d64 0e84 007c  .v.....t.d.d...|
-000002f0: 0044 0083 0183 0172 5764 0f53 007c 007c  .D.....rWd.S.|.|
-00000300: 0c76 0053 0074 0364 107c 0183 0201 0074  .v.S.t.d.|.....t
-00000310: 0364 117c 0283 0201 0074 0364 127c 0383  .d.|.....t.d.|..
-00000320: 0201 0074 0364 137c 0483 0201 0074 0364  ...t.d.|.....t.d
-00000330: 147c 0583 0201 0074 0364 157c 0683 0201  .|.....t.d.|....
-00000340: 0074 0364 167c 0783 0201 0074 0364 177c  .t.d.|.....t.d.|
-00000350: 0883 0201 0074 0364 187c 0983 0201 0074  .....t.d.|.....t
-00000360: 0364 197c 0a83 0201 0074 0364 1a7c 0b83  .d.|.....t.d.|..
-00000370: 0201 0074 0464 1b83 0101 0064 0053 0029  ...t.d.....d.S.)
-00000380: 1c4e 2909 5a09 496e 6469 616e 5265 645a  .N).Z.IndianRedZ
-00000390: 0a4c 6967 6874 436f 7261 6c5a 0653 616c  .LightCoralZ.Sal
-000003a0: 6d6f 6e5a 0a44 6172 6b53 616c 6d6f 6eda  monZ.DarkSalmon.
-000003b0: 0b4c 6967 6874 5361 6c6d 6f6e 5a07 4372  .LightSalmonZ.Cr
-000003c0: 696d 736f 6e5a 0352 6564 5a09 4669 7265  imsonZ.RedZ.Fire
-000003d0: 4272 6963 6b5a 0744 6172 6b52 6564 2906  BrickZ.DarkRed).
-000003e0: 5a04 5069 6e6b 5a09 4c69 6768 7450 696e  Z.PinkZ.LightPin
-000003f0: 6b5a 0748 6f74 5069 6e6b 5a08 4465 6570  kZ.HotPinkZ.Deep
-00000400: 5069 6e6b 5a0f 4d65 6469 756d 5669 6f6c  PinkZ.MediumViol
-00000410: 6574 5265 645a 0d50 616c 6556 696f 6c65  etRedZ.PaleViole
-00000420: 7452 6564 2906 720e 0000 005a 0543 6f72  tRed).r....Z.Cor
-00000430: 616c 5a06 546f 6d61 746f 5a09 4f72 616e  alZ.TomatoZ.Oran
-00000440: 6765 5265 645a 0a44 6172 6b4f 7261 6e67  geRedZ.DarkOrang
-00000450: 655a 064f 7261 6e67 6529 0b5a 0447 6f6c  eZ.Orange).Z.Gol
-00000460: 645a 0659 656c 6c6f 775a 0b4c 6967 6874  dZ.YellowZ.Light
-00000470: 5965 6c6c 6f77 5a0c 4c65 6d6f 6e43 6869  YellowZ.LemonChi
-00000480: 6666 6f6e 5a14 4c69 6768 7447 6f6c 6465  ffonZ.LightGolde
-00000490: 6e72 6f64 5965 6c6c 6f77 5a0a 5061 7061  nrodYellowZ.Papa
-000004a0: 7961 5768 6970 5a08 4d6f 6363 6173 696e  yaWhipZ.Moccasin
-000004b0: 5a09 5065 6163 6850 7566 665a 0d50 616c  Z.PeachPuffZ.Pal
-000004c0: 6547 6f6c 6465 6e72 6f64 5a05 4b68 616b  eGoldenrodZ.Khak
-000004d0: 695a 0944 6172 6b4b 6861 6b69 2913 5a08  iZ.DarkKhaki).Z.
-000004e0: 4c61 7665 6e64 6572 5a07 5468 6973 746c  LavenderZ.Thistl
-000004f0: 655a 0450 6c75 6d5a 0656 696f 6c65 745a  eZ.PlumZ.VioletZ
-00000500: 064f 7263 6869 645a 0746 7563 6873 6961  .OrchidZ.Fuchsia
-00000510: 5a07 4d61 6765 6e74 615a 0c4d 6564 6975  Z.MagentaZ.Mediu
-00000520: 6d4f 7263 6869 645a 0c4d 6564 6975 6d50  mOrchidZ.MediumP
-00000530: 7572 706c 655a 0d52 6562 6563 6361 5075  urpleZ.RebeccaPu
-00000540: 7270 6c65 5a0a 426c 7565 5669 6f6c 6574  rpleZ.BlueViolet
-00000550: 5a0a 4461 726b 5669 6f6c 6574 5a0a 4461  Z.DarkVioletZ.Da
-00000560: 726b 4f72 6368 6964 5a0b 4461 726b 4d61  rkOrchidZ.DarkMa
-00000570: 6765 6e74 615a 0650 7572 706c 655a 0649  gentaZ.PurpleZ.I
-00000580: 6e64 6967 6f5a 0953 6c61 7465 426c 7565  ndigoZ.SlateBlue
-00000590: 5a0d 4461 726b 536c 6174 6542 6c75 65da  Z.DarkSlateBlue.
-000005a0: 0f4d 6564 6975 6d53 6c61 7465 426c 7565  .MediumSlateBlue
-000005b0: 2917 5a0b 4772 6565 6e59 656c 6c6f 775a  ).Z.GreenYellowZ
-000005c0: 0a43 6861 7274 7265 7573 655a 094c 6177  .ChartreuseZ.Law
-000005d0: 6e47 7265 656e 5a04 4c69 6d65 5a09 4c69  nGreenZ.LimeZ.Li
-000005e0: 6d65 4772 6565 6e5a 0950 616c 6547 7265  meGreenZ.PaleGre
-000005f0: 656e 5a0a 4c69 6768 7447 7265 656e 5a11  enZ.LightGreenZ.
-00000600: 4d65 6469 756d 5370 7269 6e67 4772 6565  MediumSpringGree
-00000610: 6e5a 0b53 7072 696e 6747 7265 656e 5a0e  nZ.SpringGreenZ.
-00000620: 4d65 6469 756d 5365 6147 7265 656e 5a08  MediumSeaGreenZ.
-00000630: 5365 6147 7265 656e 5a0b 466f 7265 7374  SeaGreenZ.Forest
-00000640: 4772 6565 6e5a 0547 7265 656e 5a09 4461  GreenZ.GreenZ.Da
-00000650: 726b 4772 6565 6e5a 0b59 656c 6c6f 7747  rkGreenZ.YellowG
-00000660: 7265 656e 5a09 4f6c 6976 6544 7261 625a  reenZ.OliveDrabZ
-00000670: 054f 6c69 7665 5a0e 4461 726b 4f6c 6976  .OliveZ.DarkOliv
-00000680: 6547 7265 656e 5a10 4d65 6469 756d 4171  eGreenZ.MediumAq
-00000690: 7561 6d61 7269 6e65 5a0c 4461 726b 5365  uamarineZ.DarkSe
-000006a0: 6147 7265 656e 5a0d 4c69 6768 7453 6561  aGreenZ.LightSea
-000006b0: 4772 6565 6e5a 0844 6172 6b43 7961 6e5a  GreenZ.DarkCyanZ
-000006c0: 0454 6561 6c29 195a 0441 7175 615a 0443  .Teal).Z.AquaZ.C
-000006d0: 7961 6e5a 094c 6967 6874 4379 616e 5a0d  yanZ.LightCyanZ.
-000006e0: 5061 6c65 5475 7271 756f 6973 655a 0a41  PaleTurquoiseZ.A
-000006f0: 7175 616d 6172 696e 655a 0954 7572 7175  quamarineZ.Turqu
-00000700: 6f69 7365 5a0f 4d65 6469 756d 5475 7271  oiseZ.MediumTurq
-00000710: 756f 6973 655a 0d44 6172 6b54 7572 7175  uoiseZ.DarkTurqu
-00000720: 6f69 7365 5a09 4361 6465 7442 6c75 655a  oiseZ.CadetBlueZ
-00000730: 0953 7465 656c 426c 7565 5a0e 4c69 6768  .SteelBlueZ.Ligh
-00000740: 7453 7465 656c 426c 7565 5a0a 506f 7764  tSteelBlueZ.Powd
-00000750: 6572 426c 7565 5a09 4c69 6768 7442 6c75  erBlueZ.LightBlu
-00000760: 655a 0753 6b79 426c 7565 5a0c 4c69 6768  eZ.SkyBlueZ.Ligh
-00000770: 7453 6b79 426c 7565 5a0b 4465 6570 536b  tSkyBlueZ.DeepSk
-00000780: 7942 6c75 655a 0a44 6f64 6765 7242 6c75  yBlueZ.DodgerBlu
-00000790: 655a 0e43 6f72 6e66 6c6f 7765 7242 6c75  eZ.CornflowerBlu
-000007a0: 6572 0f00 0000 5a09 526f 7961 6c42 6c75  er....Z.RoyalBlu
-000007b0: 655a 0442 6c75 655a 0a4d 6564 6975 6d42  eZ.BlueZ.MediumB
-000007c0: 6c75 655a 0844 6172 6b42 6c75 655a 044e  lueZ.DarkBlueZ.N
-000007d0: 6176 795a 0c4d 6964 6e69 6768 7442 6c75  avyZ.MidnightBlu
-000007e0: 6529 115a 0843 6f72 6e73 696c 6b5a 0e42  e).Z.CornsilkZ.B
-000007f0: 6c61 6e63 6865 6441 6c6d 6f6e 645a 0642  lanchedAlmondZ.B
-00000800: 6973 7175 655a 0b4e 6176 616a 6f57 6869  isqueZ.NavajoWhi
-00000810: 7465 5a05 5768 6561 745a 0942 7572 6c79  teZ.WheatZ.Burly
-00000820: 576f 6f64 5a03 5461 6e5a 0952 6f73 7942  WoodZ.TanZ.RosyB
-00000830: 726f 776e 5a0a 5361 6e64 7942 726f 776e  rownZ.SandyBrown
-00000840: 5a09 476f 6c64 656e 726f 645a 0d44 6172  Z.GoldenrodZ.Dar
-00000850: 6b47 6f6c 6465 6e72 6f64 5a04 5065 7275  kGoldenrodZ.Peru
-00000860: 5a09 4368 6f63 6f6c 6174 655a 0b53 6164  Z.ChocolateZ.Sad
-00000870: 646c 6542 726f 776e 5a06 5369 656e 6e61  dleBrownZ.Sienna
-00000880: 5a05 4272 6f77 6e5a 064d 6172 6f6f 6e29  Z.BrownZ.Maroon)
-00000890: 115a 0557 6869 7465 5a04 536e 6f77 5a08  .Z.WhiteZ.SnowZ.
-000008a0: 486f 6e65 7944 6577 5a09 4d69 6e74 4372  HoneyDewZ.MintCr
-000008b0: 6561 6d5a 0541 7a75 7265 5a09 416c 6963  eamZ.AzureZ.Alic
-000008c0: 6542 6c75 655a 0a47 686f 7374 5768 6974  eBlueZ.GhostWhit
-000008d0: 655a 0a57 6869 7465 536d 6f6b 655a 0853  eZ.WhiteSmokeZ.S
-000008e0: 6561 5368 656c 6c5a 0542 6569 6765 5a07  eaShellZ.BeigeZ.
-000008f0: 4f6c 644c 6163 655a 0b46 6c6f 7261 6c57  OldLaceZ.FloralW
-00000900: 6869 7465 5a05 4976 6f72 795a 0c41 6e74  hiteZ.IvoryZ.Ant
-00000910: 6971 7565 5768 6974 655a 054c 696e 656e  iqueWhiteZ.Linen
-00000920: 5a0d 4c61 7665 6e64 6572 426c 7573 685a  Z.LavenderBlushZ
-00000930: 094d 6973 7479 526f 7365 290a 5a09 4761  .MistyRose).Z.Ga
-00000940: 696e 7362 6f72 6f5a 094c 6967 6874 4772  insboroZ.LightGr
-00000950: 6179 5a06 5369 6c76 6572 5a08 4461 726b  ayZ.SilverZ.Dark
-00000960: 4772 6179 5a04 4772 6179 5a07 4469 6d47  GrayZ.GrayZ.DimG
-00000970: 7261 795a 0e4c 6967 6874 536c 6174 6547  rayZ.LightSlateG
-00000980: 7261 795a 0953 6c61 7465 4772 6179 5a0d  rayZ.SlateGrayZ.
-00000990: 4461 726b 536c 6174 6547 7261 795a 0542  DarkSlateGrayZ.B
-000009a0: 6c61 636b 7a1c 6865 7820 7661 6c75 652e  lackz.hex value.
-000009b0: 2020 4578 616d 706c 6520 2764 6232 3966    Example 'db29f
-000009c0: 6627 da01 6863 0100 0000 0000 0000 0000  f'..hc..........
-000009d0: 0000 0200 0000 0300 0000 7300 0000 731a  ..........s...s.
-000009e0: 0000 0081 007c 005d 087d 017c 0174 006a  .....|.].}.|.t.j
-000009f0: 0176 0056 0001 0071 0264 0053 0029 014e  .v.V...q.d.S.).N
-00000a00: 2902 da06 7374 7269 6e67 da09 6865 7864  )...string..hexd
-00000a10: 6967 6974 7329 02da 022e 30da 0163 720b  igits)....0..cr.
-00000a20: 0000 0072 0b00 0000 720c 0000 00da 093c  ...r....r......<
-00000a30: 6765 6e65 7870 723e de00 0000 7304 0000  genexpr>....s...
-00000a40: 0002 8018 007a 2176 616c 6964 6174 655f  .....z!validate_
-00000a50: 636f 6c6f 722e 3c6c 6f63 616c 733e 2e3c  color.<locals>.<
-00000a60: 6765 6e65 7870 723e 547a 110a 5265 6420  genexpr>Tz..Red 
-00000a70: 636f 6c6f 7220 6e61 6d65 733a 7a12 0a50  color names:z..P
-00000a80: 696e 6b20 636f 6c6f 7220 6e61 6d65 733a  ink color names:
-00000a90: 7a14 0a4f 7261 6e67 6520 636f 6c6f 7220  z..Orange color 
-00000aa0: 6e61 6d65 733a 7a14 0a59 656c 6c6f 7720  names:z..Yellow 
-00000ab0: 636f 6c6f 7220 6e61 6d65 733a 7a14 0a50  color names:z..P
-00000ac0: 7572 706c 6520 636f 6c6f 7220 6e61 6d65  urple color name
-00000ad0: 733a 7a13 0a47 7265 656e 2063 6f6c 6f72  s:z..Green color
-00000ae0: 206e 616d 6573 3a7a 120a 426c 7565 2063   names:z..Blue c
-00000af0: 6f6c 6f72 206e 616d 6573 3a7a 130a 4272  olor names:z..Br
-00000b00: 6f77 6e20 636f 6c6f 7220 6e61 6d65 733a  own color names:
-00000b10: 7a13 0a57 6869 7465 2063 6f6c 6f72 206e  z..White color n
-00000b20: 616d 6573 3a7a 120a 4772 6179 2063 6f6c  ames:z..Gray col
-00000b30: 6f72 206e 616d 6573 3a7a 0b0a 416e 7920  or names:z..Any 
-00000b40: 636f 6c6f 723a 7201 0000 0029 0572 0300  color:r....).r..
-00000b50: 0000 da05 6465 6275 67da 0361 6c6c 720d  ....debug..allr.
-00000b60: 0000 00da 0465 7869 7429 0d5a 0974 6865  .....exit).Z.the
-00000b70: 5f63 6f6c 6f72 5a0f 7265 645f 636f 6c6f  _colorZ.red_colo
-00000b80: 725f 6e61 6d65 735a 1070 696e 6b5f 636f  r_namesZ.pink_co
-00000b90: 6c6f 725f 6e61 6d65 735a 126f 7261 6e67  lor_namesZ.orang
-00000ba0: 655f 636f 6c6f 725f 6e61 6d65 735a 1279  e_color_namesZ.y
-00000bb0: 656c 6c6f 775f 636f 6c6f 725f 6e61 6d65  ellow_color_name
-00000bc0: 735a 1270 7572 706c 655f 636f 6c6f 725f  sZ.purple_color_
-00000bd0: 6e61 6d65 735a 1167 7265 656e 5f63 6f6c  namesZ.green_col
-00000be0: 6f72 5f6e 616d 6573 5a10 626c 7565 5f63  or_namesZ.blue_c
-00000bf0: 6f6c 6f72 5f6e 616d 6573 5a11 6272 6f77  olor_namesZ.brow
-00000c00: 6e5f 636f 6c6f 725f 6e61 6d65 735a 1177  n_color_namesZ.w
-00000c10: 6869 7465 5f63 6f6c 6f72 5f6e 616d 6573  hite_color_names
-00000c20: 5a10 6772 6179 5f63 6f6c 6f72 5f6e 616d  Z.gray_color_nam
-00000c30: 6573 5a09 616e 795f 636f 6c6f 725a 0a61  esZ.any_colorZ.a
-00000c40: 6c6c 5f63 6f6c 6f72 7372 0b00 0000 720b  ll_colorsr....r.
-00000c50: 0000 0072 0c00 0000 da0e 7661 6c69 6461  ...r......valida
-00000c60: 7465 5f63 6f6c 6f72 2700 0000 7364 0000  te_color'...sd..
-00000c70: 0008 0108 0b08 0808 0808 0d08 1508 1908  ................
-00000c80: 1b08 1308 1306 0c02 0302 0102 ff02 0202  ................
-00000c90: fe02 0302 fd02 0402 fc02 0502 fb02 0602  ................
-00000ca0: fa02 0702 f902 0802 f802 0902 f702 0a02  ................
-00000cb0: f602 ff08 0e0e 0112 0204 0108 020a 010a  ................
-00000cc0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00000cd0: 010a 010c 0172 1900 0000 6302 0000 0000  .....r....c.....
-00000ce0: 0000 0000 0000 0006 0000 0005 0000 0043  ...............C
-00000cf0: 0000 0073 a800 0000 7c00 6401 6400 8502  ...s....|.d.d...
-00000d00: 1900 a000 6402 a101 7d02 7c02 6403 1900  ....d...}.|.d...
-00000d10: 7d03 7401 7c02 8301 6401 6b00 721c 7402  }.t.|...d.k.r.t.
-00000d20: 7c00 9b00 6404 9d02 6405 6406 8303 0100  |...d...d.d.....
-00000d30: 7c03 7403 7601 7229 7402 7c03 9b00 6407  |.t.v.r)t.|...d.
-00000d40: 9d02 6405 6406 8303 0100 7c02 6408 1900  ..d.d.....|.d...
-00000d50: 7d04 7404 a005 6409 7c04 9b00 9d02 a101  }.t...d.|.......
-00000d60: 0100 7406 7c04 8301 7241 7c04 7c01 7403  ..t.|...rA|.|.t.
-00000d70: 7c03 1900 3c00 6400 5300 640a 7c04 9b00  |...<.d.S.d.|...
-00000d80: 640b 7c02 6403 1900 9b00 640c 9d05 7d05  d.|.d.....d...}.
-00000d90: 7402 7c05 640d 6406 8303 0100 6400 5300  t.|.d.d.....d.S.
-00000da0: 290e 4ee9 0200 0000 fa01 3d72 0100 0000  ).N.......=r....
-00000db0: 7a2d 2068 6173 2061 6e20 696e 7661 6c69  z- has an invali
-00000dc0: 6420 2763 6f6c 6f72 272e 2020 5365 6520  d 'color'.  See 
-00000dd0: 7468 6520 6865 6c70 2028 2d63 6829 217a  the help (-ch)!z
-00000de0: 0c20 4578 6974 2063 6f64 6520 37e9 0700  . Exit code 7...
-00000df0: 0000 7a34 2069 7320 616e 2069 6e76 616c  ..z4 is an inval
-00000e00: 6964 2074 7970 6520 666f 7220 2763 6f6c  id type for 'col
-00000e10: 6f72 272e 2020 5365 6520 7468 6520 6865  or'.  See the he
-00000e20: 6c70 2028 2d68 2921 7205 0000 007a 0f20  lp (-h)!r....z. 
-00000e30: 6465 7369 7265 645f 636f 6c6f 723a 7a19  desired_color:z.
-00000e40: 496e 7661 6c69 6420 636f 6c6f 7220 7370  Invalid color sp
-00000e50: 6563 6966 6965 643a 207a 0720 666f 7220  ecified: z. for 
-00000e60: 2763 7a02 2721 7a0c 2065 7869 7420 636f  'cz.'!z. exit co
-00000e70: 6465 2037 2907 da05 7370 6c69 7472 0600  de 7)...splitr..
-00000e80: 0000 da0c 6861 6e64 6c65 5f65 7272 6f72  ....handle_error
-00000e90: 7202 0000 0072 0300 0000 7216 0000 0072  r....r....r....r
-00000ea0: 1900 0000 2906 da07 7468 655f 6172 67da  ....)...the_arg.
-00000eb0: 0863 6f6c 6f72 6d61 705a 1074 6865 5f63  .colormapZ.the_c
-00000ec0: 6f6c 6f72 5f6f 7074 696f 6e5a 0a63 6f6c  olor_optionZ.col
-00000ed0: 6f72 5f74 7970 655a 0d64 6573 6972 6564  or_typeZ.desired
-00000ee0: 5f63 6f6c 6f72 da09 6572 726f 725f 6d73  _color..error_ms
-00000ef0: 6772 0b00 0000 720b 0000 0072 0c00 0000  gr....r....r....
-00000f00: da15 6765 745f 616e 645f 7365 745f 7468  ..get_and_set_th
-00000f10: 655f 636f 6c6f 72f3 0000 0073 2a00 0000  e_color....s*...
-00000f20: 1201 0801 0c01 0201 0c01 04ff 0803 0201  ................
-00000f30: 0801 0201 0201 04fd 0805 1001 0801 0c02  ................
-00000f40: 0406 14fd 02ff 0c03 0401 7222 0000 0072  ..........r"...r
-00000f50: 2100 0000 da04 6172 6731 da04 6172 6732  !.....arg1..arg2
-00000f60: da06 7265 7475 726e 6303 0000 0000 0000  ..returnc.......
-00000f70: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00000f80: 0073 2600 0000 7400 a001 7c00 9b00 7c01  .s&...t...|...|.
-00000f90: 9b00 9d02 a101 0100 7402 7c00 8301 0100  ........t.|.....
-00000fa0: 7403 7c02 8301 0100 6401 5300 2902 7ab2  t.|.....d.S.).z.
-00000fb0: 0a20 2020 204c 6f67 2061 6e64 2070 7269  .    Log and pri
-00000fc0: 6e74 2065 7272 6f72 206d 6573 7361 6765  nt error message
-00000fd0: 2c20 616e 6420 7468 656e 2065 7869 742e  , and then exit.
-00000fe0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000ff0: 6572 726f 725f 6d73 673a 206d 6573 7361  error_msg: messa
-00001000: 6765 2074 6f20 6f75 7470 7574 0a20 2020  ge to output.   
-00001010: 2020 2020 203a 7061 7261 6d20 6172 6731       :param arg1
-00001020: 3a20 6578 6974 2063 6f64 6520 7465 7874  : exit code text
-00001030: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001040: 6172 6732 3a20 6578 6974 2063 6f64 6520  arg2: exit code 
-00001050: 6e75 6d62 6572 2061 7320 696e 740a 2020  number as int.  
-00001060: 2020 4e29 0472 0300 0000 7216 0000 0072    N).r....r....r
-00001070: 0700 0000 7218 0000 0029 0372 2100 0000  ....r....).r!...
-00001080: 7223 0000 0072 2400 0000 720b 0000 0072  r#...r$...r....r
-00001090: 0b00 0000 720c 0000 0072 1e00 0000 0d01  ....r....r......
-000010a0: 0000 7306 0000 0012 0708 010c 0172 1e00  ..s..........r..
-000010b0: 0000 290a 7211 0000 00da 166d 6170 7461  ..).r......mapta
-000010c0: 736b 6572 2e73 7263 2e73 7973 636f 6e73  sker.src.syscons
-000010d0: 7472 0200 0000 7203 0000 0072 0d00 0000  tr....r....r....
-000010e0: 7219 0000 0072 2200 0000 da03 7374 72da  r....r".....str.
-000010f0: 0369 6e74 721e 0000 0072 0b00 0000 720b  .intr....r....r.
-00001100: 0000 0072 0b00 0000 720c 0000 00da 083c  ...r....r......<
-00001110: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
-00001120: 080d 0c01 0c01 0806 0811 007f 084d 1e1a  .............M..
+00000040: 0100 6400 6403 6c01 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6404 6c04 6d05 5a05 0100 6405 6406 8400  d.l.m.Z...d.d...
+00000060: 5a06 6407 6408 8400 5a07 6409 640a 8400  Z.d.d...Z.d.d...
+00000070: 5a08 6401 5300 290b e900 0000 004e 2901  Z.d.S.)......N).
+00000080: da14 5459 5045 535f 4f46 5f43 4f4c 4f52  ..TYPES_OF_COLOR
+00000090: 5f4e 414d 4553 2901 da06 6c6f 6767 6572  _NAMES)...logger
+000000a0: 2901 da0d 6572 726f 725f 6861 6e64 6c65  )...error_handle
+000000b0: 7263 0200 0000 0000 0000 0000 0000 0600  rc..............
+000000c0: 0000 0400 0000 4300 0000 7354 0000 0064  ......C...sT...d
+000000d0: 017d 0264 027d 0374 007c 0183 0164 0318  .}.d.}.t.|...d..
+000000e0: 007d 047c 0072 1074 017c 0083 0101 007c  .}.|.r.t.|.....|
+000000f0: 0144 005d 117d 057c 01a0 027c 05a1 017c  .D.].}.|...|...|
+00000100: 046b 0272 1d64 017d 037c 027c 0517 007c  .k.r.d.}.|.|...|
+00000110: 0317 007d 0271 1274 017c 0283 0101 0064  ...}.q.t.|.....d
+00000120: 0053 0029 044e da00 7a02 2c20 e901 0000  .S.).N..z., ....
+00000130: 0029 03da 036c 656e da05 7072 696e 74da  .)...len..print.
+00000140: 0569 6e64 6578 2906 5a0a 6c69 7374 5f74  .index).Z.list_t
+00000150: 6974 6c65 da08 7468 655f 6c69 7374 5a08  itle..the_listZ.
+00000160: 6c69 6e65 5f6f 7574 5a09 7365 7065 7261  line_outZ.sepera
+00000170: 746f 725a 0b6c 6973 745f 6c65 6e67 7468  torZ.list_length
+00000180: da04 6974 656d a900 720c 0000 00fa 752f  ..item..r.....u/
+00000190: 5573 6572 732f 6d69 6b72 7562 696e 2f4c  Users/mikrubin/L
+000001a0: 6962 7261 7279 2f43 6c6f 7564 5374 6f72  ibrary/CloudStor
+000001b0: 6167 652f 476f 6f67 6c65 4472 6976 652d  age/GoogleDrive-
+000001c0: 6d69 6b72 7562 696e 4067 6d61 696c 2e63  mikrubin@gmail.c
+000001d0: 6f6d 2f4d 7920 4472 6976 652f 5079 7468  om/My Drive/Pyth
+000001e0: 6f6e 2f6d 6170 7461 736b 6572 2f6d 6170  on/maptasker/map
+000001f0: 7461 736b 6572 2f73 7263 2f63 6f6c 6f72  tasker/src/color
+00000200: 732e 7079 da0a 7072 696e 745f 6c69 7374  s.py..print_list
+00000210: 1700 0000 7316 0000 0004 0104 010c 0104  ....s...........
+00000220: 0108 0108 010e 0104 010e 0108 0104 0172  ...............r
+00000230: 0e00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000240: 000d 0000 0004 0000 0043 0000 0073 3001  .........C...s0.
+00000250: 0000 6700 6401 a201 7d01 6700 6402 a201  ..g.d...}.g.d...
+00000260: 7d02 6700 6403 a201 7d03 6700 6404 a201  }.g.d...}.g.d...
+00000270: 7d04 6700 6405 a201 7d05 6700 6406 a201  }.g.d...}.g.d...
+00000280: 7d06 6700 6407 a201 7d07 6700 6408 a201  }.g.d...}.g.d...
+00000290: 7d08 6700 6409 a201 7d09 6700 640a a201  }.g.d...}.g.d...
+000002a0: 7d0a 640b 6701 7d0b 7c01 7c02 1700 7c03  }.d.g.}.|.|...|.
+000002b0: 1700 7c04 1700 7c05 1700 7c06 1700 7c07  ..|...|...|...|.
+000002c0: 1700 7c08 1700 7c09 1700 7c0a 1700 7c0b  ..|...|...|...|.
+000002d0: 1700 7d0c 7c00 640c 6b03 725b 7400 a001  ..}.|.d.k.r[t...
+000002e0: 7c00 7c0c 7600 a101 0100 7402 640d 640e  |.|.v.....t.d.d.
+000002f0: 8400 7c00 4400 8301 8301 7257 640f 5300  ..|.D.....rWd.S.
+00000300: 7c00 7c0c 7600 5300 7403 6410 7c01 8302  |.|.v.S.t.d.|...
+00000310: 0100 7403 6411 7c02 8302 0100 7403 6412  ..t.d.|.....t.d.
+00000320: 7c03 8302 0100 7403 6413 7c04 8302 0100  |.....t.d.|.....
+00000330: 7403 6414 7c05 8302 0100 7403 6415 7c06  t.d.|.....t.d.|.
+00000340: 8302 0100 7403 6416 7c07 8302 0100 7403  ....t.d.|.....t.
+00000350: 6417 7c08 8302 0100 7403 6418 7c09 8302  d.|.....t.d.|...
+00000360: 0100 7403 6419 7c0a 8302 0100 7403 641a  ..t.d.|.....t.d.
+00000370: 7c0b 8302 0100 7404 641b 8301 0100 6400  |.....t.d.....d.
+00000380: 5300 291c 4e29 095a 0949 6e64 6961 6e52  S.).N).Z.IndianR
+00000390: 6564 5a0a 4c69 6768 7443 6f72 616c 5a06  edZ.LightCoralZ.
+000003a0: 5361 6c6d 6f6e 5a0a 4461 726b 5361 6c6d  SalmonZ.DarkSalm
+000003b0: 6f6e da0b 4c69 6768 7453 616c 6d6f 6e5a  on..LightSalmonZ
+000003c0: 0743 7269 6d73 6f6e da03 5265 645a 0946  .Crimson..RedZ.F
+000003d0: 6972 6542 7269 636b 5a07 4461 726b 5265  ireBrickZ.DarkRe
+000003e0: 6429 065a 0450 696e 6b5a 094c 6967 6874  d).Z.PinkZ.Light
+000003f0: 5069 6e6b 5a07 486f 7450 696e 6b5a 0844  PinkZ.HotPinkZ.D
+00000400: 6565 7050 696e 6b5a 0f4d 6564 6975 6d56  eepPinkZ.MediumV
+00000410: 696f 6c65 7452 6564 5a0d 5061 6c65 5669  ioletRedZ.PaleVi
+00000420: 6f6c 6574 5265 6429 0672 0f00 0000 5a05  oletRed).r....Z.
+00000430: 436f 7261 6c5a 0654 6f6d 6174 6f5a 094f  CoralZ.TomatoZ.O
+00000440: 7261 6e67 6552 6564 5a0a 4461 726b 4f72  rangeRedZ.DarkOr
+00000450: 616e 6765 5a06 4f72 616e 6765 290b 5a04  angeZ.Orange).Z.
+00000460: 476f 6c64 da06 5965 6c6c 6f77 5a0b 4c69  Gold..YellowZ.Li
+00000470: 6768 7459 656c 6c6f 775a 0c4c 656d 6f6e  ghtYellowZ.Lemon
+00000480: 4368 6966 666f 6e5a 144c 6967 6874 476f  ChiffonZ.LightGo
+00000490: 6c64 656e 726f 6459 656c 6c6f 775a 0a50  ldenrodYellowZ.P
+000004a0: 6170 6179 6157 6869 705a 084d 6f63 6361  apayaWhipZ.Mocca
+000004b0: 7369 6e5a 0950 6561 6368 5075 6666 5a0d  sinZ.PeachPuffZ.
+000004c0: 5061 6c65 476f 6c64 656e 726f 645a 054b  PaleGoldenrodZ.K
+000004d0: 6861 6b69 5a09 4461 726b 4b68 616b 6929  hakiZ.DarkKhaki)
+000004e0: 135a 084c 6176 656e 6465 725a 0754 6869  .Z.LavenderZ.Thi
+000004f0: 7374 6c65 5a04 506c 756d 5a06 5669 6f6c  stleZ.PlumZ.Viol
+00000500: 6574 5a06 4f72 6368 6964 5a07 4675 6368  etZ.OrchidZ.Fuch
+00000510: 7369 615a 074d 6167 656e 7461 5a0c 4d65  siaZ.MagentaZ.Me
+00000520: 6469 756d 4f72 6368 6964 5a0c 4d65 6469  diumOrchidZ.Medi
+00000530: 756d 5075 7270 6c65 5a0d 5265 6265 6363  umPurpleZ.Rebecc
+00000540: 6150 7572 706c 655a 0a42 6c75 6556 696f  aPurpleZ.BlueVio
+00000550: 6c65 745a 0a44 6172 6b56 696f 6c65 745a  letZ.DarkVioletZ
+00000560: 0a44 6172 6b4f 7263 6869 645a 0b44 6172  .DarkOrchidZ.Dar
+00000570: 6b4d 6167 656e 7461 5a06 5075 7270 6c65  kMagentaZ.Purple
+00000580: 5a06 496e 6469 676f 5a09 536c 6174 6542  Z.IndigoZ.SlateB
+00000590: 6c75 655a 0d44 6172 6b53 6c61 7465 426c  lueZ.DarkSlateBl
+000005a0: 7565 da0f 4d65 6469 756d 536c 6174 6542  ue..MediumSlateB
+000005b0: 6c75 6529 175a 0b47 7265 656e 5965 6c6c  lue).Z.GreenYell
+000005c0: 6f77 5a0a 4368 6172 7472 6575 7365 da09  owZ.Chartreuse..
+000005d0: 4c61 776e 4772 6565 6e5a 044c 696d 655a  LawnGreenZ.LimeZ
+000005e0: 094c 696d 6547 7265 656e 5a09 5061 6c65  .LimeGreenZ.Pale
+000005f0: 4772 6565 6e5a 0a4c 6967 6874 4772 6565  GreenZ.LightGree
+00000600: 6e5a 114d 6564 6975 6d53 7072 696e 6747  nZ.MediumSpringG
+00000610: 7265 656e 5a0b 5370 7269 6e67 4772 6565  reenZ.SpringGree
+00000620: 6e5a 0e4d 6564 6975 6d53 6561 4772 6565  nZ.MediumSeaGree
+00000630: 6e5a 0853 6561 4772 6565 6e5a 0b46 6f72  nZ.SeaGreenZ.For
+00000640: 6573 7447 7265 656e 5a05 4772 6565 6e5a  estGreenZ.GreenZ
+00000650: 0944 6172 6b47 7265 656e 5a0b 5965 6c6c  .DarkGreenZ.Yell
+00000660: 6f77 4772 6565 6e5a 094f 6c69 7665 4472  owGreenZ.OliveDr
+00000670: 6162 5a05 4f6c 6976 655a 0e44 6172 6b4f  abZ.OliveZ.DarkO
+00000680: 6c69 7665 4772 6565 6e5a 104d 6564 6975  liveGreenZ.Mediu
+00000690: 6d41 7175 616d 6172 696e 655a 0c44 6172  mAquamarineZ.Dar
+000006a0: 6b53 6561 4772 6565 6e5a 0d4c 6967 6874  kSeaGreenZ.Light
+000006b0: 5365 6147 7265 656e 5a08 4461 726b 4379  SeaGreenZ.DarkCy
+000006c0: 616e 5a04 5465 616c 2919 5a04 4171 7561  anZ.Teal).Z.Aqua
+000006d0: 5a04 4379 616e 5a09 4c69 6768 7443 7961  Z.CyanZ.LightCya
+000006e0: 6e5a 0d50 616c 6554 7572 7175 6f69 7365  nZ.PaleTurquoise
+000006f0: 5a0a 4171 7561 6d61 7269 6e65 5a09 5475  Z.AquamarineZ.Tu
+00000700: 7271 756f 6973 655a 0f4d 6564 6975 6d54  rquoiseZ.MediumT
+00000710: 7572 7175 6f69 7365 5a0d 4461 726b 5475  urquoiseZ.DarkTu
+00000720: 7271 756f 6973 655a 0943 6164 6574 426c  rquoiseZ.CadetBl
+00000730: 7565 5a09 5374 6565 6c42 6c75 655a 0e4c  ueZ.SteelBlueZ.L
+00000740: 6967 6874 5374 6565 6c42 6c75 655a 0a50  ightSteelBlueZ.P
+00000750: 6f77 6465 7242 6c75 655a 094c 6967 6874  owderBlueZ.Light
+00000760: 426c 7565 5a07 536b 7942 6c75 655a 0c4c  BlueZ.SkyBlueZ.L
+00000770: 6967 6874 536b 7942 6c75 655a 0b44 6565  ightSkyBlueZ.Dee
+00000780: 7053 6b79 426c 7565 5a0a 446f 6467 6572  pSkyBlueZ.Dodger
+00000790: 426c 7565 5a0e 436f 726e 666c 6f77 6572  BlueZ.Cornflower
+000007a0: 426c 7565 7212 0000 005a 0952 6f79 616c  Bluer....Z.Royal
+000007b0: 426c 7565 5a04 426c 7565 5a0a 4d65 6469  BlueZ.BlueZ.Medi
+000007c0: 756d 426c 7565 5a08 4461 726b 426c 7565  umBlueZ.DarkBlue
+000007d0: 5a04 4e61 7679 5a0c 4d69 646e 6967 6874  Z.NavyZ.Midnight
+000007e0: 426c 7565 2911 5a08 436f 726e 7369 6c6b  Blue).Z.Cornsilk
+000007f0: 5a0e 426c 616e 6368 6564 416c 6d6f 6e64  Z.BlanchedAlmond
+00000800: 5a06 4269 7371 7565 5a0b 4e61 7661 6a6f  Z.BisqueZ.Navajo
+00000810: 5768 6974 655a 0557 6865 6174 5a09 4275  WhiteZ.WheatZ.Bu
+00000820: 726c 7957 6f6f 645a 0354 616e 5a09 526f  rlyWoodZ.TanZ.Ro
+00000830: 7379 4272 6f77 6e5a 0a53 616e 6479 4272  syBrownZ.SandyBr
+00000840: 6f77 6e5a 0947 6f6c 6465 6e72 6f64 5a0d  ownZ.GoldenrodZ.
+00000850: 4461 726b 476f 6c64 656e 726f 645a 0450  DarkGoldenrodZ.P
+00000860: 6572 755a 0943 686f 636f 6c61 7465 5a0b  eruZ.ChocolateZ.
+00000870: 5361 6464 6c65 4272 6f77 6e5a 0653 6965  SaddleBrownZ.Sie
+00000880: 6e6e 615a 0542 726f 776e 5a06 4d61 726f  nnaZ.BrownZ.Maro
+00000890: 6f6e 2911 da05 5768 6974 655a 0453 6e6f  on)...WhiteZ.Sno
+000008a0: 775a 0848 6f6e 6579 4465 775a 094d 696e  wZ.HoneyDewZ.Min
+000008b0: 7443 7265 616d 5a05 417a 7572 655a 0941  tCreamZ.AzureZ.A
+000008c0: 6c69 6365 426c 7565 5a0a 4768 6f73 7457  liceBlueZ.GhostW
+000008d0: 6869 7465 5a0a 5768 6974 6553 6d6f 6b65  hiteZ.WhiteSmoke
+000008e0: 5a08 5365 6153 6865 6c6c 5a05 4265 6967  Z.SeaShellZ.Beig
+000008f0: 655a 074f 6c64 4c61 6365 5a0b 466c 6f72  eZ.OldLaceZ.Flor
+00000900: 616c 5768 6974 655a 0549 766f 7279 5a0c  alWhiteZ.IvoryZ.
+00000910: 416e 7469 7175 6557 6869 7465 5a05 4c69  AntiqueWhiteZ.Li
+00000920: 6e65 6e5a 0d4c 6176 656e 6465 7242 6c75  nenZ.LavenderBlu
+00000930: 7368 5a09 4d69 7374 7952 6f73 6529 0a5a  shZ.MistyRose).Z
+00000940: 0947 6169 6e73 626f 726f 5a09 4c69 6768  .GainsboroZ.Ligh
+00000950: 7447 7261 795a 0653 696c 7665 725a 0844  tGrayZ.SilverZ.D
+00000960: 6172 6b47 7261 795a 0447 7261 795a 0744  arkGrayZ.GrayZ.D
+00000970: 696d 4772 6179 5a0e 4c69 6768 7453 6c61  imGrayZ.LightSla
+00000980: 7465 4772 6179 5a09 536c 6174 6547 7261  teGrayZ.SlateGra
+00000990: 795a 0d44 6172 6b53 6c61 7465 4772 6179  yZ.DarkSlateGray
+000009a0: 5a05 426c 6163 6b7a 1c68 6578 2076 616c  Z.Blackz.hex val
+000009b0: 7565 2e20 2045 7861 6d70 6c65 2027 6462  ue.  Example 'db
+000009c0: 3239 6666 27da 0168 6301 0000 0000 0000  29ff'..hc.......
+000009d0: 0000 0000 0002 0000 0003 0000 0073 0000  .............s..
+000009e0: 0073 1a00 0000 8100 7c00 5d08 7d01 7c01  .s......|.].}.|.
+000009f0: 7400 6a01 7600 5600 0100 7102 6400 5300  t.j.v.V...q.d.S.
+00000a00: 2901 4e29 02da 0673 7472 696e 67da 0968  ).N)...string..h
+00000a10: 6578 6469 6769 7473 2902 da02 2e30 da01  exdigits)....0..
+00000a20: 6372 0c00 0000 720c 0000 0072 0d00 0000  cr....r....r....
+00000a30: da09 3c67 656e 6578 7072 3edf 0000 0073  ..<genexpr>....s
+00000a40: 0400 0000 0280 1800 7a21 7661 6c69 6461  ........z!valida
+00000a50: 7465 5f63 6f6c 6f72 2e3c 6c6f 6361 6c73  te_color.<locals
+00000a60: 3e2e 3c67 656e 6578 7072 3e54 7a11 0a52  >.<genexpr>Tz..R
+00000a70: 6564 2063 6f6c 6f72 206e 616d 6573 3a7a  ed color names:z
+00000a80: 120a 5069 6e6b 2063 6f6c 6f72 206e 616d  ..Pink color nam
+00000a90: 6573 3a7a 140a 4f72 616e 6765 2063 6f6c  es:z..Orange col
+00000aa0: 6f72 206e 616d 6573 3a7a 140a 5965 6c6c  or names:z..Yell
+00000ab0: 6f77 2063 6f6c 6f72 206e 616d 6573 3a7a  ow color names:z
+00000ac0: 140a 5075 7270 6c65 2063 6f6c 6f72 206e  ..Purple color n
+00000ad0: 616d 6573 3a7a 130a 4772 6565 6e20 636f  ames:z..Green co
+00000ae0: 6c6f 7220 6e61 6d65 733a 7a12 0a42 6c75  lor names:z..Blu
+00000af0: 6520 636f 6c6f 7220 6e61 6d65 733a 7a13  e color names:z.
+00000b00: 0a42 726f 776e 2063 6f6c 6f72 206e 616d  .Brown color nam
+00000b10: 6573 3a7a 130a 5768 6974 6520 636f 6c6f  es:z..White colo
+00000b20: 7220 6e61 6d65 733a 7a12 0a47 7261 7920  r names:z..Gray 
+00000b30: 636f 6c6f 7220 6e61 6d65 733a 7a0b 0a41  color names:z..A
+00000b40: 6e79 2063 6f6c 6f72 3a72 0100 0000 2905  ny color:r....).
+00000b50: 7203 0000 00da 0564 6562 7567 da03 616c  r......debug..al
+00000b60: 6c72 0e00 0000 da04 6578 6974 290d 5a09  lr......exit).Z.
+00000b70: 7468 655f 636f 6c6f 725a 0f72 6564 5f63  the_colorZ.red_c
+00000b80: 6f6c 6f72 5f6e 616d 6573 5a10 7069 6e6b  olor_namesZ.pink
+00000b90: 5f63 6f6c 6f72 5f6e 616d 6573 5a12 6f72  _color_namesZ.or
+00000ba0: 616e 6765 5f63 6f6c 6f72 5f6e 616d 6573  ange_color_names
+00000bb0: 5a12 7965 6c6c 6f77 5f63 6f6c 6f72 5f6e  Z.yellow_color_n
+00000bc0: 616d 6573 5a12 7075 7270 6c65 5f63 6f6c  amesZ.purple_col
+00000bd0: 6f72 5f6e 616d 6573 5a11 6772 6565 6e5f  or_namesZ.green_
+00000be0: 636f 6c6f 725f 6e61 6d65 735a 1062 6c75  color_namesZ.blu
+00000bf0: 655f 636f 6c6f 725f 6e61 6d65 735a 1162  e_color_namesZ.b
+00000c00: 726f 776e 5f63 6f6c 6f72 5f6e 616d 6573  rown_color_names
+00000c10: 5a11 7768 6974 655f 636f 6c6f 725f 6e61  Z.white_color_na
+00000c20: 6d65 735a 1067 7261 795f 636f 6c6f 725f  mesZ.gray_color_
+00000c30: 6e61 6d65 735a 0961 6e79 5f63 6f6c 6f72  namesZ.any_color
+00000c40: 5a0a 616c 6c5f 636f 6c6f 7273 720c 0000  Z.all_colorsr...
+00000c50: 0072 0c00 0000 720d 0000 00da 0e76 616c  .r....r......val
+00000c60: 6964 6174 655f 636f 6c6f 7228 0000 0073  idate_color(...s
+00000c70: 6400 0000 0801 080b 0808 0808 080d 0815  d...............
+00000c80: 0819 081b 0813 0813 060c 0203 0201 02ff  ................
+00000c90: 0202 02fe 0203 02fd 0204 02fc 0205 02fb  ................
+00000ca0: 0206 02fa 0207 02f9 0208 02f8 0209 02f7  ................
+00000cb0: 020a 02f6 02ff 080e 0e01 1202 0401 0802  ................
+00000cc0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00000cd0: 0a01 0a01 0a01 0c01 721e 0000 0063 0200  ........r....c..
+00000ce0: 0000 0000 0000 0000 0000 0500 0000 0600  ................
+00000cf0: 0000 4300 0000 73a0 0000 007c 0064 0164  ..C...s....|.d.d
+00000d00: 0085 0219 00a0 0064 02a1 017d 027c 0264  .......d...}.|.d
+00000d10: 0319 007d 0374 017c 0283 0164 016b 0072  ...}.t.|...d.k.r
+00000d20: 1b74 027c 009b 0064 049d 0264 0583 0201  .t.|...d...d....
+00000d30: 007c 0374 0376 0172 2874 027c 039b 0064  .|.t.v.r(t.|...d
+00000d40: 069d 0264 0764 0583 0301 007c 0264 0819  ...d.d.....|.d..
+00000d50: 007d 0474 04a0 0564 097c 049b 009d 02a1  .}.t...d.|......
+00000d60: 0101 0074 067c 0483 0172 407c 047c 0174  ...t.|...r@|.|.t
+00000d70: 037c 0319 003c 0064 0053 0074 0264 0a7c  .|...<.d.S.t.d.|
+00000d80: 049b 0064 0b7c 0264 0319 009b 0064 0c9d  ...d.|.d.....d..
+00000d90: 0564 0583 0201 0064 0053 0029 0d4e e902  .d.....d.S.).N..
+00000da0: 0000 00fa 013d 7201 0000 007a 2d20 6861  .....=r....z- ha
+00000db0: 7320 616e 2069 6e76 616c 6964 2027 636f  s an invalid 'co
+00000dc0: 6c6f 7227 2e20 2053 6565 2074 6865 2068  lor'.  See the h
+00000dd0: 656c 7020 282d 6368 2921 e907 0000 007a  elp (-ch)!.....z
+00000de0: 3420 6973 2061 6e20 696e 7661 6c69 6420  4 is an invalid 
+00000df0: 7479 7065 2066 6f72 2027 636f 6c6f 7227  type for 'color'
+00000e00: 2e20 2053 6565 2074 6865 2068 656c 7020  .  See the help 
+00000e10: 282d 6829 217a 0c20 4578 6974 2063 6f64  (-h)!z. Exit cod
+00000e20: 6520 3772 0600 0000 7a0f 2064 6573 6972  e 7r....z. desir
+00000e30: 6564 5f63 6f6c 6f72 3a7a 254d 6170 5461  ed_color:z%MapTa
+00000e40: 736b 6572 2e2e 2e69 6e76 616c 6964 2063  sker...invalid c
+00000e50: 6f6c 6f72 2073 7065 6369 6669 6564 3a20  olor specified: 
+00000e60: 7a07 2066 6f72 2027 637a 0227 2129 07da  z. for 'cz.'!)..
+00000e70: 0573 706c 6974 7207 0000 0072 0400 0000  .splitr....r....
+00000e80: 7202 0000 0072 0300 0000 721b 0000 0072  r....r....r....r
+00000e90: 1e00 0000 2905 da07 7468 655f 6172 67da  ....)...the_arg.
+00000ea0: 0863 6f6c 6f72 6d61 705a 1074 6865 5f63  .colormapZ.the_c
+00000eb0: 6f6c 6f72 5f6f 7074 696f 6e5a 0a63 6f6c  olor_optionZ.col
+00000ec0: 6f72 5f74 7970 655a 0d64 6573 6972 6564  or_typeZ.desired
+00000ed0: 5f63 6f6c 6f72 720c 0000 0072 0c00 0000  _colorr....r....
+00000ee0: 720d 0000 00da 1567 6574 5f61 6e64 5f73  r......get_and_s
+00000ef0: 6574 5f74 6865 5f63 6f6c 6f72 f400 0000  et_the_color....
+00000f00: 732c 0000 0012 0108 010c 0110 0108 0102  s,..............
+00000f10: 0108 0102 0102 0104 fd08 0510 0108 010c  ................
+00000f20: 0204 0902 f908 0206 0106 ff02 0304 fb04  ................
+00000f30: 0772 2500 0000 2909 7216 0000 00da 166d  .r%...).r......m
+00000f40: 6170 7461 736b 6572 2e73 7263 2e73 7973  aptasker.src.sys
+00000f50: 636f 6e73 7472 0200 0000 7203 0000 00da  constr....r.....
+00000f60: 136d 6170 7461 736b 6572 2e73 7263 2e65  .maptasker.src.e
+00000f70: 7272 6f72 7204 0000 0072 0e00 0000 721e  rrorr....r....r.
+00000f80: 0000 0072 2500 0000 720c 0000 0072 0c00  ...r%...r....r..
+00000f90: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
+00000fa0: 6f64 756c 653e 0100 0000 7310 0000 0008  odule>....s.....
+00000fb0: 0d0c 010c 010c 0108 0608 1100 7f0c 4d    ..............M
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/colrmode.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/colrmode.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/condition.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/condition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/debug.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/debug.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/frmthtml.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/frmthtml.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 16:38:32 2023 UTC, .py size: 2017 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0830 3864 e107 0000  o........08d....
+00000000: 6f0d 0d0a 0000 0000 629c 4a64 e107 0000  o.......b.Jd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6502 6403  d.l.m.Z...d.e.d.
 00000040: 6503 6404 6503 6405 6503 6406 6504 6407  e.d.e.d.e.d.e.d.
 00000050: 6503 660c 6408 6409 8404 5a05 640a 5300  e.f.d.d...Z.d.S.
 00000060: 290b e900 0000 0029 01da 0b46 4f4e 545f  )......)...FONT_
 00000070: 544f 5f55 5345 da08 636f 6c6f 726d 6170  TO_USE..colormap
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/getids.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/getids.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/getputarg.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/migrate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 10 14:52:10 2023 UTC, .py size: 3042 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,150 @@
-00000000: 6f0d 0d0a 0000 0000 9a22 3464 e20b 0000  o........"4d....
+00000000: 6f0d 0d0a 0000 0000 de26 4464 ac10 0000  o........&Dd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c01 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c04 6d05 5a05 0100 6405 6506 6406  d.l.m.Z...d.e.d.
-00000060: 6507 6407 6507 6408 6508 6507 6507 6602  e.d.e.d.e.e.e.f.
-00000070: 1900 6608 6409 640a 8404 5a09 6401 5300  ..f.d.d...Z.d.S.
-00000080: 290b e900 0000 004e 2901 da0e 4152 4755  )......N)...ARGU
-00000090: 4d45 4e54 535f 4649 4c45 2901 da06 6c6f  MENTS_FILE)...lo
-000000a0: 6767 6572 2901 da04 5061 7468 da07 746f  gger)...Path..to
-000000b0: 5f73 6176 65da 0863 6f6c 6f72 6d61 70da  _save..colormap.
-000000c0: 0974 656d 705f 6172 6773 da06 7265 7475  .temp_args..retu
-000000d0: 726e 6303 0000 0000 0000 0000 0000 0008  rnc.............
-000000e0: 0000 0008 0000 0043 0000 0073 4a01 0000  .......C...sJ...
-000000f0: 7400 a001 a100 9b00 6401 7402 9b00 9d03  t.......d.t.....
-00000100: 7d03 7c00 7235 7c01 7c02 6702 7d04 7403  }.|.r5|.|.g.}.t.
-00000110: 7c03 6402 8302 8f15 7d05 7404 a005 7c04  |.d.....}.t...|.
-00000120: 7c05 a102 0100 7c05 a006 a100 0100 5700  |.....|.......W.
-00000130: 6403 0400 0400 8303 0100 7c02 7c01 6602  d.........|.|.f.
-00000140: 5300 3100 732c 7701 0100 0100 0100 5900  S.1.s,w.......Y.
-00000150: 0100 7c02 7c01 6602 5300 7a30 7403 7c03  ..|.|.f.S.z0t.|.
-00000160: 6404 8302 8f19 7d05 7404 a007 7c05 a101  d.....}.t...|...
-00000170: 7d06 7c06 6405 1900 7d01 7c06 6406 1900  }.|.d...}.|.d...
-00000180: 7d02 7c05 a006 a100 0100 5700 6403 0400  }.|.......W.d...
-00000190: 0400 8303 0100 6e0d 3100 7357 7701 0100  ......n.1.sWw...
-000001a0: 0100 0100 5900 0100 5700 7c02 7c01 6602  ....Y...W.|.|.f.
-000001b0: 5300 5700 7c02 7c01 6602 5300 0400 7408  S.W.|.|.f.S...t.
-000001c0: 7982 0100 0100 0100 6407 7d07 7409 7c07  y.......d.}.t.|.
-000001d0: 8301 0100 740a a00b 7c07 a101 0100 6408  ....t...|.....d.
-000001e0: 6409 6901 0400 7d02 7d01 5900 7c02 7c01  d.i...}.}.Y.|.|.
-000001f0: 6602 5300 0400 7404 6a0c 6a0d 79a4 0100  f.S...t.j.j.y...
-00000200: 0100 0100 640a 7402 9b00 640b 9d03 7d07  ....d.t...d...}.
-00000210: 7409 7c07 8301 0100 740a a00b 7c07 a101  t.|.....t...|...
-00000220: 0100 6408 640c 6901 0400 7d02 7d01 5900  ..d.d.i...}.}.Y.
-00000230: 7c02 7c01 6602 5300 7700 290d 612b 0100  |.|.f.S.w.).a+..
-00000240: 000a 2020 2020 5361 7665 2061 6e64 2072  ..    Save and r
-00000250: 6573 746f 7265 2063 6f6c 6f72 7320 746f  estore colors to
-00000260: 2075 7365 2061 6e64 2070 726f 6772 616d   use and program
-00000270: 2061 7267 756d 656e 7473 0a20 2020 2020   arguments.     
-00000280: 2020 203a 7061 7261 6d20 746f 5f73 6176     :param to_sav
-00000290: 653a 2054 7275 6520 6966 2077 6520 6172  e: True if we ar
-000002a0: 6520 746f 2073 6176 6520 7468 6520 696e  e to save the in
-000002b0: 666f 2c20 4661 6c73 6520 746f 2072 6573  fo, False to res
-000002c0: 746f 7265 2074 6865 2069 6e66 6f0a 2020  tore the info.  
-000002d0: 2020 2020 2020 3a70 6172 616d 2063 6f6c        :param col
-000002e0: 6f72 6d61 703a 2063 6f6c 6f72 7320 746f  ormap: colors to
-000002f0: 2075 7365 2069 6e20 6f75 7470 7574 0a20   use in output. 
-00000300: 2020 2020 2020 203a 7061 7261 6d20 7465         :param te
-00000310: 6d70 5f61 7267 733a 2072 756e 7469 6d65  mp_args: runtime
-00000320: 2061 7267 756d 656e 7473 0a20 2020 2020   arguments.     
-00000330: 2020 203a 7265 7475 726e 3a20 636f 6c6f     :return: colo
-00000340: 7273 2061 6e64 2072 756e 7469 6d65 2061  rs and runtime a
-00000350: 7267 756d 656e 7473 2073 6176 6564 2f72  rguments saved/r
-00000360: 6573 746f 7265 640a 2020 2020 fa01 2fda  estored.    ../.
-00000370: 0177 4eda 0172 7201 0000 00e9 0100 0000  .wN..rr.........
-00000380: 7a2e 272d 7227 2045 7272 6f72 3a20 4e6f  z.'-r' Error: No
-00000390: 2073 6574 7469 6e67 7320 6669 6c65 2066   settings file f
-000003a0: 6f75 6e64 2074 6f20 7265 7374 6f72 6521  ound to restore!
-000003b0: da03 6d73 677a 224e 6f20 7365 7474 696e  ..msgz"No settin
-000003c0: 6773 2066 696c 6520 666f 756e 6420 746f  gs file found to
-000003d0: 2072 6573 746f 7265 217a 2027 2d72 2720   restore!z '-r' 
-000003e0: 4572 726f 723a 2054 6865 2073 6574 7469  Error: The setti
-000003f0: 6e67 7320 6669 6c65 2c20 207a 0c20 6973  ngs file,  z. is
-00000400: 2063 6f72 7275 7074 217a 3554 6865 2073   corrupt!z5The s
-00000410: 6574 7469 6e67 7320 6669 6c65 2069 7320  ettings file is 
-00000420: 636f 7272 7570 7421 2020 5265 2d73 6176  corrupt!  Re-sav
-00000430: 6520 796f 7572 2073 6574 7469 6e67 732e  e your settings.
-00000440: 290e 7204 0000 00da 0363 7764 7202 0000  ).r......cwdr...
-00000450: 00da 046f 7065 6eda 046a 736f 6eda 0464  ...open..json..d
-00000460: 756d 70da 0563 6c6f 7365 da04 6c6f 6164  ump..close..load
-00000470: da07 4f53 4572 726f 72da 0570 7269 6e74  ..OSError..print
-00000480: 7203 0000 00da 0564 6562 7567 da07 6465  r......debug..de
-00000490: 636f 6465 72da 0f4a 534f 4e44 6563 6f64  coder..JSONDecod
-000004a0: 6545 7272 6f72 2908 7205 0000 0072 0600  eError).r....r..
-000004b0: 0000 7207 0000 005a 0874 6865 5f66 696c  ..r....Z.the_fil
-000004c0: 655a 0c6c 6973 745f 746f 5f73 6176 65da  eZ.list_to_save.
-000004d0: 0166 5a0f 6c69 7374 5f74 6f5f 7265 7374  .fZ.list_to_rest
-000004e0: 6f72 65da 0965 7272 6f72 5f6d 7367 a900  ore..error_msg..
-000004f0: 721b 0000 00fa 782f 5573 6572 732f 6d69  r.....x/Users/mi
-00000500: 6b72 7562 696e 2f4c 6962 7261 7279 2f43  krubin/Library/C
-00000510: 6c6f 7564 5374 6f72 6167 652f 476f 6f67  loudStorage/Goog
-00000520: 6c65 4472 6976 652d 6d69 6b72 7562 696e  leDrive-mikrubin
-00000530: 4067 6d61 696c 2e63 6f6d 2f4d 7920 4472  @gmail.com/My Dr
-00000540: 6976 652f 5079 7468 6f6e 2f6d 6170 7461  ive/Python/mapta
-00000550: 736b 6572 2f6d 6170 7461 736b 6572 2f73  sker/maptasker/s
-00000560: 7263 2f67 6574 7075 7461 7267 2e70 79da  rc/getputarg.py.
-00000570: 1173 6176 655f 7265 7374 6f72 655f 6172  .save_restore_ar
-00000580: 6773 1800 0000 7344 0000 0012 0a04 0108  gs....sD........
-00000590: 020c 010c 010a 010a fe08 1a10 e608 1a02  ................
-000005a0: eb0c 010a 0108 0108 010a 011e fc08 1402  ................
-000005b0: ec08 140c f204 0108 010a 010e 0108 0a10  ................
-000005c0: f80c 0108 010a 0104 020a ff08 0402 f872  ...............r
-000005d0: 1d00 0000 290a 7210 0000 00da 166d 6170  ....).r......map
-000005e0: 7461 736b 6572 2e73 7263 2e73 7973 636f  tasker.src.sysco
-000005f0: 6e73 7472 0200 0000 7203 0000 00da 0770  nstr....r......p
-00000600: 6174 686c 6962 7204 0000 00da 0462 6f6f  athlibr......boo
-00000610: 6cda 0464 6963 74da 0574 7570 6c65 721d  l..dict..tupler.
-00000620: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
-00000630: 0000 721c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000640: 3e01 0000 0073 1a00 0000 080d 0c02 0c01  >....s..........
-00000650: 0c01 0206 0201 02ff 0201 02ff 0201 02ff  ................
-00000660: 0a02 0efe                                ....
+00000020: 0006 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
+00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6406 6506 6407 650b 650c  m.Z...d.e.d.e.e.
+00000080: 650c 6602 1900 6604 6408 6409 8404 5a0d  e.f...f.d.d...Z.
+00000090: 640a 650e 6407 650b 650c 650c 6602 1900  d.e.d.e.e.e.f...
+000000a0: 6604 640b 640c 8404 5a0f 640f 640d 640e  f.d.d...Z.d.d.d.
+000000b0: 8404 5a10 6401 5300 2910 e900 0000 004e  ..Z.d.S.)......N
+000000c0: 2901 da06 7265 6e61 6d65 2901 da04 5061  )...rename)...Pa
+000000d0: 7468 2901 da11 7361 7665 5f72 6573 746f  th)...save_resto
+000000e0: 7265 5f61 7267 73a9 01da 0d65 7272 6f72  re_args....error
+000000f0: 5f68 616e 646c 6572 da0d 6669 6c65 5f74  _handler..file_t
+00000100: 6f5f 6368 6563 6bda 0672 6574 7572 6e63  o_check..returnc
+00000110: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00000120: 0800 0000 4300 0000 73c4 0000 0069 0004  ....C...s....i..
+00000130: 007d 017d 027a 2174 007c 0064 0183 028f  .}.}.z!t.|.d....
+00000140: 127d 0374 01a0 027c 03a1 017d 0174 01a0  .}.t...|...}.t..
+00000150: 027c 03a1 017d 0257 0064 0204 0004 0083  .|...}.W.d......
+00000160: 0301 006e 0831 0073 1f77 0101 0001 0001  ...n.1.s.w......
+00000170: 0059 0001 0057 006e 3404 0074 0379 3401  .Y...W.n4..t.y4.
+00000180: 0001 0001 0074 0464 0383 015c 027d 017d  .....t.d...\.}.}
+00000190: 0259 006e 2604 0074 056a 0679 4701 0001  .Y.n&..t.j.yG...
+000001a0: 0001 0074 0464 047c 009b 0064 059d 0383  ...t.d.|...d....
+000001b0: 015c 027d 017d 0259 006e 1304 0074 0779  .\.}.}.Y.n...t.y
+000001c0: 5901 0001 0001 0074 0464 047c 009b 0064  Y......t.d.|...d
+000001d0: 069d 0383 015c 027d 017d 0259 006e 0177  .....\.}.}.Y.n.w
+000001e0: 007c 03a0 08a1 0001 007c 027c 0166 0253  .|.......|.|.f.S
+000001f0: 0029 077a a10a 2020 2020 5361 7665 2070  .).z..    Save p
+00000200: 726f 6772 616d 2061 7267 756d 656e 7473  rogram arguments
+00000210: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000220: 6669 6c65 5f74 6f5f 6368 6563 6b3a 2066  file_to_check: f
+00000230: 696c 6520 7061 7468 2f6f 626a 6563 7420  ile path/object 
+00000240: 746f 2072 6573 746f 7265 0a20 2020 2020  to restore.     
+00000250: 2020 203a 7265 7475 726e 3a20 7072 6f67     :return: prog
+00000260: 7261 6d20 7275 6e74 696d 6520 6172 6775  ram runtime argu
+00000270: 6d65 6e74 7320 616e 6420 636f 6c6f 7273  ments and colors
+00000280: 2074 6f20 7573 6520 696e 206f 7574 7075   to use in outpu
+00000290: 740a 2020 2020 da02 7262 4e7a 6b27 2d72  t.    ..rbNzk'-r
+000002a0: 2720 4572 726f 7220 2852 6573 746f 7269  ' Error (Restori
+000002b0: 6e67 204f 6c64 6572 2053 6574 7469 6e67  ng Older Setting
+000002c0: 7320 4669 6c65 293a 2054 6865 7265 2061  s File): There a
+000002d0: 7265 206e 6f20 7361 7665 6420 6974 656d  re no saved item
+000002e0: 7320 666f 756e 6420 746f 206d 6967 7261  s found to migra
+000002f0: 7465 2e20 5072 696f 7220 7365 7474 696e  te. Prior settin
+00000300: 6773 206c 6f73 742e 7a31 272d 7227 2045  gs lost.z1'-r' E
+00000310: 7272 6f72 2028 5265 7374 6f72 696e 6720  rror (Restoring 
+00000320: 4f6c 6465 7220 5365 7474 696e 6773 2046  Older Settings F
+00000330: 696c 6529 3a20 4669 6c65 207a 3620 6973  ile): File z6 is
+00000340: 2063 6f72 7275 7074 2e20 204d 6967 7261   corrupt.  Migra
+00000350: 7469 6f6e 2069 676e 6f72 6564 2e20 2050  tion ignored.  P
+00000360: 7269 6f72 2073 6574 7469 6e67 7320 6c6f  rior settings lo
+00000370: 7374 2e7a 2020 6973 2063 6f72 7275 7074  st.z  is corrupt
+00000380: 2e20 204d 6967 7261 7469 6f6e 2069 676e  .  Migration ign
+00000390: 6f72 6564 2e29 09da 046f 7065 6eda 0670  ored.)...open..p
+000003a0: 6963 6b6c 65da 046c 6f61 64da 074f 5345  ickle..load..OSE
+000003b0: 7272 6f72 da0d 7072 6f63 6573 735f 6572  rror..process_er
+000003c0: 726f 72da 075f 7069 636b 6c65 5a0f 556e  ror.._pickleZ.Un
+000003d0: 7069 636b 6c69 6e67 4572 726f 72da 0845  picklingError..E
+000003e0: 4f46 4572 726f 72da 0563 6c6f 7365 2904  OFError..close).
+000003f0: 7207 0000 00da 0863 6f6c 6f72 6d61 70da  r......colormap.
+00000400: 0c70 726f 6772 616d 5f61 7267 73da 0166  .program_args..f
+00000410: a900 7215 0000 00fa 762f 5573 6572 732f  ..r.....v/Users/
+00000420: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
+00000430: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
+00000440: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
+00000450: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
+00000460: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
+00000470: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
+00000480: 2f73 7263 2f6d 6967 7261 7465 2e70 79da  /src/migrate.py.
+00000490: 1072 6573 746f 7265 5f6f 6c64 5f61 7267  .restore_old_arg
+000004a0: 731b 0000 0073 2c00 0000 0806 0203 0c01  s....s,.........
+000004b0: 0a01 0c01 1cfe 0480 0c03 0201 0202 0cfe  ................
+000004c0: 0e07 0201 0a02 0cfe 0c06 0201 0a02 0cfe  ................
+000004d0: 02ff 0808 0802 7217 0000 00da 0965 7272  ......r......err
+000004e0: 6f72 5f6d 7367 6301 0000 0000 0000 0000  or_msgc.........
+000004f0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00000500: 1200 0000 7400 7c00 6401 8302 0100 6900  ....t.|.d.....i.
+00000510: 6900 6602 5300 2902 7abe 0a20 2020 2044  i.f.S.).z..    D
+00000520: 6973 7370 616c 7920 616e 6420 6c6f 6720  isspaly and log 
+00000530: 6572 726f 7220 6d65 7373 6167 6520 616e  error message an
+00000540: 6420 7265 7365 7420 636f 6c6f 7273 2061  d reset colors a
+00000550: 6e64 2070 726f 6772 616d 2061 7267 7320  nd program args 
+00000560: 746f 2065 6d70 7479 0a20 2020 2020 2020  to empty.       
+00000570: 203a 7061 7261 6d20 6572 726f 725f 6d73   :param error_ms
+00000580: 673a 2065 7272 6f72 2074 6f20 7072 696e  g: error to prin
+00000590: 742f 6c6f 670a 2020 2020 2020 2020 3a72  t/log.        :r
+000005a0: 6574 7572 6e3a 2065 6d70 7479 2063 6f6c  eturn: empty col
+000005b0: 6f72 6d61 7020 616e 6420 7072 6f67 7261  ormap and progra
+000005c0: 6d20 7275 6e74 696d 6520 6172 6775 6d65  m runtime argume
+000005d0: 6e74 730a 2020 2020 7201 0000 0072 0500  nts.    r....r..
+000005e0: 0000 2901 7218 0000 0072 1500 0000 7215  ..).r....r....r.
+000005f0: 0000 0072 1600 0000 720e 0000 0044 0000  ...r....r....D..
+00000600: 0073 0400 0000 0a06 0801 720e 0000 0063  .s........r....c
+00000610: 0000 0000 0000 0000 0000 0000 0600 0000  ................
+00000620: 0800 0000 4300 0000 738a 0000 0064 017d  ....C...s....d.}
+00000630: 0074 007c 009b 0083 017d 0174 00a0 01a1  .t.|.....}.t....
+00000640: 007d 0274 02a0 0374 04a1 018f 1501 0074  .}.t...t.......t
+00000650: 057c 029b 0064 029d 027c 029b 0064 037c  .|...d...|...d.|
+00000660: 009b 009d 0383 0201 0057 0064 0404 0004  .........W.d....
+00000670: 0083 0301 006e 0831 0073 2877 0101 0001  .....n.1.s(w....
+00000680: 0001 0059 0001 007c 01a0 06a1 0072 4374  ...Y...|.....rCt
+00000690: 077c 0183 015c 027d 037d 0474 0864 057c  .|...\.}.}.t.d.|
+000006a0: 047c 0383 035c 027d 057d 057c 01a0 09a1  .|...\.}.}.|....
+000006b0: 0001 0064 0453 0029 067a e10a 2020 2020  ...d.S.).z..    
+000006c0: 4d69 6772 6174 6520 6672 6f6d 206f 6c64  Migrate from old
+000006d0: 2066 696c 656e 616d 652f 666f 726d 6174   filename/format
+000006e0: 2074 6f20 6e65 7720 666f 7220 7361 7665   to new for save
+000006f0: 6420 7275 6e74 696d 6520 6172 6775 6d65  d runtime argume
+00000700: 6e74 730a 2020 2020 2020 5765 2068 6176  nts.      We hav
+00000710: 6520 6368 616e 6765 6420 6672 6f6d 2075  e changed from u
+00000720: 7369 6e67 2074 6865 2075 6e73 6563 7572  sing the unsecur
+00000730: 6520 2270 6963 6b6c 6522 2063 6f64 6520  e "pickle" code 
+00000740: 746f 2075 7369 6e67 2022 6a73 6f6e 220a  to using "json".
+00000750: 2020 2020 2020 746f 2073 6176 6520 7468        to save th
+00000760: 6520 7072 6f67 7261 6d20 6172 6775 6d65  e program argume
+00000770: 6e74 7320 616e 6420 636f 6c6f 7273 0a20  nts and colors. 
+00000780: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00000790: 6e6f 7468 696e 670a 2020 2020 7a18 2e4d  nothing.    z..M
+000007a0: 6170 5461 736b 6572 5f61 7267 756d 656e  apTasker_argumen
+000007b0: 7473 2e74 7874 7a0f 2f2e 6172 6775 6d65  ts.txtz./.argume
+000007c0: 6e74 732e 7478 74fa 012f 4e54 290a 7203  nts.txt../NT).r.
+000007d0: 0000 00da 0363 7764 da0a 636f 6e74 6578  .....cwd..contex
+000007e0: 746c 6962 da08 7375 7070 7265 7373 da11  tlib..suppress..
+000007f0: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
+00000800: 7272 0200 0000 da07 6973 5f66 696c 6572  rr......is_filer
+00000810: 1700 0000 7204 0000 00da 0675 6e6c 696e  ....r......unlin
+00000820: 6b29 065a 126f 6c64 5f61 7267 756d 656e  k).Z.old_argumen
+00000830: 7473 5f66 696c 6572 0700 0000 da08 6469  ts_filer......di
+00000840: 725f 7061 7468 7213 0000 0072 1200 0000  r_pathr....r....
+00000850: 5a04 6e61 6461 7215 0000 0072 1500 0000  Z.nadar....r....
+00000860: 7216 0000 00da 076d 6967 7261 7465 5100  r......migrateQ.
+00000870: 0000 7316 0000 0004 070a 0108 020c 021c  ..s.............
+00000880: 011c ff08 040c 0110 0208 0204 0272 2100  .............r!.
+00000890: 0000 2902 7208 0000 004e 2911 720f 0000  ..).r....N).r...
+000008a0: 0072 1b00 0000 720b 0000 00da 026f 7372  .r....r......osr
+000008b0: 0200 0000 da07 7061 7468 6c69 6272 0300  ......pathlibr..
+000008c0: 0000 5a17 6d61 7074 6173 6b65 722e 7372  ..Z.maptasker.sr
+000008d0: 632e 6765 7470 7574 6172 6772 0400 0000  c.getputargr....
+000008e0: da13 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
+000008f0: 6572 726f 7272 0600 0000 da05 7475 706c  errorr......tupl
+00000900: 65da 0464 6963 7472 1700 0000 da03 7374  e..dictr......st
+00000910: 7272 0e00 0000 7221 0000 0072 1500 0000  rr....r!...r....
+00000920: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00000930: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
+00000940: 0000 0801 0801 080d 0c01 0c01 0c02 0c01  ................
+00000950: 1a06 1a29 0e0d                           ...)..
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/initparg.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/initparg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/kidapp.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/kidapp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/mapit.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/mapit.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 17 15:14:53 2023 UTC, .py size: 15473 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,328 +1,364 @@
-00000000: 6f0d 0d0a 0000 0000 6d62 3d64 713c 0000  o.......mb=dq<..
+00000000: 6f0d 0d0a 0000 0000 839d 4a64 2940 0000  o.........Jd)@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000e 0000 0040 0000 0073 3a01 0000 6400  .....@...s:...d.
+00000020: 000e 0000 0040 0000 0073 5a01 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
-00000050: 0100 6400 6403 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
-00000060: 0100 6400 6401 6c09 6d0a 0200 0100 6d0b  ..d.d.l.m.....m.
-00000070: 5a0c 0100 6400 6401 6c0d 6d0a 0200 0100  Z...d.d.l.m.....
-00000080: 6d0e 5a0f 0100 6400 6401 6c10 6d0a 0200  m.Z...d.d.l.m...
-00000090: 0100 6d11 5a11 0100 6400 6401 6c12 6d0a  ..m.Z...d.d.l.m.
-000000a0: 0200 0100 6d13 5a14 0100 6400 6404 6c15  ....m.Z...d.d.l.
-000000b0: 6d16 5a16 0100 6400 6405 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
-000000c0: 0100 6400 6406 6c19 6d1a 5a1a 0100 6407  ..d.d.l.m.Z...d.
-000000d0: 6503 6a1b 6a1c 6408 6503 6a1b 6a1c 6409  e.j.j.d.e.j.j.d.
-000000e0: 6507 651d 1900 640a 6508 651d 6507 6503  e.e...d.e.e.e.e.
-000000f0: 6a1b 6a1c 1900 6602 1900 640b 6401 660a  j.j...f...d.d.f.
-00000100: 640c 640d 8404 5a1e 6409 6507 651d 1900  d.d...Z.d.e.e...
-00000110: 640e 651d 640f 651d 640b 6401 6608 6410  d.e.d.e.d.d.f.d.
-00000120: 6411 8404 5a1f 6412 651d 6413 651d 6407  d...Z.d.e.d.e.d.
-00000130: 6503 6a1b 6a1c 6408 6503 6a1b 6a1c 6409  e.j.j.d.e.j.j.d.
-00000140: 6520 640a 6521 640b 6401 660e 6414 6415  e d.e!d.d.f.d.d.
-00000150: 8404 5a22 0900 640b 6523 6602 6416 6417  ..Z"..d.e#f.d.d.
-00000160: 8404 5a24 6401 5300 2918 e900 0000 004e  ..Z$d.S.)......N
-00000170: 2901 da06 6765 7463 7764 2902 da04 4c69  )...getcwd)...Li
-00000180: 7374 da04 4469 6374 2901 da0f 6469 7370  st..Dict)...disp
-00000190: 6c61 795f 6361 7665 6174 7329 01da 0f67  lay_caveats)...g
-000001a0: 6574 5f70 7265 6665 7265 6e63 6573 2901  et_preferences).
-000001b0: da06 6c6f 6767 6572 da04 7472 6565 da04  ..logger..tree..
-000001c0: 726f 6f74 da0b 6f75 7470 7574 5f6c 6973  root..output_lis
-000001d0: 74da 1061 6c6c 5f74 6173 6b65 725f 6974  t..all_tasker_it
-000001e0: 656d 73da 0672 6574 7572 6e63 0400 0000  ems..returnc....
-000001f0: 0000 0000 0000 0000 0500 0000 0300 0000  ................
-00000200: 4300 0000 735a 0000 007c 00a0 00a1 0044  C...sZ...|.....D
-00000210: 005d 067d 047c 04a0 01a1 0001 0071 047c  .].}.|.......q.|
-00000220: 0364 0119 00a0 01a1 0001 007c 0364 0219  .d.........|.d..
-00000230: 00a0 01a1 0001 007c 0364 0319 00a0 01a1  .......|.d......
-00000240: 0001 007c 0364 0419 00a0 01a1 0001 007c  ...|.d.........|
-00000250: 01a0 01a1 0001 007c 02a0 01a1 0001 0064  .......|.......d
-00000260: 0553 0029 0661 1701 0000 0a20 2020 2043  .S.).a.....    C
-00000270: 6c65 616e 2075 7020 6f75 7220 6d65 6d6f  lean up our memo
-00000280: 7279 2068 6f67 730a 2020 2020 2020 2020  ry hogs.        
-00000290: 3a70 6172 616d 2074 7265 653a 2078 6d6c  :param tree: xml
-000002a0: 2074 7265 6520 746f 2065 6d70 7479 0a20   tree to empty. 
-000002b0: 2020 2020 2020 203a 7061 7261 6d20 726f         :param ro
-000002c0: 6f74 3a20 726f 6f74 2078 6d6c 2074 6861  ot: root xml tha
-000002d0: 7420 7761 7320 7061 7273 6564 2066 726f  t was parsed fro
-000002e0: 6d20 6261 636b 7570 2066 696c 650a 2020  m backup file.  
-000002f0: 2020 2020 2020 3a70 6172 616d 206f 7574        :param out
-00000300: 7075 745f 6c69 7374 3a20 6c69 7374 206f  put_list: list o
-00000310: 6620 6f75 7470 7574 206c 696e 6573 2074  f output lines t
-00000320: 6f20 636c 6561 720a 2020 2020 2020 2020  o clear.        
-00000330: 3a70 6172 616d 2061 6c6c 5f74 6173 6b65  :param all_taske
-00000340: 725f 6974 656d 733a 2041 6c6c 2050 726f  r_items: All Pro
-00000350: 6a65 6374 732f 5072 6f66 696c 6573 2f54  jects/Profiles/T
-00000360: 6173 6b73 2f53 6365 6e65 730a 2020 2020  asks/Scenes.    
-00000370: 2020 2020 3a72 6574 7572 6e3a 0a20 2020      :return:.   
-00000380: 205a 0c61 6c6c 5f70 726f 6a65 6374 735a   Z.all_projectsZ
-00000390: 0c61 6c6c 5f70 726f 6669 6c65 73da 0961  .all_profiles..a
-000003a0: 6c6c 5f74 6173 6b73 5a0a 616c 6c5f 7363  ll_tasksZ.all_sc
-000003b0: 656e 6573 4e29 02da 0469 7465 72da 0563  enesN)...iter..c
-000003c0: 6c65 6172 2905 7208 0000 0072 0900 0000  lear).r....r....
-000003d0: 720a 0000 0072 0b00 0000 da04 656c 656d  r....r......elem
-000003e0: a900 7211 0000 00fa 742f 5573 6572 732f  ..r.....t/Users/
-000003f0: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
-00000400: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
-00000410: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
-00000420: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
-00000430: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
-00000440: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
-00000450: 2f73 7263 2f6d 6170 6974 2e70 79da 0f63  /src/mapit.py..c
-00000460: 6c65 616e 5f75 705f 6d65 6d6f 7279 3800  lean_up_memory8.
-00000470: 0000 7312 0000 000c 0e0a 010c 010c 010c  ..s.............
-00000480: 010c 0108 0108 0104 0172 1300 0000 da0d  .........r......
-00000490: 6d79 5f6f 7574 7075 745f 6469 72da 0c6d  my_output_dir..m
-000004a0: 795f 6669 6c65 5f6e 616d 6563 0300 0000  y_file_namec....
-000004b0: 0000 0000 0000 0000 0a00 0000 0800 0000  ................
-000004c0: 4300 0000 73de 0000 0074 00a0 0164 017c  C...s....t...d.|
-000004d0: 019b 009d 02a1 0101 0074 027c 017c 0217  .........t.|.|..
-000004e0: 0064 0283 028f 517d 037c 0044 005d 467d  .d....Q}.|.D.]F}
-000004f0: 047c 04a0 0364 03a1 017d 057c 0564 046b  .|...d...}.|.d.k
-00000500: 0372 457c 047c 0564 0517 0064 0685 0219  .rE|.|.d...d....
-00000510: 00a0 0464 07a1 017d 067c 0664 0819 007d  ...d...}.|.d...}
-00000520: 077c 0464 067c 0585 0219 007c 0717 0064  .|.d.|.....|...d
-00000530: 0917 007c 047c 0564 0517 0074 057c 0783  ...|.|.d...t.|..
-00000540: 0117 0064 0685 0219 0017 007d 087c 087d  ...d.......}.|.}
-00000550: 096e 027c 047d 097c 09a0 0664 0a64 0ba1  .n.|.}.|...d.d..
-00000560: 027d 097c 09a0 0664 0c64 0da1 027d 097c  .}.|...d.d...}.|
-00000570: 03a0 077c 09a1 0101 0071 1257 0064 0604  ...|.....q.W.d..
-00000580: 0004 0083 0301 006e 0831 0073 6377 0101  .......n.1.scw..
-00000590: 0001 0001 0059 0001 0074 00a0 0164 0ea1  .....Y...t...d..
-000005a0: 0101 0064 0653 0029 0f61 0c01 0000 0a20  ...d.S.).a..... 
-000005b0: 2020 2077 7269 7465 5f6f 7574 5f74 6865     write_out_the
-000005c0: 5f66 696c 653a 2077 6520 6861 7665 2061  _file: we have a
-000005d0: 206c 6973 7420 6f66 206f 7574 7075 7420   list of output 
-000005e0: 6c69 6e65 732e 2020 5772 6974 6520 7468  lines.  Write th
-000005f0: 656d 206f 7574 2e0a 2020 2020 2020 2020  em out..        
-00000600: 3a70 6172 616d 206f 7574 7075 745f 6c69  :param output_li
-00000610: 7374 3a20 6c69 7374 206f 6620 616c 6c20  st: list of all 
-00000620: 6f75 7470 7574 206c 696e 6573 2067 656e  output lines gen
-00000630: 6572 6174 6564 0a20 2020 2020 2020 203a  erated.        :
-00000640: 7061 7261 6d20 6d79 5f6f 7574 7075 745f  param my_output_
-00000650: 6469 723a 2064 6972 6563 746f 7279 2074  dir: directory t
-00000660: 6f20 6f75 7470 7574 2074 6f0a 2020 2020  o output to.    
-00000670: 2020 2020 3a70 6172 616d 206d 795f 6669      :param my_fi
-00000680: 6c65 5f6e 616d 653a 206e 616d 6520 6f66  le_name: name of
-00000690: 2066 696c 6520 746f 2075 7365 0a20 2020   file to use.   
-000006a0: 2020 2020 203a 7265 7475 726e 3a20 6e6f       :return: no
-000006b0: 7468 696e 670a 2020 2020 7a27 4675 6e63  thing.    z'Func
-000006c0: 7469 6f6e 2045 6e74 7279 3a20 7772 6974  tion Entry: writ
-000006d0: 655f 6f75 745f 7468 655f 6669 6c65 2064  e_out_the_file d
-000006e0: 6972 3ada 0177 7a08 4163 7469 6f6e 3a20  ir:..wz.Action: 
-000006f0: e9ff ffff ffe9 0800 0000 4efa 0120 7201  ..........N.. r.
-00000700: 0000 00fa 013a 7a0e 3c2f 7370 616e 3e3c  .....:z.</span><
-00000710: 2f73 7061 6e3e 7a07 3c2f 7370 616e 3e7a  /span>z.</span>z
-00000720: 083c 2f70 3e3c 2f70 3e7a 043c 2f70 3e7a  .</p></p>z.</p>z
-00000730: 2146 756e 6374 696f 6e20 4578 6974 3a20  !Function Exit: 
-00000740: 7772 6974 655f 6f75 745f 7468 655f 6669  write_out_the_fi
-00000750: 6c65 2908 7207 0000 00da 0469 6e66 6fda  le).r......info.
-00000760: 046f 7065 6eda 0466 696e 64da 0573 706c  .open..find..spl
-00000770: 6974 da03 6c65 6eda 0772 6570 6c61 6365  it..len..replace
-00000780: da05 7772 6974 6529 0a72 0a00 0000 7214  ..write).r....r.
-00000790: 0000 0072 1500 0000 5a08 6f75 745f 6669  ...r....Z.out_fi
-000007a0: 6c65 da04 6974 656d 5a0f 6163 7469 6f6e  le..itemZ.action
-000007b0: 5f70 6f73 6974 696f 6e5a 1261 6374 696f  _positionZ.actio
-000007c0: 6e5f 6e75 6d62 6572 5f6c 6973 745a 0d61  n_number_listZ.a
-000007d0: 6374 696f 6e5f 6e75 6d62 6572 5a04 7465  ction_numberZ.te
-000007e0: 6d70 5a0b 6f75 7470 7574 5f6c 696e 6572  mpZ.output_liner
-000007f0: 1100 0000 7211 0000 0072 1200 0000 da12  ....r....r......
-00000800: 7772 6974 655f 6f75 745f 7468 655f 6669  write_out_the_fi
-00000810: 6c65 5400 0000 7330 0000 0010 0a10 0108  leT...s0........
-00000820: 010a 0208 0116 0108 010a 0202 0102 ff02  ................
-00000830: 0202 fe16 0302 fd02 ff06 0604 020c 010c  ................
-00000840: 010c 0102 ef1c ff0a 1304 0172 2300 0000  ...........r#...
-00000850: da04 6e61 6d65 da14 7072 6f66 696c 655f  ..name..profile_
-00000860: 6f72 5f74 6173 6b5f 6e61 6d65 6306 0000  or_task_namec...
-00000870: 0000 0000 0000 0000 0007 0000 0005 0000  ................
-00000880: 0043 0000 0073 4600 0000 7c04 a000 a100  .C...sF...|.....
-00000890: 0100 7c00 9b00 6401 7c01 9b00 6402 9d04  ..|...d.|...d...
-000008a0: 7d06 7401 7c06 8301 0100 7402 a003 7c06  }.t.|.....t...|.
-000008b0: a101 0100 7404 7c02 7c03 7c04 7c05 8304  ....t.|.|.|.|...
-000008c0: 0100 7405 a006 6403 a101 0100 6404 5300  ..t...d.....d.S.
-000008d0: 2905 61f6 0100 000a 2020 2020 436c 6561  ).a.....    Clea
-000008e0: 6e75 7020 6d65 6d6f 7279 2061 6e64 206c  nup memory and l
-000008f0: 6574 2075 7365 7220 6b6e 6f77 2074 6865  et user know the
-00000900: 7265 2077 6173 206e 6f20 6d61 7463 6820  re was no match 
-00000910: 666f 756e 6420 666f 7220 5461 736b 2f50  found for Task/P
-00000920: 726f 6669 6c65 0a20 2020 2020 2020 203a  rofile.        :
-00000930: 7061 7261 6d20 6e61 6d65 3a20 7468 6520  param name: the 
-00000940: 6e61 6d65 2074 6f20 6164 6420 746f 2074  name to add to t
-00000950: 6865 206c 6f67 2f70 7269 6e74 206f 7574  he log/print out
-00000960: 7075 740a 2020 2020 2020 2020 3a70 6172  put.        :par
-00000970: 616d 2070 726f 6669 6c65 5f6f 725f 7461  am profile_or_ta
-00000980: 736b 5f6e 616d 653a 206e 616d 6520 6f66  sk_name: name of
-00000990: 2074 6865 2050 726f 6669 6c65 206f 7220   the Profile or 
-000009a0: 5461 736b 2074 6f20 636c 6561 6e0a 2020  Task to clean.  
-000009b0: 2020 2020 2020 3a70 6172 616d 2074 7265        :param tre
-000009c0: 653a 2078 6d6c 2074 7265 6520 746f 2063  e: xml tree to c
-000009d0: 6c65 6172 0a20 2020 2020 2020 203a 7061  lear.        :pa
-000009e0: 7261 6d20 726f 6f74 3a20 726f 6f74 206f  ram root: root o
-000009f0: 6620 786d 6c20 7061 7273 6564 2066 726f  f xml parsed fro
-00000a00: 6d20 6669 6c65 2074 6f20 636c 6561 720a  m file to clear.
-00000a10: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
-00000a20: 7574 7075 745f 6c69 7374 3a20 6c69 7374  utput_list: list
-00000a30: 206f 6620 6f75 7470 7574 206c 696e 6573   of output lines
-00000a40: 2074 6f20 656d 7074 790a 2020 2020 2020   to empty.      
-00000a50: 2020 3a70 6172 616d 2061 6c6c 5f74 6173    :param all_tas
-00000a60: 6b65 725f 6974 656d 733a 2061 6c6c 2054  ker_items: all T
-00000a70: 6173 6b65 7220 5072 6f6a 6563 7473 2f50  asker Projects/P
-00000a80: 726f 6669 6c65 732f 5461 736b 732f 5363  rofiles/Tasks/Sc
-00000a90: 656e 6573 2074 6f20 636c 6561 720a 2020  enes to clear.  
-00000aa0: 2020 2020 2020 3a72 7479 7065 3a20 636f        :rtype: co
-00000ab0: 6c6f 7273 2c20 7275 6e74 696d 6520 6172  lors, runtime ar
-00000ac0: 6775 6d65 6e74 732c 0a20 2020 2072 1900  guments,.    r..
-00000ad0: 0000 7a0c 206e 6f74 2066 6f75 6e64 2121  ..z. not found!!
-00000ae0: e905 0000 004e 2907 720f 0000 00da 0570  .....N).r......p
-00000af0: 7269 6e74 7207 0000 00da 0564 6562 7567  rintr......debug
-00000b00: 7213 0000 00da 0373 7973 da04 6578 6974  r......sys..exit
-00000b10: 2907 7224 0000 0072 2500 0000 7208 0000  ).r$...r%...r...
-00000b20: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000b30: da0d 6572 726f 725f 6d65 7373 6167 6572  ..error_messager
-00000b40: 1100 0000 7211 0000 0072 1200 0000 da11  ....r....r......
-00000b50: 636c 6561 6e5f 7570 5f61 6e64 5f65 7869  clean_up_and_exi
-00000b60: 7479 0000 0073 0c00 0000 0813 1001 0801  ty...s..........
-00000b70: 0a01 0e01 0e01 722c 0000 0063 0000 0000  ......r,...c....
-00000b80: 0000 0000 0000 0000 1000 0000 0a00 0000  ................
-00000b90: 4300 0000 7328 0200 0067 0067 0067 0067  C...s(...g.g.g.g
-00000ba0: 0066 045c 047d 007d 017d 027d 0374 00a0  .f.\.}.}.}.}.t..
-00000bb0: 017c 01a1 015c 097d 047d 057d 067d 077d  .|...\.}.}.}.}.}
-00000bc0: 017d 087d 097d 0a7d 0b7c 0564 0119 0072  .}.}.}.}.|.d...r
-00000bd0: 2374 027c 017c 057c 047c 0b83 0401 0074  #t.|.|.|.|.....t
-00000be0: 03a0 047c 017c 007c 027c 057c 067c 077c  ...|.|.|.|.|.|.|
-00000bf0: 047c 0ba1 087d 007c 0564 0219 0072 427c  .|...}.|.d...rB|
-00000c00: 0664 0319 0073 4274 0564 047c 0564 0219  .d...sBt.d.|.d..
-00000c10: 007c 087c 097c 017c 0b83 0601 007c 0564  .|.|.|.|.....|.d
-00000c20: 0519 0072 557c 0664 0619 0073 5574 0564  ...rU|.d...sUt.d
-00000c30: 077c 0564 0519 007c 087c 097c 017c 0b83  .|.d...|.|.|.|..
-00000c40: 0601 007c 0564 0819 0073 777c 0564 0219  ...|.d...sw|.d..
-00000c50: 0073 777c 0564 0519 0073 7774 06a0 077c  .sw|.d...swt...|
-00000c60: 017c 037c 007c 057c 067c 077c 047c 0ba1  .|.|.|.|.|.|.|..
-00000c70: 0801 0074 06a0 087c 017c 037c 027c 067c  ...t...|.|.|.|.|
-00000c80: 047c 05a1 0601 007c 0564 0819 0072 9a7c  .|.....|.d...r.|
-00000c90: 0664 0919 0073 9a7c 0564 0519 0072 877c  .d...s.|.d...r.|
-00000ca0: 0664 0619 0072 9a7c 0564 0219 0072 8f7c  .d...r.|.d...r.|
-00000cb0: 0664 0319 0072 9a74 0564 0a7c 0564 0819  .d...r.t.d.|.d..
-00000cc0: 007c 087c 097c 017c 0b83 0601 0074 097c  .|.|.|.|.....t.|
-00000cd0: 017c 057c 0483 0301 0064 0b7d 0c74 0aa0  .|.|.....d.}.t..
-00000ce0: 0b7c 047c 057c 0164 0c7c 0ca1 0501 0074  .|.|.|.d.|.....t
-00000cf0: 0c83 007d 0d74 0da0 0e64 0d7c 0d9b 009d  ...}.t...d.|....
-00000d00: 02a1 0101 007c 0d64 0075 0072 d164 0e7d  .....|.d.u.r.d.}
-00000d10: 0c74 0da0 0e7c 0ca1 0101 0074 0f7c 0c83  .t...|.....t.|..
-00000d20: 0101 0074 107c 087c 097c 017c 0b83 0401  ...t.|.|.|.|....
-00000d30: 0074 11a0 1264 0fa1 0101 0064 107d 0e74  .t...d.....d.}.t
-00000d40: 137c 017c 0d7c 0e83 0301 0074 107c 087c  .|.|.|.....t.|.|
-00000d50: 097c 017c 0b83 0401 0074 0da0 0e64 11a1  .|.|.....t...d..
-00000d60: 0101 0064 0c7d 0f7a 0e74 146a 1564 127c  ...d.}.z.t.j.d.|
-00000d70: 0d9b 007c 0e9b 009d 0364 0f64 138d 0201  ...|.....d.d....
-00000d80: 0057 006e 1804 0074 146a 1690 0179 0d01  .W.n...t.j...y..
-00000d90: 0001 0001 0064 147d 0c74 0f7c 0c83 0101  .....d.}.t.|....
-00000da0: 0074 0da0 0e7c 0ca1 0101 0064 157d 0f59  .t...|.....d.}.Y
-00000db0: 006e 0177 0074 0f64 1683 0101 007c 0f53  .n.w.t.d.....|.S
-00000dc0: 0029 174e 5a13 6469 7370 6c61 795f 7072  .).NZ.display_pr
-00000dd0: 6566 6572 656e 6365 735a 1373 696e 676c  eferencesZ.singl
-00000de0: 655f 7072 6f6a 6563 745f 6e61 6d65 5a14  e_project_nameZ.
-00000df0: 7369 6e67 6c65 5f70 726f 6a65 6374 5f66  single_project_f
-00000e00: 6f75 6e64 5a07 5072 6f6a 6563 745a 1373  oundZ.ProjectZ.s
-00000e10: 696e 676c 655f 7072 6f66 696c 655f 6e61  ingle_profile_na
-00000e20: 6d65 5a14 7369 6e67 6c65 5f70 726f 6669  meZ.single_profi
-00000e30: 6c65 5f66 6f75 6e64 5a07 5072 6f66 696c  le_foundZ.Profil
-00000e40: 655a 1073 696e 676c 655f 7461 736b 5f6e  eZ.single_task_n
-00000e50: 616d 655a 1173 696e 676c 655f 7461 736b  ameZ.single_task
-00000e60: 5f66 6f75 6e64 da04 5461 736b 7a0f 3c2f  _found..Taskz.</
-00000e70: 626f 6479 3e0a 3c2f 6874 6d6c 3e72 0100  body>.</html>r..
-00000e80: 0000 7a11 6f75 7470 7574 2064 6972 6563  ..z.output direc
-00000e90: 746f 7279 3a7a 3c4d 6170 5461 736b 6572  tory:z<MapTasker
-00000ea0: 2063 616e 6365 6c6c 6564 2e20 2041 6e20   cancelled.  An 
-00000eb0: 6572 726f 7220 6f63 6375 7272 6564 2e20  error occurred. 
-00000ec0: 2050 726f 6772 616d 2063 616e 6365 6c6c   Program cancell
-00000ed0: 6564 2ee9 0200 0000 7a0f 2f4d 6170 5461  ed......z./MapTa
-00000ee0: 736b 6572 2e68 746d 6c7a 204d 6170 5461  sker.htmlz MapTa
-00000ef0: 736b 6572 2070 726f 6772 616d 2065 6e64  sker program end
-00000f00: 6564 206e 6f72 6d61 6c6c 797a 0766 696c  ed normallyz.fil
-00000f10: 653a 2f2f 2901 da03 6e65 777a 4745 7272  e://)...newzGErr
-00000f20: 6f72 3a20 4661 696c 6564 2074 6f20 6f70  or: Failed to op
-00000f30: 656e 206f 7574 7075 7420 696e 2062 726f  en output in bro
-00000f40: 7773 6572 3a20 796f 7572 2062 726f 7773  wser: your brows
-00000f50: 6572 2069 7320 6e6f 7420 7375 7070 6f72  er is not suppor
-00000f60: 7465 642e e901 0000 007a 4259 6f75 2063  ted......zBYou c
-00000f70: 616e 2066 696e 6420 274d 6170 5461 736b  an find 'MapTask
-00000f80: 6572 2e68 746d 6c27 2069 6e20 7468 6520  er.html' in the 
-00000f90: 6375 7272 656e 7420 666f 6c64 6572 2e20  current folder. 
-00000fa0: 2050 726f 6772 616d 2065 6e64 2e29 17da   Program end.)..
-00000fb0: 0a69 6e69 7469 616c 697a 655a 0873 7461  .initializeZ.sta
-00000fc0: 7274 5f75 7072 0600 0000 da08 7072 6f6a  rt_upr......proj
-00000fd0: 6563 7473 5a23 7072 6f63 6573 735f 7072  ectsZ#process_pr
-00000fe0: 6f6a 6563 7473 5f61 6e64 5f74 6865 6972  ojects_and_their
-00000ff0: 5f70 726f 6669 6c65 7372 2c00 0000 da0d  _profilesr,.....
-00001000: 7370 6563 6961 6c5f 7461 736b 735a 2370  special_tasksZ#p
-00001010: 726f 6365 7373 5f74 6173 6b73 5f6e 6f74  rocess_tasks_not
-00001020: 5f63 616c 6c65 645f 6279 5f70 726f 6669  _called_by_profi
-00001030: 6c65 5a22 7072 6f63 6573 735f 6d69 7373  leZ"process_miss
-00001040: 696e 675f 7461 736b 735f 616e 645f 7072  ing_tasks_and_pr
-00001050: 6f66 696c 6573 7205 0000 00da 0c62 7569  ofilesr......bui
-00001060: 6c64 5f6f 7574 7075 745a 096d 795f 6f75  ld_outputZ.my_ou
-00001070: 7470 7574 7202 0000 0072 0700 0000 7228  tputr....r....r(
-00001080: 0000 0072 2700 0000 7213 0000 0072 2900  ...r'...r....r).
-00001090: 0000 722a 0000 0072 2300 0000 da0a 7765  ..r*...r#.....we
-000010a0: 6262 726f 7773 6572 721c 0000 00da 0545  bbrowserr......E
-000010b0: 7272 6f72 2910 5a0b 666f 756e 645f 7461  rror).Z.found_ta
-000010c0: 736b 7372 0a00 0000 5a19 7072 6f6a 6563  sksr....Z.projec
-000010d0: 7473 5f77 6974 686f 7574 5f70 726f 6669  ts_without_profi
-000010e0: 6c65 735a 1670 726f 6a65 6374 735f 7769  lesZ.projects_wi
-000010f0: 7468 5f6e 6f5f 7461 736b 735a 0863 6f6c  th_no_tasksZ.col
-00001100: 6f72 6d61 705a 0c70 726f 6772 616d 5f61  ormapZ.program_a
-00001110: 7267 735a 0b66 6f75 6e64 5f69 7465 6d73  rgsZ.found_items
-00001120: da07 6865 6164 696e 6772 0800 0000 7209  ..headingr....r.
-00001130: 0000 00da 0866 696c 656e 616d 6572 0b00  .....filenamer..
-00001140: 0000 5a09 6572 726f 725f 6d73 6772 1400  ..Z.error_msgr..
-00001150: 0000 7215 0000 005a 056d 795f 7263 7211  ..r....Z.my_rcr.
-00001160: 0000 0072 1100 0000 7212 0000 00da 096d  ...r....r......m
-00001170: 6170 6974 5f61 6c6c c400 0000 73f4 0000  apit_all....s...
-00001180: 0002 0302 0102 0102 010c fc08 1202 f602  ................
-00001190: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-000011a0: 0108 0c02 0102 0102 0102 0102 0104 fc04  ................
-000011b0: 0a02 0102 0102 0102 0102 0102 0102 0102  ................
-000011c0: 0104 f810 0c02 0102 0106 0102 0102 0102  ................
-000011d0: 0102 0104 fa10 0902 0102 0106 0102 0102  ................
-000011e0: 0102 0102 0104 fa06 0d02 ff06 0202 fe06  ................
-000011f0: 0302 fd04 0502 0102 0102 0102 0102 0102  ................
-00001200: 0102 0102 0104 f804 0e02 0102 0102 0102  ................
-00001210: 0102 0102 0104 fa06 0b02 ff06 0202 fe06  ................
-00001220: 0402 fc06 0502 fb06 0802 f806 0902 f702  ................
-00001230: 0c02 0106 0102 0102 0102 0102 0104 fa0c  ................
-00001240: 0d04 0312 0106 0410 0108 0104 010a 0108  ................
-00001250: 010e 010a 0104 020c 020e 030a 0304 0102  ................
-00001260: 011c 0110 0102 0202 ff08 030a 0108 0102  ................
-00001270: fa08 0704 0172 3900 0000 2925 7229 0000  .....r9...)%r)..
-00001280: 0072 3500 0000 5a16 6465 6675 7365 6478  .r5...Z.defusedx
-00001290: 6d6c 2e45 6c65 6d65 6e74 5472 6565 5a0a  ml.ElementTreeZ.
-000012a0: 6465 6675 7365 6478 6d6c da02 6f73 7202  defusedxml..osr.
-000012b0: 0000 00da 0674 7970 696e 6772 0300 0000  .....typingr....
-000012c0: 7204 0000 005a 156d 6170 7461 736b 6572  r....Z.maptasker
-000012d0: 2e73 7263 2e6f 7574 7075 746c da03 7372  .src.outputl..sr
-000012e0: 635a 076f 7574 7075 746c 7234 0000 005a  cZ.outputlr4...Z
-000012f0: 166d 6170 7461 736b 6572 2e73 7263 2e70  .maptasker.src.p
-00001300: 726f 6769 6e69 745a 0870 726f 6769 6e69  roginitZ.progini
-00001310: 7472 3100 0000 5a16 6d61 7074 6173 6b65  tr1...Z.maptaske
-00001320: 722e 7372 632e 7072 6f6a 6563 7473 7232  r.src.projectsr2
-00001330: 0000 005a 166d 6170 7461 736b 6572 2e73  ...Z.maptasker.s
-00001340: 7263 2e74 6173 6b75 6e69 715a 0874 6173  rc.taskuniqZ.tas
-00001350: 6b75 6e69 7172 3300 0000 5a15 6d61 7074  kuniqr3...Z.mapt
-00001360: 6173 6b65 722e 7372 632e 6361 7665 6174  asker.src.caveat
-00001370: 7372 0500 0000 5a15 6d61 7074 6173 6b65  sr....Z.maptaske
-00001380: 722e 7372 632e 7072 6566 6572 7372 0600  r.src.prefersr..
-00001390: 0000 5a16 6d61 7074 6173 6b65 722e 7372  ..Z.maptasker.sr
-000013a0: 632e 7379 7363 6f6e 7374 7207 0000 005a  c.sysconstr....Z
-000013b0: 0b45 6c65 6d65 6e74 5472 6565 5a03 584d  .ElementTreeZ.XM
-000013c0: 4cda 0373 7472 7213 0000 0072 2300 0000  L..strr....r#...
-000013d0: da04 6c69 7374 da04 6469 6374 722c 0000  ..list..dictr,..
-000013e0: 00da 0369 6e74 7239 0000 0072 1100 0000  ...intr9...r....
-000013f0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00001400: 083c 6d6f 6475 6c65 3e01 0000 0073 6200  .<module>....sb.
-00001410: 0000 0820 0801 0801 0c01 1001 1202 1201  ... ............
-00001420: 1201 1201 0c01 0c01 0c01 020b 0601 02ff  ................
-00001430: 0602 02fe 0603 02fd 1204 02fc 0205 0afb  ................
-00001440: 021c 0601 02ff 0201 02ff 0201 02ff 0202  ................
-00001450: 0afe 0225 0201 02ff 0202 02fe 0603 02fd  ...%............
-00001460: 0604 02fc 0205 02fb 0206 02fa 0207 0af9  ................
-00001470: 0220 122b                                . .+
+00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
+00000050: 6402 6c05 6d06 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6400 6401 6c09 6d0a 0200  m.Z...d.d.l.m...
+00000070: 0100 6d0b 5a0c 0100 6400 6401 6c0d 6d0a  ..m.Z...d.d.l.m.
+00000080: 0200 0100 6d0e 5a0f 0100 6400 6401 6c10  ....m.Z...d.d.l.
+00000090: 6d0a 0200 0100 6d11 5a11 0100 6400 6401  m.....m.Z...d.d.
+000000a0: 6c12 6d0a 0200 0100 6d13 5a14 0100 6400  l.m.....m.Z...d.
+000000b0: 6404 6c15 6d16 5a16 0100 6400 6405 6c17  d.l.m.Z...d.d.l.
+000000c0: 6d18 5a18 0100 6400 6406 6c19 6d1a 5a1a  m.Z...d.d.l.m.Z.
+000000d0: 0100 6400 6407 6c1b 6d1c 5a1c 0100 6400  ..d.d.l.m.Z...d.
+000000e0: 6408 6c1b 6d1d 5a1d 0100 6409 6504 6a1e  d.l.m.Z...d.e.j.
+000000f0: 6a1f 640a 6504 6a1e 6a1f 640b 6508 6520  j.d.e.j.j.d.e.e 
+00000100: 1900 640c 6521 6520 6508 6504 6a1e 6a1f  ..d.e!e e.e.j.j.
+00000110: 1900 6602 1900 640d 6401 660a 640e 640f  ..f...d.d.f.d.d.
+00000120: 8404 5a22 640b 6508 6520 1900 6410 6520  ..Z"d.e.e ..d.e 
+00000130: 6411 6520 640d 6401 6608 6412 6413 8404  d.e d.d.f.d.d...
+00000140: 5a23 6414 6520 6415 6520 6409 6504 6a1e  Z#d.e d.e d.e.j.
+00000150: 6a1f 640a 6504 6a1e 6a1f 640b 6524 640c  j.d.e.j.j.d.e$d.
+00000160: 6521 640d 6401 660e 6416 6417 8404 5a25  e!d.d.f.d.d...Z%
+00000170: 0900 6418 6520 640d 6526 6604 6419 641a  ..d.e d.e&f.d.d.
+00000180: 8404 5a27 6401 5300 291b e900 0000 004e  ..Z'd.S.)......N
+00000190: 2901 da06 6765 7463 7764 2901 da04 4c69  )...getcwd)...Li
+000001a0: 7374 2901 da0f 6469 7370 6c61 795f 6361  st)...display_ca
+000001b0: 7665 6174 7329 01da 0f67 6574 5f70 7265  veats)...get_pre
+000001c0: 6665 7265 6e63 6573 2901 da0d 6572 726f  ferences)...erro
+000001d0: 725f 6861 6e64 6c65 7229 01da 066c 6f67  r_handler)...log
+000001e0: 6765 7229 01da 0964 6562 7567 5f6f 7574  ger)...debug_out
+000001f0: da04 7472 6565 da04 726f 6f74 da0b 6f75  ..tree..root..ou
+00000200: 7470 7574 5f6c 6973 74da 1061 6c6c 5f74  tput_list..all_t
+00000210: 6173 6b65 725f 6974 656d 73da 0672 6574  asker_items..ret
+00000220: 7572 6e63 0400 0000 0000 0000 0000 0000  urnc............
+00000230: 0500 0000 0300 0000 4300 0000 735a 0000  ........C...sZ..
+00000240: 007c 00a0 00a1 0044 005d 067d 047c 04a0  .|.....D.].}.|..
+00000250: 01a1 0001 0071 047c 0364 0119 00a0 01a1  .....q.|.d......
+00000260: 0001 007c 0364 0219 00a0 01a1 0001 007c  ...|.d.........|
+00000270: 0364 0319 00a0 01a1 0001 007c 0364 0419  .d.........|.d..
+00000280: 00a0 01a1 0001 007c 01a0 01a1 0001 007c  .......|.......|
+00000290: 02a0 01a1 0001 0064 0553 0029 0661 1701  .......d.S.).a..
+000002a0: 0000 0a20 2020 2043 6c65 616e 2075 7020  ...    Clean up 
+000002b0: 6f75 7220 6d65 6d6f 7279 2068 6f67 730a  our memory hogs.
+000002c0: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
+000002d0: 7265 653a 2078 6d6c 2074 7265 6520 746f  ree: xml tree to
+000002e0: 2065 6d70 7479 0a20 2020 2020 2020 203a   empty.        :
+000002f0: 7061 7261 6d20 726f 6f74 3a20 726f 6f74  param root: root
+00000300: 2078 6d6c 2074 6861 7420 7761 7320 7061   xml that was pa
+00000310: 7273 6564 2066 726f 6d20 6261 636b 7570  rsed from backup
+00000320: 2066 696c 650a 2020 2020 2020 2020 3a70   file.        :p
+00000330: 6172 616d 206f 7574 7075 745f 6c69 7374  aram output_list
+00000340: 3a20 6c69 7374 206f 6620 6f75 7470 7574  : list of output
+00000350: 206c 696e 6573 2074 6f20 636c 6561 720a   lines to clear.
+00000360: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
+00000370: 6c6c 5f74 6173 6b65 725f 6974 656d 733a  ll_tasker_items:
+00000380: 2041 6c6c 2050 726f 6a65 6374 732f 5072   All Projects/Pr
+00000390: 6f66 696c 6573 2f54 6173 6b73 2f53 6365  ofiles/Tasks/Sce
+000003a0: 6e65 730a 2020 2020 2020 2020 3a72 6574  nes.        :ret
+000003b0: 7572 6e3a 0a20 2020 205a 0c61 6c6c 5f70  urn:.    Z.all_p
+000003c0: 726f 6a65 6374 735a 0c61 6c6c 5f70 726f  rojectsZ.all_pro
+000003d0: 6669 6c65 73da 0961 6c6c 5f74 6173 6b73  files..all_tasks
+000003e0: 5a0a 616c 6c5f 7363 656e 6573 4e29 02da  Z.all_scenesN)..
+000003f0: 0469 7465 72da 0563 6c65 6172 2905 7209  .iter..clear).r.
+00000400: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000410: 0000 da04 656c 656d a900 7212 0000 00fa  ....elem..r.....
+00000420: 742f 5573 6572 732f 6d69 6b72 7562 696e  t/Users/mikrubin
+00000430: 2f4c 6962 7261 7279 2f43 6c6f 7564 5374  /Library/CloudSt
+00000440: 6f72 6167 652f 476f 6f67 6c65 4472 6976  orage/GoogleDriv
+00000450: 652d 6d69 6b72 7562 696e 4067 6d61 696c  e-mikrubin@gmail
+00000460: 2e63 6f6d 2f4d 7920 4472 6976 652f 5079  .com/My Drive/Py
+00000470: 7468 6f6e 2f6d 6170 7461 736b 6572 2f6d  thon/maptasker/m
+00000480: 6170 7461 736b 6572 2f73 7263 2f6d 6170  aptasker/src/map
+00000490: 6974 2e70 79da 0f63 6c65 616e 5f75 705f  it.py..clean_up_
+000004a0: 6d65 6d6f 7279 3b00 0000 7312 0000 000c  memory;...s.....
+000004b0: 0e0a 010c 010c 010c 010c 0108 0108 0104  ................
+000004c0: 0172 1400 0000 da0d 6d79 5f6f 7574 7075  .r......my_outpu
+000004d0: 745f 6469 72da 0c6d 795f 6669 6c65 5f6e  t_dir..my_file_n
+000004e0: 616d 6563 0300 0000 0000 0000 0000 0000  amec............
+000004f0: 0b00 0000 0800 0000 4300 0000 7364 0100  ........C...sd..
+00000500: 0074 00a0 0164 017c 019b 009d 02a1 0101  .t...d.|........
+00000510: 0074 027c 017c 0217 0064 0283 028f 947d  .t.|.|...d.....}
+00000520: 0374 037c 0083 0144 005d 875c 027d 047d  .t.|...D.].\.}.}
+00000530: 057c 05a0 04a1 0001 007c 0464 036b 0472  .|.......|.d.k.r
+00000540: 4d7c 0564 0464 0585 0219 0064 066b 0272  M|.d.d.....d.k.r
+00000550: 4d7c 007c 0464 0718 0019 0064 0464 0585  M|.|.d.....d.d..
+00000560: 0219 0064 066b 0272 4d7c 007c 0464 0818  ...d.k.rM|.|.d..
+00000570: 0019 0064 0464 0585 0219 0064 066b 0272  ...d.d.....d.k.r
+00000580: 4d7c 007c 0464 0717 0019 0064 0464 0985  M|.|.d.....d.d..
+00000590: 0219 0064 0a6b 0272 4d71 147c 05a0 0564  ...d.k.rMq.|...d
+000005a0: 0ba1 017d 067c 0664 0c6b 0372 7e7c 057c  ...}.|.d.k.r~|.|
+000005b0: 0664 0d17 0064 0485 0219 00a0 0664 0ea1  .d...d.......d..
+000005c0: 017d 077c 0764 0f19 007d 087c 0564 047c  .}.|.d...}.|.d.|
+000005d0: 0685 0219 007c 0817 0064 1017 007c 057c  .....|...d...|.|
+000005e0: 0664 0d17 0074 077c 0883 0117 0064 0485  .d...t.|.....d..
+000005f0: 0219 0017 007d 097c 097d 0a6e 027c 057d  .....}.|.}.n.|.}
+00000600: 0a7c 0aa0 0864 1164 12a1 027d 0a7c 0aa0  .|...d.d...}.|..
+00000610: 0864 1364 14a1 027d 0a7c 03a0 097c 0aa1  .d.d...}.|...|..
+00000620: 0101 0074 0a72 9b74 00a0 0b64 157c 0a9b  ...t.r.t...d.|..
+00000630: 009d 02a1 0101 0071 1457 0064 0404 0004  .......q.W.d....
+00000640: 0083 0301 006e 0831 0073 a677 0101 0001  .....n.1.s.w....
+00000650: 0001 0059 0001 0074 00a0 0164 16a1 0101  ...Y...t...d....
+00000660: 0064 0453 0029 1761 0c01 0000 0a20 2020  .d.S.).a.....   
+00000670: 2077 7269 7465 5f6f 7574 5f74 6865 5f66   write_out_the_f
+00000680: 696c 653a 2077 6520 6861 7665 2061 206c  ile: we have a l
+00000690: 6973 7420 6f66 206f 7574 7075 7420 6c69  ist of output li
+000006a0: 6e65 732e 2020 5772 6974 6520 7468 656d  nes.  Write them
+000006b0: 206f 7574 2e0a 2020 2020 2020 2020 3a70   out..        :p
+000006c0: 6172 616d 206f 7574 7075 745f 6c69 7374  aram output_list
+000006d0: 3a20 6c69 7374 206f 6620 616c 6c20 6f75  : list of all ou
+000006e0: 7470 7574 206c 696e 6573 2067 656e 6572  tput lines gener
+000006f0: 6174 6564 0a20 2020 2020 2020 203a 7061  ated.        :pa
+00000700: 7261 6d20 6d79 5f6f 7574 7075 745f 6469  ram my_output_di
+00000710: 723a 2064 6972 6563 746f 7279 2074 6f20  r: directory to 
+00000720: 6f75 7470 7574 2074 6f0a 2020 2020 2020  output to.      
+00000730: 2020 3a70 6172 616d 206d 795f 6669 6c65    :param my_file
+00000740: 5f6e 616d 653a 206e 616d 6520 6f66 2066  _name: name of f
+00000750: 696c 6520 746f 2075 7365 0a20 2020 2020  ile to use.     
+00000760: 2020 203a 7265 7475 726e 3a20 6e6f 7468     :return: noth
+00000770: 696e 670a 2020 2020 7a27 4675 6e63 7469  ing.    z'Functi
+00000780: 6f6e 2045 6e74 7279 3a20 7772 6974 655f  on Entry: write_
+00000790: 6f75 745f 7468 655f 6669 6c65 2064 6972  out_the_file dir
+000007a0: 3ada 0177 e903 0000 004e e905 0000 007a  :..w.....N.....z
+000007b0: 053c 2f75 6c3e e901 0000 00e9 0200 0000  .</ul>..........
+000007c0: e904 0000 007a 043c 6272 3e7a 0841 6374  .....z.<br>z.Act
+000007d0: 696f 6e3a 20e9 ffff ffff e908 0000 00fa  ion: ...........
+000007e0: 0120 7201 0000 00fa 013a 7a0e 3c2f 7370  . r......:z.</sp
+000007f0: 616e 3e3c 2f73 7061 6e3e 7a07 3c2f 7370  an></span>z.</sp
+00000800: 616e 3e7a 083c 2f70 3e3c 2f70 3e7a 043c  an>z.</p></p>z.<
+00000810: 2f70 3e7a 056b 616b 613a 7a21 4675 6e63  /p>z.kaka:z!Func
+00000820: 7469 6f6e 2045 7869 743a 2077 7269 7465  tion Exit: write
+00000830: 5f6f 7574 5f74 6865 5f66 696c 6529 0c72  _out_the_file).r
+00000840: 0700 0000 da04 696e 666f da04 6f70 656e  ......info..open
+00000850: da09 656e 756d 6572 6174 65da 0672 7374  ..enumerate..rst
+00000860: 7269 70da 0466 696e 64da 0573 706c 6974  rip..find..split
+00000870: da03 6c65 6eda 0772 6570 6c61 6365 da05  ..len..replace..
+00000880: 7772 6974 6572 0800 0000 da05 6465 6275  writer......debu
+00000890: 6729 0b72 0b00 0000 7215 0000 0072 1600  g).r....r....r..
+000008a0: 0000 5a08 6f75 745f 6669 6c65 5a03 6e75  ..Z.out_fileZ.nu
+000008b0: 6dda 0469 7465 6d5a 0f61 6374 696f 6e5f  m..itemZ.action_
+000008c0: 706f 7369 7469 6f6e 5a12 6163 7469 6f6e  positionZ.action
+000008d0: 5f6e 756d 6265 725f 6c69 7374 5a0d 6163  _number_listZ.ac
+000008e0: 7469 6f6e 5f6e 756d 6265 725a 0474 656d  tion_numberZ.tem
+000008f0: 705a 0b6f 7574 7075 745f 6c69 6e65 7212  pZ.output_liner.
+00000900: 0000 0072 1200 0000 7213 0000 00da 1277  ...r....r......w
+00000910: 7269 7465 5f6f 7574 5f74 6865 5f66 696c  rite_out_the_fil
+00000920: 6557 0000 0073 4400 0000 100a 1001 1001  eW...sD.........
+00000930: 0802 0802 1001 1802 1801 1801 0203 0a03  ................
+00000940: 0801 1601 0801 0a02 0201 02ff 0202 02fe  ................
+00000950: 1603 02fd 02ff 0606 0402 0c02 0c01 0a02  ................
+00000960: 0401 1001 0280 02de 1cff 0a24 0401 722c  ...........$..r,
+00000970: 0000 00da 046e 616d 65da 1470 726f 6669  .....name..profi
+00000980: 6c65 5f6f 725f 7461 736b 5f6e 616d 6563  le_or_task_namec
+00000990: 0600 0000 0000 0000 0000 0000 0600 0000  ................
+000009a0: 0500 0000 4300 0000 733a 0000 007c 04a0  ....C...s:...|..
+000009b0: 00a1 0001 0074 017c 009b 0064 017c 019b  .....t.|...d.|..
+000009c0: 0064 029d 0464 0383 0201 0074 027c 027c  .d...d.....t.|.|
+000009d0: 037c 047c 0583 0401 0074 03a0 0464 04a1  .|.|.....t...d..
+000009e0: 0101 0064 0553 0029 0661 f601 0000 0a20  ...d.S.).a..... 
+000009f0: 2020 2043 6c65 616e 7570 206d 656d 6f72     Cleanup memor
+00000a00: 7920 616e 6420 6c65 7420 7573 6572 206b  y and let user k
+00000a10: 6e6f 7720 7468 6572 6520 7761 7320 6e6f  now there was no
+00000a20: 206d 6174 6368 2066 6f75 6e64 2066 6f72   match found for
+00000a30: 2054 6173 6b2f 5072 6f66 696c 650a 2020   Task/Profile.  
+00000a40: 2020 2020 2020 3a70 6172 616d 206e 616d        :param nam
+00000a50: 653a 2074 6865 206e 616d 6520 746f 2061  e: the name to a
+00000a60: 6464 2074 6f20 7468 6520 6c6f 672f 7072  dd to the log/pr
+00000a70: 696e 7420 6f75 7470 7574 0a20 2020 2020  int output.     
+00000a80: 2020 203a 7061 7261 6d20 7072 6f66 696c     :param profil
+00000a90: 655f 6f72 5f74 6173 6b5f 6e61 6d65 3a20  e_or_task_name: 
+00000aa0: 6e61 6d65 206f 6620 7468 6520 5072 6f66  name of the Prof
+00000ab0: 696c 6520 6f72 2054 6173 6b20 746f 2063  ile or Task to c
+00000ac0: 6c65 616e 0a20 2020 2020 2020 203a 7061  lean.        :pa
+00000ad0: 7261 6d20 7472 6565 3a20 786d 6c20 7472  ram tree: xml tr
+00000ae0: 6565 2074 6f20 636c 6561 720a 2020 2020  ee to clear.    
+00000af0: 2020 2020 3a70 6172 616d 2072 6f6f 743a      :param root:
+00000b00: 2072 6f6f 7420 6f66 2078 6d6c 2070 6172   root of xml par
+00000b10: 7365 6420 6672 6f6d 2066 696c 6520 746f  sed from file to
+00000b20: 2063 6c65 6172 0a20 2020 2020 2020 203a   clear.        :
+00000b30: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
+00000b40: 743a 206c 6973 7420 6f66 206f 7574 7075  t: list of outpu
+00000b50: 7420 6c69 6e65 7320 746f 2065 6d70 7479  t lines to empty
+00000b60: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000b70: 616c 6c5f 7461 736b 6572 5f69 7465 6d73  all_tasker_items
+00000b80: 3a20 616c 6c20 5461 736b 6572 2050 726f  : all Tasker Pro
+00000b90: 6a65 6374 732f 5072 6f66 696c 6573 2f54  jects/Profiles/T
+00000ba0: 6173 6b73 2f53 6365 6e65 7320 746f 2063  asks/Scenes to c
+00000bb0: 6c65 6172 0a20 2020 2020 2020 203a 7274  lear.        :rt
+00000bc0: 7970 653a 2063 6f6c 6f72 732c 2072 756e  ype: colors, run
+00000bd0: 7469 6d65 2061 7267 756d 656e 7473 2c0a  time arguments,.
+00000be0: 2020 2020 721f 0000 007a 0c20 6e6f 7420      r....z. not 
+00000bf0: 666f 756e 6421 2172 0100 0000 7219 0000  found!!r....r...
+00000c00: 004e 2905 7210 0000 0072 0600 0000 7214  .N).r....r....r.
+00000c10: 0000 00da 0373 7973 da04 6578 6974 2906  .....sys..exit).
+00000c20: 722d 0000 0072 2e00 0000 7209 0000 0072  r-...r....r....r
+00000c30: 0a00 0000 720b 0000 0072 0c00 0000 7212  ....r....r....r.
+00000c40: 0000 0072 1200 0000 7213 0000 00da 1163  ...r....r......c
+00000c50: 6c65 616e 5f75 705f 616e 645f 6578 6974  lean_up_and_exit
+00000c60: 8d00 0000 7308 0000 0008 1316 010e 010e  ....s...........
+00000c70: 0172 3100 0000 da0b 6669 6c65 5f74 6f5f  .r1.....file_to_
+00000c80: 6765 7463 0100 0000 0000 0000 0000 0000  getc............
+00000c90: 1000 0000 0a00 0000 4300 0000 735a 0200  ........C...sZ..
+00000ca0: 0067 0067 0067 0067 0066 045c 047d 017d  .g.g.g.g.f.\.}.}
+00000cb0: 027d 037d 0474 00a0 017c 027c 00a1 025c  .}.}.t...|.|...\
+00000cc0: 097d 057d 067d 077d 087d 027d 097d 0a7d  .}.}.}.}.}.}.}.}
+00000cd0: 0b7d 0c7c 0664 0119 0072 2474 027c 027c  .}.|.d...r$t.|.|
+00000ce0: 067c 057c 0c83 0401 0074 03a0 047c 027c  .|.|.....t...|.|
+00000cf0: 017c 037c 067c 077c 087c 057c 0ca1 087d  .|.|.|.|.|.|...}
+00000d00: 017c 0664 0219 0072 437c 0764 0319 0073  .|.d...rC|.d...s
+00000d10: 4374 0564 047c 0664 0219 007c 097c 0a7c  Ct.d.|.d...|.|.|
+00000d20: 027c 0c83 0601 007c 0664 0519 0072 567c  .|.....|.d...rV|
+00000d30: 0764 0619 0073 5674 0564 077c 0664 0519  .d...sVt.d.|.d..
+00000d40: 007c 097c 0a7c 027c 0c83 0601 007c 0664  .|.|.|.|.....|.d
+00000d50: 0819 0073 787c 0664 0219 0073 787c 0664  ...sx|.d...sx|.d
+00000d60: 0519 0073 7874 06a0 077c 027c 047c 017c  ...sxt...|.|.|.|
+00000d70: 067c 077c 087c 057c 0ca1 0801 0074 06a0  .|.|.|.|.....t..
+00000d80: 087c 027c 047c 037c 077c 057c 06a1 0601  .|.|.|.|.|.|....
+00000d90: 007c 0664 0819 0072 9b7c 0764 0919 0073  .|.d...r.|.d...s
+00000da0: 9b7c 0664 0519 0072 887c 0764 0619 0072  .|.d...r.|.d...r
+00000db0: 9b7c 0664 0219 0072 907c 0764 0319 0072  .|.d...r.|.d...r
+00000dc0: 9b74 0564 0a7c 0664 0819 007c 097c 0a7c  .t.d.|.d...|.|.|
+00000dd0: 027c 0c83 0601 0074 097c 027c 067c 0583  .|.....t.|.|.|..
+00000de0: 0301 0064 0b7d 0d74 0aa0 0b7c 057c 067c  ...d.}.t...|.|.|
+00000df0: 0264 0c7c 0da1 0501 0074 0c83 007d 0e74  .d.|.....t...}.t
+00000e00: 0da0 0e64 0d7c 0e9b 009d 02a1 0101 007c  ...d.|.........|
+00000e10: 0e64 0e75 0072 cc74 0f64 0f64 0c83 0201  .d.u.r.t.d.d....
+00000e20: 0074 107c 097c 0a7c 027c 0c83 0401 0074  .t.|.|.|.|.....t
+00000e30: 11a0 1264 10a1 0101 0064 117d 0f74 137c  ...d.....d.}.t.|
+00000e40: 027c 0e7c 0f83 0301 0074 107c 097c 0a7c  .|.|.....t.|.|.|
+00000e50: 027c 0c83 0401 0074 0da0 0e64 12a1 0101  .|.....t...d....
+00000e60: 007a 0e74 146a 1564 137c 0e9b 007c 0f9b  .z.t.j.d.|...|..
+00000e70: 009d 0364 1064 148d 0201 0057 006e 0f04  ...d.d.....W.n..
+00000e80: 0074 146a 1679 fd01 0001 0001 0074 0f64  .t.j.y.......t.d
+00000e90: 1564 1683 0201 0059 006e 0177 0074 1764  .d.....Y.n.w.t.d
+00000ea0: 1783 0101 0074 18a0 1974 1aa1 018f 1b01  .....t...t......
+00000eb0: 007c 0664 1819 0090 0172 1a74 1b7c 0b6a  .|.d.....r.t.|.j
+00000ec0: 1c83 0101 0057 0064 0e04 0004 0083 0301  .....W.d........
+00000ed0: 0064 0c53 0057 0064 0e04 0004 0083 0301  .d.S.W.d........
+00000ee0: 0064 0c53 0031 0090 0173 2677 0101 0001  .d.S.1...s&w....
+00000ef0: 0001 0059 0001 0064 0c53 0029 197a 9f0a  ...Y...d.S.).z..
+00000f00: 2020 2020 5468 6520 7072 696d 6172 7920      The primary 
+00000f10: 636f 6465 2073 7461 7274 7320 6865 7265  code starts here
+00000f20: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000f30: 6669 6c65 5f74 6f5f 6765 743a 2066 696c  file_to_get: fil
+00000f40: 6520 6e61 6d65 206f 6620 696e 7075 7420  e name of input 
+00000f50: 6261 636b 7570 2e78 6d6c 2066 696c 6520  backup.xml file 
+00000f60: 6f72 206e 6f6e 650a 2020 2020 2020 2020  or none.        
+00000f70: 3a72 6574 7572 6e3a 2072 6574 7572 6e20  :return: return 
+00000f80: 636f 6465 2028 7a65 726f 206f 7220 6572  code (zero or er
+00000f90: 726f 7220 636f 6465 290a 2020 2020 5a13  ror code).    Z.
+00000fa0: 6469 7370 6c61 795f 7072 6566 6572 656e  display_preferen
+00000fb0: 6365 735a 1373 696e 676c 655f 7072 6f6a  cesZ.single_proj
+00000fc0: 6563 745f 6e61 6d65 5a14 7369 6e67 6c65  ect_nameZ.single
+00000fd0: 5f70 726f 6a65 6374 5f66 6f75 6e64 5a07  _project_foundZ.
+00000fe0: 5072 6f6a 6563 745a 1373 696e 676c 655f  ProjectZ.single_
+00000ff0: 7072 6f66 696c 655f 6e61 6d65 5a14 7369  profile_nameZ.si
+00001000: 6e67 6c65 5f70 726f 6669 6c65 5f66 6f75  ngle_profile_fou
+00001010: 6e64 5a07 5072 6f66 696c 655a 1073 696e  ndZ.ProfileZ.sin
+00001020: 676c 655f 7461 736b 5f6e 616d 655a 1173  gle_task_nameZ.s
+00001030: 696e 676c 655f 7461 736b 5f66 6f75 6e64  ingle_task_found
+00001040: da04 5461 736b 7a0f 3c2f 626f 6479 3e0a  ..Taskz.</body>.
+00001050: 3c2f 6874 6d6c 3e72 0100 0000 7a11 6f75  </html>r....z.ou
+00001060: 7470 7574 2064 6972 6563 746f 7279 3a4e  tput directory:N
+00001070: 7a3c 4d61 7054 6173 6b65 7220 6361 6e63  z<MapTasker canc
+00001080: 656c 6c65 642e 2020 416e 2065 7272 6f72  elled.  An error
+00001090: 206f 6363 7572 7265 642e 2020 5072 6f67   occurred.  Prog
+000010a0: 7261 6d20 6361 6e63 656c 6c65 642e 721b  ram cancelled.r.
+000010b0: 0000 007a 0f2f 4d61 7054 6173 6b65 722e  ...z./MapTasker.
+000010c0: 6874 6d6c 7a20 4d61 7054 6173 6b65 7220  htmlz MapTasker 
+000010d0: 7072 6f67 7261 6d20 656e 6465 6420 6e6f  program ended no
+000010e0: 726d 616c 6c79 7a07 6669 6c65 3a2f 2f29  rmallyz.file://)
+000010f0: 01da 036e 6577 7a47 4572 726f 723a 2046  ...newzGError: F
+00001100: 6169 6c65 6420 746f 206f 7065 6e20 6f75  ailed to open ou
+00001110: 7470 7574 2069 6e20 6272 6f77 7365 723a  tput in browser:
+00001120: 2079 6f75 7220 6272 6f77 7365 7220 6973   your browser is
+00001130: 206e 6f74 2073 7570 706f 7274 6564 2e72   not supported.r
+00001140: 1a00 0000 7a42 596f 7520 6361 6e20 6669  ....zBYou can fi
+00001150: 6e64 2027 4d61 7054 6173 6b65 722e 6874  nd 'MapTasker.ht
+00001160: 6d6c 2720 696e 2074 6865 2063 7572 7265  ml' in the curre
+00001170: 6e74 2066 6f6c 6465 722e 2020 5072 6f67  nt folder.  Prog
+00001180: 7261 6d20 656e 642e 5a05 7265 7275 6e29  ram end.Z.rerun)
+00001190: 1dda 0a69 6e69 7469 616c 697a 655a 0873  ...initializeZ.s
+000011a0: 7461 7274 5f75 7072 0500 0000 da08 7072  tart_upr......pr
+000011b0: 6f6a 6563 7473 5a23 7072 6f63 6573 735f  ojectsZ#process_
+000011c0: 7072 6f6a 6563 7473 5f61 6e64 5f74 6865  projects_and_the
+000011d0: 6972 5f70 726f 6669 6c65 7372 3100 0000  ir_profilesr1...
+000011e0: da0d 7370 6563 6961 6c5f 7461 736b 735a  ..special_tasksZ
+000011f0: 2370 726f 6365 7373 5f74 6173 6b73 5f6e  #process_tasks_n
+00001200: 6f74 5f63 616c 6c65 645f 6279 5f70 726f  ot_called_by_pro
+00001210: 6669 6c65 5a22 7072 6f63 6573 735f 6d69  fileZ"process_mi
+00001220: 7373 696e 675f 7461 736b 735f 616e 645f  ssing_tasks_and_
+00001230: 7072 6f66 696c 6573 7204 0000 00da 0c62  profilesr......b
+00001240: 7569 6c64 5f6f 7574 7075 745a 096d 795f  uild_outputZ.my_
+00001250: 6f75 7470 7574 7202 0000 0072 0700 0000  outputr....r....
+00001260: 722a 0000 0072 0600 0000 7214 0000 0072  r*...r....r....r
+00001270: 2f00 0000 7230 0000 0072 2c00 0000 da0a  /...r0...r,.....
+00001280: 7765 6262 726f 7773 6572 7222 0000 00da  webbrowserr"....
+00001290: 0545 7272 6f72 da05 7072 696e 74da 0a63  .Error..print..c
+000012a0: 6f6e 7465 7874 6c69 62da 0873 7570 7072  ontextlib..suppr
+000012b0: 6573 73da 084b 6579 4572 726f 72da 096d  ess..KeyError..m
+000012c0: 6170 6974 5f61 6c6c 722d 0000 0029 1072  apit_allr-...).r
+000012d0: 3200 0000 5a0b 666f 756e 645f 7461 736b  2...Z.found_task
+000012e0: 7372 0b00 0000 5a19 7072 6f6a 6563 7473  sr....Z.projects
+000012f0: 5f77 6974 686f 7574 5f70 726f 6669 6c65  _without_profile
+00001300: 735a 1670 726f 6a65 6374 735f 7769 7468  sZ.projects_with
+00001310: 5f6e 6f5f 7461 736b 735a 0863 6f6c 6f72  _no_tasksZ.color
+00001320: 6d61 705a 0c70 726f 6772 616d 5f61 7267  mapZ.program_arg
+00001330: 735a 0b66 6f75 6e64 5f69 7465 6d73 da07  sZ.found_items..
+00001340: 6865 6164 696e 6772 0900 0000 720a 0000  headingr....r...
+00001350: 00da 0866 696c 656e 616d 6572 0c00 0000  ...filenamer....
+00001360: 5a09 6572 726f 725f 6d73 6772 1500 0000  Z.error_msgr....
+00001370: 7216 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00001380: 1300 0000 723f 0000 00d6 0000 0073 fc00  ....r?.......s..
+00001390: 0000 0208 0201 0201 0201 0cfc 0a12 02f6  ................
+000013a0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+000013b0: 0201 080c 0201 0201 0201 0201 0201 04fc  ................
+000013c0: 040a 0201 0201 0201 0201 0201 0201 0201  ................
+000013d0: 0201 04f8 100c 0201 0201 0601 0201 0201  ................
+000013e0: 0201 0201 04fa 1009 0201 0201 0601 0201  ................
+000013f0: 0201 0201 0201 04fa 060d 02ff 0602 02fe  ................
+00001400: 0603 02fd 0405 0201 0201 0201 0201 0201  ................
+00001410: 0201 0201 0201 04f8 040e 0201 0201 0201  ................
+00001420: 0201 0201 0201 04fa 060b 02ff 0602 02fe  ................
+00001430: 0604 02fc 0605 02fb 0608 02f8 0609 02f7  ................
+00001440: 020c 0201 0601 0201 0201 0201 0201 04fa  ................
+00001450: 0c0d 0403 1201 0604 1001 0801 0a01 0e01  ................
+00001460: 0a01 0402 0c02 0e03 0a03 0201 1c01 0e01  ................
+00001470: 0201 0401 08ff 02ff 0805 0c03 0a01 0c01  ................
+00001480: 0afe 0403 02fe 0aff 0403 12fd 0403 723f  ..............r?
+00001490: 0000 0029 2872 3c00 0000 722f 0000 0072  ...)(r<...r/...r
+000014a0: 3900 0000 5a16 6465 6675 7365 6478 6d6c  9...Z.defusedxml
+000014b0: 2e45 6c65 6d65 6e74 5472 6565 5a0a 6465  .ElementTreeZ.de
+000014c0: 6675 7365 6478 6d6c da02 6f73 7202 0000  fusedxml..osr...
+000014d0: 00da 0674 7970 696e 6772 0300 0000 5a15  ...typingr....Z.
+000014e0: 6d61 7074 6173 6b65 722e 7372 632e 6f75  maptasker.src.ou
+000014f0: 7470 7574 6cda 0373 7263 5a07 6f75 7470  tputl..srcZ.outp
+00001500: 7574 6c72 3800 0000 5a16 6d61 7074 6173  utlr8...Z.maptas
+00001510: 6b65 722e 7372 632e 7072 6f67 696e 6974  ker.src.proginit
+00001520: 5a08 7072 6f67 696e 6974 7235 0000 005a  Z.proginitr5...Z
+00001530: 166d 6170 7461 736b 6572 2e73 7263 2e70  .maptasker.src.p
+00001540: 726f 6a65 6374 7372 3600 0000 5a16 6d61  rojectsr6...Z.ma
+00001550: 7074 6173 6b65 722e 7372 632e 7461 736b  ptasker.src.task
+00001560: 756e 6971 5a08 7461 736b 756e 6971 7237  uniqZ.taskuniqr7
+00001570: 0000 005a 156d 6170 7461 736b 6572 2e73  ...Z.maptasker.s
+00001580: 7263 2e63 6176 6561 7473 7204 0000 005a  rc.caveatsr....Z
+00001590: 156d 6170 7461 736b 6572 2e73 7263 2e70  .maptasker.src.p
+000015a0: 7265 6665 7273 7205 0000 005a 136d 6170  refersr....Z.map
+000015b0: 7461 736b 6572 2e73 7263 2e65 7272 6f72  tasker.src.error
+000015c0: 7206 0000 005a 166d 6170 7461 736b 6572  r....Z.maptasker
+000015d0: 2e73 7263 2e73 7973 636f 6e73 7472 0700  .src.sysconstr..
+000015e0: 0000 7208 0000 005a 0b45 6c65 6d65 6e74  ..r....Z.Element
+000015f0: 5472 6565 5a03 584d 4cda 0373 7472 da04  TreeZ.XML..str..
+00001600: 6469 6374 7214 0000 0072 2c00 0000 da04  dictr....r,.....
+00001610: 6c69 7374 7231 0000 00da 0369 6e74 723f  listr1.....intr?
+00001620: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
+00001630: 0000 7213 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00001640: 3e01 0000 0073 6800 0000 0820 0801 0801  >....sh.... ....
+00001650: 0801 0c01 0c01 1202 1201 1201 1201 0c01  ................
+00001660: 0c01 0c01 0c01 0c01 020b 0601 02ff 0602  ................
+00001670: 02fe 0603 02fd 1204 02fc 0205 0afb 021c  ................
+00001680: 0601 02ff 0201 02ff 0201 02ff 0202 0afe  ................
+00001690: 0236 0201 02ff 0202 02fe 0603 02fd 0604  .6..............
+000016a0: 02fc 0205 02fb 0206 02fa 0207 0af9 021e  ................
+000016b0: 162b                                     .+
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/outputl.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/outputl.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 17 15:38:49 2023 UTC, .py size: 9892 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0968 3d64 a426 0000  o........h=d.&..
+00000000: 6f0d 0d0a 0000 0000 9a0c 4864 d825 0000  o.........Hd.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0010 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6403 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6400 6404 6c0a 6d0b 5a0b 0100 6400 6405  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0c 5a0c 0100 6400 6406 6c0a 6d0d  l.m.Z...d.d.l.m.
@@ -90,175 +90,177 @@
 00000590: 2064 6574 6169 6c73 2061 6464 6564 0a20   details added. 
 000005a0: 2020 2072 1200 0000 da07 6973 5f6c 6973     r......is_lis
 000005b0: 747a 113c 6c69 2073 7479 6c65 3d22 636f  tz.<li style="co
 000005c0: 6c6f 723a da06 636f 6c6f 7231 7a15 223e  lor:..color1z.">
 000005d0: 3c73 7061 6e20 7374 796c 653d 2263 6f6c  <span style="col
 000005e0: 6f72 3ada 0663 6f6c 6f72 32da 0466 6f6e  or:..color2..fon
 000005f0: 747a 0222 3eda 0765 6c65 6d65 6e74 fa0d  tz.">..element..
-00000600: 3c2f 7370 616e 3e3c 2f6c 693e 0ada 0c69  </span></li>...i
+00000600: 3c2f 7370 616e 3e3c 2f6c 693e 0a5a 0c69  </span></li>.Z.i
 00000610: 735f 7461 736b 6572 6e65 747a 333c 7020  s_taskernetz3<p 
 00000620: 7374 796c 653d 226d 6172 6769 6e2d 6c65  style="margin-le
 00000630: 6674 3a32 3070 783b 6d61 7267 696e 2d72  ft:20px;margin-r
 00000640: 6967 6874 3a35 3070 783b 636f 6c6f 723a  ight:50px;color:
 00000650: 7a15 3c2f 703e 0a3c 7020 7374 796c 653d  z.</p>.<p style=
 00000660: 2263 6f6c 6f72 3a7a 0d3c 7370 616e 3e3c  "color:z.<span><
 00000670: 2f73 7061 6e3e 2902 7204 0000 00da 0772  /span>).r......r
 00000680: 6570 6c61 6365 2902 7219 0000 005a 0f6c  eplace).r....Z.l
 00000690: 696e 655f 7769 7468 5f73 7479 6c65 7216  ine_with_styler.
 000006a0: 0000 0072 1600 0000 7217 0000 00da 0970  ...r....r......p
 000006b0: 7574 5f73 7479 6c65 5400 0000 7330 0000  ut_styleT...s0..
 000006c0: 0004 0608 010c 0206 0102 ff06 0104 ff06  ................
 000006d0: 0206 fe02 ff04 0f08 f702 0206 0102 ff02  ................
 000006e0: 0104 ff06 0204 fe06 0306 fd02 ff0c 0604  ................
-000006f0: 0272 2200 0000 721e 0000 00da 0b66 6f6e  .r"...r......fon
+000006f0: 0272 2100 0000 721e 0000 00da 0b66 6f6e  .r!...r......fon
 00000700: 745f 746f 5f75 7365 6303 0000 0000 0000  t_to_usec.......
-00000710: 0000 0000 0004 0000 0008 0000 0043 0000  .............C..
-00000720: 0073 6001 0000 7c02 9b00 6401 9d02 7c00  .s`...|...d...|.
+00000710: 0000 0000 0004 0000 0007 0000 0043 0000  .............C..
+00000720: 0073 4a01 0000 7c02 9b00 6401 9d02 7c00  .sJ...|...d...|.
 00000730: 7600 730b 6402 7c00 7600 7216 6403 7c01  v.s.d.|.v.r.d.|.
 00000740: 6404 1900 9b00 6405 7c00 9b00 6406 9d05  d.....d.|...d...
 00000750: 5300 7c02 9b00 6407 9d02 7c00 7600 7228  S.|...d...|.v.r(
 00000760: 6403 7c01 6404 1900 9b00 6405 7c00 9b00  d.|.d.....d.|...
-00000770: 6406 9d05 5300 7c00 6400 6408 8502 1900  d...S.|.d.d.....
-00000780: 6409 6b02 7334 640a 7c00 7600 7256 7400  d.k.s4d.|.v.rVt.
-00000790: 7c00 7600 7247 7401 640b 7c01 6404 1900  |.v.rGt.d.|.d...
-000007a0: 7c01 640c 1900 7c02 7c00 640d 9c05 640e  |.d...|.|.d...d.
-000007b0: 8d01 5300 7401 640b 7c01 6404 1900 7c01  ..S.t.d.|.d...|.
-000007c0: 640f 1900 7c02 7c00 640d 9c05 640e 8d01  d...|.|.d...d...
-000007d0: 5300 7c00 6400 6410 8502 1900 6411 6b02  S.|.d.d.....d.k.
-000007e0: 726d 7401 640b 7c01 6404 1900 7c01 6412  rmt.d.|.d...|.d.
-000007f0: 1900 7c02 7c00 640d 9c05 640e 8d01 5300  ..|.|.d...d...S.
-00000800: 6413 7c00 7600 7295 6414 7c00 7600 728a  d.|.v.r.d.|.v.r.
-00000810: 7c00 6415 6400 8502 1900 6416 6b02 727f  |.d.d.....d.k.r.
-00000820: 6416 5300 7402 a003 7c00 a004 6414 6417  d.S.t...|...d.d.
-00000830: a102 a101 7d03 7c03 7d00 6403 7c01 6404  ....}.|.}.d.|.d.
-00000840: 1900 9b00 6405 7c00 9b00 6406 9d05 5300  ....d.|...d...S.
-00000850: 6418 7c00 7600 72a9 7401 6419 7c01 6404  d.|.v.r.t.d.|.d.
-00000860: 1900 7c01 641a 1900 7c02 7c00 640b 641b  ..|.d...|.|.d.d.
-00000870: 9c06 640e 8d01 5300 641c 7c00 9b00 9d02  ..d...S.d.|.....
-00000880: 6406 1700 5300 291d 4e7a 0a22 3e50 726f  d...S.).Nz.">Pro
-00000890: 6a65 6374 3a7a 1750 726f 6a65 6374 2068  ject:z.Project h
-000008a0: 6173 206e 6f20 5072 6f66 696c 6573 7a10  as no Profilesz.
-000008b0: 3c6c 6920 7374 796c 653d 636f 6c6f 723a  <li style=color:
-000008c0: 5a0c 6275 6c6c 6574 5f63 6f6c 6f72 fa01  Z.bullet_color..
-000008d0: 3e72 1f00 0000 7a0a 223e 5072 6f66 696c  >r....z.">Profil
-000008e0: 653a e905 0000 007a 0554 6173 6b3a 7a0f  e:.....z.Task:z.
-000008f0: 2623 3435 3b26 2334 353b 5461 736b 3a54  &#45;&#45;Task:T
-00000900: 5a12 756e 6b6e 6f77 6e5f 7461 736b 5f63  Z.unknown_task_c
-00000910: 6f6c 6f72 2905 721a 0000 0072 1b00 0000  olor).r....r....
-00000920: 721c 0000 0072 1d00 0000 721e 0000 0029  r....r....r....)
-00000930: 0172 1900 0000 5a0a 7461 736b 5f63 6f6c  .r....Z.task_col
-00000940: 6f72 e906 0000 007a 0653 6365 6e65 3a5a  or.....z.Scene:Z
-00000950: 0b73 6365 6e65 5f63 6f6c 6f72 7a07 4163  .scene_colorz.Ac
-00000960: 7469 6f6e 3a7a 0b41 6374 696f 6e3a 202e  tion:z.Action: .
-00000970: 2e2e e90b 0000 0072 1200 0000 7a1a 266e  .......r....z.&n
-00000980: 6273 703b 266e 6273 703b 636f 6e74 696e  bsp;&nbsp;contin
-00000990: 7565 6420 3e3e 3e20 7a0a 5461 736b 6572  ued >>> z.Tasker
-000009a0: 4e65 7420 465a 0f74 6173 6b65 726e 6574  Net FZ.taskernet
-000009b0: 5f63 6f6c 6f72 2906 721a 0000 0072 1b00  _color).r....r..
-000009c0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000009d0: 0072 2000 0000 7a04 3c6c 6920 2905 7205  .r ...z.<li ).r.
-000009e0: 0000 0072 2200 0000 da0f 6163 7469 6f6e  ...r".....action
-000009f0: 5f65 7661 6c75 6174 655a 1263 6c65 616e  _evaluateZ.clean
-00000a00: 7570 5f74 6865 5f72 6573 756c 7472 2100  up_the_resultr!.
-00000a10: 0000 2904 721e 0000 0072 0d00 0000 7223  ..).r....r....r#
-00000a20: 0000 00da 0374 6d70 7216 0000 0072 1600  .....tmpr....r..
-00000a30: 0000 7217 0000 00da 0f75 6c69 6679 5f6c  ..r......ulify_l
-00000a40: 6973 745f 6974 656d 7200 0000 736a 0000  ist_itemr...sj..
-00000a50: 0016 0416 020e 0116 0118 0208 0c02 f702  ................
-00000a60: 0206 0106 0102 0102 0104 fb04 ff02 ff02  ................
-00000a70: 0b02 0206 0106 0102 0102 0104 fb04 ff02  ................
-00000a80: f510 1502 0102 0206 0106 0102 0102 0104  ................
-00000a90: fb06 ff08 0908 0210 0204 0104 010a 0104  ................
-00000aa0: ff04 0316 0108 0102 0102 0206 0106 0102  ................
-00000ab0: 0102 0102 0104 fa06 ff0e 0b72 2a00 0000  ...........r*...
-00000ac0: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
-00000ad0: 0004 0000 0043 0000 0073 a000 0000 6401  .....C...s....d.
-00000ae0: 7d04 7c01 0400 6402 6b02 7221 0100 7c00  }.|...d.k.r!..|.
-00000af0: 6400 6403 8502 1900 6404 6b02 7218 7c00  d.d.....d.k.r.|.
-00000b00: 9b00 6405 1700 7d04 0900 7c04 5300 6406  ..d...}...|.S.d.
-00000b10: 7c00 9b00 9d02 6407 1700 7d04 7c04 5300  |.....d...}.|.S.
-00000b20: 0400 6408 6b02 722f 0100 6409 7c00 9b00  ..d.k.r/..d.|...
-00000b30: 9d02 640a 1700 7d04 7c04 5300 0400 640b  ..d...}.|.S...d.
-00000b40: 6b02 723c 0100 7400 7c00 7c02 7c03 8303  k.r<..t.|.|.|...
-00000b50: 7d04 7c04 5300 0400 640c 6b02 7245 0100  }.|.S...d.k.rE..
-00000b60: 640d 7d04 7c04 5300 640e 6b02 724e 7c00  d.}.|.S.d.k.rN|.
-00000b70: 6405 1700 7d04 7c04 5300 7c04 5300 290f  d...}.|.S.|.S.).
-00000b80: 4e72 1200 0000 7201 0000 0072 2600 0000  Nr....r....r&...
-00000b90: 7a06 3c68 746d 6c3e 7a05 3c62 723e 0a7a  z.<html>z.<br>.z
-00000ba0: 033c 623e 7a09 3c2f 623e 3c62 723e 0a72  .<b>z.</b><br>.r
-00000bb0: 1100 0000 7a04 3c75 6c3e da01 0a72 1300  ....z.<ul>...r..
-00000bc0: 0000 e903 0000 007a 053c 2f75 6c3e e904  .......z.</ul>..
-00000bd0: 0000 0029 0172 2a00 0000 2905 721e 0000  ...).r*...).r...
-00000be0: 005a 036c 766c 720d 0000 0072 2300 0000  .Z.lvlr....r#...
-00000bf0: da06 7374 7269 6e67 7216 0000 0072 1600  ..stringr....r..
-00000c00: 0000 7217 0000 00da 0575 6c69 6679 bb00  ..r......ulify..
-00000c10: 0000 732a 0000 0004 0202 010a 0110 020a  ..s*............
-00000c20: 0102 0204 090e f704 090a f80e 0104 070a  ................
-00000c30: fa0c 0104 050a fc04 0104 0306 fe08 0108  ................
-00000c40: 0172 2f00 0000 da0a 6c69 7374 5f6c 6576  .r/.....list_lev
-00000c50: 656c da0a 6f75 745f 7374 7269 6e67 6305  el..out_stringc.
-00000c60: 0000 0000 0000 0000 0000 0007 0000 0008  ................
-00000c70: 0000 0043 0000 0073 6600 0000 6401 7c04  ...C...sf...d.|.
-00000c80: 7600 7213 7c01 6402 1900 6403 7500 7213  v.r.|.d...d.u.r.
-00000c90: 7c04 a000 6401 a101 7d05 7c05 6404 1900  |...d...}.|.d...
-00000ca0: 7d04 7c02 a001 7402 7c04 7c03 7c00 7c01  }.|...t.|.|.|.|.
-00000cb0: 6405 1900 8304 a101 0100 7403 7231 6406  d.........t.r1d.
-00000cc0: 7402 7c04 7c03 7c00 7c01 6405 1900 8304  t.|.|.|.|.d.....
-00000cd0: 6602 7d06 7404 a005 7c06 a101 0100 6407  f.}.t...|.....d.
-00000ce0: 5300 2908 6154 0100 000a 2020 2020 4164  S.).aT....    Ad
-00000cf0: 6420 6c69 6e65 2074 6f20 7468 6520 6c69  d line to the li
-00000d00: 7374 206f 6620 6f75 7470 7574 206c 696e  st of output lin
-00000d10: 6573 0a20 2020 2020 2020 203a 7061 7261  es.        :para
-00000d20: 6d20 636f 6c6f 726d 6170 3a20 636f 6c6f  m colormap: colo
-00000d30: 7273 2074 6f20 7573 6520 696e 2074 6865  rs to use in the
-00000d40: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
-00000d50: 3a70 6172 616d 2070 726f 6772 616d 5f61  :param program_a
-00000d60: 7267 733a 2072 756e 7469 6d65 2061 7267  rgs: runtime arg
-00000d70: 756d 656e 7473 0a20 2020 2020 2020 203a  uments.        :
-00000d80: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
-00000d90: 743a 206c 6973 7420 6f66 2061 6c6c 206f  t: list of all o
-00000da0: 7574 7075 7420 6c69 6e65 7320 7468 7573  utput lines thus
-00000db0: 2066 6172 0a20 2020 2020 2020 203a 7061   far.        :pa
-00000dc0: 7261 6d20 6c69 7374 5f6c 6576 656c 3a20  ram list_level: 
-00000dd0: 6c65 7665 6c20 7765 2061 7265 206f 7574  level we are out
-00000de0: 7075 7474 696e 670a 2020 2020 2020 2020  putting.        
-00000df0: 3a70 6172 616d 206f 7574 5f73 7472 696e  :param out_strin
-00000e00: 673a 2074 6865 2073 7472 696e 6720 746f  g: the string to
-00000e10: 2061 6464 2074 6f20 7468 6520 6f75 7470   add to the outp
-00000e20: 7574 0a20 2020 2020 2020 203a 7265 7475  ut.        :retu
-00000e30: 726e 3a20 6e6f 6e65 0a20 2020 207a 0854  rn: none.    z.T
-00000e40: 6173 6b20 4944 3a72 1000 0000 4672 0100  ask ID:r....Fr..
-00000e50: 0000 7223 0000 007a 0b6f 7574 5f73 7472  ..r#...z.out_str
-00000e60: 696e 673a 4e29 06da 0573 706c 6974 da06  ing:N)...split..
-00000e70: 6170 7065 6e64 722f 0000 0072 0600 0000  appendr/...r....
-00000e80: 7207 0000 0072 1000 0000 2907 720d 0000  r....r....).r...
-00000e90: 0072 0e00 0000 7209 0000 0072 3000 0000  .r....r....r0...
-00000ea0: 7231 0000 005a 0c74 656d 705f 656c 656d  r1...Z.temp_elem
-00000eb0: 656e 745a 0964 6562 7567 5f6d 7367 7216  entZ.debug_msgr.
-00000ec0: 0000 0072 1600 0000 7217 0000 0072 1500  ...r....r....r..
-00000ed0: 0000 d300 0000 7318 0000 0014 110a 0208  ......s.........
-00000ee0: 0104 0110 0104 ff04 0404 010c 0106 ff0a  ................
-00000ef0: 0304 0172 1500 0000 291b da16 6465 6675  ...r....)...defu
-00000f00: 7365 6478 6d6c 2e45 6c65 6d65 6e74 5472  sedxml.ElementTr
-00000f10: 6565 da0a 6465 6675 7365 6478 6d6c 5a15  ee..defusedxmlZ.
-00000f20: 6d61 7074 6173 6b65 722e 7372 632e 6163  maptasker.src.ac
-00000f30: 7469 6f6e 65da 0373 7263 5a07 6163 7469  tione..srcZ.acti
-00000f40: 6f6e 6572 2800 0000 5a13 6d61 7074 6173  oner(...Z.maptas
-00000f50: 6b65 722e 7372 632e 6465 6275 6772 0200  ker.src.debugr..
-00000f60: 0000 5a16 6d61 7074 6173 6b65 722e 7372  ..Z.maptasker.sr
-00000f70: 632e 6672 6d74 6874 6d6c 7203 0000 00da  c.frmthtmlr.....
-00000f80: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
-00000f90: 7973 636f 6e73 7472 0400 0000 7205 0000  ysconstr....r...
-00000fa0: 0072 0600 0000 7207 0000 00da 0462 6f6f  .r....r......boo
-00000fb0: 6cda 046c 6973 74da 0373 7472 da04 6469  l..list..str..di
-00000fc0: 6374 7218 0000 0072 2200 0000 da0b 456c  ctr....r".....El
-00000fd0: 656d 656e 7454 7265 65da 0358 4d4c 722a  ementTree..XMLr*
-00000fe0: 0000 0072 2f00 0000 da03 696e 7472 1500  ...r/.....intr..
-00000ff0: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00001000: 0072 1700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001010: 0100 0000 7362 0000 0008 0e12 020c 010c  ....sb..........
-00001020: 010c 010c 010c 010c 0102 0602 0102 ff02  ................
-00001030: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
-00001040: 0602 fa02 0702 f902 080a f812 3702 1e06  ............7...
-00001050: 0102 ff02 0102 ff02 0102 ff02 020a fe08  ................
-00001060: 4902 1802 0102 ff02 0202 fe02 0302 fd02  I...............
-00001070: 0402 fc02 0502 fb02 060e fa              ...........
+00000770: 6408 9d05 5300 7c00 6400 6409 8502 1900  d...S.|.d.d.....
+00000780: 640a 6b02 7334 640b 7c00 7600 7256 7400  d.k.s4d.|.v.rVt.
+00000790: 7c00 7600 7247 7401 640c 7c01 6404 1900  |.v.rGt.d.|.d...
+000007a0: 7c01 640d 1900 7c02 7c00 640e 9c05 640f  |.d...|.|.d...d.
+000007b0: 8d01 5300 7401 640c 7c01 6404 1900 7c01  ..S.t.d.|.d...|.
+000007c0: 6410 1900 7c02 7c00 640e 9c05 640f 8d01  d...|.|.d...d...
+000007d0: 5300 7c00 6400 6411 8502 1900 6412 6b02  S.|.d.d.....d.k.
+000007e0: 726d 7401 640c 7c01 6404 1900 7c01 6413  rmt.d.|.d...|.d.
+000007f0: 1900 7c02 7c00 640e 9c05 640f 8d01 5300  ..|.|.d...d...S.
+00000800: 6414 7c00 7600 7295 6415 7c00 7600 728a  d.|.v.r.d.|.v.r.
+00000810: 7c00 6416 6400 8502 1900 6417 6b02 727f  |.d.d.....d.k.r.
+00000820: 6417 5300 7402 a003 7c00 a004 6415 6418  d.S.t...|...d.d.
+00000830: a102 a101 7d03 7c03 7d00 6419 7c01 6404  ....}.|.}.d.|.d.
+00000840: 1900 9b00 6405 7c00 9b00 6408 9d05 5300  ....d.|...d...S.
+00000850: 641a 7c00 7600 729e 7c00 9b00 641b 9d02  d.|.v.r.|...d...
+00000860: 5300 641c 7c00 9b00 9d02 6408 1700 5300  S.d.|.....d...S.
+00000870: 291d 4e7a 0a22 3e50 726f 6a65 6374 3a7a  ).Nz.">Project:z
+00000880: 1750 726f 6a65 6374 2068 6173 206e 6f20  .Project has no 
+00000890: 5072 6f66 696c 6573 7a14 3c62 723e 3c6c  Profilesz.<br><l
+000008a0: 6920 7374 796c 653d 636f 6c6f 723a 5a0c  i style=color:Z.
+000008b0: 6275 6c6c 6574 5f63 6f6c 6f72 fa01 3e7a  bullet_color..>z
+000008c0: 063c 2f6c 693e 0a7a 0a22 3e50 726f 6669  .</li>.z.">Profi
+000008d0: 6c65 3a72 1f00 0000 e905 0000 007a 0554  le:r.........z.T
+000008e0: 6173 6b3a 7a0f 2623 3435 3b26 2334 353b  ask:z.&#45;&#45;
+000008f0: 5461 736b 3a54 5a12 756e 6b6e 6f77 6e5f  Task:TZ.unknown_
+00000900: 7461 736b 5f63 6f6c 6f72 2905 721a 0000  task_color).r...
+00000910: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+00000920: 721e 0000 0029 0172 1900 0000 5a0a 7461  r....).r....Z.ta
+00000930: 736b 5f63 6f6c 6f72 e906 0000 007a 0653  sk_color.....z.S
+00000940: 6365 6e65 3a5a 0b73 6365 6e65 5f63 6f6c  cene:Z.scene_col
+00000950: 6f72 7a07 4163 7469 6f6e 3a7a 0b41 6374  orz.Action:z.Act
+00000960: 696f 6e3a 202e 2e2e e90b 0000 0072 1200  ion: ........r..
+00000970: 0000 7a1a 266e 6273 703b 266e 6273 703b  ..z.&nbsp;&nbsp;
+00000980: 636f 6e74 696e 7565 6420 3e3e 3e20 7a10  continued >>> z.
+00000990: 3c6c 6920 7374 796c 653d 636f 6c6f 723a  <li style=color:
+000009a0: 7a0a 5461 736b 6572 4e65 7420 da01 0a7a  z.TaskerNet ...z
+000009b0: 043c 6c69 2029 0572 0500 0000 7221 0000  .<li ).r....r!..
+000009c0: 00da 0f61 6374 696f 6e5f 6576 616c 7561  ...action_evalua
+000009d0: 7465 5a12 636c 6561 6e75 705f 7468 655f  teZ.cleanup_the_
+000009e0: 7265 7375 6c74 7220 0000 0029 0472 1e00  resultr ...).r..
+000009f0: 0000 720d 0000 0072 2200 0000 da03 746d  ..r....r".....tm
+00000a00: 7072 1600 0000 7216 0000 0072 1700 0000  pr....r....r....
+00000a10: da0f 756c 6966 795f 6c69 7374 5f69 7465  ..ulify_list_ite
+00000a20: 6d72 0000 0073 5a00 0000 1604 1602 0e01  mr...sZ.........
+00000a30: 1601 1802 080c 02f7 0202 0601 0601 0201  ................
+00000a40: 0201 04fb 04ff 02ff 020b 0202 0601 0601  ................
+00000a50: 0201 0201 04fb 04ff 02f5 1015 0201 0202  ................
+00000a60: 0601 0601 0201 0201 04fb 06ff 0809 0802  ................
+00000a70: 1002 0401 0401 0a01 04ff 0403 1601 0801  ................
+00000a80: 0a01 0e02 722a 0000 0063 0400 0000 0000  ....r*...c......
+00000a90: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
+00000aa0: 0000 73a0 0000 0064 017d 047c 0104 0064  ..s....d.}.|...d
+00000ab0: 026b 0272 2101 007c 0064 0064 0385 0219  .k.r!..|.d.d....
+00000ac0: 0064 046b 0272 187c 009b 0064 0517 007d  .d.k.r.|...d...}
+00000ad0: 0409 007c 0453 0064 067c 009b 009d 0264  ...|.S.d.|.....d
+00000ae0: 0717 007d 047c 0453 0004 0064 086b 0272  ...}.|.S...d.k.r
+00000af0: 2f01 0064 097c 009b 009d 0264 0a17 007d  /..d.|.....d...}
+00000b00: 047c 0453 0004 0064 0b6b 0272 3c01 0074  .|.S...d.k.r<..t
+00000b10: 007c 007c 027c 0383 037d 047c 0453 0004  .|.|.|...}.|.S..
+00000b20: 0064 0c6b 0272 4501 0064 0d7d 047c 0453  .d.k.rE..d.}.|.S
+00000b30: 0064 0e6b 0272 4e7c 0064 0517 007d 047c  .d.k.rN|.d...}.|
+00000b40: 0453 007c 0453 0029 0f4e 7212 0000 0072  .S.|.S.).Nr....r
+00000b50: 0100 0000 7225 0000 007a 063c 6874 6d6c  ....r%...z.<html
+00000b60: 3e7a 053c 6272 3e0a 7a03 3c62 3e7a 093c  >z.<br>.z.<b>z.<
+00000b70: 2f62 3e3c 6272 3e0a 7211 0000 007a 043c  /b><br>.r....z.<
+00000b80: 756c 3e72 2700 0000 7213 0000 00e9 0300  ul>r'...r.......
+00000b90: 0000 7a05 3c2f 756c 3ee9 0400 0000 2901  ..z.</ul>.....).
+00000ba0: 722a 0000 0029 0572 1e00 0000 5a03 6c76  r*...).r....Z.lv
+00000bb0: 6c72 0d00 0000 7222 0000 00da 0673 7472  lr....r".....str
+00000bc0: 696e 6772 1600 0000 7216 0000 0072 1700  ingr....r....r..
+00000bd0: 0000 da05 756c 6966 79b2 0000 0073 2a00  ....ulify....s*.
+00000be0: 0000 0402 0201 0a01 1002 0a01 0202 0409  ................
+00000bf0: 0ef7 0409 0af8 0e01 0407 0afa 0c01 0405  ................
+00000c00: 0afc 0401 0403 06fe 0801 0801 722e 0000  ............r...
+00000c10: 00da 0a6c 6973 745f 6c65 7665 6cda 0a6f  ...list_level..o
+00000c20: 7574 5f73 7472 696e 6763 0500 0000 0000  ut_stringc......
+00000c30: 0000 0000 0000 0700 0000 0800 0000 4300  ..............C.
+00000c40: 0000 735e 0000 0064 017c 0476 0072 137c  ..s^...d.|.v.r.|
+00000c50: 0164 0219 0064 0375 0072 137c 04a0 0064  .d...d.u.r.|...d
+00000c60: 01a1 017d 057c 0564 0419 007d 047c 02a0  ...}.|.d...}.|..
+00000c70: 0174 027c 047c 037c 007c 0164 0519 0083  .t.|.|.|.|.d....
+00000c80: 04a1 0101 0074 0372 2d64 067c 0264 0719  .....t.r-d.|.d..
+00000c90: 009b 009d 027d 0674 04a0 057c 06a1 0101  .....}.t...|....
+00000ca0: 0064 0853 0029 0961 a501 0000 0a20 2020  .d.S.).a.....   
+00000cb0: 2041 6464 206c 696e 6520 746f 2074 6865   Add line to the
+00000cc0: 206c 6973 7420 6f66 206f 7574 7075 7420   list of output 
+00000cd0: 6c69 6e65 732e 2020 5468 6520 6f75 7470  lines.  The outp
+00000ce0: 7574 2065 6e74 7279 2069 7320 6261 7365  ut entry is base
+00000cf0: 6420 6f6e 2074 6865 206c 6973 745f 6c65  d on the list_le
+00000d00: 7665 6c20 616e 6420 7468 6520 636f 6e74  vel and the cont
+00000d10: 656e 7473 206f 6620 7468 6520 6f75 7470  ents of the outp
+00000d20: 7574 5f73 7472 0a20 2020 2020 2020 203a  ut_str.        :
+00000d30: 7061 7261 6d20 636f 6c6f 726d 6170 3a20  param colormap: 
+00000d40: 636f 6c6f 7273 2074 6f20 7573 6520 696e  colors to use in
+00000d50: 2074 6865 206f 7574 7075 740a 2020 2020   the output.    
+00000d60: 2020 2020 3a70 6172 616d 2070 726f 6772      :param progr
+00000d70: 616d 5f61 7267 733a 2072 756e 7469 6d65  am_args: runtime
+00000d80: 2061 7267 756d 656e 7473 0a20 2020 2020   arguments.     
+00000d90: 2020 203a 7061 7261 6d20 6f75 7470 7574     :param output
+00000da0: 5f6c 6973 743a 206c 6973 7420 6f66 2061  _list: list of a
+00000db0: 6c6c 206f 7574 7075 7420 6c69 6e65 7320  ll output lines 
+00000dc0: 7468 7573 2066 6172 0a20 2020 2020 2020  thus far.       
+00000dd0: 203a 7061 7261 6d20 6c69 7374 5f6c 6576   :param list_lev
+00000de0: 656c 3a20 6c65 7665 6c20 7765 2061 7265  el: level we are
+00000df0: 206f 7574 7075 7474 696e 670a 2020 2020   outputting.    
+00000e00: 2020 2020 3a70 6172 616d 206f 7574 5f73      :param out_s
+00000e10: 7472 696e 673a 2074 6865 2073 7472 696e  tring: the strin
+00000e20: 6720 746f 2061 6464 2074 6f20 7468 6520  g to add to the 
+00000e30: 6f75 7470 7574 0a20 2020 2020 2020 203a  output.        :
+00000e40: 7265 7475 726e 3a20 6e6f 6e65 0a20 2020  return: none.   
+00000e50: 207a 0854 6173 6b20 4944 3a72 1000 0000   z.Task ID:r....
+00000e60: 4672 0100 0000 7222 0000 007a 0c6f 7574  Fr....r"...z.out
+00000e70: 5f73 7472 696e 673a 20e9 ffff ffff 4e29  _string: .....N)
+00000e80: 06da 0573 706c 6974 da06 6170 7065 6e64  ...split..append
+00000e90: 722e 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+00000ea0: 1000 0000 2907 720d 0000 0072 0e00 0000  ....).r....r....
+00000eb0: 7209 0000 0072 2f00 0000 7230 0000 005a  r....r/...r0...Z
+00000ec0: 0c74 656d 705f 656c 656d 656e 745a 0964  .temp_elementZ.d
+00000ed0: 6562 7567 5f6d 7367 7216 0000 0072 1600  ebug_msgr....r..
+00000ee0: 0000 7217 0000 0072 1500 0000 ca00 0000  ..r....r........
+00000ef0: 7314 0000 0014 110a 0208 0104 0310 0104  s...............
+00000f00: ff04 040e 010a 0104 0172 1500 0000 291b  .........r....).
+00000f10: da16 6465 6675 7365 6478 6d6c 2e45 6c65  ..defusedxml.Ele
+00000f20: 6d65 6e74 5472 6565 da0a 6465 6675 7365  mentTree..defuse
+00000f30: 6478 6d6c 5a15 6d61 7074 6173 6b65 722e  dxmlZ.maptasker.
+00000f40: 7372 632e 6163 7469 6f6e 65da 0373 7263  src.actione..src
+00000f50: 5a07 6163 7469 6f6e 6572 2800 0000 5a13  Z.actioner(...Z.
+00000f60: 6d61 7074 6173 6b65 722e 7372 632e 6465  maptasker.src.de
+00000f70: 6275 6772 0200 0000 5a16 6d61 7074 6173  bugr....Z.maptas
+00000f80: 6b65 722e 7372 632e 6672 6d74 6874 6d6c  ker.src.frmthtml
+00000f90: 7203 0000 00da 166d 6170 7461 736b 6572  r......maptasker
+00000fa0: 2e73 7263 2e73 7973 636f 6e73 7472 0400  .src.sysconstr..
+00000fb0: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00000fc0: 00da 0462 6f6f 6cda 046c 6973 74da 0373  ...bool..list..s
+00000fd0: 7472 da04 6469 6374 7218 0000 0072 2100  tr..dictr....r!.
+00000fe0: 0000 da0b 456c 656d 656e 7454 7265 65da  ....ElementTree.
+00000ff0: 0358 4d4c 722a 0000 0072 2e00 0000 da03  .XMLr*...r......
+00001000: 696e 7472 1500 0000 7216 0000 0072 1600  intr....r....r..
+00001010: 0000 7216 0000 0072 1700 0000 da08 3c6d  ..r....r......<m
+00001020: 6f64 756c 653e 0100 0000 7362 0000 0008  odule>....sb....
+00001030: 0e12 020c 010c 010c 010c 010c 010c 0102  ................
+00001040: 0602 0102 ff02 0202 fe02 0302 fd02 0402  ................
+00001050: fc02 0502 fb02 0602 fa02 0702 f902 080a  ................
+00001060: f812 3702 1e06 0102 ff02 0102 ff02 0102  ..7.............
+00001070: ff02 020a fe08 4002 1802 0102 ff02 0202  ......@.........
+00001080: fe02 0302 fd02 0402 fc02 0502 fb02 060e  ................
+00001090: fa                                       .
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/parsearg.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/parsearg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/prefers.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/prefers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/priority.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/priority.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 11 19:20:37 2023 UTC, .py size: 1684 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 05b3 3564 9406 0000  o.........5d....
+00000000: 6f0d 0d0a 0000 0000 b6cd 4264 9006 0000  o.........Bd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6402 6501 6a02 6a03 6403  d.l.Z.d.e.j.j.d.
 00000040: 6504 6404 6505 6606 6405 6406 8404 5a06  e.d.e.f.d.d...Z.
 00000050: 6401 5300 2907 e900 0000 004e da07 656c  d.S.)......N..el
 00000060: 656d 656e 74da 0565 7665 6e74 da06 7265  ement..event..re
 00000070: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
@@ -21,31 +21,31 @@
 00000140: 6d20 6576 656e 743a 2054 7275 6520 6966  m event: True if
 00000150: 2074 6869 7320 6973 2066 6f72 2061 6e20   this is for an 
 00000160: 2745 7665 6e74 2720 636f 6e64 6974 696f  'Event' conditio
 00000170: 6e2c 2046 616c 7365 2069 6620 6e6f 740a  n, False if not.
 00000180: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
 00000190: 2074 6865 2070 7269 6f72 6974 7920 6f72   the priority or
 000001a0: 206e 6f6e 650a 2020 2020 da03 7072 694e   none.    ..priN
-000001b0: da00 7a0a 2050 7269 6f72 6974 793a 7a21  ..z. Priority:z!
-000001c0: 3c62 723e 266e 6273 703b 266e 6273 703b  <br>&nbsp;&nbsp;
-000001d0: 266e 6273 703b 5b50 7269 6f72 6974 793a  &nbsp;[Priority:
-000001e0: 20fa 015d 2902 da04 6669 6e64 da04 7465   ..])...find..te
-000001f0: 7874 2903 7202 0000 0072 0300 0000 5a10  xt).r....r....Z.
-00000200: 7072 696f 7269 7479 5f65 6c65 6d65 6e74  priority_element
-00000210: a900 720a 0000 00fa 772f 5573 6572 732f  ..r.....w/Users/
-00000220: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
-00000230: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
-00000240: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
-00000250: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
-00000260: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
-00000270: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
-00000280: 2f73 7263 2f70 7269 6f72 6974 792e 7079  /src/priority.py
-00000290: da0c 6765 745f 7072 696f 7269 7479 1100  ..get_priority..
-000002a0: 0000 730c 0000 000a 0808 0104 0104 010c  ..s.............
-000002b0: 010e 0272 0c00 0000 2907 da16 6465 6675  ...r....)...defu
-000002c0: 7365 6478 6d6c 2e45 6c65 6d65 6e74 5472  sedxml.ElementTr
-000002d0: 6565 da0a 6465 6675 7365 6478 6d6c da0b  ee..defusedxml..
-000002e0: 456c 656d 656e 7454 7265 65da 0358 4d4c  ElementTree..XML
-000002f0: da04 626f 6f6c da03 7374 7272 0c00 0000  ..bool..strr....
-00000300: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00000310: 0b00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000320: 0000 7304 0000 0008 0d1e 03              ..s........
+000001b0: da00 7a0a 2050 7269 6f72 6974 793a 7a1d  ..z. Priority:z.
+000001c0: 266e 6273 703b 266e 6273 703b 266e 6273  &nbsp;&nbsp;&nbs
+000001d0: 703b 5b50 7269 6f72 6974 793a 20fa 015d  p;[Priority: ..]
+000001e0: 2902 da04 6669 6e64 da04 7465 7874 2903  )...find..text).
+000001f0: 7202 0000 0072 0300 0000 5a10 7072 696f  r....r....Z.prio
+00000200: 7269 7479 5f65 6c65 6d65 6e74 a900 720a  rity_element..r.
+00000210: 0000 00fa 772f 5573 6572 732f 6d69 6b72  ....w/Users/mikr
+00000220: 7562 696e 2f4c 6962 7261 7279 2f43 6c6f  ubin/Library/Clo
+00000230: 7564 5374 6f72 6167 652f 476f 6f67 6c65  udStorage/Google
+00000240: 4472 6976 652d 6d69 6b72 7562 696e 4067  Drive-mikrubin@g
+00000250: 6d61 696c 2e63 6f6d 2f4d 7920 4472 6976  mail.com/My Driv
+00000260: 652f 5079 7468 6f6e 2f6d 6170 7461 736b  e/Python/maptask
+00000270: 6572 2f6d 6170 7461 736b 6572 2f73 7263  er/maptasker/src
+00000280: 2f70 7269 6f72 6974 792e 7079 da0c 6765  /priority.py..ge
+00000290: 745f 7072 696f 7269 7479 1100 0000 730c  t_priority....s.
+000002a0: 0000 000a 0808 0104 0104 010c 010e 0272  ...............r
+000002b0: 0c00 0000 2907 da16 6465 6675 7365 6478  ....)...defusedx
+000002c0: 6d6c 2e45 6c65 6d65 6e74 5472 6565 da0a  ml.ElementTree..
+000002d0: 6465 6675 7365 6478 6d6c da0b 456c 656d  defusedxml..Elem
+000002e0: 656e 7454 7265 65da 0358 4d4c da04 626f  entTree..XML..bo
+000002f0: 6f6c da03 7374 7272 0c00 0000 720a 0000  ol..strr....r...
+00000300: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000310: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
+00000320: 0000 0008 0d1e 03                        .......
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/proclist.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/proclist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/profiles.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/profiles.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/progargs.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/progargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/proginit.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/proginit.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 12 16:13:37 2023 UTC, .py size: 10342 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,365 +1,420 @@
-00000000: 6f0d 0d0a 0000 0000 b1d8 3664 6628 0000  o.........6df(..
+00000000: 6f0d 0d0a 0000 0000 939c 4a64 442c 0000  o.........JdD,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000e 0000 0040 0000 0073 b801 0000 6400  .....@...s....d.
+00000020: 0010 0000 0040 0000 0073 c601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6404 6c08 5400 6400 6405 6c08  ..d.d.l.T.d.d.l.
-00000070: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6407 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6401 6c0e 6d0f 0200 0100 6d10 5a11 0100  d.l.m.....m.Z...
-000000a0: 6400 6401 6c12 6d0f 0200 0100 6d13 5a14  d.d.l.m.....m.Z.
-000000b0: 0100 6400 6401 6c15 6d0f 0200 0100 6d16  ..d.d.l.m.....m.
-000000c0: 5a17 0100 6400 6408 6c18 6d19 5a19 0100  Z...d.d.l.m.Z...
-000000d0: 6400 6409 6c1a 6d1b 5a1b 0100 6400 640a  d.d.l.m.Z...d.d.
-000000e0: 6c1c 6d1d 5a1d 0100 6400 640b 6c1c 6d1e  l.m.Z...d.d.l.m.
-000000f0: 5a1e 0100 6400 640c 6c1f 6d20 5a20 0100  Z...d.d.l.m Z ..
-00000100: 6400 640d 6c21 6d22 5a22 0100 6400 640e  d.d.l!m"Z"..d.d.
-00000110: 6c21 6d23 5a23 0100 6400 640f 6c21 6d24  l!m#Z#..d.d.l!m$
-00000120: 5a24 0100 6400 6410 6c21 6d25 5a25 0100  Z$..d.d.l!m%Z%..
-00000130: 6400 6411 6c21 6d26 5a26 0100 6400 6412  d.d.l!m&Z&..d.d.
-00000140: 6c27 6d28 5a28 0100 6413 6414 8400 5a29  l'm(Z(..d.d...Z)
-00000150: 6415 6416 8400 5a2a 6529 8300 5a2b 6500  d.d...Z*e)..Z+e.
-00000160: a02c 652a a101 0100 6417 652d 6418 652e  .,e*....d.e-d.e.
-00000170: 6604 6419 641a 8404 5a2f 6418 652d 6602  f.d.d...Z/d.e-f.
-00000180: 641b 641c 8404 5a30 641d 641e 8400 5a31  d.d...Z0d.d...Z1
-00000190: 6417 652d 641f 652d 6418 6401 6606 6420  d.e-d.e-d.d.f.d 
-000001a0: 6421 8404 5a32 641f 652d 6417 652d 6422  d!..Z2d.e-d.e-d"
-000001b0: 6533 6418 6534 650d 650d 652e 650d 6533  e3d.e4e.e.e.e.e3
-000001c0: 6535 6606 1900 6608 6423 6424 8404 5a36  e5f...f.d#d$..Z6
-000001d0: 6422 6533 6418 6534 6604 6425 6426 8404  d"e3d.e4f.d%d&..
-000001e0: 5a37 6401 5300 2927 e900 0000 004e 2902  Z7d.S.)'.....N).
-000001f0: da05 6475 6d70 73da 056c 6f61 6473 2901  ..dumps..loads).
-00000200: da04 5061 7468 2901 da01 2a29 01da 0a6d  ..Path)...*)...m
-00000210: 6573 7361 6765 626f 7829 01da 0b61 736b  essagebox)...ask
-00000220: 6f70 656e 6669 6c65 2901 da03 416e 7929  openfile)...Any)
-00000230: 01da 0b66 6f72 6d61 745f 6874 6d6c 2901  ...format_html).
-00000240: da0e 7365 745f 636f 6c6f 725f 6d6f 6465  ..set_color_mode
-00000250: 2901 da09 4441 524b 5f4d 4f44 4529 01da  )...DARK_MODE)..
-00000260: 0347 5549 2901 da06 6465 6275 6731 2901  .GUI)...debug1).
-00000270: da0c 434f 554e 5445 525f 4649 4c45 2901  ..COUNTER_FILE).
-00000280: da0b 464f 4e54 5f54 4f5f 5553 4529 01da  ..FONT_TO_USE)..
+00000060: 0100 6400 6404 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6405 6c08 6d0a 5a0a 0100 6400 6406 6c0b  d.l.m.Z...d.d.l.
+00000080: 6d0c 5a0c 0100 6400 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
+00000090: 0100 6400 6401 6c0f 6d10 0200 0100 6d11  ..d.d.l.m.....m.
+000000a0: 5a12 0100 6400 6401 6c13 6d10 0200 0100  Z...d.d.l.m.....
+000000b0: 6d14 5a15 0100 6400 6401 6c16 6d10 0200  m.Z...d.d.l.m...
+000000c0: 0100 6d17 5a18 0100 6400 6408 6c19 6d1a  ..m.Z...d.d.l.m.
+000000d0: 5a1a 0100 6400 6409 6c1b 6d1c 5a1c 0100  Z...d.d.l.m.Z...
+000000e0: 6400 640a 6c1d 6d1e 5a1e 0100 6400 640b  d.d.l.m.Z...d.d.
+000000f0: 6c1d 6d1f 5a1f 0100 6400 640c 6c20 6d21  l.m.Z...d.d.l m!
+00000100: 5a21 0100 6400 640d 6c22 6d23 5a23 0100  Z!..d.d.l"m#Z#..
+00000110: 6400 640e 6c22 6d24 5a24 0100 6400 640f  d.d.l"m$Z$..d.d.
+00000120: 6c22 6d25 5a25 0100 6400 6410 6c22 6d26  l"m%Z%..d.d.l"m&
+00000130: 5a26 0100 6400 6411 6c27 6d28 5a28 0100  Z&..d.d.l'm(Z(..
+00000140: 6400 6412 6c29 6d2a 5a2a 0100 6413 6414  d.d.l)m*Z*..d.d.
+00000150: 8400 5a2b 6415 6416 8400 5a2c 652b 8300  ..Z+d.d...Z,e+..
+00000160: 5a2d 6500 a02e 652c a101 0100 6417 652f  Z-e...e,....d.e/
+00000170: 6418 6530 6604 6419 641a 8404 5a31 6418  d.e0f.d.d...Z1d.
+00000180: 652f 6602 641b 641c 8404 5a32 6428 641d  e/f.d.d...Z2d(d.
+00000190: 641e 8404 5a33 6417 652f 641f 652f 6418  d...Z3d.e/d.e/d.
+000001a0: 6401 6606 6420 6421 8404 5a34 641f 652f  d.f.d d!..Z4d.e/
+000001b0: 6417 652f 6422 6535 6423 6536 6418 6537  d.e/d"e5d#e6d.e7
+000001c0: 650e 650e 6530 650e 6535 6536 6606 1900  e.e.e0e.e5e6f...
+000001d0: 660a 6424 6425 8404 5a38 6422 6535 6423  f.d$d%..Z8d"e5d#
+000001e0: 6536 6418 6537 6606 6426 6427 8404 5a39  e6d.e7f.d&d'..Z9
+000001f0: 6401 5300 2929 e900 0000 004e 2902 da05  d.S.)).....N)...
+00000200: 6475 6d70 73da 056c 6f61 6473 2901 da04  dumps..loads)...
+00000210: 5061 7468 2901 da02 546b 2901 da0a 6d65  Path)...Tk)...me
+00000220: 7373 6167 6562 6f78 2901 da0b 6173 6b6f  ssagebox)...asko
+00000230: 7065 6e66 696c 6529 01da 0341 6e79 2901  penfile)...Any).
+00000240: da0b 666f 726d 6174 5f68 746d 6c29 01da  ..format_html)..
+00000250: 0e73 6574 5f63 6f6c 6f72 5f6d 6f64 6529  .set_color_mode)
+00000260: 01da 0944 4152 4b5f 4d4f 4445 2901 da03  ...DARK_MODE)...
+00000270: 4755 4929 01da 0664 6562 7567 3129 01da  GUI)...debug1)..
+00000280: 0c43 4f55 4e54 4552 5f46 494c 4529 01da  .COUNTER_FILE)..
 00000290: 0a4d 595f 5645 5253 494f 4e29 01da 066c  .MY_VERSION)...l
 000002a0: 6f67 6765 7229 01da 076c 6f67 6769 6e67  ogger)...logging
 000002b0: 2901 da10 6765 745f 7468 655f 786d 6c5f  )...get_the_xml_
-000002c0: 6461 7461 6300 0000 0000 0000 0000 0000  datac...........
-000002d0: 0000 0000 0004 0000 0043 0000 0073 2c00  .........C...s,.
-000002e0: 0000 7400 a001 7400 7402 8301 a003 a100  ..t...t.t.......
-000002f0: a101 7214 7404 7405 7402 6401 8302 a006  ..r.t.t.t.d.....
-00000300: a100 8301 6402 1700 5300 6403 5300 2904  ....d...S.d.S.).
-00000310: 7a7f 5265 6164 2074 6865 2070 726f 6772  z.Read the progr
-00000320: 616d 2063 6f75 6e74 6572 0a0a 2020 2020  am counter..    
-00000330: 5061 7261 6d65 7465 7273 3a20 6e6f 6e65  Parameters: none
-00000340: 0a0a 2020 2020 5265 7475 726e 733a 2074  ..    Returns: t
-00000350: 6865 2063 6f75 6e74 206f 6620 7468 6520  he count of the 
-00000360: 6e75 6d62 6572 206f 6620 7469 6d65 7320  number of times 
-00000370: 7468 6520 7072 6f67 7261 6d20 6861 7320  the program has 
-00000380: 6265 656e 2063 616c 6c65 640a 0a20 2020  been called..   
-00000390: 20da 0172 e901 0000 0072 0100 0000 2907   ..r.....r....).
-000003a0: 7204 0000 00da 0665 7869 7374 7372 0e00  r......existsr..
-000003b0: 0000 5a07 7265 736f 6c76 6572 0300 0000  ..Z.resolver....
-000003c0: da04 6f70 656e da04 7265 6164 a900 7219  ..open..read..r.
-000003d0: 0000 0072 1900 0000 fa77 2f55 7365 7273  ...r.....w/Users
-000003e0: 2f6d 696b 7275 6269 6e2f 4c69 6272 6172  /mikrubin/Librar
-000003f0: 792f 436c 6f75 6453 746f 7261 6765 2f47  y/CloudStorage/G
-00000400: 6f6f 676c 6544 7269 7665 2d6d 696b 7275  oogleDrive-mikru
-00000410: 6269 6e40 676d 6169 6c2e 636f 6d2f 4d79  bin@gmail.com/My
-00000420: 2044 7269 7665 2f50 7974 686f 6e2f 6d61   Drive/Python/ma
-00000430: 7074 6173 6b65 722f 6d61 7074 6173 6b65  ptasker/maptaske
-00000440: 722f 7372 632f 7072 6f67 696e 6974 2e70  r/src/proginit.p
-00000450: 79da 0c72 6561 645f 636f 756e 7465 7232  y..read_counter2
-00000460: 0000 0073 0a00 0000 100a 16ff 02ff 0203  ...s............
-00000470: 02fd 721b 0000 0063 0000 0000 0000 0000  ..r....c........
-00000480: 0000 0000 0100 0000 0800 0000 4300 0000  ............C...
-00000490: 733e 0000 0074 0074 0164 0183 028f 107d  s>...t.t.d.....}
-000004a0: 007c 00a0 0274 0374 0483 01a1 0101 0057  .|...t.t.......W
-000004b0: 0064 0204 0004 0083 0301 0064 0253 0031  .d.........d.S.1
-000004c0: 0073 1877 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
-000004d0: 0253 0029 037a 4857 7269 7465 2074 6865  .S.).zHWrite the
-000004e0: 2070 726f 6772 616d 2063 6f75 6e74 6572   program counter
-000004f0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00000500: 3a20 6e6f 6e65 0a0a 2020 2020 5265 7475  : none..    Retu
-00000510: 726e 733a 206e 6f6e 650a 0a20 2020 20da  rns: none..    .
-00000520: 0177 4e29 0572 1700 0000 720e 0000 00da  .wN).r....r.....
-00000530: 0577 7269 7465 7202 0000 00da 0b72 756e  .writer......run
-00000540: 5f63 6f75 6e74 6572 2901 da01 6672 1900  _counter)...fr..
-00000550: 0000 7219 0000 0072 1a00 0000 da0d 7772  ..r....r......wr
-00000560: 6974 655f 636f 756e 7465 7241 0000 0073  ite_counterA...s
-00000570: 0c00 0000 0c08 1001 0aff 0402 10fe 0402  ................
-00000580: 7220 0000 00da 0c70 726f 6772 616d 5f61  r .....program_a
-00000590: 7267 73da 0672 6574 7572 6e63 0100 0000  rgs..returnc....
-000005a0: 0000 0000 0000 0000 0700 0000 0800 0000  ................
-000005b0: 4300 0000 7302 0100 0074 00a0 0164 01a1  C...s....t...d..
-000005c0: 0101 0064 027d 0174 0283 007d 027c 02a0  ...d.}.t...}.|..
-000005d0: 0364 03a1 0101 007c 02a0 0464 04a1 0101  .d.....|...d....
-000005e0: 0064 007d 0374 05a0 06a1 007d 0474 00a0  .d.}.t.....}.t..
-000005f0: 0164 057c 049b 009d 02a1 0101 007c 0064  .d.|.........|.d
-00000600: 0619 0072 4f7a 0b74 077c 049b 0064 079d  ...rOz.t.|...d..
-00000610: 0264 0883 027d 0357 007c 0353 0004 0074  .d...}.W.|.S...t
-00000620: 0879 4e01 0001 0001 0064 097c 049b 0064  .yN......d.|...d
-00000630: 0a9d 037d 0574 00a0 097c 05a1 0101 0074  ...}.t...|.....t
-00000640: 0a7c 0583 0101 0074 0b64 0b83 0101 0059  .|.....t.d.....Y
-00000650: 007c 0353 0077 007a 0c74 0c7c 0264 0864  .|.S.w.z.t.|.d.d
-00000660: 047c 0464 0c67 0164 0d8d 057d 0357 006e  .|.d.g.d...}.W.n
-00000670: 0b04 0074 0d79 6601 0001 0001 0064 0e7d  ...t.yf......d.}
-00000680: 0159 006e 0177 007c 0364 0075 0072 6d64  .Y.n.w.|.d.u.rmd
-00000690: 0e7d 017c 0172 7f64 0f7d 0674 0a7c 0683  .}.|.r.d.}.t.|..
-000006a0: 0101 0074 00a0 097c 06a1 0101 0074 0ea0  ...t...|.....t..
-000006b0: 0b64 10a1 0101 007c 0353 0029 114e da05  .d.....|.S.).N..
-000006c0: 656e 7472 7946 5a07 3230 3078 3130 307a  entryFZ.200x100z
-000006d0: 1d53 656c 6563 7420 5461 736b 6572 2062  .Select Tasker b
-000006e0: 6163 6b75 7020 786d 6c20 6669 6c65 7a0a  ackup xml filez.
-000006f0: 6469 725f 7061 7468 3a20 da05 6465 6275  dir_path: ..debu
-00000700: 677a 0b2f 6261 636b 7570 2e78 6d6c 7214  gz./backup.xmlr.
-00000710: 0000 007a 2c45 7272 6f72 3a20 5468 6520  ...z,Error: The 
-00000720: 6261 636b 7570 2e78 6d6c 2066 696c 6520  backup.xml file 
-00000730: 7761 7320 6e6f 7420 666f 756e 6420 696e  was not found in
-00000740: 207a 162e 2020 5072 6f67 7261 6d20 7465   z..  Program te
-00000750: 726d 696e 6174 6564 21e9 0300 0000 2902  rminated!.....).
-00000760: 7a09 584d 4c20 4669 6c65 737a 052a 2e78  z.XML Filesz.*.x
-00000770: 6d6c 2905 da06 7061 7265 6e74 da04 6d6f  ml)...parent..mo
-00000780: 6465 da05 7469 746c 655a 0a69 6e69 7469  de..titleZ.initi
-00000790: 616c 6469 725a 0966 696c 6574 7970 6573  aldirZ.filetypes
-000007a0: 547a 3042 6163 6b75 7020 6669 6c65 2073  Tz0Backup file s
-000007b0: 656c 6563 7469 6f6e 2063 616e 6365 6c6c  election cancell
-000007c0: 6564 2e20 2050 726f 6772 616d 2065 6e64  ed.  Program end
-000007d0: 6564 2ee9 0600 0000 290f 7211 0000 00da  ed......).r.....
-000007e0: 0469 6e66 6f5a 0254 6b5a 0867 656f 6d65  .infoZ.TkZ.geome
-000007f0: 7472 7972 2800 0000 7204 0000 00da 0363  tryr(...r......c
-00000800: 7764 7217 0000 00da 074f 5345 7272 6f72  wdr......OSError
-00000810: 7224 0000 00da 0570 7269 6e74 da04 6578  r$.....print..ex
-00000820: 6974 7207 0000 00da 0945 7863 6570 7469  itr......Excepti
-00000830: 6f6e da03 7379 7329 0772 2100 0000 5a0a  on..sys).r!...Z.
-00000840: 6669 6c65 5f65 7272 6f72 5a06 746b 726f  file_errorZ.tkro
-00000850: 6f74 da08 6669 6c65 6e61 6d65 5a08 6469  ot..filenameZ.di
-00000860: 725f 7061 7468 da09 6572 726f 725f 6d73  r_path..error_ms
-00000870: 675a 0e63 616e 6365 6c5f 6d65 7373 6167  gZ.cancel_messag
-00000880: 6572 1900 0000 7219 0000 0072 1a00 0000  er....r....r....
-00000890: da1c 6f70 656e 5f61 6e64 5f67 6574 5f62  ..open_and_get_b
-000008a0: 6163 6b75 705f 786d 6c5f 6669 6c65 5600  ackup_xml_fileV.
-000008b0: 0000 734e 0000 000a 0104 0106 020a 010a  ..sN............
-000008c0: 0104 0108 0310 0108 0102 0112 0104 1c0c  ................
-000008d0: e50a 0202 ff0a 0408 010a 0104 1402 e502  ................
-000008e0: 0902 0102 0102 0102 0102 0104 010a fb0c  ................
-000008f0: 0708 0102 ff08 0204 0104 0104 0108 010a  ................
-00000900: 010a 0104 0272 3300 0000 6300 0000 0000  .....r3...c.....
-00000910: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00000920: 0000 0073 1a00 0000 6900 7d00 7400 7206  ...s....i.}.t.r.
-00000930: 6401 6e01 6402 7d01 7401 7c01 7c00 8302  d.n.d.}.t.|.|...
-00000940: 5300 2903 7a51 0a20 2020 2053 6574 2075  S.).zQ.    Set u
-00000950: 7020 7468 6520 696e 6974 6961 6c20 636f  p the initial co
-00000960: 6c6f 7273 2074 6f20 7573 652e 0a20 2020  lors to use..   
-00000970: 2020 2020 203a 7265 7475 726e 3a20 636f       :return: co
-00000980: 6c6f 7220 6d61 7020 6469 6374 696f 6e61  lor map dictiona
-00000990: 7279 0a20 2020 205a 0444 6172 6b5a 054c  ry.    Z.DarkZ.L
-000009a0: 6967 6874 2902 720b 0000 0072 0a00 0000  ight).r....r....
-000009b0: 2902 da08 636f 6c6f 726d 6170 5a0a 6170  )...colormapZ.ap
-000009c0: 7065 6172 616e 6365 7219 0000 0072 1900  pearancer....r..
-000009d0: 0000 721a 0000 00da 0c73 6574 7570 5f63  ..r......setup_c
-000009e0: 6f6c 6f72 7386 0000 0073 0600 0000 0405  olors....s......
-000009f0: 0c02 0a01 7235 0000 0063 0000 0000 0000  ....r5...c......
-00000a00: 0000 0000 0000 0000 0000 0700 0000 4300  ..............C.
-00000a10: 0000 7326 0000 0074 006a 0164 0164 0264  ..s&...t.j.d.d.d
-00000a20: 0364 0474 006a 0264 058d 0501 0074 03a0  .d.t.j.d.....t..
-00000a30: 0474 056a 06a1 0101 0064 0053 0029 064e  .t.j.....d.S.).N
-00000a40: 7a0d 6d61 7074 6173 6b65 722e 6c6f 6772  z.maptasker.logr
-00000a50: 1c00 0000 7a45 2528 6173 6374 696d 6529  ....zE%(asctime)
-00000a60: 732c 2528 6d73 6563 7329 6420 2528 6c65  s,%(msecs)d %(le
-00000a70: 7665 6c6e 616d 6529 7320 2528 6e61 6d65  velname)s %(name
-00000a80: 2973 2025 2866 756e 634e 616d 6529 7320  )s %(funcName)s 
-00000a90: 2528 6d65 7373 6167 6529 737a 0825 483a  %(message)sz.%H:
-00000aa0: 254d 3a25 5329 0572 3100 0000 da08 6669  %M:%S).r1.....fi
-00000ab0: 6c65 6d6f 6465 da06 666f 726d 6174 da07  lemode..format..
-00000ac0: 6461 7465 666d 74da 056c 6576 656c 2907  datefmt..level).
-00000ad0: 7212 0000 00da 0b62 6173 6963 436f 6e66  r......basicConf
-00000ae0: 6967 da05 4445 4255 4772 1100 0000 722a  ig..DEBUGr....r*
-00000af0: 0000 0072 3000 0000 da0c 7665 7273 696f  ...r0.....versio
-00000b00: 6e5f 696e 666f 7219 0000 0072 1900 0000  n_infor....r....
-00000b10: 7219 0000 0072 1a00 0000 da0d 7365 7475  r....r......setu
-00000b20: 705f 6c6f 6767 696e 6794 0000 0073 1000  p_logging....s..
-00000b30: 0000 0401 0201 0201 0201 0201 0401 06fb  ................
-00000b40: 1007 723d 0000 0072 3400 0000 6302 0000  ..r=...r4...c...
-00000b50: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-00000b60: 0043 0000 0073 8c00 0000 7400 8300 0100  .C...s....t.....
-00000b70: 7401 a002 7403 9b00 6401 7404 7405 6a05  t...t...d.t.t.j.
-00000b80: a006 a100 8301 9b00 9d03 a101 0100 7401  ..............t.
-00000b90: a002 6402 7404 7407 6a08 8301 9b00 9d02  ..d.t.t.j.......
-00000ba0: a101 0100 7c00 a009 a100 4400 5d0e 5c02  ....|.....D.].\.
-00000bb0: 7d02 7d03 7401 a002 7c02 9b00 6403 7c03  }.}.t...|...d.|.
-00000bc0: 9b00 9d03 a101 0100 7121 7c01 a009 a100  ........q!|.....
-00000bd0: 4400 5d0f 5c02 7d02 7d03 7401 a002 6404  D.].\.}.}.t...d.
-00000be0: 7c02 9b00 6405 7c03 9b00 9d04 a101 0100  |...d.|.........
-00000bf0: 7134 6400 5300 2906 4efa 0120 7a09 7379  q4d.S.).N.. z.sy
-00000c00: 732e 6172 6776 3a7a 023a 207a 0d63 6f6c  s.argv:z.: z.col
-00000c10: 6f72 6d61 7020 666f 7220 7a08 2073 6574  ormap for z. set
-00000c20: 2074 6f20 290a 723d 0000 0072 1100 0000   to ).r=...r....
-00000c30: 722a 0000 0072 1000 0000 da03 7374 72da  r*...r......str.
-00000c40: 0864 6174 6574 696d 655a 036e 6f77 7230  .datetimeZ.nowr0
-00000c50: 0000 00da 0461 7267 76da 0569 7465 6d73  .....argv..items
-00000c60: 2904 7221 0000 0072 3400 0000 da03 6b65  ).r!...r4.....ke
-00000c70: 79da 0576 616c 7565 7219 0000 0072 1900  y..valuer....r..
-00000c80: 0000 721a 0000 00da 126c 6f67 5f73 7461  ..r......log_sta
-00000c90: 7274 7570 5f76 616c 7565 73a2 0000 0073  rtup_values....s
-00000ca0: 1000 0000 0601 1e01 1601 1001 1601 1001  ................
-00000cb0: 1801 04ff 7245 0000 00da 0b6f 7574 7075  ....rE.....outpu
-00000cc0: 745f 6c69 7374 6303 0000 0000 0000 0000  t_listc.........
-00000cd0: 0000 000b 0000 000a 0000 0043 0000 0073  ...........C...s
-00000ce0: ee00 0000 7400 6401 6b00 7210 7401 7310  ....t.d.k.r.t.s.
-00000cf0: 6402 7d03 6403 7d04 7402 a003 7c04 7c03  d.}.d.}.t...|.|.
-00000d00: a102 0100 7404 7c01 8301 7d05 7405 7c05  ....t.|...}.t.|.
-00000d10: 8301 5c03 7d06 7d07 7d08 7c07 6a06 6404  ..\.}.}.}.|.j.d.
-00000d20: 6b03 7239 6405 7d09 7407 a008 7c00 7c01  k.r9d.}.t...|.|.
-00000d30: 7c02 6406 7c09 a105 0100 7409 a00a 7c09  |.d.|.....t...|.
-00000d40: 9b00 6407 9d02 a101 0100 740b a00c 6408  ..d.......t...d.
-00000d50: a101 0100 6e23 6409 7c00 640a 1900 1700  ....n#d.|.d.....
-00000d60: 640b 1700 740d 7c00 640c 640d 640e 7c07  d...t.|.d.d.d.|.
-00000d70: 6a0e 640f 1900 9b00 6410 740f 9b00 6411  j.d.....d.t...d.
-00000d80: 9d05 6412 8305 1700 7d0a 7407 a008 7c00  ..d.....}.t...|.
-00000d90: 7c01 7c02 6406 7c0a a105 0100 7c01 6413  |.|.d.|.....|.d.
-00000da0: 1900 7266 7410 7c00 7c01 7c02 8303 0100  ..rft.|.|.|.....
-00000db0: 7407 a008 7c00 7c01 7c02 6401 640d a105  t...|.|.|.d.d...
-00000dc0: 0100 7c06 7c07 7c05 7c08 7c02 7c0a 6606  ..|.|.|.|.|.|.f.
-00000dd0: 5300 2914 6126 0100 000a 2020 2020 5065  S.).a&....    Pe
-00000de0: 7266 6f72 6d20 6261 7369 6320 7365 7475  rform basic setu
-00000df0: 700a 2020 2020 2020 2020 3a70 6172 616d  p.        :param
-00000e00: 2063 6f6c 6f72 6d61 703a 2063 6f6c 6f72   colormap: color
-00000e10: 7320 746f 2075 7365 2066 6f72 206f 7574  s to use for out
-00000e20: 7075 740a 2020 2020 2020 2020 3a70 6172  put.        :par
-00000e30: 616d 2070 726f 6772 616d 5f61 7267 733a  am program_args:
-00000e40: 2072 756e 7469 6d65 2061 7267 756d 656e   runtime argumen
-00000e50: 7473 0a20 2020 2020 2020 203a 7061 7261  ts.        :para
-00000e60: 6d20 6f75 7470 7574 5f6c 6973 743a 206c  m output_list: l
-00000e70: 696e 6573 206f 6620 6f75 7470 7574 2067  ines of output g
-00000e80: 656e 6572 6174 6564 2074 6875 7320 6661  enerated thus fa
-00000e90: 720a 2020 2020 2020 2020 3a72 6574 7572  r.        :retur
-00000ea0: 6e20 786d 6c20 7472 6565 2c20 786d 6c20  n xml tree, xml 
-00000eb0: 726f 6f74 2c20 616c 6c20 5461 736b 6572  root, all Tasker
-00000ec0: 2050 726f 6a65 6374 732f 5072 6f66 696c   Projects/Profil
-00000ed0: 6573 2f54 6173 6b73 2f53 6365 6e65 732c  es/Tasks/Scenes,
-00000ee0: 206f 7574 7075 7420 6c69 6e65 732c 2074   output lines, t
-00000ef0: 6865 2068 6561 6469 6e67 0a20 2020 2072  he heading.    r
-00000f00: 1500 0000 7a47 4c6f 6361 7465 2074 6865  ....zGLocate the
-00000f10: 2054 6173 6b65 7220 6261 636b 7570 2078   Tasker backup x
-00000f20: 6d6c 2066 696c 6520 746f 2075 7365 2074  ml file to use t
-00000f30: 6f20 6d61 7020 796f 7572 2054 6173 6b65  o map your Taske
-00000f40: 7220 656e 7669 726f 6e6d 656e 74da 094d  r environment..M
-00000f50: 6170 5461 736b 6572 5a0a 5461 736b 6572  apTaskerZ.Tasker
-00000f60: 4461 7461 7a34 596f 7520 6469 6420 6e6f  Dataz4You did no
-00000f70: 7420 7365 6c65 6374 2061 2054 6173 6b65  t select a Taske
-00000f80: 7220 6261 636b 7570 2058 4d4c 2066 696c  r backup XML fil
-00000f90: 652e 2e2e 6578 6974 2032 7201 0000 007a  e...exit 2r....z
-00000fa0: 0665 7869 7420 3372 2500 0000 7a45 3c68  .exit 3r%...zE<h
-00000fb0: 746d 6c3e 0a3c 6865 6164 3e0a 3c74 6974  tml>.<head>.<tit
-00000fc0: 6c65 3e4d 6170 5461 736b 6572 3c2f 7469  le>MapTasker</ti
-00000fd0: 746c 653e 0a3c 626f 6479 2073 7479 6c65  tle>.<body style
-00000fe0: 3d22 6261 636b 6772 6f75 6e64 2d63 6f6c  ="background-col
-00000ff0: 6f72 3ada 1062 6163 6b67 726f 756e 645f  or:..background_
-00001000: 636f 6c6f 727a 0322 3e0a 5a09 4c61 776e  colorz.">.Z.Lawn
-00001010: 4772 6565 6eda 007a 433c 623e 5461 736b  Green..zC<b>Task
-00001020: 6572 204d 6170 7069 6e67 2e2e 2e2e 2e2e  er Mapping......
-00001030: 2e2e 2e2e 2e2e 2e2e 2e2e 266e 6273 703b  ..........&nbsp;
-00001040: 266e 6273 703b 266e 6273 703b 5461 736b  &nbsp;&nbsp;Task
-00001050: 6572 2076 6572 7369 6f6e 3a20 5a02 7476  er version: Z.tv
-00001060: 7a2c 266e 6273 703b 266e 6273 703b 266e  z,&nbsp;&nbsp;&n
-00001070: 6273 703b 266e 6273 703b 4d61 702d 5461  bsp;&nbsp;Map-Ta
-00001080: 736b 6572 2076 6572 7369 6f6e 3a20 7a04  sker version: z.
-00001090: 3c2f 623e 5472 2400 0000 2911 721e 0000  </b>Tr$...).r...
-000010a0: 0072 0c00 0000 7206 0000 005a 0873 686f  .r....r....Z.sho
-000010b0: 7769 6e66 6f72 3300 0000 7213 0000 00da  winfor3...r.....
-000010c0: 0374 6167 da0c 6275 696c 645f 6f75 7470  .tag..build_outp
-000010d0: 7574 da09 6d79 5f6f 7574 7075 7472 1100  ut..my_outputr..
-000010e0: 0000 7224 0000 0072 3000 0000 722e 0000  ..r$...r0...r...
-000010f0: 0072 0900 0000 da06 6174 7472 6962 7210  .r......attribr.
-00001100: 0000 0072 0d00 0000 290b 7234 0000 0072  ...r....).r4...r
-00001110: 2100 0000 7246 0000 00da 036d 7367 7228  !...rF.....msgr(
-00001120: 0000 0072 3100 0000 da04 7472 6565 da04  ...r1.....tree..
-00001130: 726f 6f74 da10 616c 6c5f 7461 736b 6572  root..all_tasker
-00001140: 5f69 7465 6d73 7232 0000 00da 0768 6561  _itemsr2.....hea
-00001150: 6469 6e67 7219 0000 0072 1900 0000 721a  dingr....r....r.
-00001160: 0000 00da 0573 6574 7570 af00 0000 7344  .....setup....sD
-00001170: 0000 000c 0c04 0104 010c 0108 030e 030a  ................
-00001180: 0304 0112 0110 010c 0102 0406 0102 ff02  ................
-00001190: 0202 fe02 0302 0102 0102 0102 0208 0104  ................
-000011a0: ff02 0206 fe02 0402 f702 fd02 ff12 1108  ................
-000011b0: 030c 0112 0310 0272 5300 0000 6301 0000  .......rS...c...
-000011c0: 0000 0000 0000 0000 0009 0000 0009 0000  ................
-000011d0: 0043 0000 0073 aa00 0000 7400 8300 7d01  .C...s....t...}.
-000011e0: 7401 a002 6401 7403 7404 6a05 8301 9b00  t...d.t.t.j.....
-000011f0: 9d02 a101 0100 7406 a007 a100 0100 7408  ......t.......t.
-00001200: a009 7c01 a101 5c02 7d02 7d01 740a 7c01  ..|...\.}.}.t.|.
-00001210: 7c02 7c00 8303 5c06 7d03 7d04 7d05 7d06  |.|...\.}.}.}.}.
-00001220: 7d00 7d07 7c02 6402 1900 722e 740b 7c02  }.}.|.d...r.t.|.
-00001230: 7c01 8302 0100 7c02 6403 1900 723f 7401  |.....|.d...r?t.
-00001240: a00c 6404 7c02 6403 1900 1700 a101 0100  ..d.|.d.........
-00001250: 6405 7c02 6406 3c00 6407 6407 6407 6408  d.|.d.<.d.d.d.d.
-00001260: 9c03 7d08 7401 a002 6409 a101 0100 7c01  ..}.t...d.....|.
-00001270: 7c02 7c08 7c07 7c00 7c03 7c04 7c05 7c06  |.|.|.|.|.|.|.|.
-00001280: 6609 5300 290a 7a48 0a20 2020 2049 6e69  f.S.).zH.    Ini
-00001290: 7469 616c 697a 6520 7072 6f67 7261 6d20  tialize program 
-000012a0: 7661 7269 6162 6c65 730a 2020 2020 2020  variables.      
-000012b0: 2020 3a74 7970 6520 6f75 7470 7574 5f6c    :type output_l
-000012c0: 6973 743a 2074 7570 6c65 5b0a 2020 2020  ist: tuple[.    
-000012d0: 7a08 7379 732e 6172 6776 7224 0000 00da  z.sys.argvr$....
-000012e0: 1073 696e 676c 655f 7461 736b 5f6e 616d  .single_task_nam
-000012f0: 657a 0c53 696e 676c 6520 5461 736b 3d72  ez.Single Task=r
-00001300: 2500 0000 da14 6469 7370 6c61 795f 6465  %.....display_de
-00001310: 7461 696c 5f6c 6576 656c 4629 03da 1473  tail_levelF)...s
-00001320: 696e 676c 655f 7072 6f6a 6563 745f 666f  ingle_project_fo
-00001330: 756e 64da 1473 696e 676c 655f 7072 6f66  und..single_prof
-00001340: 696c 655f 666f 756e 64da 1173 696e 676c  ile_found..singl
-00001350: 655f 7461 736b 5f66 6f75 6e64 722e 0000  e_task_foundr...
-00001360: 0029 0d72 3500 0000 7211 0000 0072 2a00  .).r5...r....r*.
-00001370: 0000 723f 0000 0072 3000 0000 7241 0000  ..r?...r0...rA..
-00001380: 00da 0a6f 6c64 5f74 6f5f 6e65 77da 076d  ...old_to_new..m
-00001390: 6967 7261 7465 da08 6765 745f 6172 6773  igrate..get_args
-000013a0: 5a15 6765 745f 7072 6f67 7261 6d5f 6172  Z.get_program_ar
-000013b0: 6775 6d65 6e74 7372 5300 0000 7245 0000  gumentsrS...rE..
-000013c0: 0072 2400 0000 2909 7246 0000 0072 3400  .r$...).rF...r4.
-000013d0: 0000 7221 0000 0072 4f00 0000 7250 0000  ..r!...rO...rP..
-000013e0: 0072 3100 0000 7251 0000 0072 5200 0000  .r1...rQ...rR...
-000013f0: da0b 666f 756e 645f 6974 656d 7372 1900  ..found_itemsr..
-00001400: 0000 7219 0000 0072 1a00 0000 da08 7374  ..r....r......st
-00001410: 6172 745f 7570 ee00 0000 7336 0000 0006  art_up....s6....
-00001420: 0516 0308 030e 0302 0306 0110 ff08 050a  ................
-00001430: 0108 0312 0108 0102 0402 0102 0106 fd0a  ................
-00001440: 0502 0202 0102 0102 0102 0102 0102 0102  ................
-00001450: 0102 0104 f772 5d00 0000 2938 da06 6174  .....r]...)8..at
-00001460: 6578 6974 7240 0000 0072 3000 0000 5a04  exitr@...r0...Z.
-00001470: 6a73 6f6e 7202 0000 0072 0300 0000 5a07  jsonr....r....Z.
-00001480: 7061 7468 6c69 6272 0400 0000 5a07 746b  pathlibr....Z.tk
-00001490: 696e 7465 7272 0600 0000 5a12 746b 696e  interr....Z.tkin
-000014a0: 7465 722e 6669 6c65 6469 616c 6f67 7207  ter.filedialogr.
-000014b0: 0000 00da 0674 7970 696e 6772 0800 0000  .....typingr....
-000014c0: 5a15 6d61 7074 6173 6b65 722e 7372 632e  Z.maptasker.src.
-000014d0: 6d69 6772 6174 65da 0373 7263 725a 0000  migrate..srcrZ..
-000014e0: 0072 5900 0000 da15 6d61 7074 6173 6b65  .rY.....maptaske
-000014f0: 722e 7372 632e 6f75 7470 7574 6cda 076f  r.src.outputl..o
-00001500: 7574 7075 746c 724b 0000 005a 166d 6170  utputlrK...Z.map
-00001510: 7461 736b 6572 2e73 7263 2e70 726f 6761  tasker.src.proga
-00001520: 7267 735a 0870 726f 6761 7267 7372 5b00  rgsZ.progargsr[.
-00001530: 0000 da16 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
-00001540: 632e 6672 6d74 6874 6d6c 7209 0000 005a  c.frmthtmlr....Z
-00001550: 166d 6170 7461 736b 6572 2e73 7263 2e63  .maptasker.src.c
-00001560: 6f6c 726d 6f64 6572 0a00 0000 da14 6d61  olrmoder......ma
-00001570: 7074 6173 6b65 722e 7372 632e 636f 6e66  ptasker.src.conf
-00001580: 6967 720b 0000 0072 0c00 0000 da13 6d61  igr....r......ma
-00001590: 7074 6173 6b65 722e 7372 632e 6465 6275  ptasker.src.debu
-000015a0: 6772 0d00 0000 da16 6d61 7074 6173 6b65  gr......maptaske
-000015b0: 722e 7372 632e 7379 7363 6f6e 7374 720e  r.src.sysconstr.
-000015c0: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
-000015d0: 0000 7212 0000 005a 156d 6170 7461 736b  ..r....Z.maptask
-000015e0: 6572 2e73 7263 2e74 6173 6b65 7264 7213  er.src.taskerdr.
-000015f0: 0000 0072 1b00 0000 7220 0000 0072 1e00  ...r....r ...r..
-00001600: 0000 da08 7265 6769 7374 6572 da04 6469  ....register..di
-00001610: 6374 da06 6f62 6a65 6374 7233 0000 0072  ct..objectr3...r
-00001620: 3500 0000 723d 0000 0072 4500 0000 da04  5...r=...rE.....
-00001630: 6c69 7374 da05 7475 706c 6572 3f00 0000  list..tupler?...
-00001640: 7253 0000 0072 5d00 0000 7219 0000 0072  rS...r]...r....r
-00001650: 1900 0000 7219 0000 0072 1a00 0000 da08  ....r....r......
-00001660: 3c6d 6f64 756c 653e 0100 0000 7352 0000  <module>....sR..
-00001670: 0008 0e08 0108 0110 010c 0108 030c 010c  ................
-00001680: 040c 0112 0212 0112 010c 010c 010c 010c  ................
-00001690: 010c 010c 010c 010c 010c 010c 010c 0108  ................
-000016a0: 0708 0f06 0d0a 0112 070e 3008 0e16 0e02  ..........0.....
-000016b0: 0d02 0102 ff02 0102 ff02 0102 ff12 020a  ................
-000016c0: fe16 3f                                  ..?
+000002c0: 6461 7461 2901 da0d 6572 726f 725f 6861  data)...error_ha
+000002d0: 6e64 6c65 7263 0000 0000 0000 0000 0000  ndlerc..........
+000002e0: 0000 0000 0000 0400 0000 4300 0000 732c  ..........C...s,
+000002f0: 0000 0074 00a0 0174 0074 0283 01a0 03a1  ...t...t.t......
+00000300: 00a1 0172 1474 0474 0574 0264 0183 02a0  ...r.t.t.t.d....
+00000310: 06a1 0083 0164 0217 0053 0064 0353 0029  .....d...S.d.S.)
+00000320: 047a c852 6561 6420 7468 6520 7072 6f67  .z.Read the prog
+00000330: 7261 6d20 636f 756e 7465 720a 2020 2020  ram counter.    
+00000340: 4765 7420 7468 6520 636f 756e 7420 6f66  Get the count of
+00000350: 2074 6865 206e 756d 6265 7220 6f66 2074   the number of t
+00000360: 696d 6573 204d 6170 5461 736b 6572 2068  imes MapTasker h
+00000370: 6173 2062 6565 6e20 6361 6c6c 6564 0a20  as been called. 
+00000380: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00000390: 733a 206e 6f6e 650a 2020 2020 2020 2020  s: none.        
+000003a0: 5265 7475 726e 733a 2074 6865 2063 6f75  Returns: the cou
+000003b0: 6e74 206f 6620 7468 6520 6e75 6d62 6572  nt of the number
+000003c0: 206f 6620 7469 6d65 7320 7468 6520 7072   of times the pr
+000003d0: 6f67 7261 6d20 6861 7320 6265 656e 2063  ogram has been c
+000003e0: 616c 6c65 640a 0a20 2020 20da 0172 e901  alled..    ..r..
+000003f0: 0000 0072 0100 0000 2907 7204 0000 00da  ...r....).r.....
+00000400: 0665 7869 7374 7372 0e00 0000 5a07 7265  .existsr....Z.re
+00000410: 736f 6c76 6572 0300 0000 da04 6f70 656e  solver......open
+00000420: da04 7265 6164 a900 7219 0000 0072 1900  ..read..r....r..
+00000430: 0000 fa77 2f55 7365 7273 2f6d 696b 7275  ...w/Users/mikru
+00000440: 6269 6e2f 4c69 6272 6172 792f 436c 6f75  bin/Library/Clou
+00000450: 6453 746f 7261 6765 2f47 6f6f 676c 6544  dStorage/GoogleD
+00000460: 7269 7665 2d6d 696b 7275 6269 6e40 676d  rive-mikrubin@gm
+00000470: 6169 6c2e 636f 6d2f 4d79 2044 7269 7665  ail.com/My Drive
+00000480: 2f50 7974 686f 6e2f 6d61 7074 6173 6b65  /Python/maptaske
+00000490: 722f 6d61 7074 6173 6b65 722f 7372 632f  r/maptasker/src/
+000004a0: 7072 6f67 696e 6974 2e70 79da 0c72 6561  proginit.py..rea
+000004b0: 645f 636f 756e 7465 7232 0000 0073 0a00  d_counter2...s..
+000004c0: 0000 1009 16ff 02ff 0203 02fd 721b 0000  ............r...
+000004d0: 0063 0000 0000 0000 0000 0000 0000 0100  .c..............
+000004e0: 0000 0800 0000 4300 0000 733e 0000 0074  ......C...s>...t
+000004f0: 0074 0164 0183 028f 107d 007c 00a0 0274  .t.d.....}.|...t
+00000500: 0374 0483 01a1 0101 0057 0064 0204 0004  .t.......W.d....
+00000510: 0083 0301 0064 0253 0031 0073 1877 0101  .....d.S.1.s.w..
+00000520: 0001 0001 0059 0001 0064 0253 0029 037a  .....Y...d.S.).z
+00000530: 8a57 7269 7465 2074 6865 2070 726f 6772  .Write the progr
+00000540: 616d 2063 6f75 6e74 6572 0a20 2020 2057  am counter.    W
+00000550: 7269 7465 206f 7574 2074 6865 206e 756d  rite out the num
+00000560: 6265 7220 6f66 2074 696d 6573 204d 6170  ber of times Map
+00000570: 5461 736b 6572 2068 6173 2062 6565 6e20  Tasker has been 
+00000580: 6361 6c6c 6564 0a20 2020 2020 2020 2050  called.        P
+00000590: 6172 616d 6574 6572 733a 206e 6f6e 650a  arameters: none.
+000005a0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+000005b0: 206e 6f6e 650a 0a20 2020 20da 0177 4e29   none..    ..wN)
+000005c0: 0572 1700 0000 720e 0000 00da 0577 7269  .r....r......wri
+000005d0: 7465 7202 0000 00da 0b72 756e 5f63 6f75  ter......run_cou
+000005e0: 6e74 6572 2901 da01 6672 1900 0000 7219  nter)...fr....r.
+000005f0: 0000 0072 1a00 0000 da0d 7772 6974 655f  ...r......write_
+00000600: 636f 756e 7465 7240 0000 0073 0c00 0000  counter@...s....
+00000610: 0c07 1001 0aff 0402 10fe 0402 7220 0000  ............r ..
+00000620: 00da 0c70 726f 6772 616d 5f61 7267 73da  ...program_args.
+00000630: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
+00000640: 0000 0000 0600 0000 0800 0000 4300 0000  ............C...
+00000650: 730c 0100 0074 00a0 0164 01a1 0101 0064  s....t...d.....d
+00000660: 027d 0174 0283 007d 027c 02a0 0364 03a1  .}.t...}.|...d..
+00000670: 0101 007c 02a0 0464 04a1 0101 0064 057d  ...|...d.....d.}
+00000680: 0374 05a0 06a1 007d 0474 00a0 0164 067c  .t.....}.t...d.|
+00000690: 049b 009d 02a1 0101 007c 0064 0719 0072  .........|.d...r
+000006a0: 437a 0a74 077c 049b 0064 089d 0264 0983  Cz.t.|...d...d..
+000006b0: 027d 0357 006e 4e04 0074 0879 4201 0001  .}.W.nN..t.yB...
+000006c0: 0001 0074 0964 0a7c 049b 0064 0b9d 0364  ...t.d.|...d...d
+000006d0: 0c83 0201 0059 006e 3d77 007c 0064 0d19  .....Y.n=w.|.d..
+000006e0: 0072 4f74 077c 0064 0d19 0064 0983 027d  .rOt.|.d...d...}
+000006f0: 036e 307a 0c74 0a7c 0264 0964 047c 0464  .n0z.t.|.d.d.|.d
+00000700: 0e67 0164 0f8d 057d 0357 006e 0b04 0074  .g.d...}.W.n...t
+00000710: 0b79 6601 0001 0001 0064 107d 0159 006e  .yf......d.}.Y.n
+00000720: 0177 007c 0364 0575 0072 6d64 107d 017c  .w.|.d.u.rmd.}.|
+00000730: 0172 7f64 117d 0574 0c7c 0583 0101 0074  .r.d.}.t.|.....t
+00000740: 00a0 0d7c 05a1 0101 0074 0ea0 0f64 12a1  ...|.....t...d..
+00000750: 0101 007c 02a0 10a1 0001 007e 027c 0353  ...|.......~.|.S
+00000760: 0029 137a 9a0a 2020 2020 4f70 656e 2074  .).z..    Open t
+00000770: 6865 2054 6173 6b65 7220 6261 636b 7570  he Tasker backup
+00000780: 2066 696c 6520 616e 6420 7265 7475 726e   file and return
+00000790: 2074 6865 2066 696c 6520 6f62 6a65 6374   the file object
+000007a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000007b0: 7072 6f67 7261 6d5f 6172 6773 3a20 7275  program_args: ru
+000007c0: 6e74 696d 6520 6172 6775 6d65 6e74 730a  ntime arguments.
+000007d0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+000007e0: 2054 6173 6b65 7220 6261 636b 7570 2066   Tasker backup f
+000007f0: 696c 6520 6f62 6a65 6374 0a20 2020 20da  ile object.    .
+00000800: 0565 6e74 7279 465a 0732 3030 7831 3030  .entryFZ.200x100
+00000810: 7a1d 5365 6c65 6374 2054 6173 6b65 7220  z.Select Tasker 
+00000820: 6261 636b 7570 2078 6d6c 2066 696c 654e  backup xml fileN
+00000830: 7a0a 6469 725f 7061 7468 3a20 da05 6465  z.dir_path: ..de
+00000840: 6275 677a 0b2f 6261 636b 7570 2e78 6d6c  bugz./backup.xml
+00000850: 7214 0000 007a 2c45 7272 6f72 3a20 5468  r....z,Error: Th
+00000860: 6520 6261 636b 7570 2e78 6d6c 2066 696c  e backup.xml fil
+00000870: 6520 7761 7320 6e6f 7420 666f 756e 6420  e was not found 
+00000880: 696e 207a 162e 2020 5072 6f67 7261 6d20  in z..  Program 
+00000890: 7465 726d 696e 6174 6564 21e9 0300 0000  terminated!.....
+000008a0: da04 6669 6c65 2902 7a09 584d 4c20 4669  ..file).z.XML Fi
+000008b0: 6c65 737a 052a 2e78 6d6c 2905 da06 7061  lesz.*.xml)...pa
+000008c0: 7265 6e74 da04 6d6f 6465 da05 7469 746c  rent..mode..titl
+000008d0: 655a 0a69 6e69 7469 616c 6469 725a 0966  eZ.initialdirZ.f
+000008e0: 696c 6574 7970 6573 547a 3042 6163 6b75  iletypesTz0Backu
+000008f0: 7020 6669 6c65 2073 656c 6563 7469 6f6e  p file selection
+00000900: 2063 616e 6365 6c6c 6564 2e20 2050 726f   cancelled.  Pro
+00000910: 6772 616d 2065 6e64 6564 2ee9 0600 0000  gram ended......
+00000920: 2911 7210 0000 00da 0469 6e66 6f72 0500  ).r......infor..
+00000930: 0000 5a08 6765 6f6d 6574 7279 7229 0000  ..Z.geometryr)..
+00000940: 0072 0400 0000 da03 6377 6472 1700 0000  .r......cwdr....
+00000950: da07 4f53 4572 726f 7272 1300 0000 7207  ..OSErrorr....r.
+00000960: 0000 00da 0945 7863 6570 7469 6f6e da05  .....Exception..
+00000970: 7072 696e 7472 2400 0000 da03 7379 73da  printr$.....sys.
+00000980: 0465 7869 745a 0764 6573 7472 6f79 2906  .exitZ.destroy).
+00000990: 7221 0000 005a 0a66 696c 655f 6572 726f  r!...Z.file_erro
+000009a0: 725a 0674 6b72 6f6f 74da 0866 696c 656e  rZ.tkroot..filen
+000009b0: 616d 655a 0864 6972 5f70 6174 685a 0e63  ameZ.dir_pathZ.c
+000009c0: 616e 6365 6c5f 6d65 7373 6167 6572 1900  ancel_messager..
+000009d0: 0000 7219 0000 0072 1a00 0000 da1c 6f70  ..r....r......op
+000009e0: 656e 5f61 6e64 5f67 6574 5f62 6163 6b75  en_and_get_backu
+000009f0: 705f 786d 6c5f 6669 6c65 5400 0000 7350  p_xml_fileT...sP
+00000a00: 0000 000a 0604 0106 020a 010a 0104 0108  ................
+00000a10: 0310 0108 0102 0114 010c 0102 010a 0202  ................
+00000a20: 0308 fb02 ff08 0910 0202 0302 0102 0102  ................
+00000a30: 0102 0102 0104 010a fb0c 0708 0102 ff08  ................
+00000a40: 0204 0104 0104 0108 010a 010a 0108 0102  ................
+00000a50: 0104 0272 3300 0000 6300 0000 0000 0000  ...r3...c.......
+00000a60: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000a70: 0073 1a00 0000 6900 7d00 7400 7206 6401  .s....i.}.t.r.d.
+00000a80: 6e01 6402 7d01 7401 7c01 7c00 8302 5300  n.d.}.t.|.|...S.
+00000a90: 2903 7a51 0a20 2020 2053 6574 2075 7020  ).zQ.    Set up 
+00000aa0: 7468 6520 696e 6974 6961 6c20 636f 6c6f  the initial colo
+00000ab0: 7273 2074 6f20 7573 652e 0a20 2020 2020  rs to use..     
+00000ac0: 2020 203a 7265 7475 726e 3a20 636f 6c6f     :return: colo
+00000ad0: 7220 6d61 7020 6469 6374 696f 6e61 7279  r map dictionary
+00000ae0: 0a20 2020 205a 0444 6172 6b5a 054c 6967  .    Z.DarkZ.Lig
+00000af0: 6874 2902 720b 0000 0072 0a00 0000 2902  ht).r....r....).
+00000b00: da08 636f 6c6f 726d 6170 5a0a 6170 7065  ..colormapZ.appe
+00000b10: 6172 616e 6365 7219 0000 0072 1900 0000  arancer....r....
+00000b20: 721a 0000 00da 0c73 6574 7570 5f63 6f6c  r......setup_col
+00000b30: 6f72 7390 0000 0073 0600 0000 0405 0c02  ors....s........
+00000b40: 0a01 7235 0000 0063 0000 0000 0000 0000  ..r5...c........
+00000b50: 0000 0000 0000 0000 0700 0000 4300 0000  ............C...
+00000b60: 7326 0000 0074 006a 0164 0164 0264 0364  s&...t.j.d.d.d.d
+00000b70: 0474 006a 0264 058d 0501 0074 03a0 0474  .t.j.d.....t...t
+00000b80: 056a 06a1 0101 0064 0653 0029 077a 510a  .j.....d.S.).zQ.
+00000b90: 2020 2020 5365 7420 7570 2074 6865 206c      Set up the l
+00000ba0: 6f67 6769 6e67 3a20 6e61 6d65 2074 6865  ogging: name the
+00000bb0: 2066 696c 6520 616e 6420 6573 7461 626c   file and establ
+00000bc0: 6973 6820 7468 6520 6c6f 6720 7479 7065  ish the log type
+00000bd0: 2061 6e64 2066 6f72 6d61 740a 2020 2020   and format.    
+00000be0: 7a0d 6d61 7074 6173 6b65 722e 6c6f 6772  z.maptasker.logr
+00000bf0: 1c00 0000 7a45 2528 6173 6374 696d 6529  ....zE%(asctime)
+00000c00: 732c 2528 6d73 6563 7329 6420 2528 6c65  s,%(msecs)d %(le
+00000c10: 7665 6c6e 616d 6529 7320 2528 6e61 6d65  velname)s %(name
+00000c20: 2973 2025 2866 756e 634e 616d 6529 7320  )s %(funcName)s 
+00000c30: 2528 6d65 7373 6167 6529 737a 0825 483a  %(message)sz.%H:
+00000c40: 254d 3a25 5329 0572 3200 0000 da08 6669  %M:%S).r2.....fi
+00000c50: 6c65 6d6f 6465 da06 666f 726d 6174 da07  lemode..format..
+00000c60: 6461 7465 666d 74da 056c 6576 656c 4e29  datefmt..levelN)
+00000c70: 0772 1100 0000 da0b 6261 7369 6343 6f6e  .r......basicCon
+00000c80: 6669 67da 0544 4542 5547 7210 0000 0072  fig..DEBUGr....r
+00000c90: 2b00 0000 7230 0000 00da 0c76 6572 7369  +...r0.....versi
+00000ca0: 6f6e 5f69 6e66 6f72 1900 0000 7219 0000  on_infor....r...
+00000cb0: 0072 1900 0000 721a 0000 00da 0d73 6574  .r....r......set
+00000cc0: 7570 5f6c 6f67 6769 6e67 9e00 0000 7310  up_logging....s.
+00000cd0: 0000 0004 0402 0102 0102 0102 0104 0106  ................
+00000ce0: fb10 0772 3d00 0000 7234 0000 0063 0200  ...r=...r4...c..
+00000cf0: 0000 0000 0000 0000 0000 0400 0000 0700  ................
+00000d00: 0000 4300 0000 738c 0000 0074 0083 0001  ..C...s....t....
+00000d10: 0074 01a0 0274 039b 0064 0174 0474 056a  .t...t...d.t.t.j
+00000d20: 05a0 06a1 0083 019b 009d 03a1 0101 0074  ...............t
+00000d30: 01a0 0264 0274 0474 076a 0883 019b 009d  ...d.t.t.j......
+00000d40: 02a1 0101 007c 00a0 09a1 0044 005d 0e5c  .....|.....D.].\
+00000d50: 027d 027d 0374 01a0 027c 029b 0064 037c  .}.}.t...|...d.|
+00000d60: 039b 009d 03a1 0101 0071 217c 01a0 09a1  .........q!|....
+00000d70: 0044 005d 0f5c 027d 027d 0374 01a0 0264  .D.].\.}.}.t...d
+00000d80: 047c 029b 0064 057c 039b 009d 04a1 0101  .|...d.|........
+00000d90: 0071 3464 0653 0029 077a 880a 2020 2020  .q4d.S.).z..    
+00000da0: 4c6f 6720 7468 6520 7275 6e74 696d 6520  Log the runtime 
+00000db0: 6172 6775 6d65 6e74 730a 2020 2020 2020  arguments.      
+00000dc0: 2020 3a70 6172 616d 2070 726f 6772 616d    :param program
+00000dd0: 5f61 7267 733a 2072 756e 7472 696d 6520  _args: runtrime 
+00000de0: 6172 6775 6d65 6e74 730a 2020 2020 2020  arguments.      
+00000df0: 2020 3a70 6172 616d 2063 6f6c 6f72 6d61    :param colorma
+00000e00: 703a 2063 6f6c 6f72 7320 746f 2075 7365  p: colors to use
+00000e10: 2069 6e20 7468 6520 6f75 7470 7574 0a20   in the output. 
+00000e20: 2020 20da 0120 7a09 7379 732e 6172 6776     .. z.sys.argv
+00000e30: 3a7a 023a 207a 0d63 6f6c 6f72 6d61 7020  :z.: z.colormap 
+00000e40: 666f 7220 7a08 2073 6574 2074 6f20 4e29  for z. set to N)
+00000e50: 0a72 3d00 0000 7210 0000 0072 2b00 0000  .r=...r....r+...
+00000e60: 720f 0000 00da 0373 7472 da08 6461 7465  r......str..date
+00000e70: 7469 6d65 5a03 6e6f 7772 3000 0000 da04  timeZ.nowr0.....
+00000e80: 6172 6776 da05 6974 656d 7329 0472 2100  argv..items).r!.
+00000e90: 0000 7234 0000 00da 036b 6579 da05 7661  ..r4.....key..va
+00000ea0: 6c75 6572 1900 0000 7219 0000 0072 1a00  luer....r....r..
+00000eb0: 0000 da12 6c6f 675f 7374 6172 7475 705f  ....log_startup_
+00000ec0: 7661 6c75 6573 af00 0000 7310 0000 0006  values....s.....
+00000ed0: 061e 0116 0110 0116 0110 0118 0104 ff72  ...............r
+00000ee0: 4500 0000 da0b 6f75 7470 7574 5f6c 6973  E.....output_lis
+00000ef0: 74da 0b66 696c 655f 746f 5f67 6574 6304  t..file_to_getc.
+00000f00: 0000 0000 0000 0000 0000 000b 0000 000a  ................
+00000f10: 0000 0043 0000 0073 f600 0000 7c03 7c01  ...C...s....|.|.
+00000f20: 6401 3c00 7c03 7314 7400 6402 6b00 7214  d.<.|.s.t.d.k.r.
+00000f30: 7401 7314 6403 7d04 7402 a003 6404 7c04  t.s.d.}.t...d.|.
+00000f40: a102 0100 7404 7c01 8301 7d05 7405 7c05  ....t.|...}.t.|.
+00000f50: 8301 5c03 7d06 7d07 7d08 7c07 6a06 6405  ..\.}.}.}.|.j.d.
+00000f60: 6b03 723d 6406 7d09 7407 a008 7c00 7c01  k.r=d.}.t...|.|.
+00000f70: 7c02 6407 7c09 a105 0100 7409 a00a 7c09  |.d.|.....t...|.
+00000f80: 9b00 6408 9d02 a101 0100 740b a00c 6409  ..d.......t...d.
+00000f90: a101 0100 6e23 640a 7c00 640b 1900 9b00  ....n#d.|.d.....
+00000fa0: 640c 9d03 740d 7c00 640d 640e 640f 7c07  d...t.|.d.d.d.|.
+00000fb0: 6a0e 6410 1900 9b00 6411 740f 9b00 6412  j.d.....d.t...d.
+00000fc0: 9d05 6413 8305 1700 7d0a 7407 a008 7c00  ..d.....}.t...|.
+00000fd0: 7c01 7c02 6407 7c0a a105 0100 7c01 6414  |.|.d.|.....|.d.
+00000fe0: 1900 726a 7410 7c00 7c01 7c02 8303 0100  ..rjt.|.|.|.....
+00000ff0: 7407 a008 7c00 7c01 7c02 6402 640e a105  t...|.|.|.d.d...
+00001000: 0100 7c06 7c07 7c05 7c08 7c02 7c0a 6606  ..|.|.|.|.|.|.f.
+00001010: 5300 2915 6184 0100 000a 2020 2020 5065  S.).a.....    Pe
+00001020: 7266 6f72 6d20 6261 7369 6320 7365 7475  rform basic setu
+00001030: 700a 2020 2020 2020 2020 3a70 6172 616d  p.        :param
+00001040: 2063 6f6c 6f72 6d61 703a 2063 6f6c 6f72   colormap: color
+00001050: 7320 746f 2075 7365 2066 6f72 206f 7574  s to use for out
+00001060: 7075 740a 2020 2020 2020 2020 3a70 6172  put.        :par
+00001070: 616d 2070 726f 6772 616d 5f61 7267 733a  am program_args:
+00001080: 2072 756e 7469 6d65 2061 7267 756d 656e   runtime argumen
+00001090: 7473 0a20 2020 2020 2020 203a 7061 7261  ts.        :para
+000010a0: 6d20 6f75 7470 7574 5f6c 6973 743a 206c  m output_list: l
+000010b0: 696e 6573 206f 6620 6f75 7470 7574 2067  ines of output g
+000010c0: 656e 6572 6174 6564 2074 6875 7320 6661  enerated thus fa
+000010d0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
+000010e0: 2066 696c 655f 746f 5f67 6574 3a20 6669   file_to_get: fi
+000010f0: 6c65 206f 626a 6563 7420 2869 6620 6669  le object (if fi
+00001100: 6c65 2061 6c72 6561 6479 2064 6566 696e  le already defin
+00001110: 6564 2c20 646f 6e27 7420 7072 6f6d 7074  ed, don't prompt
+00001120: 2075 7365 7229 2c20 6f72 204e 6f6e 650a   user), or None.
+00001130: 2020 2020 2020 2020 3a72 6574 7572 6e20          :return 
+00001140: 786d 6c20 7472 6565 2c20 786d 6c20 726f  xml tree, xml ro
+00001150: 6f74 2c20 616c 6c20 5461 736b 6572 2050  ot, all Tasker P
+00001160: 726f 6a65 6374 732f 5072 6f66 696c 6573  rojects/Profiles
+00001170: 2f54 6173 6b73 2f53 6365 6e65 732c 206f  /Tasks/Scenes, o
+00001180: 7574 7075 7420 6c69 6e65 732c 2074 6865  utput lines, the
+00001190: 2068 6561 6469 6e67 0a20 2020 2072 2600   heading.    r&.
+000011a0: 0000 7215 0000 007a 474c 6f63 6174 6520  ..r....zGLocate 
+000011b0: 7468 6520 5461 736b 6572 2062 6163 6b75  the Tasker backu
+000011c0: 7020 786d 6c20 6669 6c65 2074 6f20 7573  p xml file to us
+000011d0: 6520 746f 206d 6170 2079 6f75 7220 5461  e to map your Ta
+000011e0: 736b 6572 2065 6e76 6972 6f6e 6d65 6e74  sker environment
+000011f0: da09 4d61 7054 6173 6b65 725a 0a54 6173  ..MapTaskerZ.Tas
+00001200: 6b65 7244 6174 617a 3459 6f75 2064 6964  kerDataz4You did
+00001210: 206e 6f74 2073 656c 6563 7420 6120 5461   not select a Ta
+00001220: 736b 6572 2062 6163 6b75 7020 584d 4c20  sker backup XML 
+00001230: 6669 6c65 2e2e 2e65 7869 7420 3272 0100  file...exit 2r..
+00001240: 0000 7a06 6578 6974 2033 7225 0000 007a  ..z.exit 3r%...z
+00001250: 453c 6874 6d6c 3e0a 3c68 6561 643e 0a3c  E<html>.<head>.<
+00001260: 7469 746c 653e 4d61 7054 6173 6b65 723c  title>MapTasker<
+00001270: 2f74 6974 6c65 3e0a 3c62 6f64 7920 7374  /title>.<body st
+00001280: 796c 653d 2262 6163 6b67 726f 756e 642d  yle="background-
+00001290: 636f 6c6f 723a da10 6261 636b 6772 6f75  color:..backgrou
+000012a0: 6e64 5f63 6f6c 6f72 7a03 223e 0a5a 094c  nd_colorz.">.Z.L
+000012b0: 6177 6e47 7265 656e da00 7a43 3c62 3e54  awnGreen..zC<b>T
+000012c0: 6173 6b65 7220 4d61 7070 696e 672e 2e2e  asker Mapping...
+000012d0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e26 6e62  .............&nb
+000012e0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b54  sp;&nbsp;&nbsp;T
+000012f0: 6173 6b65 7220 7665 7273 696f 6e3a 205a  asker version: Z
+00001300: 0274 767a 2c26 6e62 7370 3b26 6e62 7370  .tvz,&nbsp;&nbsp
+00001310: 3b26 6e62 7370 3b26 6e62 7370 3b4d 6170  ;&nbsp;&nbsp;Map
+00001320: 2d54 6173 6b65 7220 7665 7273 696f 6e3a  -Tasker version:
+00001330: 207a 043c 2f62 3e54 7224 0000 0029 1172   z.</b>Tr$...).r
+00001340: 1e00 0000 720c 0000 0072 0600 0000 5a08  ....r....r....Z.
+00001350: 7368 6f77 696e 666f 7233 0000 0072 1200  showinfor3...r..
+00001360: 0000 da03 7461 67da 0c62 7569 6c64 5f6f  ....tag..build_o
+00001370: 7574 7075 74da 096d 795f 6f75 7470 7574  utput..my_output
+00001380: 7210 0000 0072 2400 0000 7230 0000 0072  r....r$...r0...r
+00001390: 3100 0000 7209 0000 00da 0661 7474 7269  1...r......attri
+000013a0: 6272 0f00 0000 720d 0000 0029 0b72 3400  br....r....).r4.
+000013b0: 0000 7221 0000 0072 4600 0000 7247 0000  ..r!...rF...rG..
+000013c0: 00da 036d 7367 7232 0000 00da 0474 7265  ...msgr2.....tre
+000013d0: 65da 0472 6f6f 74da 1061 6c6c 5f74 6173  e..root..all_tas
+000013e0: 6b65 725f 6974 656d 73da 0965 7272 6f72  ker_items..error
+000013f0: 5f6d 7367 da07 6865 6164 696e 6772 1900  _msg..headingr..
+00001400: 0000 7219 0000 0072 1a00 0000 da05 7365  ..r....r......se
+00001410: 7475 70c1 0000 0073 4000 0000 080c 1003  tup....s@.......
+00001420: 0401 0c01 0803 0e03 0a03 0401 1201 1001  ................
+00001430: 0c01 0204 0601 06ff 0202 0201 0201 0201  ................
+00001440: 0202 0801 04ff 0202 06fe 0204 02f7 02fe  ................
+00001450: 02ff 1210 0803 0c01 1203 1002 7255 0000  ............rU..
+00001460: 0063 0200 0000 0000 0000 0000 0000 0a00  .c..............
+00001470: 0000 0900 0000 4300 0000 73ac 0000 0074  ......C...s....t
+00001480: 0083 007d 0274 01a0 0264 0174 0374 046a  ...}.t...d.t.t.j
+00001490: 0583 019b 009d 02a1 0101 0074 06a0 07a1  ...........t....
+000014a0: 0001 0074 08a0 097c 02a1 015c 027d 037d  ...t...|...\.}.}
+000014b0: 0274 0a7c 027c 037c 007c 0183 045c 067d  .t.|.|.|.|...\.}
+000014c0: 047d 057d 067d 077d 007d 087c 0364 0219  .}.}.}.}.}.|.d..
+000014d0: 0072 2f74 0b7c 037c 0283 0201 007c 0364  .r/t.|.|.....|.d
+000014e0: 0319 0072 4074 01a0 0c64 047c 0364 0319  ...r@t...d.|.d..
+000014f0: 0017 00a1 0101 0064 057c 0364 063c 0064  .......d.|.d.<.d
+00001500: 0764 0764 0764 089c 037d 0974 01a0 0264  .d.d.d...}.t...d
+00001510: 09a1 0101 007c 027c 037c 097c 087c 007c  .....|.|.|.|.|.|
+00001520: 047c 057c 067c 0766 0953 0029 0a7a ee0a  .|.|.|.f.S.).z..
+00001530: 2020 2020 5065 7266 6f72 6d20 6d61 7074      Perform mapt
+00001540: 6173 6b65 7220 7072 6f67 7261 6d20 696e  asker program in
+00001550: 6974 6961 6c69 7a61 7469 6f6e 2066 756e  itialization fun
+00001560: 6374 696f 6e73 0a20 2020 2020 2020 203a  ctions.        :
+00001570: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
+00001580: 743a 206c 6973 7420 6f66 206f 7574 7075  t: list of outpu
+00001590: 7420 6c69 6e65 7320 746f 2061 6464 2074  t lines to add t
+000015a0: 6f2e 0a20 2020 2020 2020 203a 7061 7261  o..        :para
+000015b0: 6d20 6669 6c65 5f74 6f5f 6765 743a 2066  m file_to_get: f
+000015c0: 696c 6520 6e61 6d65 2028 6675 6c6c 7920  ile name (fully 
+000015d0: 7175 616c 6966 6965 6429 2069 6620 7072  qualified) if pr
+000015e0: 6576 696f 7573 6c79 2064 6566 696e 6564  eviously defined
+000015f0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00001600: 3a20 7365 6520 2272 6574 7572 6e22 2073  : see "return" s
+00001610: 7461 7465 6d65 6e74 0a20 2020 207a 0873  tatement.    z.s
+00001620: 7973 2e61 7267 7672 2400 0000 da10 7369  ys.argvr$.....si
+00001630: 6e67 6c65 5f74 6173 6b5f 6e61 6d65 7a0c  ngle_task_namez.
+00001640: 5369 6e67 6c65 2054 6173 6b3d 7225 0000  Single Task=r%..
+00001650: 00da 1464 6973 706c 6179 5f64 6574 6169  ...display_detai
+00001660: 6c5f 6c65 7665 6c46 2903 da14 7369 6e67  l_levelF)...sing
+00001670: 6c65 5f70 726f 6a65 6374 5f66 6f75 6e64  le_project_found
+00001680: da14 7369 6e67 6c65 5f70 726f 6669 6c65  ..single_profile
+00001690: 5f66 6f75 6e64 da11 7369 6e67 6c65 5f74  _found..single_t
+000016a0: 6173 6b5f 666f 756e 6472 3100 0000 290d  ask_foundr1...).
+000016b0: 7235 0000 0072 1000 0000 722b 0000 0072  r5...r....r+...r
+000016c0: 3f00 0000 7230 0000 0072 4100 0000 da0a  ?...r0...rA.....
+000016d0: 6f6c 645f 746f 5f6e 6577 da07 6d69 6772  old_to_new..migr
+000016e0: 6174 65da 0867 6574 5f61 7267 735a 1567  ate..get_argsZ.g
+000016f0: 6574 5f70 726f 6772 616d 5f61 7267 756d  et_program_argum
+00001700: 656e 7473 7255 0000 0072 4500 0000 7224  entsrU...rE...r$
+00001710: 0000 0029 0a72 4600 0000 7247 0000 0072  ...).rF...rG...r
+00001720: 3400 0000 7221 0000 0072 5000 0000 7251  4...r!...rP...rQ
+00001730: 0000 0072 3200 0000 7252 0000 0072 5400  ...r2...rR...rT.
+00001740: 0000 da0b 666f 756e 645f 6974 656d 7372  ....found_itemsr
+00001750: 1900 0000 7219 0000 0072 1a00 0000 da08  ....r....r......
+00001760: 7374 6172 745f 7570 0101 0000 7336 0000  start_up....s6..
+00001770: 0006 0716 0308 030e 0302 0308 0110 ff08  ................
+00001780: 050a 0108 0312 0108 0102 0402 0102 0106  ................
+00001790: fd0a 0502 0202 0102 0102 0102 0102 0102  ................
+000017a0: 0102 0102 0104 f772 5f00 0000 2902 7222  .......r_...).r"
+000017b0: 0000 004e 293a da06 6174 6578 6974 7240  ...N):..atexitr@
+000017c0: 0000 0072 3000 0000 5a04 6a73 6f6e 7202  ...r0...Z.jsonr.
+000017d0: 0000 0072 0300 0000 5a07 7061 7468 6c69  ...r....Z.pathli
+000017e0: 6272 0400 0000 5a07 746b 696e 7465 7272  br....Z.tkinterr
+000017f0: 0500 0000 7206 0000 005a 1274 6b69 6e74  ....r....Z.tkint
+00001800: 6572 2e66 696c 6564 6961 6c6f 6772 0700  er.filedialogr..
+00001810: 0000 da06 7479 7069 6e67 7208 0000 005a  ....typingr....Z
+00001820: 156d 6170 7461 736b 6572 2e73 7263 2e6d  .maptasker.src.m
+00001830: 6967 7261 7465 da03 7372 6372 5c00 0000  igrate..srcr\...
+00001840: 725b 0000 00da 156d 6170 7461 736b 6572  r[.....maptasker
+00001850: 2e73 7263 2e6f 7574 7075 746c da07 6f75  .src.outputl..ou
+00001860: 7470 7574 6c72 4c00 0000 5a16 6d61 7074  tputlrL...Z.mapt
+00001870: 6173 6b65 722e 7372 632e 7072 6f67 6172  asker.src.progar
+00001880: 6773 5a08 7072 6f67 6172 6773 725d 0000  gsZ.progargsr]..
+00001890: 00da 166d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
+000018a0: 2e66 726d 7468 746d 6c72 0900 0000 5a16  .frmthtmlr....Z.
+000018b0: 6d61 7074 6173 6b65 722e 7372 632e 636f  maptasker.src.co
+000018c0: 6c72 6d6f 6465 720a 0000 00da 146d 6170  lrmoder......map
+000018d0: 7461 736b 6572 2e73 7263 2e63 6f6e 6669  tasker.src.confi
+000018e0: 6772 0b00 0000 720c 0000 00da 136d 6170  gr....r......map
+000018f0: 7461 736b 6572 2e73 7263 2e64 6562 7567  tasker.src.debug
+00001900: 720d 0000 00da 166d 6170 7461 736b 6572  r......maptasker
+00001910: 2e73 7263 2e73 7973 636f 6e73 7472 0e00  .src.sysconstr..
+00001920: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00001930: 005a 156d 6170 7461 736b 6572 2e73 7263  .Z.maptasker.src
+00001940: 2e74 6173 6b65 7264 7212 0000 00da 136d  .taskerdr......m
+00001950: 6170 7461 736b 6572 2e73 7263 2e65 7272  aptasker.src.err
+00001960: 6f72 7213 0000 0072 1b00 0000 7220 0000  orr....r....r ..
+00001970: 0072 1e00 0000 da08 7265 6769 7374 6572  .r......register
+00001980: da04 6469 6374 da06 6f62 6a65 6374 7233  ..dict..objectr3
+00001990: 0000 0072 3500 0000 723d 0000 0072 4500  ...r5...r=...rE.
+000019a0: 0000 da04 6c69 7374 723f 0000 00da 0574  ....listr?.....t
+000019b0: 7570 6c65 7255 0000 0072 5f00 0000 7219  uplerU...r_...r.
+000019c0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+000019d0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000019e0: 7356 0000 0008 0e08 0108 0110 010c 010c  sV..............
+000019f0: 030c 010c 040c 0112 0212 0112 010c 010c  ................
+00001a00: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001a10: 010c 0108 0708 0e06 0c0a 0112 070e 3c0a  ..............<.
+00001a20: 0e16 1102 1202 0102 ff02 0102 ff02 0102  ................
+00001a30: ff02 0102 ff12 020a fe1a 40              ..........@
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/projects.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/projects.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 16 16:33:54 2023 UTC, .py size: 15066 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7223 3c64 da3a 0000  o.......r#<d.:..
+00000000: 6f0d 0d0a 0000 0000 67fd 4764 783b 0000  o.......g.Gdx;..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0014 0000 0040 0000 0073 7801 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a04 0100 6400 6402 6c05 6d06  ..m.Z...d.d.l.m.
 00000050: 5a06 0100 6400 6403 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 6400 6404 6c09 6d0a 5a0a 0100 6400 6405  d.d.l.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 6400 6406 6c0b 6d0d  l.m.Z...d.d.l.m.
@@ -239,213 +239,215 @@
 00000ee0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00000ef0: 0202 0201 06ff 0203 02f8 04fb 1010 0401  ................
 00000f00: 0604 0201 06ff 04ff 0406 0201 0201 0201  ................
 00000f10: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00000f20: 0201 0201 04f3 0280 1010 0401 7231 0000  ............r1..
 00000f30: 0072 2500 0000 6308 0000 0000 0000 0000  .r%...c.........
 00000f40: 0000 000b 0000 000a 0000 0043 0000 0073  ...........C...s
-00000f50: ac00 0000 6401 0400 7d08 7d09 7c00 6402  ....d...}.}.|.d.
-00000f60: 1900 6403 6b02 7213 7400 7c02 8301 7d08  ..d.k.r.t.|...}.
-00000f70: 7401 7c02 6404 8302 7d09 7402 7c01 6405  t.|.d...}.t.|.d.
-00000f80: 6401 6406 7c03 9b00 9d02 6407 8305 7d0a  d.d.|.....d...}.
-00000f90: 7c00 6408 1900 7243 7c03 7c00 6408 1900  |.d...rC|.|.d...
-00000fa0: 6b03 722a 6407 5300 6407 7c04 6409 3c00  k.r*d.S.d.|.d.<.
-00000fb0: 7403 6404 7c06 7c0a 9b00 640a 7c07 9b00  t.d.|.|...d.|...
-00000fc0: 7c09 9b00 7c08 9b00 9d05 6401 7c05 7c01  |...|.....d.|.|.
-00000fd0: 7c00 8307 0100 6404 5300 7404 7c01 7c00  |.....d.S.t.|.|.
-00000fe0: 7c06 640b 7c0a 9b00 640a 7c07 9b00 7c09  |.d.|...d.|...|.
-00000ff0: 9b00 7c08 9b00 9d05 8305 0100 6404 5300  ..|.........d.S.
-00001000: 290c 616f 0200 000a 2020 2020 4164 6420  ).ao....    Add 
-00001010: 6578 7472 6120 696e 666f 2074 6f20 5072  extra info to Pr
-00001020: 6f6a 6563 7420 6f75 7470 7574 206c 696e  oject output lin
-00001030: 6520 6173 2061 7070 726f 7072 6961 7465  e as appropriate
-00001040: 2061 6e64 2074 6865 6e20 6f75 7470 7574   and then output
-00001050: 2069 742e 0a20 2020 2020 2020 203a 7061   it..        :pa
-00001060: 7261 6d20 7072 6f67 7261 6d5f 6172 6773  ram program_args
-00001070: 3a20 7275 6e74 696d 6520 6172 6775 6d65  : runtime argume
-00001080: 6e74 730a 2020 2020 2020 2020 3a70 6172  nts.        :par
-00001090: 616d 2063 6f6c 6f72 6d61 703a 2063 6f6c  am colormap: col
-000010a0: 6f72 7320 746f 2075 7365 2069 6e20 7075  ors to use in pu
-000010b0: 7470 7574 0a20 2020 2020 2020 203a 7061  tput.        :pa
-000010c0: 7261 6d20 7072 6f6a 6563 743a 2050 726f  ram project: Pro
-000010d0: 6a65 6374 2078 6d6c 2065 6c65 6d65 6e74  ject xml element
-000010e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000010f0: 7072 6f6a 6563 745f 6e61 6d65 3a20 6e61  project_name: na
-00001100: 6d65 206f 6620 5072 6f6a 6563 740a 2020  me of Project.  
-00001110: 2020 2020 2020 3a70 6172 616d 2066 6f75        :param fou
-00001120: 6e64 5f69 7465 6d73 3a20 7369 6e67 6c65  nd_items: single
-00001130: 206e 616d 6520 666f 7220 5072 6f6a 6563   name for Projec
-00001140: 742f 5072 6f66 696c 652f 5461 736b 2069  t/Profile/Task i
-00001150: 6620 7072 6f76 6964 6564 0a20 2020 2020  f provided.     
-00001160: 2020 203a 7061 7261 6d20 6865 6164 696e     :param headin
-00001170: 673a 206c 6173 7420 6f75 7470 7574 2068  g: last output h
-00001180: 6561 6469 6e67 0a20 2020 2020 2020 203a  eading.        :
-00001190: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
-000011a0: 743a 206c 6973 7420 6f66 206f 7574 7075  t: list of outpu
-000011b0: 7420 6c69 6e65 7320 6765 6e65 7261 7465  t lines generate
-000011c0: 6420 7468 7573 2066 6172 0a20 2020 2020  d thus far.     
-000011d0: 2020 203a 7061 7261 6d20 6c61 756e 6368     :param launch
-000011e0: 6572 5f74 6173 6b5f 696e 666f 3a20 6465  er_task_info: de
-000011f0: 7461 696c 7320 6162 6f75 7420 2861 6e79  tails about (any
-00001200: 2920 6c61 756e 6368 6572 2054 6173 6b0a  ) launcher Task.
-00001210: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00001220: 2054 7275 6520 6966 2077 6520 6172 6520   True if we are 
-00001230: 6c6f 6f6b 696e 6720 666f 7220 6120 7369  looking for a si
-00001240: 6e67 6c65 2050 726f 6a65 6374 2061 6e64  ngle Project and
-00001250: 2074 6869 7320 6973 6e27 7420 6974 2e20   this isn't it. 
-00001260: 2046 616c 7365 206f 7468 6572 7769 7365   False otherwise
-00001270: 2e0a 2020 2020 7215 0000 00da 1464 6973  ..    r......dis
-00001280: 706c 6179 5f64 6574 6169 6c5f 6c65 7665  play_detail_leve
-00001290: 6c72 1600 0000 46da 0d70 726f 6a65 6374  lr....F..project
-000012a0: 5f63 6f6c 6f72 7a09 5072 6f6a 6563 743a  _colorz.Project:
-000012b0: 2054 da13 7369 6e67 6c65 5f70 726f 6a65   T..single_proje
-000012c0: 6374 5f6e 616d 65da 1473 696e 676c 655f  ct_name..single_
-000012d0: 7072 6f6a 6563 745f 666f 756e 64fa 0120  project_found.. 
-000012e0: e902 0000 0029 0572 0400 0000 7207 0000  .....).r....r...
-000012f0: 0072 0200 0000 7206 0000 0072 0500 0000  .r....r....r....
-00001300: 290b 720f 0000 0072 1200 0000 7220 0000  ).r....r....r ..
-00001310: 0072 2800 0000 7210 0000 0072 1100 0000  .r(...r....r....
-00001320: 720c 0000 0072 2500 0000 5a0c 6b69 645f  r....r%...Z.kid_
-00001330: 6170 705f 696e 666f da08 7072 696f 7269  app_info..priori
-00001340: 7479 5a14 7072 6f6a 6563 745f 6e61 6d65  tyZ.project_name
-00001350: 5f64 6574 6169 6c73 721d 0000 0072 1d00  _detailsr....r..
-00001360: 0000 721e 0000 00da 1c67 6574 5f65 7874  ..r......get_ext
-00001370: 7261 5f61 6e64 5f6f 7574 7075 745f 7072  ra_and_output_pr
-00001380: 6f6a 6563 74c9 0000 0073 3a00 0000 0817  oject....s:.....
-00001390: 0c01 0801 0a01 0203 1001 04ff 0805 0c01  ................
-000013a0: 0401 0802 0201 0201 0201 1401 0201 0201  ................
-000013b0: 0201 0201 04f9 0411 02f9 0201 0201 0201  ................
-000013c0: 0201 1401 04fb 0407 7239 0000 0072 1c00  ........r9...r..
-000013d0: 0000 6309 0000 0000 0000 0000 0000 000e  ..c.............
-000013e0: 0000 000c 0000 0043 0000 0073 6a01 0000  .......C...sj...
-000013f0: 7c08 6401 1900 4400 5dae 7d09 7c00 6402  |.d...D.].}.|.d.
-00001400: 1900 730e 7c00 6403 1900 7211 0100 6700  ..s.|.d...r...g.
-00001410: 5300 7c09 a000 6404 a101 6a01 7d0a 7402  S.|...d...j.}.t.
-00001420: 7c09 7c06 8302 7d0b 7403 7c07 7c06 7c09  |.|...}.t.|.|.|.
-00001430: 7c0a 7c00 7c02 7c01 7c0b 8308 7228 7104  |.|.|.|.|...r(q.
-00001440: 7c07 6405 1900 7233 7404 7c09 7c06 7c07  |.d...r3t.|.|.|.
-00001450: 7c01 8304 0100 7405 6406 7c07 7c06 7c01  |.....t.d.|.|.|.
-00001460: 7c09 7c0a 7c03 8307 0400 7d0c 7256 7406  |.|.|.....}.rVt.
-00001470: 7c01 7c09 7c0a 7c0c 7c04 7c07 7c02 7c06  |.|.|.|.|.|.|.|.
-00001480: 7c08 7c00 830a 7d05 7c07 6407 1900 7255  |.|...}.|.d...rU
-00001490: 7c00 6403 1900 7355 7104 6e0e 7407 7c06  |.d...sUq.n.t.|.
-000014a0: 7c07 7c01 6408 7408 7c06 6409 640a 640b  |.|.d.t.|.d.d.d.
-000014b0: 640c 8305 8305 0100 7407 7c06 7c07 7c01  d.......t.|.|.|.
-000014c0: 640d 640a 8305 0100 7405 640c 6900 6900  d.d.....t.d.i.i.
-000014d0: 6700 7c09 7c0a 6700 8307 0400 7d0d 7284  g.|.|.g.....}.r.
-000014e0: 7409 7c0d 7c04 7c01 7c0a 7c06 7c07 7c02  t.|.|.|.|.|.|.|.
-000014f0: 7c08 7c00 8309 0100 7c07 640e 1900 7392  |.|.....|.d...s.
-00001500: 740a 7c09 7c06 7c07 7c01 7c05 7c04 7c08  t.|.|.|.|.|.|.|.
-00001510: 8307 0100 7407 7c06 7c07 7c01 640d 640a  ....t.|.|.|.d.d.
-00001520: 8305 0100 7c00 640f 1900 73a6 7c00 6403  ....|.d...s.|.d.
-00001530: 1900 73a6 7c00 6402 1900 72b2 7407 7c06  ..s.|.d...r.t.|.
-00001540: 7c07 7c01 640d 640a 8305 0100 7c04 0200  |.|.d.d.....|...
-00001550: 0100 5300 7104 6700 5300 2910 6160 0200  ..S.q.g.S.).a`..
-00001560: 000a 2020 2020 476f 2074 6872 6f75 6768  ..    Go through
-00001570: 2061 6c6c 2074 6865 2050 726f 6a65 6374   all the Project
-00001580: 732c 2067 6574 2074 6865 6972 2064 6574  s, get their det
-00001590: 6169 6c20 616e 6420 6f75 7470 7574 2069  ail and output i
-000015a0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-000015b0: 2066 6f75 6e64 5f69 7465 6d73 3a20 616c   found_items: al
-000015c0: 6c20 6974 656d 7320 666f 756e 6420 736f  l items found so
-000015d0: 2066 6172 0a20 2020 2020 2020 203a 7061   far.        :pa
-000015e0: 7261 6d20 6f75 7470 7574 5f6c 6973 743a  ram output_list:
-000015f0: 206c 6973 7420 6f66 206f 7574 7075 7420   list of output 
-00001600: 6c69 6e65 7320 6765 6e65 7261 7465 6420  lines generated 
-00001610: 736f 2066 6172 0a20 2020 2020 2020 203a  so far.        :
-00001620: 7061 7261 6d20 6865 6164 696e 673a 2074  param heading: t
-00001630: 6865 206f 7574 7075 7420 6865 6164 696e  he output headin
-00001640: 670a 2020 2020 2020 2020 3a70 6172 616d  g.        :param
-00001650: 2070 726f 6a65 6374 735f 7769 7468 6f75   projects_withou
-00001660: 745f 7072 6f66 696c 6573 3a20 6c69 7374  t_profiles: list
-00001670: 206f 6620 5072 6f6a 6563 7473 2077 6974   of Projects wit
-00001680: 6820 6e6f 2050 726f 6669 6c65 730a 2020  h no Profiles.  
-00001690: 2020 2020 2020 3a70 6172 616d 2066 6f75        :param fou
-000016a0: 6e64 5f74 6173 6b73 3a20 6c69 7374 206f  nd_tasks: list o
-000016b0: 6620 5461 736b 7320 666f 756e 640a 2020  f Tasks found.  
-000016c0: 2020 2020 2020 3a70 6172 616d 206f 7572        :param our
-000016d0: 5f74 6173 6b5f 656c 656d 656e 743a 2078  _task_element: x
-000016e0: 6d6c 2065 6c65 6d65 6e74 206f 6620 6f75  ml element of ou
-000016f0: 7220 5461 736b 0a20 2020 2020 2020 203a  r Task.        :
-00001700: 7061 7261 6d20 636f 6c6f 726d 6170 3a20  param colormap: 
-00001710: 6f75 7470 7574 2063 6f6c 6f72 7320 746f  output colors to
-00001720: 2075 7365 0a20 2020 2020 2020 203a 7061   use.        :pa
-00001730: 7261 6d20 7072 6f67 7261 6d5f 6172 6773  ram program_args
-00001740: 3a20 7275 6e74 696d 6520 6172 6775 6d65  : runtime argume
-00001750: 6e74 730a 2020 2020 2020 2020 3a70 6172  nts.        :par
-00001760: 616d 2061 6c6c 5f74 6173 6b65 725f 6974  am all_tasker_it
-00001770: 656d 733a 2061 6c6c 2050 726f 6a65 6374  ems: all Project
-00001780: 732f 5072 6f66 696c 6573 2f54 6173 6b73  s/Profiles/Tasks
-00001790: 2f53 6365 6e65 730a 2020 2020 2020 2020  /Scenes.        
-000017a0: 3a72 6574 7572 6e3a 206c 6973 7420 6f66  :return: list of
-000017b0: 2066 6f75 6e64 2054 6173 6b73 0a20 2020   found Tasks.   
-000017c0: 20da 0c61 6c6c 5f70 726f 6a65 6374 7372   ..all_projectsr
-000017d0: 2a00 0000 7229 0000 00da 046e 616d 65da  *...r).....name.
-000017e0: 1164 6973 706c 6179 5f74 6173 6b65 726e  .display_taskern
-000017f0: 6574 54da 1373 696e 676c 655f 7072 6f66  etT..single_prof
-00001800: 696c 655f 6e61 6d65 7237 0000 00da 0d70  ile_namer7.....p
-00001810: 726f 6669 6c65 5f63 6f6c 6f72 7215 0000  rofile_colorr...
-00001820: 007a 203c 656d 3e50 726f 6a65 6374 2068  .z <em>Project h
-00001830: 6173 206e 6f20 5072 6f66 696c 6573 3c2f  as no Profiles</
-00001840: 656d 3e46 7216 0000 00da 1073 696e 676c  em>Fr......singl
-00001850: 655f 7461 736b 5f6e 616d 6572 3500 0000  e_task_namer5...
-00001860: 290b 7223 0000 0072 2400 0000 7226 0000  ).r#...r$...r&..
-00001870: 0072 3900 0000 720a 0000 0072 0300 0000  .r9...r....r....
-00001880: 7208 0000 0072 0500 0000 7202 0000 0072  r....r....r....r
-00001890: 3100 0000 7209 0000 0029 0e72 1000 0000  1...r....).r....
-000018a0: 720c 0000 0072 1100 0000 720e 0000 0072  r....r....r....r
-000018b0: 0d00 0000 721c 0000 0072 1200 0000 720f  ....r....r....r.
-000018c0: 0000 0072 1300 0000 7220 0000 0072 2800  ...r....r ...r(.
-000018d0: 0000 7225 0000 005a 0b70 726f 6669 6c65  ..r%...Z.profile
-000018e0: 5f69 6473 7227 0000 0072 1d00 0000 721d  _idsr'...r....r.
-000018f0: 0000 0072 1e00 0000 7217 0000 0007 0100  ...r....r.......
-00001900: 0073 ba00 0000 0c19 1002 0201 0468 0c99  .s...........h..
-00001910: 0a03 0203 0201 0201 0201 0201 0201 0201  ................
-00001920: 0201 0201 04f8 020a 0803 0e01 0202 0201  ................
-00001930: 0201 0201 0201 0201 0201 0201 08f9 0209  ................
-00001940: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001950: 0201 0201 04f6 060f 02ff 0602 02fe 0204  ................
-00001960: 0280 0202 0201 0201 0201 0201 0201 0201  ................
-00001970: 0201 0201 0201 0201 02fb 04fb 100d 1803  ................
-00001980: 0202 0201 0201 0201 0201 0201 0201 0201  ................
-00001990: 0201 0201 04f7 080d 0201 0201 0201 0201  ................
-000019a0: 0201 0201 0201 0201 04f9 100a 0602 02ff  ................
-000019b0: 0602 02fe 0603 02fd 1005 0801 02fa 0409  ................
-000019c0: 7217 0000 0029 23da 1664 6566 7573 6564  r....)#..defused
-000019d0: 786d 6c2e 456c 656d 656e 7454 7265 65da  xml.ElementTree.
-000019e0: 0a64 6566 7573 6564 786d 6c5a 136d 6170  .defusedxmlZ.map
-000019f0: 7461 736b 6572 2e73 7263 2e74 6173 6b73  tasker.src.tasks
-00001a00: da03 7372 6372 2f00 0000 da16 6d61 7074  ..srcr/.....mapt
-00001a10: 6173 6b65 722e 7372 632e 6672 6d74 6874  asker.src.frmtht
-00001a20: 6d6c 7202 0000 005a 146d 6170 7461 736b  mlr....Z.maptask
-00001a30: 6572 2e73 7263 2e67 6574 6964 7372 0300  er.src.getidsr..
-00001a40: 0000 5a14 6d61 7074 6173 6b65 722e 7372  ..Z.maptasker.sr
-00001a50: 632e 6b69 6461 7070 7204 0000 00da 156d  c.kidappr......m
-00001a60: 6170 7461 736b 6572 2e73 7263 2e6f 7574  aptasker.src.out
-00001a70: 7075 746c 7205 0000 0072 0600 0000 5a16  putlr....r....Z.
-00001a80: 6d61 7074 6173 6b65 722e 7372 632e 7072  maptasker.src.pr
-00001a90: 696f 7269 7479 7207 0000 005a 166d 6170  iorityr....Z.map
-00001aa0: 7461 736b 6572 2e73 7263 2e70 726f 6669  tasker.src.profi
-00001ab0: 6c65 7372 0800 0000 5a14 6d61 7074 6173  lesr....Z.maptas
-00001ac0: 6b65 722e 7372 632e 7363 656e 6573 7209  ker.src.scenesr.
-00001ad0: 0000 005a 136d 6170 7461 736b 6572 2e73  ...Z.maptasker.s
-00001ae0: 7263 2e73 6861 7265 720a 0000 00da 166d  rc.sharer......m
-00001af0: 6170 7461 736b 6572 2e73 7263 2e73 7973  aptasker.src.sys
-00001b00: 636f 6e73 7472 0b00 0000 7218 0000 0072  constr....r....r
-00001b10: 1900 0000 da03 7374 7272 1f00 0000 da0b  ......strr......
-00001b20: 456c 656d 656e 7454 7265 65da 0358 4d4c  ElementTree..XML
-00001b30: 7226 0000 0072 3100 0000 da04 626f 6f6c  r&...r1.....bool
-00001b40: 7239 0000 0072 1700 0000 721d 0000 0072  r9...r....r....r
-00001b50: 1d00 0000 721d 0000 0072 1e00 0000 da08  ....r....r......
-00001b60: 3c6d 6f64 756c 653e 0100 0000 73ba 0000  <module>....s...
-00001b70: 0008 0e12 020c 010c 010c 010c 010c 010c  ................
-00001b80: 010c 010c 010c 010c 0102 0602 0102 ff02  ................
-00001b90: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
-00001ba0: 0602 fa02 0702 f902 0802 f802 090a f71a  ................
-00001bb0: 2a02 1902 0102 ff02 0202 fe02 0302 fd02  *...............
-00001bc0: 0402 fc02 0502 fb02 0602 fa02 0702 f902  ................
-00001bd0: 0802 f802 0902 f702 0a0a f602 6502 0102  ............e...
-00001be0: ff02 0202 fe06 0302 fd02 0402 fc02 0502  ................
-00001bf0: fb02 0602 fa02 0702 f902 0802 f802 090a  ................
-00001c00: f702 3e02 0102 ff02 0202 fe02 0302 fd02  ..>.............
-00001c10: 0402 fc02 0502 fb06 0602 fa02 0702 f902  ................
-00001c20: 0802 f802 0902 f702 0a0e f6              ...........
+00000f50: c000 0000 6401 0400 7d08 7d09 7c00 6402  ....d...}.}.|.d.
+00000f60: 1900 6403 6b02 721d 7400 7c02 8301 7d08  ..d.k.r.t.|...}.
+00000f70: 7c08 7218 7401 7c01 6404 6401 7c08 6405  |.r.t.|.d.d.|.d.
+00000f80: 8305 7d08 7402 7c02 6406 8302 7d09 7401  ..}.t.|.d...}.t.
+00000f90: 7c01 6404 6401 6407 7c03 9b00 9d02 6405  |.d.d.d.|.....d.
+00000fa0: 8305 7d0a 7c00 6408 1900 724d 7c03 7c00  ..}.|.d...rM|.|.
+00000fb0: 6408 1900 6b03 7234 6405 5300 6405 7c04  d...k.r4d.S.d.|.
+00000fc0: 6409 3c00 7403 6406 7c06 7c0a 9b00 640a  d.<.t.d.|.|...d.
+00000fd0: 7c07 9b00 7c09 9b00 7c08 9b00 9d05 6401  |...|...|.....d.
+00000fe0: 7c05 7c01 7c00 8307 0100 6406 5300 7404  |.|.|.....d.S.t.
+00000ff0: 7c01 7c00 7c06 640b 7c0a 9b00 640a 7c07  |.|.|.d.|...d.|.
+00001000: 9b00 7c09 9b00 7c08 9b00 9d05 8305 0100  ..|...|.........
+00001010: 6406 5300 290c 616f 0200 000a 2020 2020  d.S.).ao....    
+00001020: 4164 6420 6578 7472 6120 696e 666f 2074  Add extra info t
+00001030: 6f20 5072 6f6a 6563 7420 6f75 7470 7574  o Project output
+00001040: 206c 696e 6520 6173 2061 7070 726f 7072   line as appropr
+00001050: 6961 7465 2061 6e64 2074 6865 6e20 6f75  iate and then ou
+00001060: 7470 7574 2069 742e 0a20 2020 2020 2020  tput it..       
+00001070: 203a 7061 7261 6d20 7072 6f67 7261 6d5f   :param program_
+00001080: 6172 6773 3a20 7275 6e74 696d 6520 6172  args: runtime ar
+00001090: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
+000010a0: 3a70 6172 616d 2063 6f6c 6f72 6d61 703a  :param colormap:
+000010b0: 2063 6f6c 6f72 7320 746f 2075 7365 2069   colors to use i
+000010c0: 6e20 7075 7470 7574 0a20 2020 2020 2020  n putput.       
+000010d0: 203a 7061 7261 6d20 7072 6f6a 6563 743a   :param project:
+000010e0: 2050 726f 6a65 6374 2078 6d6c 2065 6c65   Project xml ele
+000010f0: 6d65 6e74 0a20 2020 2020 2020 203a 7061  ment.        :pa
+00001100: 7261 6d20 7072 6f6a 6563 745f 6e61 6d65  ram project_name
+00001110: 3a20 6e61 6d65 206f 6620 5072 6f6a 6563  : name of Projec
+00001120: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+00001130: 2066 6f75 6e64 5f69 7465 6d73 3a20 7369   found_items: si
+00001140: 6e67 6c65 206e 616d 6520 666f 7220 5072  ngle name for Pr
+00001150: 6f6a 6563 742f 5072 6f66 696c 652f 5461  oject/Profile/Ta
+00001160: 736b 2069 6620 7072 6f76 6964 6564 0a20  sk if provided. 
+00001170: 2020 2020 2020 203a 7061 7261 6d20 6865         :param he
+00001180: 6164 696e 673a 206c 6173 7420 6f75 7470  ading: last outp
+00001190: 7574 2068 6561 6469 6e67 0a20 2020 2020  ut heading.     
+000011a0: 2020 203a 7061 7261 6d20 6f75 7470 7574     :param output
+000011b0: 5f6c 6973 743a 206c 6973 7420 6f66 206f  _list: list of o
+000011c0: 7574 7075 7420 6c69 6e65 7320 6765 6e65  utput lines gene
+000011d0: 7261 7465 6420 7468 7573 2066 6172 0a20  rated thus far. 
+000011e0: 2020 2020 2020 203a 7061 7261 6d20 6c61         :param la
+000011f0: 756e 6368 6572 5f74 6173 6b5f 696e 666f  uncher_task_info
+00001200: 3a20 6465 7461 696c 7320 6162 6f75 7420  : details about 
+00001210: 2861 6e79 2920 6c61 756e 6368 6572 2054  (any) launcher T
+00001220: 6173 6b0a 2020 2020 2020 2020 3a72 6574  ask.        :ret
+00001230: 7572 6e3a 2054 7275 6520 6966 2077 6520  urn: True if we 
+00001240: 6172 6520 6c6f 6f6b 696e 6720 666f 7220  are looking for 
+00001250: 6120 7369 6e67 6c65 2050 726f 6a65 6374  a single Project
+00001260: 2061 6e64 2074 6869 7320 6973 6e27 7420   and this isn't 
+00001270: 6974 2e20 2046 616c 7365 206f 7468 6572  it.  False other
+00001280: 7769 7365 2e0a 2020 2020 7215 0000 00da  wise..    r.....
+00001290: 1464 6973 706c 6179 5f64 6574 6169 6c5f  .display_detail_
+000012a0: 6c65 7665 6c72 1600 0000 da0d 7072 6f6a  levelr......proj
+000012b0: 6563 745f 636f 6c6f 7254 467a 0950 726f  ect_colorTFz.Pro
+000012c0: 6a65 6374 3a20 da13 7369 6e67 6c65 5f70  ject: ..single_p
+000012d0: 726f 6a65 6374 5f6e 616d 65da 1473 696e  roject_name..sin
+000012e0: 676c 655f 7072 6f6a 6563 745f 666f 756e  gle_project_foun
+000012f0: 64fa 0120 e902 0000 0029 0572 0400 0000  d.. .....).r....
+00001300: 7202 0000 0072 0700 0000 7206 0000 0072  r....r....r....r
+00001310: 0500 0000 290b 720f 0000 0072 1200 0000  ....).r....r....
+00001320: 7220 0000 0072 2800 0000 7210 0000 0072  r ...r(...r....r
+00001330: 1100 0000 720c 0000 0072 2500 0000 5a0c  ....r....r%...Z.
+00001340: 6b69 645f 6170 705f 696e 666f da08 7072  kid_app_info..pr
+00001350: 696f 7269 7479 5a14 7072 6f6a 6563 745f  iorityZ.project_
+00001360: 6e61 6d65 5f64 6574 6169 6c73 721d 0000  name_detailsr...
+00001370: 0072 1d00 0000 721e 0000 00da 1c67 6574  .r....r......get
+00001380: 5f65 7874 7261 5f61 6e64 5f6f 7574 7075  _extra_and_outpu
+00001390: 745f 7072 6f6a 6563 74c9 0000 0073 4200  t_project....sB.
+000013a0: 0000 0817 0c01 0801 0401 0201 0a01 04ff  ................
+000013b0: 0a03 0203 1001 04ff 0805 0c01 0401 0802  ................
+000013c0: 0201 0201 0201 1401 0201 0201 0201 0201  ................
+000013d0: 04f9 0411 02f9 0201 0201 0201 0201 1401  ................
+000013e0: 04fb 0407 7239 0000 0072 1c00 0000 6309  ....r9...r....c.
+000013f0: 0000 0000 0000 0000 0000 000e 0000 000c  ................
+00001400: 0000 0043 0000 0073 6a01 0000 7c08 6401  ...C...sj...|.d.
+00001410: 1900 4400 5dae 7d09 7c00 6402 1900 730e  ..D.].}.|.d...s.
+00001420: 7c00 6403 1900 7211 0100 6700 5300 7c09  |.d...r...g.S.|.
+00001430: a000 6404 a101 6a01 7d0a 7402 7c09 7c06  ..d...j.}.t.|.|.
+00001440: 8302 7d0b 7403 7c07 7c06 7c09 7c0a 7c00  ..}.t.|.|.|.|.|.
+00001450: 7c02 7c01 7c0b 8308 7228 7104 7c07 6405  |.|.|...r(q.|.d.
+00001460: 1900 7233 7404 7c09 7c06 7c07 7c01 8304  ..r3t.|.|.|.|...
+00001470: 0100 7405 6406 7c07 7c06 7c01 7c09 7c0a  ..t.d.|.|.|.|.|.
+00001480: 7c03 8307 0400 7d0c 7256 7406 7c01 7c09  |.....}.rVt.|.|.
+00001490: 7c0a 7c0c 7c04 7c07 7c02 7c06 7c08 7c00  |.|.|.|.|.|.|.|.
+000014a0: 830a 7d05 7c07 6407 1900 7255 7c00 6403  ..}.|.d...rU|.d.
+000014b0: 1900 7355 7104 6e0e 7407 7c06 7c07 7c01  ..sUq.n.t.|.|.|.
+000014c0: 6408 7408 7c06 6409 640a 640b 6406 8305  d.t.|.d.d.d.d...
+000014d0: 8305 0100 7407 7c06 7c07 7c01 640c 640a  ....t.|.|.|.d.d.
+000014e0: 8305 0100 7405 640d 6900 6900 6700 7c09  ....t.d.i.i.g.|.
+000014f0: 7c0a 6700 8307 0400 7d0d 7284 7409 7c0d  |.g.....}.r.t.|.
+00001500: 7c04 7c01 7c0a 7c06 7c07 7c02 7c08 7c00  |.|.|.|.|.|.|.|.
+00001510: 8309 0100 7c07 640e 1900 7392 740a 7c09  ....|.d...s.t.|.
+00001520: 7c06 7c07 7c01 7c05 7c04 7c08 8307 0100  |.|.|.|.|.|.....
+00001530: 7407 7c06 7c07 7c01 640c 640a 8305 0100  t.|.|.|.d.d.....
+00001540: 7c00 640f 1900 73a6 7c00 6403 1900 73a6  |.d...s.|.d...s.
+00001550: 7c00 6402 1900 72b2 7407 7c06 7c07 7c01  |.d...r.t.|.|.|.
+00001560: 640c 640a 8305 0100 7c04 0200 0100 5300  d.d.....|.....S.
+00001570: 7104 6700 5300 2910 6160 0200 000a 2020  q.g.S.).a`....  
+00001580: 2020 476f 2074 6872 6f75 6768 2061 6c6c    Go through all
+00001590: 2074 6865 2050 726f 6a65 6374 732c 2067   the Projects, g
+000015a0: 6574 2074 6865 6972 2064 6574 6169 6c20  et their detail 
+000015b0: 616e 6420 6f75 7470 7574 2069 740a 2020  and output it.  
+000015c0: 2020 2020 2020 3a70 6172 616d 2066 6f75        :param fou
+000015d0: 6e64 5f69 7465 6d73 3a20 616c 6c20 6974  nd_items: all it
+000015e0: 656d 7320 666f 756e 6420 736f 2066 6172  ems found so far
+000015f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001600: 6f75 7470 7574 5f6c 6973 743a 206c 6973  output_list: lis
+00001610: 7420 6f66 206f 7574 7075 7420 6c69 6e65  t of output line
+00001620: 7320 6765 6e65 7261 7465 6420 736f 2066  s generated so f
+00001630: 6172 0a20 2020 2020 2020 203a 7061 7261  ar.        :para
+00001640: 6d20 6865 6164 696e 673a 2074 6865 206f  m heading: the o
+00001650: 7574 7075 7420 6865 6164 696e 670a 2020  utput heading.  
+00001660: 2020 2020 2020 3a70 6172 616d 2070 726f        :param pro
+00001670: 6a65 6374 735f 7769 7468 6f75 745f 7072  jects_without_pr
+00001680: 6f66 696c 6573 3a20 6c69 7374 206f 6620  ofiles: list of 
+00001690: 5072 6f6a 6563 7473 2077 6974 6820 6e6f  Projects with no
+000016a0: 2050 726f 6669 6c65 730a 2020 2020 2020   Profiles.      
+000016b0: 2020 3a70 6172 616d 2066 6f75 6e64 5f74    :param found_t
+000016c0: 6173 6b73 3a20 6c69 7374 206f 6620 5461  asks: list of Ta
+000016d0: 736b 7320 666f 756e 640a 2020 2020 2020  sks found.      
+000016e0: 2020 3a70 6172 616d 206f 7572 5f74 6173    :param our_tas
+000016f0: 6b5f 656c 656d 656e 743a 2078 6d6c 2065  k_element: xml e
+00001700: 6c65 6d65 6e74 206f 6620 6f75 7220 5461  lement of our Ta
+00001710: 736b 0a20 2020 2020 2020 203a 7061 7261  sk.        :para
+00001720: 6d20 636f 6c6f 726d 6170 3a20 6f75 7470  m colormap: outp
+00001730: 7574 2063 6f6c 6f72 7320 746f 2075 7365  ut colors to use
+00001740: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001750: 7072 6f67 7261 6d5f 6172 6773 3a20 7275  program_args: ru
+00001760: 6e74 696d 6520 6172 6775 6d65 6e74 730a  ntime arguments.
+00001770: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
+00001780: 6c6c 5f74 6173 6b65 725f 6974 656d 733a  ll_tasker_items:
+00001790: 2061 6c6c 2050 726f 6a65 6374 732f 5072   all Projects/Pr
+000017a0: 6f66 696c 6573 2f54 6173 6b73 2f53 6365  ofiles/Tasks/Sce
+000017b0: 6e65 730a 2020 2020 2020 2020 3a72 6574  nes.        :ret
+000017c0: 7572 6e3a 206c 6973 7420 6f66 2066 6f75  urn: list of fou
+000017d0: 6e64 2054 6173 6b73 0a20 2020 20da 0c61  nd Tasks.    ..a
+000017e0: 6c6c 5f70 726f 6a65 6374 7372 2a00 0000  ll_projectsr*...
+000017f0: 7229 0000 00da 046e 616d 65da 1164 6973  r).....name..dis
+00001800: 706c 6179 5f74 6173 6b65 726e 6574 54da  play_taskernetT.
+00001810: 1373 696e 676c 655f 7072 6f66 696c 655f  .single_profile_
+00001820: 6e61 6d65 7237 0000 00da 0d70 726f 6669  namer7.....profi
+00001830: 6c65 5f63 6f6c 6f72 7215 0000 007a 203c  le_colorr....z <
+00001840: 656d 3e50 726f 6a65 6374 2068 6173 206e  em>Project has n
+00001850: 6f20 5072 6f66 696c 6573 3c2f 656d 3e72  o Profiles</em>r
+00001860: 1600 0000 46da 1073 696e 676c 655f 7461  ....F..single_ta
+00001870: 736b 5f6e 616d 6572 3500 0000 290b 7223  sk_namer5...).r#
+00001880: 0000 0072 2400 0000 7226 0000 0072 3900  ...r$...r&...r9.
+00001890: 0000 720a 0000 0072 0300 0000 7208 0000  ..r....r....r...
+000018a0: 0072 0500 0000 7202 0000 0072 3100 0000  .r....r....r1...
+000018b0: 7209 0000 0029 0e72 1000 0000 720c 0000  r....).r....r...
+000018c0: 0072 1100 0000 720e 0000 0072 0d00 0000  .r....r....r....
+000018d0: 721c 0000 0072 1200 0000 720f 0000 0072  r....r....r....r
+000018e0: 1300 0000 7220 0000 0072 2800 0000 7225  ....r ...r(...r%
+000018f0: 0000 005a 0b70 726f 6669 6c65 5f69 6473  ...Z.profile_ids
+00001900: 7227 0000 0072 1d00 0000 721d 0000 0072  r'...r....r....r
+00001910: 1e00 0000 7217 0000 000b 0100 0073 ba00  ....r........s..
+00001920: 0000 0c19 1002 0201 0468 0c99 0a03 0203  .........h......
+00001930: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001940: 04f8 020a 0803 0e01 0202 0201 0201 0201  ................
+00001950: 0201 0201 0201 0201 08f9 0209 0201 0201  ................
+00001960: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001970: 04f6 060f 02ff 0602 02fe 0204 0280 0202  ................
+00001980: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001990: 0201 0201 02fb 04fb 100d 1803 0202 0201  ................
+000019a0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+000019b0: 04f7 080d 0201 0201 0201 0201 0201 0201  ................
+000019c0: 0201 0201 04f9 100a 0602 02ff 0602 02fe  ................
+000019d0: 0603 02fd 1005 0801 02fa 0409 7217 0000  ............r...
+000019e0: 0029 23da 1664 6566 7573 6564 786d 6c2e  .)#..defusedxml.
+000019f0: 456c 656d 656e 7454 7265 65da 0a64 6566  ElementTree..def
+00001a00: 7573 6564 786d 6c5a 136d 6170 7461 736b  usedxmlZ.maptask
+00001a10: 6572 2e73 7263 2e74 6173 6b73 da03 7372  er.src.tasks..sr
+00001a20: 6372 2f00 0000 da16 6d61 7074 6173 6b65  cr/.....maptaske
+00001a30: 722e 7372 632e 6672 6d74 6874 6d6c 7202  r.src.frmthtmlr.
+00001a40: 0000 005a 146d 6170 7461 736b 6572 2e73  ...Z.maptasker.s
+00001a50: 7263 2e67 6574 6964 7372 0300 0000 5a14  rc.getidsr....Z.
+00001a60: 6d61 7074 6173 6b65 722e 7372 632e 6b69  maptasker.src.ki
+00001a70: 6461 7070 7204 0000 00da 156d 6170 7461  dappr......mapta
+00001a80: 736b 6572 2e73 7263 2e6f 7574 7075 746c  sker.src.outputl
+00001a90: 7205 0000 0072 0600 0000 5a16 6d61 7074  r....r....Z.mapt
+00001aa0: 6173 6b65 722e 7372 632e 7072 696f 7269  asker.src.priori
+00001ab0: 7479 7207 0000 005a 166d 6170 7461 736b  tyr....Z.maptask
+00001ac0: 6572 2e73 7263 2e70 726f 6669 6c65 7372  er.src.profilesr
+00001ad0: 0800 0000 5a14 6d61 7074 6173 6b65 722e  ....Z.maptasker.
+00001ae0: 7372 632e 7363 656e 6573 7209 0000 005a  src.scenesr....Z
+00001af0: 136d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
+00001b00: 6861 7265 720a 0000 00da 166d 6170 7461  harer......mapta
+00001b10: 736b 6572 2e73 7263 2e73 7973 636f 6e73  sker.src.syscons
+00001b20: 7472 0b00 0000 7218 0000 0072 1900 0000  tr....r....r....
+00001b30: da03 7374 7272 1f00 0000 da0b 456c 656d  ..strr......Elem
+00001b40: 656e 7454 7265 65da 0358 4d4c 7226 0000  entTree..XMLr&..
+00001b50: 0072 3100 0000 da04 626f 6f6c 7239 0000  .r1.....boolr9..
+00001b60: 0072 1700 0000 721d 0000 0072 1d00 0000  .r....r....r....
+00001b70: 721d 0000 0072 1e00 0000 da08 3c6d 6f64  r....r......<mod
+00001b80: 756c 653e 0100 0000 73ba 0000 0008 0e12  ule>....s.......
+00001b90: 020c 010c 010c 010c 010c 010c 010c 010c  ................
+00001ba0: 010c 010c 0102 0602 0102 ff02 0202 fe02  ................
+00001bb0: 0302 fd02 0402 fc02 0502 fb02 0602 fa02  ................
+00001bc0: 0702 f902 0802 f802 090a f71a 2a02 1902  ............*...
+00001bd0: 0102 ff02 0202 fe02 0302 fd02 0402 fc02  ................
+00001be0: 0502 fb02 0602 fa02 0702 f902 0802 f802  ................
+00001bf0: 0902 f702 0a0a f602 6502 0102 ff02 0202  ........e.......
+00001c00: fe06 0302 fd02 0402 fc02 0502 fb02 0602  ................
+00001c10: fa02 0702 f902 0802 f802 090a f702 4202  ..............B.
+00001c20: 0102 ff02 0202 fe02 0302 fd02 0402 fc02  ................
+00001c30: 0502 fb06 0602 fa02 0702 f902 0802 f802  ................
+00001c40: 0902 f702 0a0e f6                        .......
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/runcli.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/runcli.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 23 17:42:41 2023 UTC, .py size: 8999 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,268 +1,269 @@
-00000000: 6f0d 0d0a 0000 0000 918f 1c64 2723 0000  o..........d'#..
+00000000: 6f0d 0d0a 0000 0000 731e 4464 0123 0000  o.......s.Dd.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c01 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c04 6d05 5a05 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6400 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000080: 6408 6c0c 6d0d 5a0d 0100 6400 6409 6c0c  d.l.m.Z...d.d.l.
 00000090: 6d0e 5a0e 0100 6400 640a 6c0c 6d0f 5a0f  m.Z...d.d.l.m.Z.
-000000a0: 0100 6400 640b 6c0c 6d10 5a10 0100 640c  ..d.d.l.m.Z...d.
-000000b0: 6511 640d 6512 640e 6512 640f 6513 6608  e.d.e.d.e.d.e.f.
-000000c0: 6410 6411 8404 5a14 640d 6512 640e 6512  d.d...Z.d.e.d.e.
-000000d0: 640f 6513 6606 6412 6413 8404 5a15 640f  d.e.f.d.d...Z.d.
-000000e0: 6511 6602 6414 6415 8404 5a16 640e 6512  e.f.d.d...Z.d.e.
-000000f0: 640f 6513 6604 6416 6417 8404 5a17 6401  d.e.f.d.d...Z.d.
-00000100: 5300 2918 e900 0000 004e 2901 da15 6765  S.)......N)...ge
-00000110: 745f 616e 645f 7365 745f 7468 655f 636f  t_and_set_the_co
-00000120: 6c6f 7229 01da 0e76 616c 6964 6174 655f  lor)...validate_
-00000130: 636f 6c6f 7229 01da 1173 6176 655f 7265  color)...save_re
-00000140: 7374 6f72 655f 6172 6773 2901 da0e 7275  store_args)...ru
-00000150: 6e74 696d 655f 7061 7273 6572 2901 da0b  ntime_parser)...
-00000160: 7072 6f63 6573 735f 6775 6929 01da 1c69  process_gui)...i
-00000170: 6e69 7469 616c 697a 655f 7275 6e74 696d  nitialize_runtim
-00000180: 655f 6172 6775 6d65 6e74 7329 01da 0a4d  e_arguments)...M
-00000190: 595f 4c49 4345 4e53 4529 01da 0a4d 595f  Y_LICENSE)...MY_
-000001a0: 5645 5253 494f 4e29 01da 0f54 5950 4553  VERSION)...TYPES
-000001b0: 5f4f 465f 434f 4c4f 5253 2901 da06 6c6f  _OF_COLORS)...lo
-000001c0: 6767 6572 da04 6172 6773 da09 7072 6f67  gger..args..prog
-000001d0: 5f61 7267 73da 0863 6f6c 6f72 6d61 70da  _args..colormap.
-000001e0: 0672 6574 7572 6e63 0300 0000 0000 0000  .returnc........
-000001f0: 0000 0000 0500 0000 0700 0000 4300 0000  ............C...
-00000200: 7384 0100 0074 007c 0064 0183 0272 0974  s....t.|.d...r.t
-00000210: 0164 0283 0101 0074 007c 0064 0383 0272  .d.....t.|.d...r
-00000220: 1f64 047c 0164 053c 0064 067c 0164 073c  .d.|.d.<.d.|.d.<
-00000230: 0064 067c 0164 083c 0064 067c 0164 093c  .d.|.d.<.d.|.d.<
-00000240: 006e 1c74 007c 0064 0a83 027c 0164 053c  .n.t.|.d...|.d.<
-00000250: 0074 007c 0064 0b83 027c 0164 073c 0074  .t.|.d...|.d.<.t
-00000260: 007c 0064 0c83 027c 0164 083c 0074 007c  .|.d...|.d.<.t.|
-00000270: 0064 0d83 027c 0164 093c 0074 007c 0064  .d...|.d.<.t.|.d
-00000280: 0e83 027d 037c 0364 0075 0172 4a7c 0364  ...}.|.d.u.rJ|.d
-00000290: 0f19 007c 0164 103c 0074 007c 0064 1183  ...|.d.<.t.|.d..
-000002a0: 027d 037c 0364 0075 0172 597c 0364 0f19  .}.|.d.u.rY|.d..
-000002b0: 007c 0164 123c 0074 007c 0064 1383 027d  .|.d.<.t.|.d...}
-000002c0: 037c 0364 0075 0172 687c 0364 0f19 007c  .|.d.u.rh|.d...|
-000002d0: 0164 143c 0074 007c 0064 1583 0272 7164  .d.<.t.|.d...rqd
-000002e0: 067c 0164 163c 0074 007c 0064 1783 0272  .|.d.<.t.|.d...r
-000002f0: 8374 0274 039b 0064 1874 049b 009d 0383  .t.t...d.t......
-00000300: 0101 0074 0564 0f83 0101 0074 0644 005d  ...t.d.....t.D.]
-00000310: 2d7d 0474 007c 0064 197c 049b 009d 0283  -}.t.|.d.|......
-00000320: 027d 037c 0364 0075 0172 b274 077c 0383  .}.|.d.u.r.t.|..
-00000330: 0174 0875 0072 a774 0964 1a7c 049b 0064  .t.u.r.t.d.|...d
-00000340: 1b7c 0364 0f19 009b 009d 047c 0283 0201  .|.d.......|....
-00000350: 0071 8574 0964 1a7c 049b 0064 1b7c 039b  .q.t.d.|...d.|..
-00000360: 009d 047c 0283 0201 0071 8574 007c 0064  ...|.....q.t.|.d
-00000370: 1c83 0272 be74 0a64 067c 027c 0183 0301  ...r.t.d.|.|....
-00000380: 007c 017c 0266 0253 0029 1d4e da02 6368  .|.|.f.S.).N..ch
-00000390: da01 68da 0165 e903 0000 00da 1464 6973  ..h..e.......dis
-000003a0: 706c 6179 5f64 6574 6169 6c5f 6c65 7665  play_detail_leve
-000003b0: 6c54 da1a 6469 7370 6c61 795f 7072 6f66  lT..display_prof
-000003c0: 696c 655f 636f 6e64 6974 696f 6e73 da13  ile_conditions..
-000003d0: 6469 7370 6c61 795f 7072 6566 6572 656e  display_preferen
-000003e0: 6365 73da 1164 6973 706c 6179 5f74 6173  ces..display_tas
-000003f0: 6b65 726e 6574 da06 6465 7461 696c da0a  kernet..detail..
-00000400: 636f 6e64 6974 696f 6e73 da01 70da 0974  conditions..p..t
-00000410: 6173 6b65 726e 6574 da07 7072 6f6a 6563  askernet..projec
-00000420: 7472 0100 0000 da13 7369 6e67 6c65 5f70  tr......single_p
-00000430: 726f 6a65 6374 5f6e 616d 65da 0770 726f  roject_name..pro
-00000440: 6669 6c65 da13 7369 6e67 6c65 5f70 726f  file..single_pro
-00000450: 6669 6c65 5f6e 616d 65da 0474 6173 6bda  file_name..task.
-00000460: 1073 696e 676c 655f 7461 736b 5f6e 616d  .single_task_nam
-00000470: 65da 0164 da05 6465 6275 67da 0176 7a10  e..d..debug..vz.
-00000480: 2c20 756e 6465 7220 6c69 6365 6e73 6520  , under license 
-00000490: da01 637a 022d 63fa 013d da01 7329 0bda  ..cz.-c..=..s)..
-000004a0: 0767 6574 6174 7472 7203 0000 00da 0570  .getattrr......p
-000004b0: 7269 6e74 7209 0000 0072 0800 0000 da04  rintr....r......
-000004c0: 6578 6974 720a 0000 00da 0474 7970 65da  exitr......type.
-000004d0: 046c 6973 7472 0200 0000 7204 0000 0029  .listr....r....)
-000004e0: 0572 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-000004f0: 5a08 7468 655f 6e61 6d65 da04 6974 656d  Z.the_name..item
-00000500: a900 722e 0000 00fa 752f 5573 6572 732f  ..r.....u/Users/
-00000510: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
-00000520: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
-00000530: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
-00000540: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
-00000550: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
-00000560: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
-00000570: 2f73 7263 2f72 756e 636c 692e 7079 da11  /src/runcli.py..
-00000580: 7072 6f63 6573 735f 6172 6775 6d65 6e74  process_argument
-00000590: 7325 0000 0073 4600 0000 0a02 0801 0a02  s%...sF.........
-000005a0: 0801 0801 0801 0a01 0e02 0e01 0e01 0e01  ................
-000005b0: 0a01 0801 0c01 0a01 0801 0c01 0a01 0801  ................
-000005c0: 0c01 0a01 0801 0a01 1201 0801 0803 1001  ................
-000005d0: 0801 0c01 1c01 1602 0280 0a03 0c01 0802  ................
-000005e0: 7230 0000 0063 0200 0000 0000 0000 0000  r0...c..........
-000005f0: 0000 0700 0000 0400 0000 4300 0000 7312  ..........C...s.
-00000600: 0100 0069 007d 0274 0064 017c 017c 0283  ...i.}.t.d.|.|..
-00000610: 035c 027d 027d 037c 02a0 01a1 0044 005d  .\.}.}.|.....D.]
-00000620: 655c 027d 047d 057c 0464 0075 0172 737c  e\.}.}.|.d.u.rs|
-00000630: 0404 0064 026b 0272 2101 007c 057c 0064  ...d.k.r!..|.|.d
-00000640: 023c 006e 5204 0064 036b 0272 2d01 0074  .<.nR..d.k.r-..t
-00000650: 027c 0583 017c 0064 033c 006e 4604 0064  .|...|.d.<.nF..d
-00000660: 046b 0272 3701 007c 057c 0064 043c 006e  .k.r7..|.|.d.<.n
-00000670: 3c04 0064 056b 0272 4101 007c 057c 0064  <..d.k.rA..|.|.d
-00000680: 053c 006e 3204 0064 066b 0272 4b01 007c  .<.n2..d.k.rK..|
-00000690: 057c 0064 063c 006e 2804 0064 076b 0272  .|.d.<.n(..d.k.r
-000006a0: 5501 007c 057c 0064 073c 006e 1e04 0064  U..|.|.d.<.n...d
-000006b0: 086b 0272 5f01 007c 057c 0064 083c 006e  .k.r_..|.|.d.<.n
-000006c0: 1464 096b 0272 677c 057c 0064 093c 006e  .d.k.rg|.|.d.<.n
-000006d0: 0c09 0064 0a7d 0674 037c 0683 0101 0074  ...d.}.t.|.....t
-000006e0: 04a0 057c 06a1 0101 0071 0e7c 03a0 01a1  ...|.....q.|....
-000006f0: 0044 005d 0c5c 027d 047d 057c 0464 0075  .D.].\.}.}.|.d.u
-00000700: 0172 847c 057c 017c 043c 0071 787c 007c  .r.|.|.|.<.qx|.|
-00000710: 0166 0253 0029 0b4e 4672 2300 0000 7214  .f.S.).NFr#...r.
-00000720: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
-00000730: 0000 721f 0000 0072 1d00 0000 7221 0000  ..r....r....r!..
-00000740: 007a 2145 7272 6f72 3a20 496e 7661 6c69  .z!Error: Invali
-00000750: 6420 6172 6775 6d65 6e74 2072 6573 746f  d argument resto
-00000760: 7265 6421 2906 7204 0000 00da 0569 7465  red!).r......ite
-00000770: 6d73 da03 696e 7472 2900 0000 720b 0000  ms..intr)...r...
-00000780: 0072 2300 0000 2907 720d 0000 0072 0e00  .r#...).r....r..
-00000790: 0000 5a09 7465 6d70 5f61 7267 735a 0d74  ..Z.temp_argsZ.t
-000007a0: 656d 705f 636f 6c6f 726d 6170 da03 6b65  emp_colormap..ke
-000007b0: 79da 0576 616c 7565 da09 6572 726f 725f  y..value..error_
-000007c0: 6d73 6772 2e00 0000 722e 0000 0072 2f00  msgr....r....r/.
-000007d0: 0000 da11 7265 7374 6f72 655f 6172 6775  ....restore_argu
-000007e0: 6d65 6e74 7356 0000 0073 3e00 0000 0401  mentsV...s>.....
-000007f0: 1001 1001 0801 0201 0a01 0a01 0a01 0e01  ................
-00000800: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00000810: 0a01 0a01 0601 0a01 0201 0401 0801 0a01  ................
-00000820: 0280 1003 0801 0801 0280 0802 7236 0000  ............r6..
-00000830: 0063 0000 0000 0000 0000 0000 0000 0500  .c..............
-00000840: 0000 0600 0000 4300 0000 736e 0100 0067  ......C...sn...g
-00000850: 0064 01a2 017d 0047 0064 0264 0384 0064  .d...}.G.d.d...d
-00000860: 0383 027d 017c 0164 2c69 0064 0464 0593  ...}.|.d,i.d.d..
-00000870: 0164 0664 0793 0164 0864 0793 0164 0964  .d.d...d.d...d.d
-00000880: 0793 0164 0a64 0793 0164 0b64 0793 0164  ...d.d...d.d...d
-00000890: 0c64 0d93 0164 0e64 0d93 0164 0f64 0d93  .d...d.d...d.d..
-000008a0: 0164 1064 0d93 0164 1164 0d93 0164 1264  .d.d...d.d...d.d
-000008b0: 0d93 0164 1364 0d93 0164 1464 0d93 0164  ...d.d...d.d...d
-000008c0: 1564 0d93 0164 1664 0d93 0164 1764 0d93  .d...d.d...d.d..
-000008d0: 0164 1864 0d93 0164 1964 0d93 0164 1a64  .d.d...d.d...d.d
-000008e0: 0d93 0164 1b64 0d93 0164 1c64 0d93 0164  ...d.d...d.d...d
-000008f0: 1d64 0d93 0164 1e64 0d93 0164 1f64 0d93  .d...d.d...d.d..
-00000900: 0164 2064 0d93 0164 2164 0d93 0164 2264  .d d...d!d...d"d
-00000910: 0793 0164 2364 2493 0164 2564 0793 0164  ...d#d$..d%d...d
-00000920: 2664 0793 0164 2764 0793 018e 017d 0274  &d...d'd.....}.t
-00000930: 006a 0144 005d 417d 037c 0364 286b 0272  .j.D.]A}.|.d(k.r
-00000940: 7a71 737c 03a0 0264 29a1 017d 0474 037c  zqs|...d)..}.t.|
-00000950: 0483 0164 056b 0272 8a7c 04a0 0464 2aa1  ...d.k.r.|...d*.
-00000960: 0101 007c 0464 2b19 0064 046b 0272 9874  ...|.d+..d.k.r.t
-00000970: 057c 0464 0519 0083 017c 0464 053c 007c  .|.d.....|.d.<.|
-00000980: 0464 2b19 007c 0076 0072 aa74 067c 027c  .d+..|.v.r.t.|.|
-00000990: 0464 2b19 007c 0464 0519 0067 0183 0301  .d+..|.d...g....
-000009a0: 0071 7374 067c 027c 0464 2b19 007c 0464  .qst.|.|.d+..|.d
-000009b0: 0519 0083 0301 0071 737c 0253 0029 2d7a  .......qs|.S.)-z
-000009c0: 760a 2020 2020 2320 4765 7420 6172 6775  v.    # Get argu
-000009d0: 6d65 6e74 7320 6672 6f6d 2072 756e 5f74  ments from run_t
-000009e0: 6573 742e 7079 2061 6e64 2070 726f 6365  est.py and proce
-000009f0: 7373 2074 6865 6d20 666f 7220 756e 6974  ss them for unit
-00000a00: 2074 6573 7469 6e67 0a20 2020 2020 2020   testing.       
-00000a10: 203a 7265 7475 726e 3a20 4e61 6d65 7370   :return: Namesp
-00000a20: 6163 6520 7769 7468 2061 7267 756d 656e  ace with argumen
-00000a30: 7473 0a20 2020 2029 0372 1c00 0000 721e  ts.    ).r....r.
-00000a40: 0000 0072 2000 0000 6300 0000 0000 0000  ...r ...c.......
-00000a50: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00000a60: 0073 1400 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00000a70: 6402 8400 5a03 6403 5300 2904 7a1c 756e  d...Z.d.S.).z.un
-00000a80: 6974 5f74 6573 742e 3c6c 6f63 616c 733e  it_test.<locals>
-00000a90: 2e4e 616d 6573 7061 6365 6301 0000 0000  .Namespacec.....
-00000aa0: 0000 0000 0000 0002 0000 0003 0000 005b  ...............[
-00000ab0: 0000 0073 1000 0000 7c00 6a00 a001 7c01  ...s....|.j...|.
-00000ac0: a101 0100 6400 5300 2901 4e29 02da 085f  ....d.S.).N)..._
-00000ad0: 5f64 6963 745f 5fda 0675 7064 6174 6529  _dict__..update)
-00000ae0: 02da 0473 656c 66da 066b 7761 7267 7372  ...self..kwargsr
-00000af0: 2e00 0000 722e 0000 0072 2f00 0000 da08  ....r....r/.....
-00000b00: 5f5f 696e 6974 5f5f 8400 0000 7302 0000  __init__....s...
-00000b10: 0010 017a 2575 6e69 745f 7465 7374 2e3c  ...z%unit_test.<
-00000b20: 6c6f 6361 6c73 3e2e 4e61 6d65 7370 6163  locals>.Namespac
-00000b30: 652e 5f5f 696e 6974 5f5f 4e29 04da 085f  e.__init__N)..._
-00000b40: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000b50: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000b60: 5f72 3b00 0000 722e 0000 0072 2e00 0000  _r;...r....r....
-00000b70: 722e 0000 0072 2f00 0000 da09 4e61 6d65  r....r/.....Name
-00000b80: 7370 6163 6583 0000 0073 0400 0000 0800  space....s......
-00000b90: 0c01 723f 0000 0072 1800 0000 e901 0000  ..r?...r........
-00000ba0: 0072 1900 0000 4672 1200 0000 da01 6772  .r....Fr......gr
-00000bb0: 1a00 0000 721b 0000 0072 1c00 0000 4e72  ....r....r....Nr
-00000bc0: 1e00 0000 7220 0000 005a 0863 5072 6f6a  ....r ...Z.cProj
-00000bd0: 6563 745a 0863 5072 6f66 696c 655a 0563  ectZ.cProfileZ.c
-00000be0: 5461 736b 5a07 6341 6374 696f 6e5a 1063  TaskZ.cActionZ.c
-00000bf0: 4469 7361 626c 6564 5072 6f66 696c 655a  DisabledProfileZ
-00000c00: 0c63 556e 6b6e 6f77 6e54 6173 6b5a 0f63  .cUnknownTaskZ.c
-00000c10: 4469 7361 626c 6564 4163 7469 6f6e 5a10  DisabledActionZ.
-00000c20: 6341 6374 696f 6e43 6f6e 6469 7469 6f6e  cActionCondition
-00000c30: 5a11 6350 726f 6669 6c65 436f 6e64 6974  Z.cProfileCondit
-00000c40: 696f 6e5a 0d63 4c61 756e 6368 6572 5461  ionZ.cLauncherTa
-00000c50: 736b 5a0b 6342 6163 6b67 726f 756e 645a  skZ.cBackgroundZ
-00000c60: 0663 5363 656e 655a 0763 4275 6c6c 6574  .cSceneZ.cBullet
-00000c70: 5a0c 6341 6374 696f 6e4c 6162 656c 5a0b  Z.cActionLabelZ.
-00000c80: 6341 6374 696f 6e4e 616d 655a 0e63 5461  cActionNameZ.cTa
-00000c90: 736b 6572 4e65 7449 6e66 6f5a 0c63 5072  skerNetInfoZ.cPr
-00000ca0: 6566 6572 656e 6365 735a 1163 5472 6169  eferencesZ.cTrai
-00000cb0: 6c69 6e67 436f 6d6d 656e 7473 7210 0000  lingCommentsr...
-00000cc0: 0072 2200 0000 5472 2700 0000 da01 7272  .r"...Tr'.....rr
-00000cd0: 2400 0000 fa09 2d74 6573 743d 7965 7372  $.....-test=yesr
-00000ce0: 2600 0000 da01 3172 0100 0000 722e 0000  &.....1r....r...
-00000cf0: 0029 07da 0373 7973 da04 6172 6776 da05  .)...sys..argv..
-00000d00: 7370 6c69 74da 036c 656e da06 6170 7065  split..len..appe
-00000d10: 6e64 7232 0000 00da 0773 6574 6174 7472  ndr2.....setattr
-00000d20: 2905 5a0c 7369 6e67 6c65 5f6e 616d 6573  ).Z.single_names
-00000d30: 723f 0000 0072 0c00 0000 5a0c 7468 655f  r?...r....Z.the_
-00000d40: 6172 6775 6d65 6e74 5a07 6e65 775f 6172  argumentZ.new_ar
-00000d50: 6772 2e00 0000 722e 0000 0072 2f00 0000  gr....r....r/...
-00000d60: da09 756e 6974 5f74 6573 747c 0000 0073  ..unit_test|...s
-00000d70: 9e00 0000 0805 0e02 0805 0401 02ff 0402  ................
-00000d80: 02fe 0403 02fd 0404 02fc 0405 02fb 0406  ................
-00000d90: 02fa 0407 02f9 0408 02f8 0409 02f7 040a  ................
-00000da0: 02f6 040b 02f5 040c 02f4 040d 02f3 040e  ................
-00000db0: 02f2 040f 02f1 0410 02f0 0411 02ef 0412  ................
-00000dc0: 02ee 0413 02ed 0414 02ec 0415 02eb 0416  ................
-00000dd0: 02ea 0417 02e9 0418 02e8 0419 02e7 041a  ................
-00000de0: 02e6 041b 02e5 041c 02e4 041d 02e3 041e  ................
-00000df0: 02e2 041f 02e1 0420 04e0 0a23 0801 0201  ....... ...#....
-00000e00: 0a01 0c02 0a01 0c02 1001 0c02 1801 1602  ................
-00000e10: 0402 724b 0000 0063 0100 0000 0000 0000  ..rK...c........
-00000e20: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00000e30: 7384 0000 0074 0083 007d 0164 0174 016a  s....t...}.d.t.j
-00000e40: 0276 0072 0b74 0383 006e 0274 0483 007d  .v.r.t...n.t...}
-00000e50: 0274 05a0 0664 027c 029b 009d 02a1 0101  .t...d.|........
-00000e60: 0074 077c 0264 0383 0272 2674 087c 0064  .t.|.d...r&t.|.d
-00000e70: 0483 025c 027d 017d 007c 017c 0066 0253  ...\.}.}.|.|.f.S
-00000e80: 0074 077c 0264 0583 0272 3674 097c 017c  .t.|.d...r6t.|.|
-00000e90: 0083 025c 027d 017d 007c 017c 0066 0253  ...\.}.}.|.|.f.S
-00000ea0: 0074 0a7c 027c 017c 0083 035c 027d 017d  .t.|.|.|...\.}.}
-00000eb0: 007c 017c 0066 0253 0029 064e 7243 0000  .|.|.f.S.).NrC..
-00000ec0: 007a 1350 726f 6772 616d 2061 7267 756d  .z.Program argum
-00000ed0: 656e 7473 3a20 7241 0000 0054 7242 0000  ents: rA...TrB..
-00000ee0: 0029 0b72 0700 0000 7245 0000 0072 4600  .).r....rE...rF.
-00000ef0: 0000 724b 0000 0072 0500 0000 720b 0000  ..rK...r....r...
-00000f00: 0072 2300 0000 7228 0000 0072 0600 0000  .r#...r(...r....
-00000f10: 7236 0000 0072 3000 0000 2903 720e 0000  r6...r0...).r...
-00000f20: 0072 0d00 0000 720c 0000 0072 2e00 0000  .r....r....r....
-00000f30: 722e 0000 0072 2f00 0000 da0b 7072 6f63  r....r/.....proc
-00000f40: 6573 735f 636c 69c2 0000 0073 2800 0000  ess_cli....s(...
-00000f50: 0602 1603 1001 0a03 0804 02fd 0201 0201  ................
-00000f60: 020d 0201 04fe 0af7 0e02 0208 0201 04fe  ................
-00000f70: 10fd 0204 0201 04fe 724c 0000 0029 1872  ........rL...).r
-00000f80: 4500 0000 5a14 6d61 7074 6173 6b65 722e  E...Z.maptasker.
-00000f90: 7372 632e 636f 6c6f 7273 7202 0000 0072  src.colorsr....r
-00000fa0: 0300 0000 5a17 6d61 7074 6173 6b65 722e  ....Z.maptasker.
-00000fb0: 7372 632e 6765 7470 7574 6172 6772 0400  src.getputargr..
-00000fc0: 0000 5a16 6d61 7074 6173 6b65 722e 7372  ..Z.maptasker.sr
-00000fd0: 632e 7061 7273 6561 7267 7205 0000 00da  c.parseargr.....
-00000fe0: 146d 6170 7461 736b 6572 2e73 7263 2e72  .maptasker.src.r
-00000ff0: 756e 6775 6972 0600 0000 5a16 6d61 7074  unguir....Z.mapt
-00001000: 6173 6b65 722e 7372 632e 696e 6974 7061  asker.src.initpa
-00001010: 7267 7207 0000 00da 166d 6170 7461 736b  rgr......maptask
-00001020: 6572 2e73 7263 2e73 7973 636f 6e73 7472  er.src.sysconstr
-00001030: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
-00001040: 0000 00da 066f 626a 6563 74da 0464 6963  .....object..dic
-00001050: 74da 0574 7570 6c65 7230 0000 0072 3600  t..tupler0...r6.
-00001060: 0000 724b 0000 0072 4c00 0000 722e 0000  ..rK...rL...r...
-00001070: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00001080: da08 3c6d 6f64 756c 653e 0100 0000 731e  ..<module>....s.
-00001090: 0000 0008 120c 020c 010c 010c 010c 010c  ................
-000010a0: 010c 020c 010c 010c 011a 0616 310e 2616  ............1.&.
-000010b0: 46                                       F
+000000a0: 0100 6400 640b 6c0c 6d10 5a10 0100 6400  ..d.d.l.m.Z...d.
+000000b0: 640c 6c11 6d12 5a12 0100 640d 6513 640e  d.l.m.Z...d.e.d.
+000000c0: 6514 640f 6514 6410 6515 6608 6411 6412  e.d.e.d.e.f.d.d.
+000000d0: 8404 5a16 640e 6514 640f 6514 6410 6515  ..Z.d.e.d.e.d.e.
+000000e0: 6606 6413 6414 8404 5a17 6410 6513 6602  f.d.d...Z.d.e.f.
+000000f0: 6415 6416 8404 5a18 640f 6514 6410 6515  d.d...Z.d.e.d.e.
+00000100: 6604 6417 6418 8404 5a19 6401 5300 2919  f.d.d...Z.d.S.).
+00000110: e900 0000 004e 2901 da15 6765 745f 616e  .....N)...get_an
+00000120: 645f 7365 745f 7468 655f 636f 6c6f 7229  d_set_the_color)
+00000130: 01da 0e76 616c 6964 6174 655f 636f 6c6f  ...validate_colo
+00000140: 7229 01da 1173 6176 655f 7265 7374 6f72  r)...save_restor
+00000150: 655f 6172 6773 2901 da0e 7275 6e74 696d  e_args)...runtim
+00000160: 655f 7061 7273 6572 2901 da0b 7072 6f63  e_parser)...proc
+00000170: 6573 735f 6775 6929 01da 1c69 6e69 7469  ess_gui)...initi
+00000180: 616c 697a 655f 7275 6e74 696d 655f 6172  alize_runtime_ar
+00000190: 6775 6d65 6e74 7329 01da 0a4d 595f 4c49  guments)...MY_LI
+000001a0: 4345 4e53 4529 01da 0a4d 595f 5645 5253  CENSE)...MY_VERS
+000001b0: 494f 4e29 01da 0f54 5950 4553 5f4f 465f  ION)...TYPES_OF_
+000001c0: 434f 4c4f 5253 2901 da06 6c6f 6767 6572  COLORS)...logger
+000001d0: 2901 da0d 6572 726f 725f 6861 6e64 6c65  )...error_handle
+000001e0: 72da 0461 7267 73da 0970 726f 675f 6172  r..args..prog_ar
+000001f0: 6773 da08 636f 6c6f 726d 6170 da06 7265  gs..colormap..re
+00000200: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
+00000210: 0005 0000 0007 0000 0043 0000 0073 8401  .........C...s..
+00000220: 0000 7400 7c00 6401 8302 7209 7401 6402  ..t.|.d...r.t.d.
+00000230: 8301 0100 7400 7c00 6403 8302 721f 6404  ....t.|.d...r.d.
+00000240: 7c01 6405 3c00 6406 7c01 6407 3c00 6406  |.d.<.d.|.d.<.d.
+00000250: 7c01 6408 3c00 6406 7c01 6409 3c00 6e1c  |.d.<.d.|.d.<.n.
+00000260: 7400 7c00 640a 8302 7c01 6405 3c00 7400  t.|.d...|.d.<.t.
+00000270: 7c00 640b 8302 7c01 6407 3c00 7400 7c00  |.d...|.d.<.t.|.
+00000280: 640c 8302 7c01 6408 3c00 7400 7c00 640d  d...|.d.<.t.|.d.
+00000290: 8302 7c01 6409 3c00 7400 7c00 640e 8302  ..|.d.<.t.|.d...
+000002a0: 7d03 7c03 6400 7501 724a 7c03 640f 1900  }.|.d.u.rJ|.d...
+000002b0: 7c01 6410 3c00 7400 7c00 6411 8302 7d03  |.d.<.t.|.d...}.
+000002c0: 7c03 6400 7501 7259 7c03 640f 1900 7c01  |.d.u.rY|.d...|.
+000002d0: 6412 3c00 7400 7c00 6413 8302 7d03 7c03  d.<.t.|.d...}.|.
+000002e0: 6400 7501 7268 7c03 640f 1900 7c01 6414  d.u.rh|.d...|.d.
+000002f0: 3c00 7400 7c00 6415 8302 7271 6406 7c01  <.t.|.d...rqd.|.
+00000300: 6416 3c00 7400 7c00 6417 8302 7283 7402  d.<.t.|.d...r.t.
+00000310: 7403 9b00 6418 7404 9b00 9d03 8301 0100  t...d.t.........
+00000320: 7405 640f 8301 0100 7406 4400 5d2d 7d04  t.d.....t.D.]-}.
+00000330: 7400 7c00 6419 7c04 9b00 9d02 8302 7d03  t.|.d.|.......}.
+00000340: 7c03 6400 7501 72b2 7407 7c03 8301 7408  |.d.u.r.t.|...t.
+00000350: 7500 72a7 7409 641a 7c04 9b00 641b 7c03  u.r.t.d.|...d.|.
+00000360: 640f 1900 9b00 9d04 7c02 8302 0100 7185  d.......|.....q.
+00000370: 7409 641a 7c04 9b00 641b 7c03 9b00 9d04  t.d.|...d.|.....
+00000380: 7c02 8302 0100 7185 7400 7c00 641c 8302  |.....q.t.|.d...
+00000390: 72be 740a 6406 7c02 7c01 8303 0100 7c01  r.t.d.|.|.....|.
+000003a0: 7c02 6602 5300 291d 4eda 0263 68da 0168  |.f.S.).N..ch..h
+000003b0: da01 65e9 0300 0000 da14 6469 7370 6c61  ..e.......displa
+000003c0: 795f 6465 7461 696c 5f6c 6576 656c 54da  y_detail_levelT.
+000003d0: 1a64 6973 706c 6179 5f70 726f 6669 6c65  .display_profile
+000003e0: 5f63 6f6e 6469 7469 6f6e 73da 1364 6973  _conditions..dis
+000003f0: 706c 6179 5f70 7265 6665 7265 6e63 6573  play_preferences
+00000400: da11 6469 7370 6c61 795f 7461 736b 6572  ..display_tasker
+00000410: 6e65 74da 0664 6574 6169 6cda 0a63 6f6e  net..detail..con
+00000420: 6469 7469 6f6e 73da 0170 da09 7461 736b  ditions..p..task
+00000430: 6572 6e65 74da 0770 726f 6a65 6374 7201  ernet..projectr.
+00000440: 0000 00da 1373 696e 676c 655f 7072 6f6a  .....single_proj
+00000450: 6563 745f 6e61 6d65 da07 7072 6f66 696c  ect_name..profil
+00000460: 65da 1373 696e 676c 655f 7072 6f66 696c  e..single_profil
+00000470: 655f 6e61 6d65 da04 7461 736b da10 7369  e_name..task..si
+00000480: 6e67 6c65 5f74 6173 6b5f 6e61 6d65 da01  ngle_task_name..
+00000490: 64da 0564 6562 7567 da01 767a 102c 2075  d..debug..vz., u
+000004a0: 6e64 6572 206c 6963 656e 7365 20da 0163  nder license ..c
+000004b0: 7a02 2d63 fa01 3dda 0173 290b da07 6765  z.-c..=..s)...ge
+000004c0: 7461 7474 7272 0300 0000 da05 7072 696e  tattrr......prin
+000004d0: 7472 0900 0000 7208 0000 00da 0465 7869  tr....r......exi
+000004e0: 7472 0a00 0000 da04 7479 7065 da04 6c69  tr......type..li
+000004f0: 7374 7202 0000 0072 0400 0000 2905 720d  str....r....).r.
+00000500: 0000 0072 0e00 0000 720f 0000 005a 0874  ...r....r....Z.t
+00000510: 6865 5f6e 616d 65da 0469 7465 6da9 0072  he_name..item..r
+00000520: 2f00 0000 fa75 2f55 7365 7273 2f6d 696b  /....u/Users/mik
+00000530: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
+00000540: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
+00000550: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
+00000560: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
+00000570: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
+00000580: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
+00000590: 632f 7275 6e63 6c69 2e70 79da 1170 726f  c/runcli.py..pro
+000005a0: 6365 7373 5f61 7267 756d 656e 7473 2600  cess_arguments&.
+000005b0: 0000 7346 0000 000a 0208 010a 0208 0108  ..sF............
+000005c0: 0108 010a 010e 020e 010e 010e 010a 0108  ................
+000005d0: 010c 010a 0108 010c 010a 0108 010c 010a  ................
+000005e0: 0108 010a 0112 0108 0108 0310 0108 010c  ................
+000005f0: 011c 0116 0202 800a 030c 0108 0272 3100  .............r1.
+00000600: 0000 6302 0000 0000 0000 0000 0000 0006  ..c.............
+00000610: 0000 0004 0000 0043 0000 0073 0601 0000  .......C...s....
+00000620: 6900 7d02 7400 6401 7c01 7c02 8303 5c02  i.}.t.d.|.|...\.
+00000630: 7d02 7d03 7c02 a001 a100 4400 5d5f 5c02  }.}.|.....D.]_\.
+00000640: 7d04 7d05 7c04 6400 7501 726d 7c04 0400  }.}.|.d.u.rm|...
+00000650: 6402 6b02 7221 0100 7c05 7c00 6402 3c00  d.k.r!..|.|.d.<.
+00000660: 6e4c 0400 6403 6b02 722d 0100 7402 7c05  nL..d.k.r-..t.|.
+00000670: 8301 7c00 6403 3c00 6e40 0400 6404 6b02  ..|.d.<.n@..d.k.
+00000680: 7237 0100 7c05 7c00 6404 3c00 6e36 0400  r7..|.|.d.<.n6..
+00000690: 6405 6b02 7241 0100 7c05 7c00 6405 3c00  d.k.rA..|.|.d.<.
+000006a0: 6e2c 0400 6406 6b02 724b 0100 7c05 7c00  n,..d.k.rK..|.|.
+000006b0: 6406 3c00 6e22 0400 6407 6b02 7255 0100  d.<.n"..d.k.rU..
+000006c0: 7c05 7c00 6407 3c00 6e18 0400 6408 6b02  |.|.d.<.n...d.k.
+000006d0: 725f 0100 7c05 7c00 6408 3c00 6e0e 6409  r_..|.|.d.<.n.d.
+000006e0: 6b02 7267 7c05 7c00 6409 3c00 6e06 0900  k.rg|.|.d.<.n...
+000006f0: 7403 640a 640b 8302 0100 710e 7c03 a001  t.d.d.....q.|...
+00000700: a100 4400 5d0c 5c02 7d04 7d05 7c04 6400  ..D.].\.}.}.|.d.
+00000710: 7501 727e 7c05 7c01 7c04 3c00 7172 7c00  u.r~|.|.|.<.qr|.
+00000720: 7c01 6602 5300 290c 4e46 7224 0000 0072  |.f.S.).NFr$...r
+00000730: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00000740: 0000 0072 2000 0000 721e 0000 0072 2200  ...r ...r....r".
+00000750: 0000 7a1a 496e 7661 6c69 6420 6172 6775  ..z.Invalid argu
+00000760: 6d65 6e74 2072 6573 746f 7265 6421 7201  ment restored!r.
+00000770: 0000 0029 0472 0400 0000 da05 6974 656d  ...).r......item
+00000780: 73da 0369 6e74 720c 0000 0029 0672 0e00  s..intr....).r..
+00000790: 0000 720f 0000 00da 0974 656d 705f 6172  ..r......temp_ar
+000007a0: 6773 5a0d 7465 6d70 5f63 6f6c 6f72 6d61  gsZ.temp_colorma
+000007b0: 70da 036b 6579 da05 7661 6c75 6572 2f00  p..key..valuer/.
+000007c0: 0000 722f 0000 0072 3000 0000 da11 7265  ..r/...r0.....re
+000007d0: 7374 6f72 655f 6172 6775 6d65 6e74 7357  store_argumentsW
+000007e0: 0000 0073 3a00 0000 0401 1001 1001 0801  ...s:...........
+000007f0: 0201 0a01 0a01 0a01 0e01 0a01 0a01 0a01  ................
+00000800: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0601  ................
+00000810: 0a01 0201 0a01 0280 1003 0801 0801 0280  ................
+00000820: 0802 7237 0000 0063 0000 0000 0000 0000  ..r7...c........
+00000830: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
+00000840: 736e 0100 0067 0064 01a2 017d 0047 0064  sn...g.d...}.G.d
+00000850: 0264 0384 0064 0383 027d 017c 0164 2c69  .d...d...}.|.d,i
+00000860: 0064 0464 0593 0164 0664 0793 0164 0864  .d.d...d.d...d.d
+00000870: 0793 0164 0964 0793 0164 0a64 0793 0164  ...d.d...d.d...d
+00000880: 0b64 0793 0164 0c64 0d93 0164 0e64 0d93  .d...d.d...d.d..
+00000890: 0164 0f64 0d93 0164 1064 0d93 0164 1164  .d.d...d.d...d.d
+000008a0: 0d93 0164 1264 0d93 0164 1364 0d93 0164  ...d.d...d.d...d
+000008b0: 1464 0d93 0164 1564 0d93 0164 1664 0d93  .d...d.d...d.d..
+000008c0: 0164 1764 0d93 0164 1864 0d93 0164 1964  .d.d...d.d...d.d
+000008d0: 0d93 0164 1a64 0d93 0164 1b64 0d93 0164  ...d.d...d.d...d
+000008e0: 1c64 0d93 0164 1d64 0d93 0164 1e64 0d93  .d...d.d...d.d..
+000008f0: 0164 1f64 0d93 0164 2064 0d93 0164 2164  .d.d...d d...d!d
+00000900: 0d93 0164 2264 0793 0164 2364 2493 0164  ...d"d...d#d$..d
+00000910: 2564 0793 0164 2664 0793 0164 2764 0793  %d...d&d...d'd..
+00000920: 018e 017d 0274 006a 0144 005d 417d 037c  ...}.t.j.D.]A}.|
+00000930: 0364 286b 0272 7a71 737c 03a0 0264 29a1  .d(k.rzqs|...d).
+00000940: 017d 0474 037c 0483 0164 056b 0272 8a7c  .}.t.|...d.k.r.|
+00000950: 04a0 0464 2aa1 0101 007c 0464 2b19 0064  ...d*....|.d+..d
+00000960: 046b 0272 9874 057c 0464 0519 0083 017c  .k.r.t.|.d.....|
+00000970: 0464 053c 007c 0464 2b19 007c 0076 0072  .d.<.|.d+..|.v.r
+00000980: aa74 067c 027c 0464 2b19 007c 0464 0519  .t.|.|.d+..|.d..
+00000990: 0067 0183 0301 0071 7374 067c 027c 0464  .g.....qst.|.|.d
+000009a0: 2b19 007c 0464 0519 0083 0301 0071 737c  +..|.d.......qs|
+000009b0: 0253 0029 2d7a 760a 2020 2020 2320 4765  .S.)-zv.    # Ge
+000009c0: 7420 6172 6775 6d65 6e74 7320 6672 6f6d  t arguments from
+000009d0: 2072 756e 5f74 6573 742e 7079 2061 6e64   run_test.py and
+000009e0: 2070 726f 6365 7373 2074 6865 6d20 666f   process them fo
+000009f0: 7220 756e 6974 2074 6573 7469 6e67 0a20  r unit testing. 
+00000a00: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00000a10: 4e61 6d65 7370 6163 6520 7769 7468 2061  Namespace with a
+00000a20: 7267 756d 656e 7473 0a20 2020 2029 0372  rguments.    ).r
+00000a30: 1d00 0000 721f 0000 0072 2100 0000 6300  ....r....r!...c.
+00000a40: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00000a50: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
+00000a60: 6400 5a02 6401 6402 8400 5a03 6403 5300  d.Z.d.d...Z.d.S.
+00000a70: 2904 7a1c 756e 6974 5f74 6573 742e 3c6c  ).z.unit_test.<l
+00000a80: 6f63 616c 733e 2e4e 616d 6573 7061 6365  ocals>.Namespace
+00000a90: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000aa0: 0003 0000 005b 0000 0073 1000 0000 7c00  .....[...s....|.
+00000ab0: 6a00 a001 7c01 a101 0100 6400 5300 2901  j...|.....d.S.).
+00000ac0: 4e29 02da 085f 5f64 6963 745f 5fda 0675  N)...__dict__..u
+00000ad0: 7064 6174 6529 02da 0473 656c 66da 066b  pdate)...self..k
+00000ae0: 7761 7267 7372 2f00 0000 722f 0000 0072  wargsr/...r/...r
+00000af0: 3000 0000 da08 5f5f 696e 6974 5f5f 8300  0.....__init__..
+00000b00: 0000 7302 0000 0010 017a 2575 6e69 745f  ..s......z%unit_
+00000b10: 7465 7374 2e3c 6c6f 6361 6c73 3e2e 4e61  test.<locals>.Na
+00000b20: 6d65 7370 6163 652e 5f5f 696e 6974 5f5f  mespace.__init__
+00000b30: 4e29 04da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000b40: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000b50: 6c6e 616d 655f 5f72 3c00 0000 722f 0000  lname__r<...r/..
+00000b60: 0072 2f00 0000 722f 0000 0072 3000 0000  .r/...r/...r0...
+00000b70: da09 4e61 6d65 7370 6163 6582 0000 0073  ..Namespace....s
+00000b80: 0400 0000 0800 0c01 7240 0000 0072 1900  ........r@...r..
+00000b90: 0000 e901 0000 0072 1a00 0000 4672 1300  .......r....Fr..
+00000ba0: 0000 da01 6772 1b00 0000 721c 0000 0072  ....gr....r....r
+00000bb0: 1d00 0000 4e72 1f00 0000 7221 0000 005a  ....Nr....r!...Z
+00000bc0: 0863 5072 6f6a 6563 745a 0863 5072 6f66  .cProjectZ.cProf
+00000bd0: 696c 655a 0563 5461 736b 5a07 6341 6374  ileZ.cTaskZ.cAct
+00000be0: 696f 6e5a 1063 4469 7361 626c 6564 5072  ionZ.cDisabledPr
+00000bf0: 6f66 696c 655a 0c63 556e 6b6e 6f77 6e54  ofileZ.cUnknownT
+00000c00: 6173 6b5a 0f63 4469 7361 626c 6564 4163  askZ.cDisabledAc
+00000c10: 7469 6f6e 5a10 6341 6374 696f 6e43 6f6e  tionZ.cActionCon
+00000c20: 6469 7469 6f6e 5a11 6350 726f 6669 6c65  ditionZ.cProfile
+00000c30: 436f 6e64 6974 696f 6e5a 0d63 4c61 756e  ConditionZ.cLaun
+00000c40: 6368 6572 5461 736b 5a0b 6342 6163 6b67  cherTaskZ.cBackg
+00000c50: 726f 756e 645a 0663 5363 656e 655a 0763  roundZ.cSceneZ.c
+00000c60: 4275 6c6c 6574 5a0c 6341 6374 696f 6e4c  BulletZ.cActionL
+00000c70: 6162 656c 5a0b 6341 6374 696f 6e4e 616d  abelZ.cActionNam
+00000c80: 655a 0e63 5461 736b 6572 4e65 7449 6e66  eZ.cTaskerNetInf
+00000c90: 6f5a 0c63 5072 6566 6572 656e 6365 735a  oZ.cPreferencesZ
+00000ca0: 1163 5472 6169 6c69 6e67 436f 6d6d 656e  .cTrailingCommen
+00000cb0: 7473 7211 0000 0072 2300 0000 5472 2800  tsr....r#...Tr(.
+00000cc0: 0000 da01 7272 2500 0000 fa09 2d74 6573  ....rr%.....-tes
+00000cd0: 743d 7965 7372 2700 0000 da01 3172 0100  t=yesr'.....1r..
+00000ce0: 0000 722f 0000 0029 07da 0373 7973 da04  ..r/...)...sys..
+00000cf0: 6172 6776 da05 7370 6c69 74da 036c 656e  argv..split..len
+00000d00: da06 6170 7065 6e64 7233 0000 00da 0773  ..appendr3.....s
+00000d10: 6574 6174 7472 2905 5a0c 7369 6e67 6c65  etattr).Z.single
+00000d20: 5f6e 616d 6573 7240 0000 0072 0d00 0000  _namesr@...r....
+00000d30: 5a0c 7468 655f 6172 6775 6d65 6e74 5a07  Z.the_argumentZ.
+00000d40: 6e65 775f 6172 6772 2f00 0000 722f 0000  new_argr/...r/..
+00000d50: 0072 3000 0000 da09 756e 6974 5f74 6573  .r0.....unit_tes
+00000d60: 747b 0000 0073 9e00 0000 0805 0e02 0805  t{...s..........
+00000d70: 0401 02ff 0402 02fe 0403 02fd 0404 02fc  ................
+00000d80: 0405 02fb 0406 02fa 0407 02f9 0408 02f8  ................
+00000d90: 0409 02f7 040a 02f6 040b 02f5 040c 02f4  ................
+00000da0: 040d 02f3 040e 02f2 040f 02f1 0410 02f0  ................
+00000db0: 0411 02ef 0412 02ee 0413 02ed 0414 02ec  ................
+00000dc0: 0415 02eb 0416 02ea 0417 02e9 0418 02e8  ................
+00000dd0: 0419 02e7 041a 02e6 041b 02e5 041c 02e4  ................
+00000de0: 041d 02e3 041e 02e2 041f 02e1 0420 04e0  ............. ..
+00000df0: 0a23 0801 0201 0a01 0c02 0a01 0c02 1001  .#..............
+00000e00: 0c02 1801 1602 0402 724c 0000 0063 0100  ........rL...c..
+00000e10: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00000e20: 0000 4300 0000 7384 0000 0074 0083 007d  ..C...s....t...}
+00000e30: 0164 0174 016a 0276 0072 0b74 0383 006e  .d.t.j.v.r.t...n
+00000e40: 0274 0483 007d 0274 05a0 0664 027c 029b  .t...}.t...d.|..
+00000e50: 009d 02a1 0101 0074 077c 0264 0383 0272  .......t.|.d...r
+00000e60: 2674 087c 0064 0483 025c 027d 017d 007c  &t.|.d...\.}.}.|
+00000e70: 017c 0066 0253 0074 077c 0264 0583 0272  .|.f.S.t.|.d...r
+00000e80: 3674 097c 017c 0083 025c 027d 017d 007c  6t.|.|...\.}.}.|
+00000e90: 017c 0066 0253 0074 0a7c 027c 017c 0083  .|.f.S.t.|.|.|..
+00000ea0: 035c 027d 017d 007c 017c 0066 0253 0029  .\.}.}.|.|.f.S.)
+00000eb0: 064e 7244 0000 007a 1350 726f 6772 616d  .NrD...z.Program
+00000ec0: 2061 7267 756d 656e 7473 3a20 7242 0000   arguments: rB..
+00000ed0: 0054 7243 0000 0029 0b72 0700 0000 7246  .TrC...).r....rF
+00000ee0: 0000 0072 4700 0000 724c 0000 0072 0500  ...rG...rL...r..
+00000ef0: 0000 720b 0000 0072 2400 0000 7229 0000  ..r....r$...r)..
+00000f00: 0072 0600 0000 7237 0000 0072 3100 0000  .r....r7...r1...
+00000f10: 2903 720f 0000 0072 0e00 0000 720d 0000  ).r....r....r...
+00000f20: 0072 2f00 0000 722f 0000 0072 3000 0000  .r/...r/...r0...
+00000f30: da0b 7072 6f63 6573 735f 636c 69c1 0000  ..process_cli...
+00000f40: 0073 2800 0000 0602 1603 1001 0a03 0804  .s(.............
+00000f50: 02fd 0201 0201 020d 0201 04fe 0af7 0e02  ................
+00000f60: 0208 0201 04fe 10fd 0204 0201 04fe 724d  ..............rM
+00000f70: 0000 0029 1a72 4600 0000 5a14 6d61 7074  ...).rF...Z.mapt
+00000f80: 6173 6b65 722e 7372 632e 636f 6c6f 7273  asker.src.colors
+00000f90: 7202 0000 0072 0300 0000 da17 6d61 7074  r....r......mapt
+00000fa0: 6173 6b65 722e 7372 632e 6765 7470 7574  asker.src.getput
+00000fb0: 6172 6772 0400 0000 5a16 6d61 7074 6173  argr....Z.maptas
+00000fc0: 6b65 722e 7372 632e 7061 7273 6561 7267  ker.src.parsearg
+00000fd0: 7205 0000 00da 146d 6170 7461 736b 6572  r......maptasker
+00000fe0: 2e73 7263 2e72 756e 6775 6972 0600 0000  .src.runguir....
+00000ff0: 5a16 6d61 7074 6173 6b65 722e 7372 632e  Z.maptasker.src.
+00001000: 696e 6974 7061 7267 7207 0000 00da 166d  initpargr......m
+00001010: 6170 7461 736b 6572 2e73 7263 2e73 7973  aptasker.src.sys
+00001020: 636f 6e73 7472 0800 0000 7209 0000 0072  constr....r....r
+00001030: 0a00 0000 720b 0000 00da 136d 6170 7461  ....r......mapta
+00001040: 736b 6572 2e73 7263 2e65 7272 6f72 720c  sker.src.errorr.
+00001050: 0000 00da 066f 626a 6563 74da 0464 6963  .....object..dic
+00001060: 74da 0574 7570 6c65 7231 0000 0072 3700  t..tupler1...r7.
+00001070: 0000 724c 0000 0072 4d00 0000 722f 0000  ..rL...rM...r/..
+00001080: 0072 2f00 0000 722f 0000 0072 3000 0000  .r/...r/...r0...
+00001090: da08 3c6d 6f64 756c 653e 0100 0000 7320  ..<module>....s 
+000010a0: 0000 0008 120c 020c 010c 010c 010c 010c  ................
+000010b0: 010c 020c 010c 010c 010c 011a 0616 310e  ..............1.
+000010c0: 2416 46                                  $.F
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/rungui.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/rungui.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 10 15:06:22 2023 UTC, .py size: 4149 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,94 @@
-00000000: 6f0d 0d0a 0000 0000 ee25 3464 3510 0000  o........%4d5...
+00000000: 6f0d 0d0a 0000 0000 c28f 4164 2410 0000  o.........Ad$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
+00000020: 0002 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c06 6d08 5a08 0100 6501 7226 6400  d.l.m.Z...e.r&d.
-00000070: 6406 6c09 6d0a 610a 0100 6407 6408 8400  d.l.m.a...d.d...
-00000080: 5a0b 6409 640a 8400 5a0c 640b 5300 290c  Z.d.d...Z.d.S.).
-00000090: e900 0000 0029 01da 0347 5549 2901 da1c  .....)...GUI)...
-000000a0: 696e 6974 6961 6c69 7a65 5f72 756e 7469  initialize_runti
-000000b0: 6d65 5f61 7267 756d 656e 7473 2901 da0e  me_arguments)...
-000000c0: 7365 745f 636f 6c6f 725f 6d6f 6465 2901  set_color_mode).
-000000d0: da0b 464f 4e54 5f54 4f5f 5553 4529 01da  ..FONT_TO_USE)..
-000000e0: 066c 6f67 6765 72a9 01da 054d 7947 7569  .logger....MyGui
-000000f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000100: 0003 0000 0043 0000 0073 1a00 0000 7c00  .....C...s....|.
-00000110: 7d01 7400 7c01 8301 0100 7401 a002 7c01  }.t.|.....t...|.
-00000120: a101 0100 6400 5300 2901 4e29 03da 0570  ....d.S.).N)...p
-00000130: 7269 6e74 7206 0000 00da 0564 6562 7567  rintr......debug
-00000140: 2902 5a04 6172 6730 5a0b 6f75 745f 6d65  ).Z.arg0Z.out_me
-00000150: 7373 6167 65a9 0072 0b00 0000 fa75 2f55  ssage..r.....u/U
-00000160: 7365 7273 2f6d 696b 7275 6269 6e2f 4c69  sers/mikrubin/Li
-00000170: 6272 6172 792f 436c 6f75 6453 746f 7261  brary/CloudStora
-00000180: 6765 2f47 6f6f 676c 6544 7269 7665 2d6d  ge/GoogleDrive-m
-00000190: 696b 7275 6269 6e40 676d 6169 6c2e 636f  ikrubin@gmail.co
-000001a0: 6d2f 4d79 2044 7269 7665 2f50 7974 686f  m/My Drive/Pytho
-000001b0: 6e2f 6d61 7074 6173 6b65 722f 6d61 7074  n/maptasker/mapt
-000001c0: 6173 6b65 722f 7372 632f 7275 6e67 7569  asker/src/rungui
-000001d0: 2e70 79da 0f6f 7574 7075 745f 616e 645f  .py..output_and_
-000001e0: 7175 6974 2100 0000 7306 0000 0004 0108  quit!...s.......
-000001f0: 010e 0172 0d00 0000 6302 0000 0000 0000  ...r....c.......
-00000200: 0000 0000 0007 0000 0008 0000 0043 0000  .............C..
-00000210: 0073 0201 0000 7c01 7208 6401 6402 6c00  .s....|.r.d.d.l.
-00000220: 6d01 6101 0100 7401 8300 7d02 7c02 a002  m.a...t...}.|...
-00000230: a100 0100 7c02 6a03 7219 7404 6403 8301  ....|.j.r.t.d...
-00000240: 0100 7403 8300 0100 7c02 6a05 7324 7404  ..t.....|.j.s$t.
-00000250: 6404 8301 0100 7403 6405 8301 0100 7406  d.....t.d.....t.
-00000260: 8300 7d03 7a09 7407 7c02 6a08 8301 7c03  ..}.z.t.|.j...|.
-00000270: 6406 3c00 5700 6e0b 0400 7409 793b 0100  d.<.W.n...t.y;..
-00000280: 0100 0100 6407 7d04 5900 6e01 7700 7c02  ....d.}.Y.n.w.|.
-00000290: 6a0a 7c03 6408 3c00 7c02 6a0b 7c03 6409  j.|.d.<.|.j.|.d.
-000002a0: 3c00 7c02 6a0c 7c03 640a 3c00 7c02 6a0d  <.|.j.|.d.<.|.j.
-000002b0: 7c03 640b 3c00 7c02 6a0e 7c03 640c 3c00  |.d.<.|.j.|.d.<.
-000002c0: 7c02 6a0f 7c03 640d 3c00 7410 7c02 6a11  |.j.|.d.<.t.|.j.
-000002d0: 7c00 8302 7d00 7c02 6a12 7271 7c02 6a12  |...}.|.j.rq|.j.
-000002e0: a013 a100 4400 5d08 5c02 7d05 7d06 7c06  ....D.].\.}.}.|.
-000002f0: 7c00 7c05 3c00 7168 7c02 6a14 7c03 640e  |.|.<.qh|.j.|.d.
-00000300: 3c00 7401 a015 7c02 a101 0100 7e02 6201  <.t...|.....~.b.
-00000310: 7c03 7c00 6602 5300 290f 4e72 0100 0000  |.|.f.S.).Nr....
-00000320: 7207 0000 007a 1850 726f 6772 616d 2065  r....z.Program e
-00000330: 7869 7465 642e 2047 6f6f 6462 7965 2e7a  xited. Goodbye.z
-00000340: 2650 726f 6772 616d 2063 616e 6365 6c6c  &Program cancell
-00000350: 6564 2062 6520 7573 6572 2028 6b69 6c6c  ed be user (kill
-00000360: 6564 2047 5549 29e9 6300 0000 da14 6469  ed GUI).c.....di
-00000370: 7370 6c61 795f 6465 7461 696c 5f6c 6576  splay_detail_lev
-00000380: 656c e901 0000 00da 1a64 6973 706c 6179  el.......display
-00000390: 5f70 726f 6669 6c65 5f63 6f6e 6469 7469  _profile_conditi
-000003a0: 6f6e 73da 1364 6973 706c 6179 5f70 7265  ons..display_pre
-000003b0: 6665 7265 6e63 6573 da11 6469 7370 6c61  ferences..displa
-000003c0: 795f 7461 736b 6572 6e65 74da 1373 696e  y_taskernet..sin
-000003d0: 676c 655f 7072 6f6a 6563 745f 6e61 6d65  gle_project_name
-000003e0: da13 7369 6e67 6c65 5f70 726f 6669 6c65  ..single_profile
-000003f0: 5f6e 616d 65da 1073 696e 676c 655f 7461  _name..single_ta
-00000400: 736b 5f6e 616d 6572 0a00 0000 2916 da16  sk_namer....)...
-00000410: 6d61 7074 6173 6b65 722e 7372 632e 7573  maptasker.src.us
-00000420: 6572 696e 7472 7208 0000 00da 086d 6169  erintrr......mai
-00000430: 6e6c 6f6f 70da 0465 7869 7472 0d00 0000  nloop..exitr....
-00000440: 5a0a 676f 5f70 726f 6772 616d 7203 0000  Z.go_programr...
-00000450: 00da 0369 6e74 720f 0000 00da 0954 7970  ...intr......Typ
-00000460: 6545 7272 6f72 7211 0000 0072 1200 0000  eErrorr....r....
-00000470: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00000480: 1600 0000 7204 0000 005a 0f61 7070 6561  ....r....Z.appea
-00000490: 7261 6e63 655f 6d6f 6465 5a0c 636f 6c6f  rance_modeZ.colo
-000004a0: 725f 6c6f 6f6b 7570 da05 6974 656d 7372  r_lookup..itemsr
-000004b0: 0a00 0000 da04 7175 6974 2907 da08 636f  ......quit)...co
-000004c0: 6c6f 726d 6170 5a07 7573 655f 6775 695a  lormapZ.use_guiZ
-000004d0: 0a75 7365 725f 696e 7075 74da 0970 726f  .user_input..pro
-000004e0: 675f 6172 6773 720f 0000 00da 036b 6579  g_argsr......key
-000004f0: da05 7661 6c75 6572 0b00 0000 720b 0000  ..valuer....r...
-00000500: 0072 0c00 0000 da0b 7072 6f63 6573 735f  .r......process_
-00000510: 6775 692a 0000 0073 4200 0000 0402 0c01  gui*...sB.......
-00000520: 0603 0801 0602 0801 0601 0603 0801 0801  ................
-00000530: 0603 0203 1201 0c01 0801 02ff 0a03 0a01  ................
-00000540: 0a01 0a01 0a01 0a01 0c02 0602 1201 0a01  ................
-00000550: 0a03 0a03 0201 0201 0203 0201 04fe 7222  ..............r"
-00000560: 0000 004e 290d da14 6d61 7074 6173 6b65  ...N)...maptaske
-00000570: 722e 7372 632e 636f 6e66 6967 7202 0000  r.src.configr...
-00000580: 00da 166d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
-00000590: 2e69 6e69 7470 6172 6772 0300 0000 da16  .initpargr......
-000005a0: 6d61 7074 6173 6b65 722e 7372 632e 636f  maptasker.src.co
-000005b0: 6c72 6d6f 6465 7204 0000 00da 166d 6170  lrmoder......map
-000005c0: 7461 736b 6572 2e73 7263 2e73 7973 636f  tasker.src.sysco
-000005d0: 6e73 7472 0500 0000 7206 0000 0072 1700  nstr....r....r..
-000005e0: 0000 7208 0000 0072 0d00 0000 7222 0000  ..r....r....r"..
-000005f0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000600: 720c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000610: 0000 0073 1200 0000 0c13 0c01 0c01 0c01  ...s............
-00000620: 0c01 0402 0c01 0806 0c09                 ..........
+00000050: 0100 6404 6405 8400 5a06 6406 6407 8400  ..d.d...Z.d.d...
+00000060: 5a07 6408 5300 2909 e900 0000 0029 01da  Z.d.S.)......)..
+00000070: 1c69 6e69 7469 616c 697a 655f 7275 6e74  .initialize_runt
+00000080: 696d 655f 6172 6775 6d65 6e74 7329 01da  ime_arguments)..
+00000090: 0e73 6574 5f63 6f6c 6f72 5f6d 6f64 6529  .set_color_mode)
+000000a0: 01da 066c 6f67 6765 7263 0100 0000 0000  ...loggerc......
+000000b0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+000000c0: 0000 731a 0000 007c 007d 0174 007c 0183  ..s....|.}.t.|..
+000000d0: 0101 0074 01a0 027c 01a1 0101 0064 0053  ...t...|.....d.S
+000000e0: 0029 014e 2903 da05 7072 696e 7472 0400  .).N)...printr..
+000000f0: 0000 da05 6465 6275 6729 025a 0461 7267  ....debug).Z.arg
+00000100: 305a 0b6f 7574 5f6d 6573 7361 6765 a900  0Z.out_message..
+00000110: 7207 0000 00fa 752f 5573 6572 732f 6d69  r.....u/Users/mi
+00000120: 6b72 7562 696e 2f4c 6962 7261 7279 2f43  krubin/Library/C
+00000130: 6c6f 7564 5374 6f72 6167 652f 476f 6f67  loudStorage/Goog
+00000140: 6c65 4472 6976 652d 6d69 6b72 7562 696e  leDrive-mikrubin
+00000150: 4067 6d61 696c 2e63 6f6d 2f4d 7920 4472  @gmail.com/My Dr
+00000160: 6976 652f 5079 7468 6f6e 2f6d 6170 7461  ive/Python/mapta
+00000170: 736b 6572 2f6d 6170 7461 736b 6572 2f73  sker/maptasker/s
+00000180: 7263 2f72 756e 6775 692e 7079 da0f 6f75  rc/rungui.py..ou
+00000190: 7470 7574 5f61 6e64 5f71 7569 741c 0000  tput_and_quit...
+000001a0: 0073 0600 0000 0401 0801 0e01 7209 0000  .s..........r...
+000001b0: 0063 0200 0000 0000 0000 0000 0000 0600  .c..............
+000001c0: 0000 0800 0000 4300 0000 7316 0100 007c  ......C...s....|
+000001d0: 0172 0864 0164 026c 006d 0161 0101 0074  .r.d.d.l.m.a...t
+000001e0: 0183 007d 027c 02a0 02a1 0001 007c 026a  ...}.|.......|.j
+000001f0: 0372 1974 0464 0383 0101 0074 0383 0001  .r.t.d.....t....
+00000200: 007c 026a 0573 277c 026a 0673 2774 0464  .|.j.s'|.j.s't.d
+00000210: 0483 0101 0074 0364 0583 0101 0074 0783  .....t.d.....t..
+00000220: 007d 037a 0974 087c 026a 0983 017c 0364  .}.z.t.|.j...|.d
+00000230: 063c 0057 006e 0d04 0074 0a79 4001 0001  .<.W.n...t.y@...
+00000240: 0001 0064 077c 0364 063c 0059 006e 0177  ...d.|.d.<.Y.n.w
+00000250: 007c 026a 0b7c 0364 083c 007c 026a 0c7c  .|.j.|.d.<.|.j.|
+00000260: 0364 093c 007c 026a 0d7c 0364 0a3c 007c  .d.<.|.j.|.d.<.|
+00000270: 026a 0e7c 0364 0b3c 007c 026a 0f7c 0364  .j.|.d.<.|.j.|.d
+00000280: 0c3c 007c 026a 107c 0364 0d3c 0074 117c  .<.|.j.|.d.<.t.|
+00000290: 026a 127c 0083 027d 007c 026a 1372 767c  .j.|...}.|.j.rv|
+000002a0: 026a 13a0 14a1 0044 005d 085c 027d 047d  .j.....D.].\.}.}
+000002b0: 057c 057c 007c 043c 0071 6d7c 026a 157c  .|.|.|.<.qm|.j.|
+000002c0: 0364 0e3c 007c 026a 067c 0364 0f3c 0074  .d.<.|.j.|.d.<.t
+000002d0: 01a0 167c 02a1 0101 007e 0262 017c 037c  ...|.....~.b.|.|
+000002e0: 0066 0253 0029 104e 7201 0000 0029 01da  .f.S.).Nr....)..
+000002f0: 054d 7947 7569 7a18 5072 6f67 7261 6d20  .MyGuiz.Program 
+00000300: 6578 6974 6564 2e20 476f 6f64 6279 652e  exited. Goodbye.
+00000310: 7a26 5072 6f67 7261 6d20 6361 6e63 656c  z&Program cancel
+00000320: 6c65 6420 6265 2075 7365 7220 286b 696c  led be user (kil
+00000330: 6c65 6420 4755 4929 e963 0000 00da 1464  led GUI).c.....d
+00000340: 6973 706c 6179 5f64 6574 6169 6c5f 6c65  isplay_detail_le
+00000350: 7665 6ce9 0100 0000 da1a 6469 7370 6c61  vel.......displa
+00000360: 795f 7072 6f66 696c 655f 636f 6e64 6974  y_profile_condit
+00000370: 696f 6e73 da13 6469 7370 6c61 795f 7072  ions..display_pr
+00000380: 6566 6572 656e 6365 73da 1164 6973 706c  eferences..displ
+00000390: 6179 5f74 6173 6b65 726e 6574 da13 7369  ay_taskernet..si
+000003a0: 6e67 6c65 5f70 726f 6a65 6374 5f6e 616d  ngle_project_nam
+000003b0: 65da 1373 696e 676c 655f 7072 6f66 696c  e..single_profil
+000003c0: 655f 6e61 6d65 da10 7369 6e67 6c65 5f74  e_name..single_t
+000003d0: 6173 6b5f 6e61 6d65 7206 0000 00da 0572  ask_namer......r
+000003e0: 6572 756e 2917 5a16 6d61 7074 6173 6b65  erun).Z.maptaske
+000003f0: 722e 7372 632e 7573 6572 696e 7472 720a  r.src.userintrr.
+00000400: 0000 00da 086d 6169 6e6c 6f6f 70da 0465  .....mainloop..e
+00000410: 7869 7472 0900 0000 5a0a 676f 5f70 726f  xitr....Z.go_pro
+00000420: 6772 616d 5a0d 7265 7275 6e5f 7072 6f67  gramZ.rerun_prog
+00000430: 7261 6d72 0200 0000 da03 696e 7472 0c00  ramr......intr..
+00000440: 0000 da09 5479 7065 4572 726f 7272 0e00  ....TypeErrorr..
+00000450: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00000460: 0072 1200 0000 7213 0000 0072 0300 0000  .r....r....r....
+00000470: 5a0f 6170 7065 6172 616e 6365 5f6d 6f64  Z.appearance_mod
+00000480: 655a 0c63 6f6c 6f72 5f6c 6f6f 6b75 70da  eZ.color_lookup.
+00000490: 0569 7465 6d73 7206 0000 00da 0471 7569  .itemsr......qui
+000004a0: 7429 06da 0863 6f6c 6f72 6d61 705a 0775  t)...colormapZ.u
+000004b0: 7365 5f67 7569 5a0a 7573 6572 5f69 6e70  se_guiZ.user_inp
+000004c0: 7574 da09 7072 6f67 5f61 7267 73da 036b  ut..prog_args..k
+000004d0: 6579 da05 7661 6c75 6572 0700 0000 7207  ey..valuer....r.
+000004e0: 0000 0072 0800 0000 da0b 7072 6f63 6573  ...r......proces
+000004f0: 735f 6775 6925 0000 0073 4400 0000 0402  s_gui%...sD.....
+00000500: 0c01 0603 0801 0602 0801 0601 0c03 0801  ................
+00000510: 0801 0603 0203 1201 0c01 0c01 02ff 0a03  ................
+00000520: 0a01 0a01 0a01 0a01 0a01 0c02 0602 1201  ................
+00000530: 0a01 0a03 0a02 0a03 0201 0201 0203 0201  ................
+00000540: 04fe 721f 0000 004e 2908 da16 6d61 7074  ..r....N)...mapt
+00000550: 6173 6b65 722e 7372 632e 696e 6974 7061  asker.src.initpa
+00000560: 7267 7202 0000 00da 166d 6170 7461 736b  rgr......maptask
+00000570: 6572 2e73 7263 2e63 6f6c 726d 6f64 6572  er.src.colrmoder
+00000580: 0300 0000 da16 6d61 7074 6173 6b65 722e  ......maptasker.
+00000590: 7372 632e 7379 7363 6f6e 7374 7204 0000  src.sysconstr...
+000005a0: 0072 0900 0000 721f 0000 0072 0700 0000  .r....r....r....
+000005b0: 7207 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
+000005c0: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
+000005d0: 0000 0c13 0c01 0c01 0806 0c09            ............
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/scenes.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/scenes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/servicec.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/servicec.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/share.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/share.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 16 19:08:14 2023 UTC, .py size: 4290 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,158 @@
-00000000: 6f0d 0d0a 0000 0000 9e47 3c64 c210 0000  o........G<d....
+00000000: 6f0d 0d0a 0000 0000 31ee 4764 4314 0000  o.......1.GdC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
+00000020: 000a 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6404  ..d.d.l.m.Z...d.
-00000050: 6501 6a06 6a07 6405 6508 6406 6508 6407  e.j.j.d.e.d.e.d.
-00000060: 6509 6408 6401 660a 6409 640a 8404 5a0a  e.d.d.f.d.d...Z.
-00000070: 640b 6501 6a06 6405 6508 6406 6508 6407  d.e.j.d.e.d.e.d.
-00000080: 6509 6408 6401 660a 640c 640d 8404 5a0b  e.d.d.f.d.d...Z.
-00000090: 6401 5300 290e e900 0000 004e 2901 da09  d.S.)......N)...
-000000a0: 6d79 5f6f 7574 7075 7429 01da 0b46 4f4e  my_output)...FON
-000000b0: 545f 544f 5f55 5345 da0c 726f 6f74 5f65  T_TO_USE..root_e
-000000c0: 6c65 6d65 6e74 da08 636f 6c6f 726d 6170  lement..colormap
-000000d0: da0c 7072 6f67 7261 6d5f 6172 6773 da0b  ..program_args..
-000000e0: 6f75 7470 7574 5f6c 6973 74da 0672 6574  output_list..ret
-000000f0: 7572 6e63 0400 0000 0000 0000 0000 0000  urnc............
-00000100: 0800 0000 0600 0000 4300 0000 7376 0000  ........C...sv..
-00000110: 007c 00a0 0064 01a1 017d 047c 0464 0075  .|...d...}.|.d.u
-00000120: 0172 357c 04a0 0064 02a1 017d 057c 0564  .r5|...d...}.|.d
-00000130: 0075 0172 1974 017c 057c 017c 027c 0383  .u.r.t.|.|.|.|..
-00000140: 0401 007c 04a0 0064 03a1 017d 067c 0664  ...|...d...}.|.d
-00000150: 0075 0172 377c 066a 0272 3964 047c 066a  .u.r7|.j.r9d.|.j
-00000160: 029b 009d 027d 0774 037c 017c 027c 0364  .....}.t.|.|.|.d
-00000170: 057c 0783 0501 0064 0053 0064 0053 0064  .|.....d.S.d.S.d
-00000180: 0053 0064 0053 0029 064e da05 5368 6172  .S.d.S.).N..Shar
-00000190: 65da 0164 da01 677a 2126 6e62 7370 3b26  e..d..gz!&nbsp;&
-000001a0: 6e62 7370 3b54 6173 6b65 724e 6574 2073  nbsp;TaskerNet s
-000001b0: 6561 7263 6820 6f6e 3a20 e902 0000 0029  earch on: .....)
-000001c0: 04da 0466 696e 64da 1a64 6573 6372 6970  ...find..descrip
-000001d0: 7469 6f6e 5f65 6c65 6d65 6e74 5f6f 7574  tion_element_out
-000001e0: 7075 74da 0474 6578 7472 0200 0000 2908  put..textr....).
-000001f0: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-00000200: 0700 0000 da0d 7368 6172 655f 656c 656d  ......share_elem
-00000210: 656e 74da 1364 6573 6372 6970 7469 6f6e  ent..description
-00000220: 5f65 6c65 6d65 6e74 5a0e 7365 6172 6368  _elementZ.search
-00000230: 5f65 6c65 6d65 6e74 da0a 6f75 745f 7374  _element..out_st
-00000240: 7269 6e67 a900 7213 0000 00fa 742f 5573  ring..r.....t/Us
-00000250: 6572 732f 6d69 6b72 7562 696e 2f4c 6962  ers/mikrubin/Lib
-00000260: 7261 7279 2f43 6c6f 7564 5374 6f72 6167  rary/CloudStorag
-00000270: 652f 476f 6f67 6c65 4472 6976 652d 6d69  e/GoogleDrive-mi
-00000280: 6b72 7562 696e 4067 6d61 696c 2e63 6f6d  krubin@gmail.com
-00000290: 2f4d 7920 4472 6976 652f 5079 7468 6f6e  /My Drive/Python
-000002a0: 2f6d 6170 7461 736b 6572 2f6d 6170 7461  /maptasker/mapta
-000002b0: 736b 6572 2f73 7263 2f73 6861 7265 2e70  sker/src/share.p
-000002c0: 79da 0573 6861 7265 1500 0000 731a 0000  y..share....s...
-000002d0: 000a 0708 010a 0208 0202 0108 0104 ff0a  ................
-000002e0: 040e 010c 0314 0104 f208 0a72 1500 0000  ...........r....
-000002f0: 7211 0000 0063 0400 0000 0000 0000 0000  r....c..........
-00000300: 0000 0900 0000 0600 0000 4300 0000 73f6  ..........C...s.
-00000310: 0000 0064 017c 006a 009b 009d 027d 0464  ...d.|.j.....}.d
-00000320: 027c 0164 0319 009b 0074 019b 0064 049d  .|.d.....t...d..
-00000330: 047d 057c 04a0 0264 057c 05a1 027d 047c  .}.|...d.|...}.|
-00000340: 04a0 0264 067c 05a1 027d 047c 04a0 0264  ...d.|...}.|...d
-00000350: 077c 05a1 027d 047c 04a0 0264 087c 05a1  .|...}.|...d.|..
-00000360: 027d 047c 04a0 0264 097c 059b 00a1 027d  .}.|...d.|.....}
-00000370: 047c 04a0 0264 0a64 0ba1 027d 0464 0b7d  .|...d.d...}.d.}
-00000380: 067c 057c 0476 0172 6e74 037c 0483 0144  .|.|.v.rnt.|...D
-00000390: 005d 2c5c 027d 077d 087c 0864 0c6b 0272  .],\.}.}.|.d.k.r
-000003a0: 4f7c 047c 0764 0d17 0019 0064 0c6b 0273  O|.|.d.....d.k.s
-000003b0: 5b7c 0864 0e6b 0272 677c 047c 0764 0d17  [|.d.k.rg|.|.d..
-000003c0: 0019 0064 0c6b 0272 677c 069b 0064 0f7c  ...d.k.rg|...d.|
-000003d0: 0164 0319 009b 0074 019b 0064 049d 056e  .d.....t...d...n
-000003e0: 037c 067c 0817 007d 0671 3f7c 067d 047c  .|.|...}.q?|.}.|
-000003f0: 049b 007d 0474 047c 017c 027c 0364 107c  ...}.t.|.|.|.d.|
-00000400: 0483 0501 0064 1153 0029 1261 2c01 0000  .....d.S.).a,...
-00000410: 0a20 2020 2057 6520 6861 7665 2061 2054  .    We have a T
-00000420: 6173 6b65 726e 6574 2064 6573 6372 6970  askernet descrip
-00000430: 7469 6f6e 2028 3c53 6861 7265 3e29 2e20  tion (<Share>). 
-00000440: 2050 726f 6365 7373 2069 740a 2020 2020   Process it.    
-00000450: 2020 2020 3a70 6172 616d 2064 6573 6372      :param descr
-00000460: 6970 7469 6f6e 5f65 6c65 6d65 6e74 3a20  iption_element: 
-00000470: 7468 6520 786d 6c20 656c 656d 656e 7420  the xml element 
-00000480: 7769 7468 2074 6865 2064 6573 6372 6970  with the descrip
-00000490: 7469 6f6e 0a20 2020 2020 2020 203a 7061  tion.        :pa
-000004a0: 7261 6d20 636f 6c6f 726d 6170 3a20 7468  ram colormap: th
-000004b0: 6520 636f 6c6f 7273 2074 6f20 7573 6520  e colors to use 
-000004c0: 666f 7220 7468 6520 6f75 7470 7574 0a20  for the output. 
-000004d0: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
-000004e0: 6f67 7261 6d5f 6172 6773 3a20 7468 6520  ogram_args: the 
-000004f0: 7275 6e74 696d 6520 6172 6775 6d65 6e74  runtime argument
-00000500: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
-00000510: 206f 7574 7075 745f 6c69 7374 3a20 7468   output_list: th
-00000520: 6520 6f75 7470 7574 206c 696e 6573 2074  e output lines t
-00000530: 6875 7320 6661 720a 2020 2020 7a17 5461  hus far.    z.Ta
-00000540: 736b 6572 4e65 7420 6465 7363 7269 7074  skerNet descript
-00000550: 696f 6e3a 207a 373c 2f70 3e3c 7020 7374  ion: z7</p><p st
-00000560: 796c 653d 226d 6172 6769 6e2d 6c65 6674  yle="margin-left
-00000570: 3a32 3070 783b 6d61 7267 696e 2d72 6967  :20px;margin-rig
-00000580: 6874 3a35 3070 783b 636f 6c6f 723a da0f  ht:50px;color:..
-00000590: 7461 736b 6572 6e65 745f 636f 6c6f 72fa  taskernet_color.
-000005a0: 013e 7a03 3c70 3e7a 053c 6272 2f3e 7a04  .>z.<p>z.<br/>z.
-000005b0: 3c68 313e fa01 0d7a 043c 6c69 3e7a 053c  <h1>...z.<li>z.<
-000005c0: 2f6c 693e da00 fa01 20e9 0100 0000 fa01  /li>.... .......
-000005d0: 2d7a 333c 7020 7374 796c 653d 226d 6172  -z3<p style="mar
-000005e0: 6769 6e2d 6c65 6674 3a32 3070 783b 6d61  gin-left:20px;ma
-000005f0: 7267 696e 2d72 6967 6874 3a35 3070 783b  rgin-right:50px;
-00000600: 636f 6c6f 723a 720c 0000 004e 2905 720f  color:r....N).r.
-00000610: 0000 0072 0300 0000 da07 7265 706c 6163  ...r......replac
-00000620: 65da 0965 6e75 6d65 7261 7465 7202 0000  e..enumerater...
-00000630: 0029 0972 1100 0000 7205 0000 0072 0600  .).r....r....r..
-00000640: 0000 7207 0000 0072 1200 0000 5a0b 696e  ..r....r....Z.in
-00000650: 6465 6e74 5f68 746d 6c5a 086e 6577 5f6c  dent_htmlZ.new_l
-00000660: 696e 65da 0870 6f73 6974 696f 6e5a 0f63  ine..positionZ.c
-00000670: 6861 7261 6374 6572 5f69 6e64 6578 7213  haracter_indexr.
-00000680: 0000 0072 1300 0000 7214 0000 0072 0e00  ...r....r....r..
-00000690: 0000 2f00 0000 7338 0000 000c 0e02 0206  ../...s8........
-000006a0: 0102 ff02 0106 ff02 ff0c 060c 010c 010c  ................
-000006b0: 010e 010c 0104 0408 0110 0118 0418 0106  ................
-000006c0: fd06 0102 ff02 0108 ff06 0404 fb04 0706  ................
-000006d0: 0114 0272 0e00 0000 290c da16 6465 6675  ...r....)...defu
-000006e0: 7365 6478 6d6c 2e45 6c65 6d65 6e74 5472  sedxml.ElementTr
-000006f0: 6565 da0a 6465 6675 7365 6478 6d6c da15  ee..defusedxml..
-00000700: 6d61 7074 6173 6b65 722e 7372 632e 6f75  maptasker.src.ou
-00000710: 7470 7574 6c72 0200 0000 da16 6d61 7074  tputlr......mapt
-00000720: 6173 6b65 722e 7372 632e 7379 7363 6f6e  asker.src.syscon
-00000730: 7374 7203 0000 00da 0b45 6c65 6d65 6e74  str......Element
-00000740: 5472 6565 da03 584d 4cda 0464 6963 74da  Tree..XML..dict.
-00000750: 046c 6973 7472 1500 0000 720e 0000 0072  .listr....r....r
-00000760: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-00000770: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000780: 0073 3200 0000 080d 0c03 0c01 0203 0601  .s2.............
-00000790: 02ff 0202 02fe 0203 02fd 0204 02fc 0205  ................
-000007a0: 0afb 021a 0401 02ff 0202 02fe 0203 02fd  ................
-000007b0: 0204 02fc 0205 0efb                      ........
+00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6404 6c06 6d07 5a07 0100 6405 6501 6a08  d.l.m.Z...d.e.j.
+00000060: 6a09 6406 650a 6407 650a 6408 650b 6409  j.d.e.d.e.d.e.d.
+00000070: 6401 660a 640a 640b 8404 5a0c 640c 6501  d.f.d.d...Z.d.e.
+00000080: 6a08 6406 650a 6407 650a 6408 650b 6409  j.d.e.d.e.d.e.d.
+00000090: 6401 660a 640d 640e 8404 5a0d 6401 5300  d.f.d.d...Z.d.S.
+000000a0: 290f e900 0000 004e 2901 da09 6d79 5f6f  )......N)...my_o
+000000b0: 7574 7075 7429 01da 0b46 4f4e 545f 544f  utput)...FONT_TO
+000000c0: 5f55 5345 2901 da0b 666f 726d 6174 5f68  _USE)...format_h
+000000d0: 746d 6cda 0c72 6f6f 745f 656c 656d 656e  tml..root_elemen
+000000e0: 74da 0863 6f6c 6f72 6d61 70da 0c70 726f  t..colormap..pro
+000000f0: 6772 616d 5f61 7267 73da 0b6f 7574 7075  gram_args..outpu
+00000100: 745f 6c69 7374 da06 7265 7475 726e 6304  t_list..returnc.
+00000110: 0000 0000 0000 0000 0000 0008 0000 0006  ................
+00000120: 0000 0043 0000 0073 7600 0000 7c00 a000  ...C...sv...|...
+00000130: 6401 a101 7d04 7c04 6402 7501 7235 7c04  d...}.|.d.u.r5|.
+00000140: a000 6403 a101 7d05 7c05 6402 7501 7219  ..d...}.|.d.u.r.
+00000150: 7401 7c05 7c01 7c02 7c03 8304 0100 7c04  t.|.|.|.|.....|.
+00000160: a000 6404 a101 7d06 7c06 6402 7501 7237  ..d...}.|.d.u.r7
+00000170: 7c06 6a02 7239 6405 7c06 6a02 9b00 9d02  |.j.r9d.|.j.....
+00000180: 7d07 7403 7c01 7c02 7c03 6406 7c07 8305  }.t.|.|.|.d.|...
+00000190: 0100 6402 5300 6402 5300 6402 5300 6402  ..d.S.d.S.d.S.d.
+000001a0: 5300 2907 6150 0100 000a 2020 2020 476f  S.).aP....    Go
+000001b0: 2074 6872 6f75 6768 2078 6d6c 203c 5368   through xml <Sh
+000001c0: 6172 653e 2065 6c65 6d65 6e74 7320 746f  are> elements to
+000001d0: 2067 7261 6220 616e 6420 6f75 7470 7574   grab and output
+000001e0: 2054 6173 6b65 724e 6574 2064 6573 6372   TaskerNet descr
+000001f0: 6970 7469 6f6e 2061 6e64 2073 6561 7263  iption and searc
+00000200: 682d 6f6e 206c 696e 6573 0a20 2020 2020  h-on lines.     
+00000210: 2020 203a 7061 7261 6d20 726f 6f74 5f65     :param root_e
+00000220: 6c65 6d65 6e74 3a20 6265 6769 6e6e 696e  lement: beginnin
+00000230: 6720 786d 6c20 656c 656d 656e 7420 2865  g xml element (e
+00000240: 2e67 2e20 5072 6f6a 6563 7420 6f72 2054  .g. Project or T
+00000250: 6173 6b29 0a20 2020 2020 2020 203a 7061  ask).        :pa
+00000260: 7261 6d20 636f 6c6f 726d 6170 3a20 636f  ram colormap: co
+00000270: 6c6f 7273 2074 6f20 7573 6520 696e 206f  lors to use in o
+00000280: 7574 7075 740a 2020 2020 2020 2020 3a70  utput.        :p
+00000290: 6172 616d 2070 726f 6772 616d 5f61 7267  aram program_arg
+000002a0: 733a 2072 756e 7469 6d65 2061 7267 756d  s: runtime argum
+000002b0: 656e 7473 0a20 2020 2020 2020 203a 7061  ents.        :pa
+000002c0: 7261 6d20 6f75 7470 7574 5f6c 6973 743a  ram output_list:
+000002d0: 2077 6865 7265 2061 6c6c 206f 7574 7075   where all outpu
+000002e0: 7420 6c69 6e65 7320 6172 6520 6164 6465  t lines are adde
+000002f0: 6420 746f 0a20 2020 20da 0553 6861 7265  d to.    ..Share
+00000300: 4eda 0164 da01 677a 2126 6e62 7370 3b26  N..d..gz!&nbsp;&
+00000310: 6e62 7370 3b54 6173 6b65 724e 6574 2073  nbsp;TaskerNet s
+00000320: 6561 7263 6820 6f6e 3a20 e902 0000 0029  earch on: .....)
+00000330: 04da 0466 696e 64da 1a64 6573 6372 6970  ...find..descrip
+00000340: 7469 6f6e 5f65 6c65 6d65 6e74 5f6f 7574  tion_element_out
+00000350: 7075 74da 0474 6578 7472 0200 0000 2908  put..textr....).
+00000360: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+00000370: 0800 0000 da0d 7368 6172 655f 656c 656d  ......share_elem
+00000380: 656e 74da 1364 6573 6372 6970 7469 6f6e  ent..description
+00000390: 5f65 6c65 6d65 6e74 5a0e 7365 6172 6368  _elementZ.search
+000003a0: 5f65 6c65 6d65 6e74 da0a 6f75 745f 7374  _element..out_st
+000003b0: 7269 6e67 a900 7214 0000 00fa 742f 5573  ring..r.....t/Us
+000003c0: 6572 732f 6d69 6b72 7562 696e 2f4c 6962  ers/mikrubin/Lib
+000003d0: 7261 7279 2f43 6c6f 7564 5374 6f72 6167  rary/CloudStorag
+000003e0: 652f 476f 6f67 6c65 4472 6976 652d 6d69  e/GoogleDrive-mi
+000003f0: 6b72 7562 696e 4067 6d61 696c 2e63 6f6d  krubin@gmail.com
+00000400: 2f4d 7920 4472 6976 652f 5079 7468 6f6e  /My Drive/Python
+00000410: 2f6d 6170 7461 736b 6572 2f6d 6170 7461  /maptasker/mapta
+00000420: 736b 6572 2f73 7263 2f73 6861 7265 2e70  sker/src/share.p
+00000430: 79da 0573 6861 7265 1600 0000 731a 0000  y..share....s...
+00000440: 000a 0e08 010a 0208 0202 0108 0104 ff0a  ................
+00000450: 040e 010c 0314 0104 f208 0a72 1600 0000  ...........r....
+00000460: 7212 0000 0063 0400 0000 0000 0000 0000  r....c..........
+00000470: 0000 0900 0000 0600 0000 4300 0000 733a  ..........C...s:
+00000480: 0100 0074 007c 0164 0164 0264 037c 006a  ...t.|.d.d.d.|.j
+00000490: 019b 009d 0264 0483 057d 0464 057c 0164  .....d...}.d.|.d
+000004a0: 0119 009b 0074 029b 0064 069d 047d 057c  .....t...d...}.|
+000004b0: 04a0 0364 077c 05a1 027d 047c 04a0 0364  ...d.|...}.|...d
+000004c0: 087c 05a1 027d 047c 04a0 0364 0964 02a1  .|...}.|...d.d..
+000004d0: 027d 047c 04a0 0364 0a64 02a1 027d 047c  .}.|...d.d...}.|
+000004e0: 04a0 0364 0b7c 05a1 027d 047c 04a0 0364  ...d.|...}.|...d
+000004f0: 0c7c 05a1 027d 047c 04a0 0364 0d7c 05a1  .|...}.|...d.|..
+00000500: 027d 047c 04a0 0364 0e7c 059b 00a1 027d  .}.|...d.|.....}
+00000510: 047c 04a0 0364 0f64 02a1 027d 0464 027d  .|...d.d...}.d.}
+00000520: 067c 057c 0476 0172 9374 047c 0483 0144  .|.|.v.r.t.|...D
+00000530: 005d 2c5c 027d 077d 087c 0864 106b 0272  .],\.}.}.|.d.k.r
+00000540: 677c 047c 0764 1117 0019 0064 106b 0273  g|.|.d.....d.k.s
+00000550: 737c 0864 126b 0272 7f7c 047c 0764 1117  s|.d.k.r.|.|.d..
+00000560: 0019 0064 106b 0272 7f7c 069b 0064 137c  ...d.k.r.|...d.|
+00000570: 0164 0119 009b 0074 029b 0064 069d 056e  .d.....t...d...n
+00000580: 037c 067c 0817 007d 0671 5764 147c 0476  .|.|...}.qWd.|.v
+00000590: 0172 9174 007c 0164 0164 027c 0664 0483  .r.t.|.d.d.|.d..
+000005a0: 057d 046e 027c 067d 0474 057c 017c 027c  .}.n.|.}.t.|.|.|
+000005b0: 0364 157c 0483 0501 0064 1653 0029 1761  .d.|.....d.S.).a
+000005c0: 4c01 0000 0a20 2020 2057 6520 6861 7665  L....    We have
+000005d0: 2061 2054 6173 6b65 726e 6574 2064 6573   a Taskernet des
+000005e0: 6372 6970 7469 6f6e 2028 3c53 6861 7265  cription (<Share
+000005f0: 3e29 2e20 2043 6c65 616e 2069 7420 7569  >).  Clean it ui
+00000600: 7020 616e 6420 6164 6420 6974 2074 6f20  p and add it to 
+00000610: 7468 6520 6f75 7470 7574 206c 6973 740a  the output list.
+00000620: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00000630: 6573 6372 6970 7469 6f6e 5f65 6c65 6d65  escription_eleme
+00000640: 6e74 3a20 7468 6520 786d 6c20 656c 656d  nt: the xml elem
+00000650: 656e 7420 7769 7468 2074 6865 2064 6573  ent with the des
+00000660: 6372 6970 7469 6f6e 0a20 2020 2020 2020  cription.       
+00000670: 203a 7061 7261 6d20 636f 6c6f 726d 6170   :param colormap
+00000680: 3a20 7468 6520 636f 6c6f 7273 2074 6f20  : the colors to 
+00000690: 7573 6520 666f 7220 7468 6520 6f75 7470  use for the outp
+000006a0: 7574 0a20 2020 2020 2020 203a 7061 7261  ut.        :para
+000006b0: 6d20 7072 6f67 7261 6d5f 6172 6773 3a20  m program_args: 
+000006c0: 7468 6520 7275 6e74 696d 6520 6172 6775  the runtime argu
+000006d0: 6d65 6e74 730a 2020 2020 2020 2020 3a70  ments.        :p
+000006e0: 6172 616d 206f 7574 7075 745f 6c69 7374  aram output_list
+000006f0: 3a20 7468 6520 6f75 7470 7574 206c 696e  : the output lin
+00000700: 6573 2074 6875 7320 6661 720a 2020 2020  es thus far.    
+00000710: da0f 7461 736b 6572 6e65 745f 636f 6c6f  ..taskernet_colo
+00000720: 72da 007a 1754 6173 6b65 724e 6574 2064  r..z.TaskerNet d
+00000730: 6573 6372 6970 7469 6f6e 3a20 547a 373c  escription: Tz7<
+00000740: 2f70 3e3c 7020 7374 796c 653d 226d 6172  /p><p style="mar
+00000750: 6769 6e2d 6c65 6674 3a32 3070 783b 6d61  gin-left:20px;ma
+00000760: 7267 696e 2d72 6967 6874 3a35 3070 783b  rgin-right:50px;
+00000770: 636f 6c6f 723a 7a02 223e 7a03 3c70 3e7a  color:z.">z.<p>z
+00000780: 033c 503e 7a04 3c2f 703e 7a04 3c2f 503e  .<P>z.</p>z.</P>
+00000790: 7a05 3c62 722f 3e7a 043c 6831 3efa 010d  z.<br/>z.<h1>...
+000007a0: 7a04 3c6c 693e 7a05 3c2f 6c69 3efa 0120  z.<li>z.</li>.. 
+000007b0: e901 0000 00fa 012d 7a33 3c70 2073 7479  .......-z3<p sty
+000007c0: 6c65 3d22 6d61 7267 696e 2d6c 6566 743a  le="margin-left:
+000007d0: 3230 7078 3b6d 6172 6769 6e2d 7269 6768  20px;margin-righ
+000007e0: 743a 3530 7078 3b63 6f6c 6f72 3a7a 063c  t:50px;color:z.<
+000007f0: 7370 616e 2072 0d00 0000 4e29 0672 0400  span r....N).r..
+00000800: 0000 7210 0000 0072 0300 0000 da07 7265  ..r....r......re
+00000810: 706c 6163 65da 0965 6e75 6d65 7261 7465  place..enumerate
+00000820: 7202 0000 0029 0972 1200 0000 7206 0000  r....).r....r...
+00000830: 0072 0700 0000 7208 0000 0072 1300 0000  .r....r....r....
+00000840: 5a0b 696e 6465 6e74 5f68 746d 6c5a 086e  Z.indent_htmlZ.n
+00000850: 6577 5f6c 696e 65da 0870 6f73 6974 696f  ew_line..positio
+00000860: 6e5a 0f63 6861 7261 6374 6572 5f69 6e64  nZ.character_ind
+00000870: 6578 7214 0000 0072 1400 0000 7215 0000  exr....r....r...
+00000880: 0072 0f00 0000 3700 0000 734c 0000 0002  .r....7...sL....
+00000890: 0e02 0102 0102 010a 0102 0104 fb02 0806  ................
+000008a0: 0102 ff02 0106 ff02 ff0c 060c 010c 010c  ................
+000008b0: 010c 010c 010c 010e 010c 0104 0408 0110  ................
+000008c0: 0118 0418 0106 fd06 0102 ff02 0108 ff06  ................
+000008d0: 0404 fb08 0a12 0104 0214 0372 0f00 0000  ...........r....
+000008e0: 290e da16 6465 6675 7365 6478 6d6c 2e45  )...defusedxml.E
+000008f0: 6c65 6d65 6e74 5472 6565 da0a 6465 6675  lementTree..defu
+00000900: 7365 6478 6d6c da15 6d61 7074 6173 6b65  sedxml..maptaske
+00000910: 722e 7372 632e 6f75 7470 7574 6c72 0200  r.src.outputlr..
+00000920: 0000 da16 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
+00000930: 632e 7379 7363 6f6e 7374 7203 0000 00da  c.sysconstr.....
+00000940: 166d 6170 7461 736b 6572 2e73 7263 2e66  .maptasker.src.f
+00000950: 726d 7468 746d 6c72 0400 0000 da0b 456c  rmthtmlr......El
+00000960: 656d 656e 7454 7265 65da 0358 4d4c da04  ementTree..XML..
+00000970: 6469 6374 da04 6c69 7374 7216 0000 0072  dict..listr....r
+00000980: 0f00 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
+00000990: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
+000009a0: 653e 0100 0000 7334 0000 0008 0d0c 030c  e>....s4........
+000009b0: 010c 0102 0306 0102 ff02 0202 fe02 0302  ................
+000009c0: fd02 0402 fc02 050a fb02 2104 0102 ff02  ..........!.....
+000009d0: 0202 fe02 0302 fd02 0402 fc02 050e fb    ...............
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/shellsort.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/shellsort.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/sysconst.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/sysconst.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 16:19:33 2023 UTC, .py size: 4055 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 952b 3864 d70f 0000  o........+8d....
+00000000: 6f0d 0d0a 0000 0000 cb29 4864 d80f 0000  o........)Hd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9001 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6403 5a03 6404 5a04 6405 5a05 6406  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a06 6407 5a07 6408 5a08 6409 6501 9b00  Z.d.Z.d.Z.d.e...
 00000060: 9d02 5a09 640a 5a0a 6900 640b 640c 9301  ..Z.d.Z.i.d.d...
 00000070: 640d 640c 9301 640e 640f 9301 6410 640f  d.d...d.d...d.d.
@@ -21,20 +21,20 @@
 00000140: 640e 9301 6413 6411 9301 6416 643e 9301  d...d.d...d.d>..
 00000150: 6419 643f 9301 641a 6440 9301 641c 6441  d.d?..d.d@..d.dA
 00000160: 9301 6420 6442 9301 6423 6443 9301 6426  ..d dB..d#dC..d&
 00000170: 6444 9301 6427 6445 9301 642b 6429 9301  dD..d'dE..d+d)..
 00000180: 642e 6446 9301 6431 6447 9301 6434 6448  d.dF..d1dG..d4dH
 00000190: 9301 6437 6449 9301 643a 644a 9301 643d  ..d7dI..d:dJ..d=
 000001a0: 643b 6901 a501 5a0c 6502 a00d 644b a101  d;i...Z.e...dK..
-000001b0: 5a0e 644c 5a0f 644d 5a10 6402 5300 294e  Z.dLZ.dMZ.d.S.)N
+000001b0: 5a0e 644c 5a0f 644c 5a10 6402 5300 294d  Z.dLZ.dLZ.d.S.)M
 000001c0: e900 0000 0029 01da 0b4f 5554 5055 545f  .....)...OUTPUT_
 000001d0: 464f 4e54 4e7a 1255 6e6e 616d 6564 2f41  FONTNz.Unnamed/A
 000001e0: 6e6f 6e79 6d6f 7573 2e7a 174d 6170 5461  nonymous.z.MapTa
 000001f0: 736b 6572 2076 6572 7369 6f6e 2031 2e33  sker version 1.3
-00000200: 2e33 7a34 474e 5520 4745 4e45 5241 4c20  .3z4GNU GENERAL 
+00000200: 2e34 7a34 474e 5520 4745 4e45 5241 4c20  .4z4GNU GENERAL 
 00000210: 5055 424c 4943 204c 4943 454e 5345 2028  PUBLIC LICENSE (
 00000220: 5665 7273 696f 6e20 332c 2032 3920 4a75  Version 3, 29 Ju
 00000230: 6e65 2032 3030 3729 7a0c 2d6e 6f6e 6520  ne 2007)z.-none 
 00000240: 666f 756e 642e 7a17 2e4d 6170 5461 736b  found.z..MapTask
 00000250: 6572 5f52 756e 436f 756e 742e 7478 747a  er_RunCount.txtz
 00000260: 192e 4d61 7054 6173 6b65 725f 6172 6775  ..MapTasker_argu
 00000270: 6d65 6e74 732e 6a73 6f6e 7a0d 3b66 6f6e  ments.jsonz.;fon
@@ -43,15 +43,15 @@
 000002a0: 6a65 6374 73da 0d70 726f 6a65 6374 5f63  jects..project_c
 000002b0: 6f6c 6f72 da07 5072 6f6a 6563 745a 0850  olor..ProjectZ.P
 000002c0: 726f 6669 6c65 73da 0d70 726f 6669 6c65  rofiles..profile
 000002d0: 5f63 6f6c 6f72 da07 5072 6f66 696c 655a  _color..ProfileZ
 000002e0: 0554 6173 6b73 da0a 7461 736b 5f63 6f6c  .Tasks..task_col
 000002f0: 6f72 da04 5461 736b 7a0e 2854 6173 6b29  or..Taskz.(Task)
 00000300: 2041 6374 696f 6e73 da0c 6163 7469 6f6e   Actions..action
-00000310: 5f63 6f6c 6f72 5a06 4163 7469 6f6e 7a11  _colorZ.Actionz.
+00000310: 5f63 6f6c 6f72 da06 4163 7469 6f6e 7a11  _color..Actionz.
 00000320: 4469 7361 626c 6564 2050 726f 6669 6c65  Disabled Profile
 00000330: 735a 1664 6973 6162 6c65 645f 7072 6f66  sZ.disabled_prof
 00000340: 696c 655f 636f 6c6f 725a 0f44 6973 6162  ile_colorZ.Disab
 00000350: 6c65 6450 726f 6669 6c65 5a0b 556e 6b6e  ledProfileZ.Unkn
 00000360: 6f77 6e54 6173 6bda 1275 6e6b 6e6f 776e  ownTask..unknown
 00000370: 5f74 6173 6b5f 636f 6c6f 725a 0e44 6973  _task_colorZ.Dis
 00000380: 6162 6c65 6441 6374 696f 6eda 1564 6973  abledAction..dis
@@ -75,15 +75,15 @@
 000004a0: 5a06 4275 6c6c 6574 7a0d 4163 7469 6f6e  Z.Bulletz.Action
 000004b0: 204c 6162 656c 73da 1261 6374 696f 6e5f   Labels..action_
 000004c0: 6c61 6265 6c5f 636f 6c6f 725a 0b41 6374  label_colorZ.Act
 000004d0: 696f 6e4c 6162 656c 7a0c 4163 7469 6f6e  ionLabelz.Action
 000004e0: 204e 616d 6573 da11 6163 7469 6f6e 5f6e   Names..action_n
 000004f0: 616d 655f 636f 6c6f 725a 0a41 6374 696f  ame_colorZ.Actio
 00000500: 6e4e 616d 657a 1554 6173 6b65 724e 6574  nNamez.TaskerNet
-00000510: 2049 6e66 6f72 6d61 7469 6f6e da0f 7461   Information..ta
+00000510: 2049 6e66 6f72 6d61 7469 6f6e 5a0f 7461   InformationZ.ta
 00000520: 736b 6572 6e65 745f 636f 6c6f 725a 0d54  skernet_colorZ.T
 00000530: 6173 6b65 724e 6574 496e 666f 7a12 5461  askerNetInfoz.Ta
 00000540: 736b 6572 2050 7265 6665 7265 6e63 6573  sker Preferences
 00000550: 5a11 7072 6566 6572 656e 6365 735f 636f  Z.preferences_co
 00000560: 6c6f 725a 0b50 7265 6665 7265 6e63 6573  lorZ.Preferences
 00000570: 7a11 5472 6169 6c69 6e67 2043 6f6d 6d65  z.Trailing Comme
 00000580: 6e74 735a 1774 7261 696c 696e 675f 636f  ntsZ.trailing_co
@@ -102,47 +102,47 @@
 00000650: 2062 6163 6b67 726f 756e 647a 0c6c 6973   backgroundz.lis
 00000660: 7420 6275 6c6c 6574 737a 1454 6173 6b20  t bulletsz.Task 
 00000670: 6163 7469 6f6e 2027 6c61 6265 6c73 277a  action 'labels'z
 00000680: 1354 6173 6b20 6163 7469 6f6e 2027 6e61  .Task action 'na
 00000690: 6d65 7327 7a17 5461 736b 6572 4e65 7420  mes'z.TaskerNet 
 000006a0: 2769 6e66 6f72 6d61 7469 6f6e 277a 1454  'information'z.T
 000006b0: 6173 6b65 7220 2770 7265 6665 7265 6e63  asker 'preferenc
-000006c0: 6573 275a 094d 6170 5461 736b 6572 4654  es'Z.MapTaskerFT
-000006d0: 2911 da14 6d61 7074 6173 6b65 722e 7372  )...maptasker.sr
-000006e0: 632e 636f 6e66 6967 7202 0000 005a 076c  c.configr....Z.l
-000006f0: 6f67 6769 6e67 da11 554e 4b4e 4f57 4e5f  ogging..UNKNOWN_
-00000700: 5441 534b 5f4e 414d 455a 0a4d 595f 5645  TASK_NAMEZ.MY_VE
-00000710: 5253 494f 4e5a 0a4d 595f 4c49 4345 4e53  RSIONZ.MY_LICENS
-00000720: 455a 0a4e 4f5f 5052 4f4a 4543 545a 0c43  EZ.NO_PROJECTZ.C
-00000730: 4f55 4e54 4552 5f46 494c 455a 0e41 5247  OUNTER_FILEZ.ARG
-00000740: 554d 454e 5453 5f46 494c 45da 0b46 4f4e  UMENTS_FILE..FON
-00000750: 545f 544f 5f55 5345 5a0a 4e4f 5f50 524f  T_TO_USEZ.NO_PRO
-00000760: 4649 4c45 5a14 5459 5045 535f 4f46 5f43  FILEZ.TYPES_OF_C
-00000770: 4f4c 4f52 5f4e 414d 4553 5a0f 5459 5045  OLOR_NAMESZ.TYPE
-00000780: 535f 4f46 5f43 4f4c 4f52 535a 0967 6574  S_OF_COLORSZ.get
-00000790: 4c6f 6767 6572 da06 6c6f 6767 6572 da09  Logger..logger..
-000007a0: 6465 6275 675f 6f75 745a 0d44 4542 5547  debug_outZ.DEBUG
-000007b0: 5f50 524f 4752 414d a900 7217 0000 0072  _PROGRAM..r....r
-000007c0: 1700 0000 fa77 2f55 7365 7273 2f6d 696b  .....w/Users/mik
-000007d0: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
-000007e0: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
-000007f0: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
-00000800: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
-00000810: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
-00000820: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
-00000830: 632f 7379 7363 6f6e 7374 2e70 79da 083c  c/sysconst.py..<
-00000840: 6d6f 6475 6c65 3e01 0000 0073 ea00 0000  module>....s....
-00000850: 0c0d 0801 0403 0401 0401 0401 0401 0401  ................
-00000860: 0a01 0401 0207 0401 02ff 0402 02fe 0403  ................
-00000870: 02fd 0404 02fc 0405 02fb 0406 02fa 0407  ................
-00000880: 02f9 0408 02f8 0409 02f7 040a 02f6 040b  ................
-00000890: 02f5 040c 02f4 040d 02f3 040e 02f2 040f  ................
-000008a0: 02f1 0410 02f0 0411 04ef 0412 02ee 0413  ................
-000008b0: 02ed 0414 02ec 0415 02eb 0416 02ea 0417  ................
-000008c0: 02e9 0418 02e8 0419 02e7 041a 02e6 041b  ................
-000008d0: 02e5 041c 02e4 041d 02e3 041e 02e2 041f  ................
-000008e0: 02e1 0420 02e0 0421 06df 0225 0401 02ff  ... ...!...%....
-000008f0: 0402 02fe 0403 02fd 0404 02fc 0405 02fb  ................
-00000900: 0406 02fa 0407 02f9 0408 02f8 0409 02f7  ................
-00000910: 040a 02f6 040b 02f5 040c 02f4 040d 02f3  ................
-00000920: 040e 02f2 040f 02f1 0410 02f0 0411 02ef  ................
-00000930: 0412 06ee 0a15 0401 0801                 ..........
+000006c0: 6573 275a 094d 6170 5461 736b 6572 4629  es'Z.MapTaskerF)
+000006d0: 11da 146d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
+000006e0: 2e63 6f6e 6669 6772 0200 0000 da07 6c6f  .configr......lo
+000006f0: 6767 696e 67da 1155 4e4b 4e4f 574e 5f54  gging..UNKNOWN_T
+00000700: 4153 4b5f 4e41 4d45 5a0a 4d59 5f56 4552  ASK_NAMEZ.MY_VER
+00000710: 5349 4f4e 5a0a 4d59 5f4c 4943 454e 5345  SIONZ.MY_LICENSE
+00000720: 5a0a 4e4f 5f50 524f 4a45 4354 5a0c 434f  Z.NO_PROJECTZ.CO
+00000730: 554e 5445 525f 4649 4c45 5a0e 4152 4755  UNTER_FILEZ.ARGU
+00000740: 4d45 4e54 535f 4649 4c45 da0b 464f 4e54  MENTS_FILE..FONT
+00000750: 5f54 4f5f 5553 455a 0a4e 4f5f 5052 4f46  _TO_USEZ.NO_PROF
+00000760: 494c 455a 1454 5950 4553 5f4f 465f 434f  ILEZ.TYPES_OF_CO
+00000770: 4c4f 525f 4e41 4d45 535a 0f54 5950 4553  LOR_NAMESZ.TYPES
+00000780: 5f4f 465f 434f 4c4f 5253 da09 6765 744c  _OF_COLORS..getL
+00000790: 6f67 6765 72da 066c 6f67 6765 72da 0964  ogger..logger..d
+000007a0: 6562 7567 5f6f 7574 5a0d 4445 4255 475f  ebug_outZ.DEBUG_
+000007b0: 5052 4f47 5241 4da9 0072 1900 0000 7219  PROGRAM..r....r.
+000007c0: 0000 00fa 772f 5573 6572 732f 6d69 6b72  ....w/Users/mikr
+000007d0: 7562 696e 2f4c 6962 7261 7279 2f43 6c6f  ubin/Library/Clo
+000007e0: 7564 5374 6f72 6167 652f 476f 6f67 6c65  udStorage/Google
+000007f0: 4472 6976 652d 6d69 6b72 7562 696e 4067  Drive-mikrubin@g
+00000800: 6d61 696c 2e63 6f6d 2f4d 7920 4472 6976  mail.com/My Driv
+00000810: 652f 5079 7468 6f6e 2f6d 6170 7461 736b  e/Python/maptask
+00000820: 6572 2f6d 6170 7461 736b 6572 2f73 7263  er/maptasker/src
+00000830: 2f73 7973 636f 6e73 742e 7079 da08 3c6d  /sysconst.py..<m
+00000840: 6f64 756c 653e 0100 0000 73ea 0000 000c  odule>....s.....
+00000850: 0d08 0104 0304 0104 0104 0104 0104 010a  ................
+00000860: 0104 0102 0704 0102 ff04 0202 fe04 0302  ................
+00000870: fd04 0402 fc04 0502 fb04 0602 fa04 0702  ................
+00000880: f904 0802 f804 0902 f704 0a02 f604 0b02  ................
+00000890: f504 0c02 f404 0d02 f304 0e02 f204 0f02  ................
+000008a0: f104 1002 f004 1104 ef04 1202 ee04 1302  ................
+000008b0: ed04 1402 ec04 1502 eb04 1602 ea04 1702  ................
+000008c0: e904 1802 e804 1902 e704 1a02 e604 1b02  ................
+000008d0: e504 1c02 e404 1d02 e304 1e02 e204 1f02  ................
+000008e0: e104 2002 e004 2106 df02 2504 0102 ff04  .. ...!...%.....
+000008f0: 0202 fe04 0302 fd04 0402 fc04 0502 fb04  ................
+00000900: 0602 fa04 0702 f904 0802 f804 0902 f704  ................
+00000910: 0a02 f604 0b02 f504 0c02 f404 0d02 f304  ................
+00000920: 0e02 f204 0f02 f104 1002 f004 1102 ef04  ................
+00000930: 1206 ee0a 1504 0108 01                   .........
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/taskactn.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/taskactn.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 13 17:20:50 2023 UTC, .py size: 5820 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,155 +1,154 @@
-00000000: 6f0d 0d0a 0000 0000 f239 3864 bc16 0000  o........98d....
+00000000: 6f0d 0d0a 0000 0000 689e 4a64 1d16 0000  o.......h.Jd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0012 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a04 0100 6400 6402 6c05 6d06  ..m.Z...d.d.l.m.
 00000050: 5a06 0100 6400 6403 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
-00000060: 6400 6404 6c07 6d09 5a09 0100 6400 6405  d.d.l.m.Z...d.d.
-00000070: 6c0a 6d0b 5a0b 0100 6406 6501 6a0c 6a0d  l.m.Z...d.e.j.j.
-00000080: 6407 650e 650f 1900 6408 6510 6409 650f  d.e.e...d.e.d.e.
-00000090: 640a 650f 640b 650e 650f 1900 640c 6510  d.e.d.e.e...d.e.
-000000a0: 640d 6510 640e 6401 6612 640f 6410 8404  d.e.d.d.f.d.d...
-000000b0: 5a11 640c 6510 6408 6510 6407 650e 6411  Z.d.e.d.e.d.e.d.
-000000c0: 6512 6412 650e 640a 6501 6a0c 6a0d 640e  e.d.e.d.e.j.j.d.
-000000d0: 6401 660e 6413 6414 8404 5a13 6401 5300  d.f.d.d...Z.d.S.
+00000060: 6400 6404 6c09 6d0a 5a0a 0100 6400 6405  d.d.l.m.Z...d.d.
+00000070: 6c0b 6d0c 5a0c 0100 6406 6501 6a0d 6a0e  l.m.Z...d.e.j.j.
+00000080: 6407 650f 6510 1900 6408 6511 6409 6510  d.e.e...d.e.d.e.
+00000090: 640a 6510 640b 650f 6510 1900 640c 6511  d.e.d.e.e...d.e.
+000000a0: 640d 6511 640e 6401 6612 640f 6410 8404  d.e.d.d.f.d.d...
+000000b0: 5a12 640c 6511 6408 6511 6407 650f 6411  Z.d.e.d.e.d.e.d.
+000000c0: 6513 6412 650f 640a 6501 6a0d 6a0e 640e  e.d.e.d.e.j.j.d.
+000000d0: 6401 660e 6413 6414 8404 5a14 6401 5300  d.f.d.d...Z.d.S.
 000000e0: 2915 e900 0000 004e 2901 da09 6d79 5f6f  )......N)...my_o
-000000f0: 7574 7075 7429 01da 066c 6f67 6765 7229  utput)...logger)
-00000100: 01da 1155 4e4b 4e4f 574e 5f54 4153 4b5f  ...UNKNOWN_TASK_
-00000110: 4e41 4d45 2901 da0b 666f 726d 6174 5f68  NAME)...format_h
-00000120: 746d 6cda 0874 6865 5f74 6173 6bda 0b6f  tml..the_task..o
-00000130: 7574 7075 745f 6c69 7374 da0c 7072 6f67  utput_list..prog
-00000140: 7261 6d5f 6172 6773 da09 6c69 7374 5f74  ram_args..list_t
-00000150: 7970 65da 0874 6865 5f69 7465 6dda 0b74  ype..the_item..t
-00000160: 6173 6b73 5f66 6f75 6e64 da08 636f 6c6f  asks_found..colo
-00000170: 726d 6170 da09 616c 6c5f 7461 736b 73da  rmap..all_tasks.
-00000180: 0672 6574 7572 6e63 0800 0000 0000 0000  .returnc........
-00000190: 0000 0000 0d00 0000 0700 0000 4300 0000  ............C...
-000001a0: 73f0 0000 0074 007c 0476 0073 0a7c 0264  s....t.|.v.s.|.d
-000001b0: 0119 0064 026b 0472 7664 037c 0376 0072  ...d.k.rvd.|.v.r
-000001c0: 1064 046e 047c 04a0 0164 05a1 017d 0874  .d.n.|...d...}.t
-000001d0: 027c 0883 0164 066b 0472 377c 0864 0619  .|...d.k.r7|.d..
-000001e0: 00a0 0164 0764 06a1 0264 0219 007c 0864  ...d.d...d...|.d
-000001f0: 063c 0074 03a0 047c 0864 0619 007c 057c  .<.t...|.d...|.|
-00000200: 0864 0619 0067 0164 087c 07a1 055c 027d  .d...g.d.|...\.}
-00000210: 007d 097c 0072 6b74 03a0 057c 007c 067c  .}.|.rkt...|.|.|
-00000220: 02a1 0304 007d 0a72 6974 067c 067c 027c  .....}.rit.|.|.|
-00000230: 0164 0664 0883 0501 0064 067d 0b74 077c  .d.d.....d.}.t.|
-00000240: 067c 027c 017c 0b7c 0a7c 0483 0601 0064  .|.|.|.|.|.....d
-00000250: 037c 0376 0072 6974 067c 067c 027c 0164  .|.v.rit.|.|.|.d
-00000260: 0964 0883 0501 0074 067c 067c 027c 0164  .d.....t.|.|.|.d
-00000270: 0964 0883 0501 0064 0053 0064 0a7d 0c74  .d.....d.S.d.}.t
-00000280: 08a0 097c 0ca1 0101 0074 0a7c 0c83 0101  ...|.....t.|....
-00000290: 0064 0053 0029 0b4e da14 6469 7370 6c61  .d.S.).N..displa
-000002a0: 795f 6465 7461 696c 5f6c 6576 656c 7201  y_detail_levelr.
-000002b0: 0000 007a 0f26 2334 353b 2623 3435 3b54  ...z.&#45;&#45;T
-000002c0: 6173 6b3a da01 787a 0954 6173 6b20 4944  ask:..xz.Task ID
-000002d0: 3a20 e901 0000 00fa 0120 da00 e903 0000  : ....... ......
-000002e0: 007a 1745 7272 6f72 3a20 4e6f 2054 6173  .z.Error: No Tas
-000002f0: 6b20 666f 756e 6421 2121 290b 7204 0000  k found!!!).r...
-00000300: 00da 0573 706c 6974 da03 6c65 6eda 0574  ...split..len..t
-00000310: 6173 6b73 da0d 6765 745f 7461 736b 5f6e  asks..get_task_n
-00000320: 616d 65da 0b67 6574 5f61 6374 696f 6e73  ame..get_actions
-00000330: 7202 0000 00da 166f 7574 7075 745f 6c69  r......output_li
-00000340: 7374 5f6f 665f 6163 7469 6f6e 7372 0300  st_of_actionsr..
-00000350: 0000 da05 6465 6275 67da 0570 7269 6e74  ....debug..print
-00000360: 290d 7206 0000 0072 0700 0000 7208 0000  ).r....r....r...
-00000370: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000380: 720c 0000 0072 0d00 0000 5a07 7465 6d70  r....r....Z.temp
-00000390: 5f69 64da 046b 616b 61da 0561 6c69 7374  _id..kaka..alist
-000003a0: da0c 6163 7469 6f6e 5f63 6f75 6e74 da09  ..action_count..
-000003b0: 6572 726f 725f 6d73 67a9 0072 2100 0000  error_msg..r!...
-000003c0: fa77 2f55 7365 7273 2f6d 696b 7275 6269  .w/Users/mikrubi
-000003d0: 6e2f 4c69 6272 6172 792f 436c 6f75 6453  n/Library/CloudS
-000003e0: 746f 7261 6765 2f47 6f6f 676c 6544 7269  torage/GoogleDri
-000003f0: 7665 2d6d 696b 7275 6269 6e40 676d 6169  ve-mikrubin@gmai
-00000400: 6c2e 636f 6d2f 4d79 2044 7269 7665 2f50  l.com/My Drive/P
-00000410: 7974 686f 6e2f 6d61 7074 6173 6b65 722f  ython/maptasker/
-00000420: 6d61 7074 6173 6b65 722f 7372 632f 7461  maptasker/src/ta
-00000430: 736b 6163 746e 2e70 79da 1b67 6574 5f74  skactn.py..get_t
-00000440: 6173 6b5f 6163 7469 6f6e 735f 616e 645f  ask_actions_and_
-00000450: 6f75 7470 7574 1a00 0000 7330 0000 0014  output....s0....
-00000460: 0b16 030c 0218 0104 0114 0108 ff04 0412  ................
-00000470: 0102 010a 0104 ff04 0302 010c 0104 ff08  ................
-00000480: 0410 0110 0104 0504 fd0a 0108 0104 0172  ...............r
-00000490: 2300 0000 721f 0000 0072 1e00 0000 6306  #...r....r....c.
-000004a0: 0000 0000 0000 0000 0000 0007 0000 000e  ................
-000004b0: 0000 0043 0000 0073 cc00 0000 7c04 4400  ...C...s....|.D.
-000004c0: 5d59 7d06 7c06 6401 7501 725b 7c06 6401  ]Y}.|.d.u.r[|.d.
-000004d0: 6402 8502 1900 6403 6b02 7222 7400 7c00  d.....d.k.r"t.|.
-000004e0: 7c01 7c02 6404 7401 7c00 6405 6406 6407  |.|.d.t.|.d.d.d.
-000004f0: 7c06 9b00 9d02 6408 8305 8305 0100 6e1d  |.....d.......n.
-00000500: 7400 7c00 7c01 7c02 6404 7401 7c00 6405  t.|.|.|.d.t.|.d.
-00000510: 6406 6407 7402 7c03 8301 a003 6404 a101  d.d.t.|.....d...
-00000520: 9b00 6409 7c06 9b00 9d04 6408 8305 8305  ..d.|.....d.....
-00000530: 0100 7c03 640a 3700 7d03 7c03 6404 6b02  ..|.d.7.}.|.d.k.
-00000540: 724f 7c01 640b 1900 640c 6b02 724f 7404  rO|.d...d.k.rOt.
-00000550: 7c05 7600 724f 0100 6e0d 7c01 640b 1900  |.v.rO..n.|.d...
-00000560: 640a 6b02 725b 7404 7c05 7601 725b 0100  d.k.r[t.|.v.r[..
-00000570: 6e01 7102 7400 7c00 7c01 7c02 6402 6406  n.q.t.|.|.|.d.d.
-00000580: 8305 0100 6401 5300 290d 61d8 0100 006f  ....d.S.).a....o
-00000590: 7574 7075 7420 7468 6520 6c69 7374 206f  utput the list o
-000005a0: 6620 5461 736b 2041 6374 696f 6e73 0a0a  f Task Actions..
-000005b0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-000005c0: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-000005d0: 6f6c 6f72 6d61 703a 2064 6963 7469 6f6e  olormap: diction
-000005e0: 6172 7920 6f66 2063 6f6c 6f72 7320 746f  ary of colors to
-000005f0: 2075 7365 0a20 2020 2020 2020 203a 7061   use.        :pa
-00000600: 7261 6d20 7072 6f67 7261 6d5f 6172 6773  ram program_args
-00000610: 3a20 6469 6374 696f 6e61 7279 206f 6620  : dictionary of 
-00000620: 7072 6f67 7261 6d20 7275 6e74 696d 6520  program runtime 
-00000630: 6172 6775 6d65 6e74 730a 2020 2020 2020  arguments.      
-00000640: 2020 3a70 6172 616d 206f 7574 7075 745f    :param output_
-00000650: 6c69 7374 3a20 6c69 7374 2069 6e74 6f20  list: list into 
-00000660: 7768 6963 6820 746f 2061 6464 2074 6865  which to add the
-00000670: 206f 7574 7075 7420 6c69 6e65 730a 2020   output lines.  
-00000680: 2020 2020 2020 3a70 6172 616d 2061 6374        :param act
-00000690: 696f 6e5f 636f 756e 743a 2063 6f75 6e74  ion_count: count
-000006a0: 206f 6620 5461 736b 2061 6374 696f 6e73   of Task actions
-000006b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000006c0: 616c 6973 743a 206c 6973 7420 6f66 2074  alist: list of t
-000006d0: 6173 6b20 6163 7469 6f6e 730a 2020 2020  ask actions.    
-000006e0: 2020 2020 3a70 6172 616d 2074 6865 5f69      :param the_i
-000006f0: 7465 6d3a 2074 6865 2073 7065 6369 6669  tem: the specifi
-00000700: 6320 5461 736b 2773 2064 6574 6169 6c65  c Task's detaile
-00000710: 6420 6c69 6e65 0a0a 2020 2020 5265 7475  d line..    Retu
-00000720: 726e 733a 2074 6865 2063 6f75 6e74 206f  rns: the count o
-00000730: 6620 7468 6520 6e75 6d62 6572 206f 6620  f the number of 
-00000740: 7469 6d65 7320 7468 6520 7072 6f67 7261  times the progra
-00000750: 6d20 6861 7320 6265 656e 2063 616c 6c65  m has been calle
-00000760: 640a 0a20 2020 204e 7214 0000 007a 032e  d..    Nr....z..
-00000770: 2e2e e902 0000 00da 0c61 6374 696f 6e5f  .........action_
-00000780: 636f 6c6f 7272 1300 0000 7a08 4163 7469  colorr....z.Acti
-00000790: 6f6e 3a20 467a 083c 2f73 7061 6e3e 2072  on: Fz.</span> r
-000007a0: 1100 0000 720f 0000 0072 0100 0000 2905  ....r....r....).
-000007b0: 7202 0000 0072 0500 0000 da03 7374 72da  r....r......str.
-000007c0: 057a 6669 6c6c 7204 0000 0029 0772 0c00  .zfillr....).r..
-000007d0: 0000 7208 0000 0072 0700 0000 721f 0000  ..r....r....r...
-000007e0: 0072 1e00 0000 720a 0000 005a 0774 6163  .r....r....Z.tac
-000007f0: 7469 6f6e 7221 0000 0072 2100 0000 7222  tionr!...r!...r"
-00000800: 0000 0072 1a00 0000 4700 0000 7348 0000  ...r....G...sH..
-00000810: 0008 1508 0110 0302 0102 0102 0102 0102  ................
-00000820: 0102 0110 0102 ff06 fb02 0b02 0102 0102  ................
-00000830: 0102 0102 0102 0102 0102 0118 0102 0102  ................
-00000840: fb04 fb08 0d08 020c 0108 0104 020c 0208  ................
-00000850: 0104 0202 8010 0104 0172 1a00 0000 2914  .........r....).
-00000860: da16 6465 6675 7365 6478 6d6c 2e45 6c65  ..defusedxml.Ele
-00000870: 6d65 6e74 5472 6565 da0a 6465 6675 7365  mentTree..defuse
-00000880: 6478 6d6c da13 6d61 7074 6173 6b65 722e  dxml..maptasker.
-00000890: 7372 632e 7461 736b 73da 0373 7263 7217  src.tasks..srcr.
-000008a0: 0000 00da 156d 6170 7461 736b 6572 2e73  .....maptasker.s
-000008b0: 7263 2e6f 7574 7075 746c 7202 0000 00da  rc.outputlr.....
-000008c0: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
-000008d0: 7973 636f 6e73 7472 0300 0000 7204 0000  ysconstr....r...
-000008e0: 00da 166d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
-000008f0: 2e66 726d 7468 746d 6c72 0500 0000 da0b  .frmthtmlr......
-00000900: 456c 656d 656e 7454 7265 65da 0358 4d4c  ElementTree..XML
-00000910: da04 6c69 7374 7226 0000 00da 0464 6963  ..listr&.....dic
-00000920: 7472 2300 0000 da03 696e 7472 1a00 0000  tr#.....intr....
-00000930: 7221 0000 0072 2100 0000 7221 0000 0072  r!...r!...r!...r
-00000940: 2200 0000 da08 3c6d 6f64 756c 653e 0100  ".....<module>..
-00000950: 0000 7350 0000 0008 0d12 020c 010c 010c  ..sP............
-00000960: 010c 0102 0606 0102 ff06 0202 fe02 0302  ................
-00000970: fd02 0402 fc02 0502 fb06 0602 fa02 0702  ................
-00000980: f902 0802 f802 090a f702 2d02 0102 ff02  ..........-.....
-00000990: 0202 fe02 0302 fd02 0402 fc02 0502 fb06  ................
-000009a0: 0602 fa02 070e f9                        .......
+000000f0: 7574 7075 7429 01da 1155 4e4b 4e4f 574e  utput)...UNKNOWN
+00000100: 5f54 4153 4b5f 4e41 4d45 2901 da0b 666f  _TASK_NAME)...fo
+00000110: 726d 6174 5f68 746d 6c29 01da 0d65 7272  rmat_html)...err
+00000120: 6f72 5f68 616e 646c 6572 da08 7468 655f  or_handler..the_
+00000130: 7461 736b da0b 6f75 7470 7574 5f6c 6973  task..output_lis
+00000140: 74da 0c70 726f 6772 616d 5f61 7267 73da  t..program_args.
+00000150: 096c 6973 745f 7479 7065 da08 7468 655f  .list_type..the_
+00000160: 6974 656d da0b 7461 736b 735f 666f 756e  item..tasks_foun
+00000170: 64da 0863 6f6c 6f72 6d61 70da 0961 6c6c  d..colormap..all
+00000180: 5f74 6173 6b73 da06 7265 7475 726e 6308  _tasks..returnc.
+00000190: 0000 0000 0000 0000 0000 000c 0000 0007  ................
+000001a0: 0000 0043 0000 0073 e800 0000 7400 7c04  ...C...s....t.|.
+000001b0: 7600 730a 7c02 6401 1900 6402 6b04 7272  v.s.|.d...d.k.rr
+000001c0: 6403 7c03 7600 7210 6404 6e04 7c04 a001  d.|.v.r.d.n.|...
+000001d0: 6405 a101 7d08 6406 7d09 7402 7c08 8301  d...}.d.}.t.|...
+000001e0: 6407 6b04 7239 7c08 6407 1900 a001 6408  d.k.r9|.d.....d.
+000001f0: 6407 a102 6402 1900 7c08 6407 3c00 7403  d...d...|.d.<.t.
+00000200: a004 7c08 6407 1900 7c05 7c08 6407 1900  ..|.d...|.|.d...
+00000210: 6701 6406 7c07 a105 5c02 7d00 7d09 7c00  g.d.|...\.}.}.|.
+00000220: 726d 7403 a005 7c00 7c06 7c02 a103 0400  rmt...|.|.|.....
+00000230: 7d0a 726b 7406 7c06 7c02 7c01 6407 6406  }.rkt.|.|.|.d.d.
+00000240: 8305 0100 6407 7d0b 7407 7c06 7c02 7c01  ....d.}.t.|.|.|.
+00000250: 7c0b 7c0a 7c04 8306 0100 6403 7c03 7600  |.|.|.....d.|.v.
+00000260: 726b 7406 7c06 7c02 7c01 6409 6406 8305  rkt.|.|.|.d.d...
+00000270: 0100 7406 7c06 7c02 7c01 6409 6406 8305  ..t.|.|.|.d.d...
+00000280: 0100 6400 5300 7408 640a 6402 8302 0100  ..d.S.t.d.d.....
+00000290: 6400 5300 290b 4eda 1464 6973 706c 6179  d.S.).N..display
+000002a0: 5f64 6574 6169 6c5f 6c65 7665 6c72 0100  _detail_levelr..
+000002b0: 0000 7a0f 2623 3435 3b26 2334 353b 5461  ..z.&#45;&#45;Ta
+000002c0: 736b 3ada 0178 7a09 5461 736b 2049 443a  sk:..xz.Task ID:
+000002d0: 20da 00e9 0100 0000 da01 20e9 0300 0000   ......... .....
+000002e0: 7a10 4e6f 2054 6173 6b20 666f 756e 6421  z.No Task found!
+000002f0: 2121 2909 7203 0000 00da 0573 706c 6974  !!).r......split
+00000300: da03 6c65 6eda 0574 6173 6b73 da0d 6765  ..len..tasks..ge
+00000310: 745f 7461 736b 5f6e 616d 65da 0b67 6574  t_task_name..get
+00000320: 5f61 6374 696f 6e73 7202 0000 00da 166f  _actionsr......o
+00000330: 7574 7075 745f 6c69 7374 5f6f 665f 6163  utput_list_of_ac
+00000340: 7469 6f6e 7372 0500 0000 290c 7206 0000  tionsr....).r...
+00000350: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
+00000360: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000370: 0d00 0000 5a07 7465 6d70 5f69 64da 046b  ....Z.temp_id..k
+00000380: 616b 61da 0561 6c69 7374 da0c 6163 7469  aka..alist..acti
+00000390: 6f6e 5f63 6f75 6e74 a900 721e 0000 00fa  on_count..r.....
+000003a0: 772f 5573 6572 732f 6d69 6b72 7562 696e  w/Users/mikrubin
+000003b0: 2f4c 6962 7261 7279 2f43 6c6f 7564 5374  /Library/CloudSt
+000003c0: 6f72 6167 652f 476f 6f67 6c65 4472 6976  orage/GoogleDriv
+000003d0: 652d 6d69 6b72 7562 696e 4067 6d61 696c  e-mikrubin@gmail
+000003e0: 2e63 6f6d 2f4d 7920 4472 6976 652f 5079  .com/My Drive/Py
+000003f0: 7468 6f6e 2f6d 6170 7461 736b 6572 2f6d  thon/maptasker/m
+00000400: 6170 7461 736b 6572 2f73 7263 2f74 6173  aptasker/src/tas
+00000410: 6b61 6374 6e2e 7079 da1b 6765 745f 7461  kactn.py..get_ta
+00000420: 736b 5f61 6374 696f 6e73 5f61 6e64 5f6f  sk_actions_and_o
+00000430: 7574 7075 741a 0000 0073 2e00 0000 140b  utput....s......
+00000440: 1603 0401 0c02 1801 0401 1401 08ff 0405  ................
+00000450: 1201 0201 0a01 04ff 0403 0201 0c01 04ff  ................
+00000460: 0804 1001 1001 0404 0afe 0402 7220 0000  ............r ..
+00000470: 0072 1d00 0000 721c 0000 0063 0600 0000  .r....r....c....
+00000480: 0000 0000 0000 0000 0700 0000 0e00 0000  ................
+00000490: 4300 0000 73cc 0000 007c 0444 005d 597d  C...s....|.D.]Y}
+000004a0: 067c 0664 0175 0172 5b7c 0664 0164 0285  .|.d.u.r[|.d.d..
+000004b0: 0219 0064 036b 0272 2274 007c 007c 017c  ...d.k.r"t.|.|.|
+000004c0: 0264 0474 017c 0064 0564 0664 077c 069b  .d.t.|.d.d.d.|..
+000004d0: 009d 0264 0883 0583 0501 006e 1d74 007c  ...d.......n.t.|
+000004e0: 007c 017c 0264 0474 017c 0064 0564 0664  .|.|.d.t.|.d.d.d
+000004f0: 0774 027c 0383 01a0 0364 04a1 019b 0064  .t.|.....d.....d
+00000500: 097c 069b 009d 0464 0883 0583 0501 007c  .|.....d.......|
+00000510: 0364 0a37 007d 037c 0364 046b 0272 4f7c  .d.7.}.|.d.k.rO|
+00000520: 0164 0b19 0064 0c6b 0272 4f74 047c 0576  .d...d.k.rOt.|.v
+00000530: 0072 4f01 006e 0d7c 0164 0b19 0064 0a6b  .rO..n.|.d...d.k
+00000540: 0272 5b74 047c 0576 0172 5b01 006e 0171  .r[t.|.v.r[..n.q
+00000550: 0274 007c 007c 017c 0264 0264 0683 0501  .t.|.|.|.d.d....
+00000560: 0064 0153 0029 0d61 d801 0000 6f75 7470  .d.S.).a....outp
+00000570: 7574 2074 6865 206c 6973 7420 6f66 2054  ut the list of T
+00000580: 6173 6b20 4163 7469 6f6e 730a 0a20 2020  ask Actions..   
+00000590: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+000005a0: 2020 2020 203a 7061 7261 6d20 636f 6c6f       :param colo
+000005b0: 726d 6170 3a20 6469 6374 696f 6e61 7279  rmap: dictionary
+000005c0: 206f 6620 636f 6c6f 7273 2074 6f20 7573   of colors to us
+000005d0: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
+000005e0: 2070 726f 6772 616d 5f61 7267 733a 2064   program_args: d
+000005f0: 6963 7469 6f6e 6172 7920 6f66 2070 726f  ictionary of pro
+00000600: 6772 616d 2072 756e 7469 6d65 2061 7267  gram runtime arg
+00000610: 756d 656e 7473 0a20 2020 2020 2020 203a  uments.        :
+00000620: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
+00000630: 743a 206c 6973 7420 696e 746f 2077 6869  t: list into whi
+00000640: 6368 2074 6f20 6164 6420 7468 6520 6f75  ch to add the ou
+00000650: 7470 7574 206c 696e 6573 0a20 2020 2020  tput lines.     
+00000660: 2020 203a 7061 7261 6d20 6163 7469 6f6e     :param action
+00000670: 5f63 6f75 6e74 3a20 636f 756e 7420 6f66  _count: count of
+00000680: 2054 6173 6b20 6163 7469 6f6e 730a 2020   Task actions.  
+00000690: 2020 2020 2020 3a70 6172 616d 2061 6c69        :param ali
+000006a0: 7374 3a20 6c69 7374 206f 6620 7461 736b  st: list of task
+000006b0: 2061 6374 696f 6e73 0a20 2020 2020 2020   actions.       
+000006c0: 203a 7061 7261 6d20 7468 655f 6974 656d   :param the_item
+000006d0: 3a20 7468 6520 7370 6563 6966 6963 2054  : the specific T
+000006e0: 6173 6b27 7320 6465 7461 696c 6564 206c  ask's detailed l
+000006f0: 696e 650a 0a20 2020 2052 6574 7572 6e73  ine..    Returns
+00000700: 3a20 7468 6520 636f 756e 7420 6f66 2074  : the count of t
+00000710: 6865 206e 756d 6265 7220 6f66 2074 696d  he number of tim
+00000720: 6573 2074 6865 2070 726f 6772 616d 2068  es the program h
+00000730: 6173 2062 6565 6e20 6361 6c6c 6564 0a0a  as been called..
+00000740: 2020 2020 4e72 1400 0000 7a03 2e2e 2ee9      Nr....z.....
+00000750: 0200 0000 da0c 6163 7469 6f6e 5f63 6f6c  ......action_col
+00000760: 6f72 7211 0000 007a 0841 6374 696f 6e3a  orr....z.Action:
+00000770: 2046 7a08 3c2f 7370 616e 3e20 7212 0000   Fz.</span> r...
+00000780: 0072 0f00 0000 7201 0000 0029 0572 0200  .r....r....).r..
+00000790: 0000 7204 0000 00da 0373 7472 da05 7a66  ..r......str..zf
+000007a0: 696c 6c72 0300 0000 2907 720c 0000 0072  illr....).r....r
+000007b0: 0800 0000 7207 0000 0072 1d00 0000 721c  ....r....r....r.
+000007c0: 0000 0072 0a00 0000 5a07 7461 6374 696f  ...r....Z.tactio
+000007d0: 6e72 1e00 0000 721e 0000 0072 1f00 0000  nr....r....r....
+000007e0: 721a 0000 0048 0000 0073 4800 0000 0815  r....H...sH.....
+000007f0: 0801 1001 0201 0201 0201 0201 0201 0201  ................
+00000800: 1001 02ff 06fb 020b 0201 0201 0201 0201  ................
+00000810: 0201 0201 0201 0201 1801 0201 02fb 04fb  ................
+00000820: 080d 0802 0c01 0801 0402 0c02 0801 0402  ................
+00000830: 0280 1002 0401 721a 0000 0029 15da 1664  ......r....)...d
+00000840: 6566 7573 6564 786d 6c2e 456c 656d 656e  efusedxml.Elemen
+00000850: 7454 7265 65da 0a64 6566 7573 6564 786d  tTree..defusedxm
+00000860: 6cda 136d 6170 7461 736b 6572 2e73 7263  l..maptasker.src
+00000870: 2e74 6173 6b73 da03 7372 6372 1700 0000  .tasks..srcr....
+00000880: da15 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
+00000890: 6f75 7470 7574 6c72 0200 0000 da16 6d61  outputlr......ma
+000008a0: 7074 6173 6b65 722e 7372 632e 7379 7363  ptasker.src.sysc
+000008b0: 6f6e 7374 7203 0000 00da 166d 6170 7461  onstr......mapta
+000008c0: 736b 6572 2e73 7263 2e66 726d 7468 746d  sker.src.frmthtm
+000008d0: 6c72 0400 0000 da13 6d61 7074 6173 6b65  lr......maptaske
+000008e0: 722e 7372 632e 6572 726f 7272 0500 0000  r.src.errorr....
+000008f0: da0b 456c 656d 656e 7454 7265 65da 0358  ..ElementTree..X
+00000900: 4d4c da04 6c69 7374 7223 0000 00da 0464  ML..listr#.....d
+00000910: 6963 7472 2000 0000 da03 696e 7472 1a00  ictr .....intr..
+00000920: 0000 721e 0000 0072 1e00 0000 721e 0000  ..r....r....r...
+00000930: 0072 1f00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000940: 0100 0000 7350 0000 0008 0d12 020c 010c  ....sP..........
+00000950: 010c 010c 0102 0606 0102 ff06 0202 fe02  ................
+00000960: 0302 fd02 0402 fc02 0502 fb06 0602 fa02  ................
+00000970: 0702 f902 0802 f802 090a f702 2e02 0102  ................
+00000980: ff02 0202 fe02 0302 fd02 0402 fc02 0502  ................
+00000990: fb06 0602 fa02 070e f9                   .........
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/taskerd.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/taskerd.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 10 15:03:06 2023 UTC, .py size: 3100 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-00000000: 6f0d 0d0a 0000 0000 2a25 3464 1c0c 0000  o.......*%4d....
+00000000: 6f0d 0d0a 0000 0000 731e 4464 1d0c 0000  o.......s.Dd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
+00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
-00000050: 6505 6602 6405 6406 8404 5a06 6407 6408  e.f.d.d...Z.d.d.
-00000060: 8400 5a07 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
-00000070: 2901 da05 7061 7273 6529 01da 066c 6f67  )...parse)...log
-00000080: 6765 72da 0869 735f 7363 656e 6563 0200  ger..is_scenec..
-00000090: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-000000a0: 0000 4300 0000 733a 0000 0069 007d 027c  ..C...s:...i.}.|
-000000b0: 0172 0664 016e 0164 027d 037c 0044 005d  .r.d.n.d.}.|.D.]
-000000c0: 0c7d 047c 04a0 007c 03a1 016a 017d 057c  .}.|...|...j.}.|
-000000d0: 047c 027c 053c 0071 0a7c 00a0 02a1 0001  .|.|.<.q.|......
-000000e0: 007c 0253 0029 034e da03 6e6d 65da 0269  .|.S.).N..nme..i
-000000f0: 6429 03da 0466 696e 64da 0474 6578 74da  d)...find..text.
-00000100: 0563 6c65 6172 2906 5a07 616c 6c5f 786d  .clear).Z.all_xm
-00000110: 6c72 0400 0000 5a09 6e65 775f 7461 626c  lr....Z.new_tabl
-00000120: 655a 0b6b 6579 5f74 6f5f 6669 6e64 da04  eZ.key_to_find..
-00000130: 6974 656d 5a07 6974 656d 5f69 64a9 0072  itemZ.item_id..r
-00000140: 0b00 0000 fa76 2f55 7365 7273 2f6d 696b  .....v/Users/mik
-00000150: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
-00000160: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
-00000170: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
-00000180: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
-00000190: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
-000001a0: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
-000001b0: 632f 7461 736b 6572 642e 7079 da11 6d6f  c/taskerd.py..mo
-000001c0: 7665 5f78 6d6c 5f74 6f5f 7461 626c 6516  ve_xml_to_table.
-000001d0: 0000 0073 0e00 0000 0401 0c01 0801 0c01  ...s............
-000001e0: 0a01 0801 0401 720d 0000 0063 0100 0000  ......r....c....
-000001f0: 0000 0000 0000 0000 0d00 0000 0800 0000  ................
-00000200: 4300 0000 73ce 0000 0074 00a0 0164 01a1  C...s....t...d..
-00000210: 0101 007a 0674 027c 0083 017d 0157 006e  ...z.t.|...}.W.n
-00000220: 1d04 0074 036a 046a 0579 2801 0001 0001  ...t.j.j.y(.....
-00000230: 0064 027c 009b 009d 027d 0274 067c 0283  .d.|.....}.t.|..
-00000240: 0101 0074 00a0 077c 02a1 0101 0074 0864  ...t...|.....t.d
-00000250: 0383 0101 0059 006e 0177 007c 01a0 09a1  .....Y.n.w.|....
-00000260: 007d 037c 03a0 0a64 04a1 017d 047c 03a0  .}.|...d...}.|..
-00000270: 0a64 05a1 017d 057c 03a0 0a64 06a1 017d  .d...}.|...d...}
-00000280: 067c 03a0 0a64 07a1 017d 077c 03a0 0a64  .|...d...}.|...d
-00000290: 08a1 017d 0874 0b7c 0664 0983 027d 0974  ...}.t.|.d...}.t
-000002a0: 0b7c 0864 0983 027d 0a74 0b7c 0764 0a83  .|.d...}.t.|.d..
-000002b0: 027d 0b7c 057c 097c 0b7c 0a7c 0464 0b9c  .}.|.|.|.|.|.d..
-000002c0: 057d 0c74 00a0 0164 0ca1 0101 007c 017c  .}.t...d.....|.|
-000002d0: 037c 0c66 0353 0029 0d4e da05 656e 7472  .|.f.S.).N..entr
-000002e0: 797a 0e45 7272 6f72 2070 6172 7369 6e67  yz.Error parsing
-000002f0: 20e9 0100 0000 5a07 5365 7474 696e 67da   .....Z.Setting.
-00000300: 0750 726f 6a65 6374 da07 5072 6f66 696c  .Project..Profil
-00000310: 65da 0553 6365 6e65 da04 5461 736b 4654  e..Scene..TaskFT
-00000320: 2905 da0c 616c 6c5f 7072 6f6a 6563 7473  )...all_projects
-00000330: da0c 616c 6c5f 7072 6f66 696c 6573 da0a  ..all_profiles..
-00000340: 616c 6c5f 7363 656e 6573 da09 616c 6c5f  all_scenes..all_
-00000350: 7461 736b 73da 0c61 6c6c 5f73 6572 7669  tasks..all_servi
-00000360: 6365 73da 0465 7869 7429 0c72 0300 0000  ces..exit).r....
-00000370: da04 696e 666f 7202 0000 00da 0a64 6566  ..infor......def
-00000380: 7573 6564 786d 6cda 0b45 6c65 6d65 6e74  usedxml..Element
-00000390: 5472 6565 da0a 5061 7273 6545 7272 6f72  Tree..ParseError
-000003a0: da05 7072 696e 74da 0564 6562 7567 7219  ..print..debugr.
-000003b0: 0000 00da 0767 6574 726f 6f74 da07 6669  .....getroot..fi
-000003c0: 6e64 616c 6c72 0d00 0000 290d da08 6669  ndallr....)...fi
-000003d0: 6c65 6e61 6d65 da04 7472 6565 da09 6572  lename..tree..er
-000003e0: 726f 725f 6d73 67da 0472 6f6f 7472 1800  ror_msg..rootr..
-000003f0: 0000 7214 0000 005a 1161 6c6c 5f70 726f  ..r....Z.all_pro
-00000400: 6669 6c65 735f 6c69 7374 5a0f 616c 6c5f  files_listZ.all_
-00000410: 7363 656e 6573 5f6c 6973 745a 0e61 6c6c  scenes_listZ.all
-00000420: 5f74 6173 6b73 5f6c 6973 7472 1500 0000  _tasks_listr....
-00000430: 7217 0000 0072 1600 0000 da10 616c 6c5f  r....r......all_
-00000440: 7461 736b 6572 5f69 7465 6d73 720b 0000  tasker_itemsr...
-00000450: 0072 0b00 0000 720c 0000 00da 1067 6574  .r....r......get
-00000460: 5f74 6865 5f78 6d6c 5f64 6174 6123 0000  _the_xml_data#..
-00000470: 0073 3400 0000 0a01 0202 0c01 1001 0a01  .s4.............
-00000480: 0801 0a01 0c01 02fc 0806 0a02 0a01 0a01  ................
-00000490: 0a01 0a01 0a03 0a01 0a01 0204 0201 0201  ................
-000004a0: 0201 0201 06fb 0a07 0a01 7227 0000 0029  ..........r'...)
-000004b0: 0872 1b00 0000 da16 6465 6675 7365 6478  .r......defusedx
-000004c0: 6d6c 2e45 6c65 6d65 6e74 5472 6565 7202  ml.ElementTreer.
-000004d0: 0000 00da 166d 6170 7461 736b 6572 2e73  .....maptasker.s
-000004e0: 7263 2e73 7973 636f 6e73 7472 0300 0000  rc.sysconstr....
-000004f0: da04 626f 6f6c 720d 0000 0072 2700 0000  ..boolr....r'...
-00000500: 720b 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-00000510: 0c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000520: 0000 730a 0000 0008 010c 010c 0d0e 060c  ..s.............
-00000530: 0d                                       .
+00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6404 6c05 6d06 5a06 0100 6405 6507 6602  d.l.m.Z...d.e.f.
+00000060: 6406 6407 8404 5a08 6408 6409 8400 5a09  d.d...Z.d.d...Z.
+00000070: 6401 5300 290a e900 0000 004e 2901 da05  d.S.)......N)...
+00000080: 7061 7273 6529 01da 066c 6f67 6765 7229  parse)...logger)
+00000090: 01da 0d65 7272 6f72 5f68 616e 646c 6572  ...error_handler
+000000a0: da08 6973 5f73 6365 6e65 6302 0000 0000  ..is_scenec.....
+000000b0: 0000 0000 0000 0006 0000 0004 0000 0043  ...............C
+000000c0: 0000 0073 3a00 0000 6900 7d02 7c01 7206  ...s:...i.}.|.r.
+000000d0: 6401 6e01 6402 7d03 7c00 4400 5d0c 7d04  d.n.d.}.|.D.].}.
+000000e0: 7c04 a000 7c03 a101 6a01 7d05 7c04 7c02  |...|...j.}.|.|.
+000000f0: 7c05 3c00 710a 7c00 a002 a100 0100 7c02  |.<.q.|.......|.
+00000100: 5300 2903 4eda 036e 6d65 da02 6964 2903  S.).N..nme..id).
+00000110: da04 6669 6e64 da04 7465 7874 da05 636c  ..find..text..cl
+00000120: 6561 7229 065a 0761 6c6c 5f78 6d6c 7205  ear).Z.all_xmlr.
+00000130: 0000 005a 096e 6577 5f74 6162 6c65 5a0b  ...Z.new_tableZ.
+00000140: 6b65 795f 746f 5f66 696e 64da 0469 7465  key_to_find..ite
+00000150: 6d5a 0769 7465 6d5f 6964 a900 720c 0000  mZ.item_id..r...
+00000160: 00fa 762f 5573 6572 732f 6d69 6b72 7562  ..v/Users/mikrub
+00000170: 696e 2f4c 6962 7261 7279 2f43 6c6f 7564  in/Library/Cloud
+00000180: 5374 6f72 6167 652f 476f 6f67 6c65 4472  Storage/GoogleDr
+00000190: 6976 652d 6d69 6b72 7562 696e 4067 6d61  ive-mikrubin@gma
+000001a0: 696c 2e63 6f6d 2f4d 7920 4472 6976 652f  il.com/My Drive/
+000001b0: 5079 7468 6f6e 2f6d 6170 7461 736b 6572  Python/maptasker
+000001c0: 2f6d 6170 7461 736b 6572 2f73 7263 2f74  /maptasker/src/t
+000001d0: 6173 6b65 7264 2e70 79da 116d 6f76 655f  askerd.py..move_
+000001e0: 786d 6c5f 746f 5f74 6162 6c65 1700 0000  xml_to_table....
+000001f0: 730e 0000 0004 010c 0108 010c 010a 0108  s...............
+00000200: 0104 0172 0e00 0000 6301 0000 0000 0000  ...r....c.......
+00000210: 0000 0000 000c 0000 0008 0000 0043 0000  .............C..
+00000220: 0073 ba00 0000 7400 a001 6401 a101 0100  .s....t...d.....
+00000230: 7a06 7402 7c00 8301 7d01 5700 6e13 0400  z.t.|...}.W.n...
+00000240: 7403 6a04 6a05 791e 0100 0100 0100 7406  t.j.j.y.......t.
+00000250: 6402 7c00 9b00 9d02 6403 8302 0100 5900  d.|.....d.....Y.
+00000260: 6e01 7700 7c01 a007 a100 7d02 7c02 a008  n.w.|.....}.|...
+00000270: 6404 a101 7d03 7c02 a008 6405 a101 7d04  d...}.|...d...}.
+00000280: 7c02 a008 6406 a101 7d05 7c02 a008 6407  |...d...}.|...d.
+00000290: a101 7d06 7c02 a008 6408 a101 7d07 7409  ..}.|...d...}.t.
+000002a0: 7c05 6409 8302 7d08 7409 7c07 6409 8302  |.d...}.t.|.d...
+000002b0: 7d09 7409 7c06 640a 8302 7d0a 7c04 7c08  }.t.|.d...}.|.|.
+000002c0: 7c0a 7c09 7c03 640b 9c05 7d0b 7400 a001  |.|.|.d...}.t...
+000002d0: 640c a101 0100 7c01 7c02 7c0b 6603 5300  d.....|.|.|.f.S.
+000002e0: 290d 4eda 0565 6e74 7279 7a0e 4572 726f  ).N..entryz.Erro
+000002f0: 7220 7061 7273 696e 6720 e901 0000 005a  r parsing .....Z
+00000300: 0753 6574 7469 6e67 da07 5072 6f6a 6563  .Setting..Projec
+00000310: 74da 0750 726f 6669 6c65 da05 5363 656e  t..Profile..Scen
+00000320: 65da 0454 6173 6b46 5429 05da 0c61 6c6c  e..TaskFT)...all
+00000330: 5f70 726f 6a65 6374 73da 0c61 6c6c 5f70  _projects..all_p
+00000340: 726f 6669 6c65 73da 0a61 6c6c 5f73 6365  rofiles..all_sce
+00000350: 6e65 73da 0961 6c6c 5f74 6173 6b73 da0c  nes..all_tasks..
+00000360: 616c 6c5f 7365 7276 6963 6573 da04 6578  all_services..ex
+00000370: 6974 290a 7203 0000 00da 0469 6e66 6f72  it).r......infor
+00000380: 0200 0000 da0a 6465 6675 7365 6478 6d6c  ......defusedxml
+00000390: da0b 456c 656d 656e 7454 7265 65da 0a50  ..ElementTree..P
+000003a0: 6172 7365 4572 726f 7272 0400 0000 da07  arseErrorr......
+000003b0: 6765 7472 6f6f 74da 0766 696e 6461 6c6c  getroot..findall
+000003c0: 720e 0000 0029 0cda 0866 696c 656e 616d  r....)...filenam
+000003d0: 65da 0474 7265 65da 0472 6f6f 7472 1900  e..tree..rootr..
+000003e0: 0000 7215 0000 005a 1161 6c6c 5f70 726f  ..r....Z.all_pro
+000003f0: 6669 6c65 735f 6c69 7374 5a0f 616c 6c5f  files_listZ.all_
+00000400: 7363 656e 6573 5f6c 6973 745a 0e61 6c6c  scenes_listZ.all
+00000410: 5f74 6173 6b73 5f6c 6973 7472 1600 0000  _tasks_listr....
+00000420: 7218 0000 0072 1700 0000 da10 616c 6c5f  r....r......all_
+00000430: 7461 736b 6572 5f69 7465 6d73 720c 0000  tasker_itemsr...
+00000440: 0072 0c00 0000 720d 0000 00da 1067 6574  .r....r......get
+00000450: 5f74 6865 5f78 6d6c 5f64 6174 6124 0000  _the_xml_data$..
+00000460: 0073 2e00 0000 0a01 0202 0c01 1001 1401  .s..............
+00000470: 02ff 0803 0a02 0a01 0a01 0a01 0a01 0a03  ................
+00000480: 0a01 0a01 0204 0201 0201 0201 0201 06fb  ................
+00000490: 0a07 0a01 7225 0000 0029 0a72 1c00 0000  ....r%...).r....
+000004a0: da16 6465 6675 7365 6478 6d6c 2e45 6c65  ..defusedxml.Ele
+000004b0: 6d65 6e74 5472 6565 7202 0000 00da 166d  mentTreer......m
+000004c0: 6170 7461 736b 6572 2e73 7263 2e73 7973  aptasker.src.sys
+000004d0: 636f 6e73 7472 0300 0000 da13 6d61 7074  constr......mapt
+000004e0: 6173 6b65 722e 7372 632e 6572 726f 7272  asker.src.errorr
+000004f0: 0400 0000 da04 626f 6f6c 720e 0000 0072  ......boolr....r
+00000500: 2500 0000 720c 0000 0072 0c00 0000 720c  %...r....r....r.
+00000510: 0000 0072 0d00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000520: 653e 0100 0000 730c 0000 0008 010c 010c  e>....s.........
+00000530: 0d0c 010e 060c 0d                        .......
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/tasks.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/tasks.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 16 19:14:51 2023 UTC, .py size: 15369 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,501 +1,508 @@
-00000000: 6f0d 0d0a 0000 0000 2b49 3c64 093c 0000  o.......+I<d.<..
+00000000: 6f0d 0d0a 0000 0000 18b3 4a64 c23c 0000  o.........Jd.<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 001c 0000 0040 0000 0073 9e01 0000 6400  .....@...s....d.
+00000020: 001c 0000 0040 0000 0073 b601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 6d03  ..m.Z...d.d.l.m.
 00000050: 0200 0100 6d07 5a08 0100 6400 6402 6c09  ....m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6400 6403 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6404 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
 00000080: 6405 6c0f 6d10 5a10 0100 6400 6406 6c11  d.l.m.Z...d.d.l.
 00000090: 6d12 5a12 0100 6400 6407 6c11 6d13 5a13  m.Z...d.d.l.m.Z.
 000000a0: 0100 6400 6408 6c11 6d14 5a14 0100 6400  ..d.d.l.m.Z...d.
-000000b0: 6409 6c15 6d16 5a16 0100 640a 6501 6a17  d.l.m.Z...d.e.j.
-000000c0: 6a18 640b 6519 640c 6519 640d 651a 6608  j.d.e.d.e.d.e.f.
-000000d0: 640e 640f 8404 5a1b 6410 651c 6411 651a  d.d...Z.d.e.d.e.
-000000e0: 6412 651a 6413 651c 6414 6519 640d 651d  d.e.d.e.d.e.d.e.
-000000f0: 6501 6a17 6a18 651c 6602 1900 660c 6415  e.j.j.e.f...f.d.
-00000100: 6416 8404 5a1e 6410 651c 6417 651a 6418  d...Z.d.e.d.e.d.
-00000110: 6519 640d 651d 651c 6501 6a17 6602 1900  e.d.e.e.e.j.f...
-00000120: 6608 6419 641a 8404 5a1f 6410 651c 641b  f.d.d...Z.d.e.d.
-00000130: 6519 640d 6520 6606 641c 641d 8404 5a21  e.d.e f.d.d...Z!
-00000140: 641e 651c 641f 651a 6420 651c 6421 651c  d.e.d.e.d e.d!e.
-00000150: 6422 651c 6423 6519 6424 651a 6425 6501  d"e.d#e.d$e.d%e.
-00000160: 6a17 6a18 6426 651a 6427 6519 640b 6519  j.j.d&e.d'e.d.e.
-00000170: 6428 6519 640d 6401 661a 6429 642a 8404  d(e.d.d.f.d)d*..
-00000180: 5a22 641f 651a 641e 651c 6425 6501 6a17  Z"d.e.d.e.d%e.j.
-00000190: 6a18 6424 651a 6420 651c 6421 651c 6426  j.d$e.d e.d!e.d&
-000001a0: 651a 6422 651c 640b 6519 6428 6519 6427  e.d"e.d.e.d(e.d'
-000001b0: 6519 6423 6519 642b 6520 640d 6520 661c  e.d#e.d+e d.e f.
-000001c0: 642c 642d 8404 5a23 6401 5300 292e e900  d,d-..Z#d.S.)...
-000001d0: 0000 004e 2901 da0b 7461 675f 696e 5f74  ...N)...tag_in_t
-000001e0: 7970 6529 01da 0b67 6574 5f6b 6964 5f61  ype)...get_kid_a
-000001f0: 7070 2901 da0c 6765 745f 7072 696f 7269  pp)...get_priori
-00000200: 7479 2901 da07 6765 745f 6964 7329 01da  ty)...get_ids)..
-00000210: 1155 4e4b 4e4f 574e 5f54 4153 4b5f 4e41  .UNKNOWN_TASK_NA
-00000220: 4d45 2901 da0a 4e4f 5f50 524f 4a45 4354  ME)...NO_PROJECT
-00000230: 2901 da06 6c6f 6767 6572 2901 da0a 7368  )...logger)...sh
-00000240: 656c 6c5f 736f 7274 da0c 6375 7272 656e  ell_sort..curren
-00000250: 745f 7461 736b da08 636f 6c6f 726d 6170  t_task..colormap
-00000260: da09 7072 6f67 5f61 7267 73da 0672 6574  ..prog_args..ret
-00000270: 7572 6e63 0300 0000 0000 0000 0000 0000  urnc............
-00000280: 0c00 0000 0900 0000 4300 0000 7346 0100  ........C...sF..
-00000290: 0067 007d 037a 077c 00a0 0064 01a1 017d  .g.}.z.|...d...}
-000002a0: 0457 006e 1c04 0074 016a 0279 2501 0001  .W.n...t.j.y%...
-000002b0: 0001 0074 0364 027c 0083 0201 0064 037d  ...t.d.|.....d.}
-000002c0: 0574 037c 0583 0101 0074 04a0 057c 05a1  .t.|.....t...|..
-000002d0: 0101 0067 0006 0059 0053 0077 007c 0472  ...g...Y.S.w.|.r
-000002e0: a164 047d 0664 057d 0774 067c 0483 0164  .d.}.d.}.t.|...d
-000002f0: 056b 0472 3874 077c 0464 0664 0783 0301  .k.r8t.|.d.d....
-00000300: 007c 0444 005d 667d 087c 08a0 0864 08a1  .|.D.]f}.|...d..
-00000310: 017d 0974 09a0 0a7c 097c 0864 067c 0164  .}.t...|.|.d.|.d
-00000320: 097c 02a1 067d 0a74 04a0 0564 0a74 0b7c  .|...}.t...d.t.|
-00000330: 086a 0c64 0b19 0083 0117 0064 0c17 007c  .j.d.......d...|
-00000340: 096a 0d17 0064 0d17 007c 0a17 0064 0e17  .j...d...|...d..
-00000350: 0074 0b7c 086a 0c83 0117 00a1 0101 0064  .t.|.j.........d
-00000360: 0f7c 0a76 0073 7364 107c 0a76 0073 7364  .|.v.ssd.|.v.ssd
-00000370: 117c 0a76 0072 817c 0764 1238 007d 0774  .|.v.r.|.d.8.}.t
-00000380: 067c 0683 017d 0b7c 0664 137c 0b85 0219  .|...}.|.d.|....
-00000390: 007d 0674 09a0 0e7c 017c 037c 0a7c 097c  .}.t...|.|.|.|.|
-000003a0: 077c 06a1 0601 0064 147c 0a76 0073 9764  .|.....d.|.v.s.d
-000003b0: 107c 0a76 0073 9764 157c 0a76 0072 a07c  .|.v.s.d.|.v.r.|
-000003c0: 0764 1237 007d 077c 069b 0064 169d 027d  .d.7.}.|...d...}
-000003d0: 0671 3a7c 0353 0029 1761 1d01 0000 0a20  .q:|.S.).a..... 
-000003e0: 2020 2052 6574 7572 6e20 6120 6c69 7374     Return a list
-000003f0: 206f 6620 5461 736b 2773 2061 6374 696f   of Task's actio
-00000400: 6e73 2066 6f72 2074 6865 2067 6976 656e  ns for the given
-00000410: 2054 6173 6b0a 2020 2020 2020 2020 3a70   Task.        :p
-00000420: 6172 616d 2063 7572 7265 6e74 5f74 6173  aram current_tas
-00000430: 6b3a 2078 6d6c 2065 6c65 6d65 6e74 206f  k: xml element o
-00000440: 6620 7468 6520 5461 736b 2077 6520 6172  f the Task we ar
-00000450: 6520 6765 7474 696e 6720 6163 7469 6f6e  e getting action
-00000460: 7320 666f 720a 2020 2020 2020 2020 3a70  s for.        :p
-00000470: 6172 616d 2063 6f6c 6f72 6d61 703a 2063  aram colormap: c
-00000480: 6f6c 6f72 7320 746f 2075 7365 2069 6e20  olors to use in 
-00000490: 6f75 7470 7574 0a20 2020 2020 2020 203a  output.        :
-000004a0: 7061 7261 6d20 7072 6f67 5f61 7267 733a  param prog_args:
-000004b0: 2072 756e 7469 6d65 2061 7267 756d 656e   runtime argumen
-000004c0: 7473 0a20 2020 2020 2020 203a 7265 7475  ts.        :retu
-000004d0: 726e 3a20 6c69 7374 206f 6620 5461 736b  rn: list of Task
-000004e0: 2027 6163 7469 6f6e 2720 6f75 7470 7574   'action' output
-000004f0: 206c 696e 6573 0a20 2020 20da 0641 6374   lines.    ..Act
-00000500: 696f 6e7a 1674 6173 6b73 2e70 7920 6375  ionz.tasks.py cu
-00000510: 7272 656e 7420 5461 736b 3a7a 1945 7272  rrent Task:z.Err
-00000520: 6f72 3a20 4e6f 2061 6374 696f 6e20 666f  or: No action fo
-00000530: 756e 6421 2121 da00 7201 0000 0054 46da  und!!!..r....TF.
-00000540: 0463 6f64 65da 0174 7a08 5461 736b 2049  .code..tz.Task I
-00000550: 443a da02 7372 7a06 2043 6f64 653a 7a0b  D:..srz. Code:z.
-00000560: 2074 6173 6b5f 636f 6465 3a7a 0c41 6374   task_code:z.Act
-00000570: 696f 6e20 6174 7472 3a7a 073e 456e 6420  ion attr:z.>End 
-00000580: 4966 7a05 3e45 6c73 657a 083e 456e 6420  Ifz.>Elsez.>End 
-00000590: 466f 72e9 0100 0000 e918 0000 007a 033e  For..........z.>
-000005a0: 4966 7a04 3e46 6f72 7a18 266e 6273 703b  Ifz.>Forz.&nbsp;
-000005b0: 266e 6273 703b 266e 6273 703b 266e 6273  &nbsp;&nbsp;&nbs
-000005c0: 703b 290f da07 6669 6e64 616c 6cda 0a64  p;)...findall..d
-000005d0: 6566 7573 6564 786d 6cda 1344 6566 7573  efusedxml..Defus
-000005e0: 6564 586d 6c45 7863 6570 7469 6f6e da05  edXmlException..
-000005f0: 7072 696e 7472 0800 0000 da05 6465 6275  printr......debu
-00000600: 67da 036c 656e 7209 0000 00da 0466 696e  g..lenr......fin
-00000610: 64da 0f61 6374 696f 6e5f 6576 616c 7561  d..action_evalua
-00000620: 7465 da0f 6765 745f 6163 7469 6f6e 5f63  te..get_action_c
-00000630: 6f64 65da 0373 7472 da06 6174 7472 6962  ode..str..attrib
-00000640: da04 7465 7874 da0c 6275 696c 645f 6163  ..text..build_ac
-00000650: 7469 6f6e 290c 720a 0000 0072 0b00 0000  tion).r....r....
-00000660: 720c 0000 005a 0874 6173 6b6c 6973 745a  r....Z.tasklistZ
-00000670: 0c74 6173 6b5f 6163 7469 6f6e 73da 0965  .task_actions..e
-00000680: 7272 6f72 5f6d 7367 5a12 696e 6465 6e74  rror_msgZ.indent
-00000690: 6174 696f 6e5f 616d 6f75 6e74 5a0b 696e  ation_amountZ.in
-000006a0: 6465 6e74 6174 696f 6eda 0661 6374 696f  dentation..actio
-000006b0: 6eda 0563 6869 6c64 5a09 7461 736b 5f63  n..childZ.task_c
-000006c0: 6f64 655a 0d6c 656e 6774 685f 696e 6465  odeZ.length_inde
-000006d0: 6e74 a900 7225 0000 00fa 742f 5573 6572  nt..r%....t/User
-000006e0: 732f 6d69 6b72 7562 696e 2f4c 6962 7261  s/mikrubin/Libra
-000006f0: 7279 2f43 6c6f 7564 5374 6f72 6167 652f  ry/CloudStorage/
-00000700: 476f 6f67 6c65 4472 6976 652d 6d69 6b72  GoogleDrive-mikr
-00000710: 7562 696e 4067 6d61 696c 2e63 6f6d 2f4d  ubin@gmail.com/M
-00000720: 7920 4472 6976 652f 5079 7468 6f6e 2f6d  y Drive/Python/m
-00000730: 6170 7461 736b 6572 2f6d 6170 7461 736b  aptasker/maptask
-00000740: 6572 2f73 7263 2f74 6173 6b73 2e70 79da  er/src/tasks.py.
-00000750: 0b67 6574 5f61 6374 696f 6e73 2100 0000  .get_actions!...
-00000760: 7366 0000 0004 0a02 020e 010e 010a 0104  sf..............
-00000770: 0108 010a 0108 0102 fb04 0604 0104 010c  ................
-00000780: 030c 0108 020a 0104 020c 0104 ff04 0302  ................
-00000790: 010c 0102 ff02 0202 fe04 0302 fd02 0402  ................
-000007a0: fc02 0502 fb02 0602 fa08 0702 f904 ff08  ................
-000007b0: 0c08 0108 0108 0208 010c 0104 010c 0104  ................
-000007c0: ff18 0408 020a 0102 8004 0272 2700 0000  ...........r'...
-000007d0: da0b 7468 655f 7461 736b 5f69 64da 1a74  ..the_task_id..t
-000007e0: 6173 6b73 5f74 6861 745f 6861 7665 5f62  asks_that_have_b
-000007f0: 6565 6e5f 666f 756e 64da 1174 6173 6b5f  een_found..task_
-00000800: 6f75 7470 7574 5f6c 696e 6573 da09 7461  output_lines..ta
-00000810: 736b 5f74 7970 65da 0961 6c6c 5f74 6173  sk_type..all_tas
-00000820: 6b73 6305 0000 0000 0000 0000 0000 0009  ksc.............
-00000830: 0000 000a 0000 0043 0000 0073 fa00 0000  .......C...s....
-00000840: 7c00 a000 a100 7275 7c04 7c00 1900 7d05  |.....ru|.|...}.
-00000850: 7c01 a001 7c00 a101 0100 6401 7c00 9b00  |...|.....d.|...
-00000860: 9d02 7d06 7a29 7c05 a002 6402 a101 6a03  ..}.z)|...d...j.
-00000870: 7d07 7c03 6403 6b02 7228 7c02 a001 7c07  }.|.d.k.r(|...|.
-00000880: 9b00 6404 7c06 9b00 9d03 a101 0100 6e0f  ..d.|.........n.
-00000890: 7c02 a001 7c07 9b00 6405 7c06 9b00 9d03  |...|...d.|.....
-000008a0: a101 0100 5700 7c05 7c07 6602 5300 5700  ....W.|.|.f.S.W.
-000008b0: 7c05 7c07 6602 5300 0400 7404 7974 0100  |.|.f.S...t.yt..
-000008c0: 7d08 0100 7a2d 7405 7d07 7c03 6403 6b02  }...z-t.}.|.d.k.
-000008d0: 7254 7c02 a001 7405 9b00 6404 7c06 9b00  rT|...t...d.|...
-000008e0: 9d03 a101 0100 6e13 7c02 a001 7405 9b00  ......n.|...t...
-000008f0: 6405 7c06 9b00 9d03 a101 0100 5700 5900  d.|.........W.Y.
-00000900: 6406 7d08 7e08 7c05 7c07 6602 5300 5700  d.}.~.|.|.f.S.W.
-00000910: 5900 6406 7d08 7e08 7c05 7c07 6602 5300  Y.d.}.~.|.|.f.S.
-00000920: 6406 7d08 7e08 7701 7700 6406 7d05 6407  d.}.~.w.w.d.}.d.
-00000930: 7d07 7c05 7c07 6602 5300 2908 6178 0100  }.|.|.f.S.).ax..
-00000940: 000a 2020 2020 4765 7420 7468 6520 6e61  ..    Get the na
-00000950: 6d65 206f 6620 7468 6520 7461 736b 2067  me of the task g
-00000960: 6976 656e 2074 6865 2054 6173 6b20 4944  iven the Task ID
-00000970: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000980: 7468 655f 7461 736b 5f69 643a 2074 6865  the_task_id: the
-00000990: 2054 6173 6b27 7320 4944 2028 652e 672e   Task's ID (e.g.
-000009a0: 2027 3437 2729 0a20 2020 2020 2020 203a   '47').        :
-000009b0: 7061 7261 6d20 7461 736b 735f 7468 6174  param tasks_that
-000009c0: 5f68 6176 655f 6265 656e 5f66 6f75 6e64  _have_been_found
-000009d0: 3a20 6c69 7374 206f 6620 5461 736b 7320  : list of Tasks 
-000009e0: 666f 756e 6420 736f 2066 6172 0a20 2020  found so far.   
-000009f0: 2020 2020 203a 7061 7261 6d20 7461 736b       :param task
-00000a00: 5f6f 7574 7075 745f 6c69 6e65 733a 206c  _output_lines: l
-00000a10: 6973 7420 6f66 2054 6173 6b73 0a20 2020  ist of Tasks.   
-00000a20: 2020 2020 203a 7061 7261 6d20 7461 736b       :param task
-00000a30: 5f74 7970 653a 2054 7970 6520 6f66 2054  _type: Type of T
-00000a40: 6173 6b20 2845 6e74 7279 2c20 4578 6974  ask (Entry, Exit
-00000a50: 2c20 5363 656e 6529 0a20 2020 2020 2020  , Scene).       
-00000a60: 203a 7061 7261 6d20 616c 6c5f 7461 736b   :param all_task
-00000a70: 733a 2061 6c6c 2054 6173 6b73 2069 6e20  s: all Tasks in 
-00000a80: 786d 6c0a 2020 2020 2020 2020 3a72 6574  xml.        :ret
-00000a90: 7572 6e3a 2054 6173 6b27 7320 786d 6c20  urn: Task's xml 
-00000aa0: 656c 656d 656e 742c 2054 6173 6b27 7320  element, Task's 
-00000ab0: 6e61 6d65 0a20 2020 207a 1526 6e62 7370  name.    z.&nbsp
-00000ac0: 3b26 6e62 7370 3b54 6173 6b20 4944 3a20  ;&nbsp;Task ID: 
-00000ad0: da03 6e6d 655a 0445 7869 747a 2526 6e62  ..nmeZ.Exitz%&nb
-00000ae0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
-00000af0: 6e62 7370 3b3c 3c3c 2045 7869 7420 5461  nbsp;<<< Exit Ta
-00000b00: 736b 7a26 266e 6273 703b 266e 6273 703b  skz&&nbsp;&nbsp;
-00000b10: 266e 6273 703b 266e 6273 703b 3c3c 3c20  &nbsp;&nbsp;<<< 
-00000b20: 456e 7472 7920 5461 736b 4e72 0f00 0000  Entry TaskNr....
-00000b30: 2906 da07 6973 6469 6769 74da 0661 7070  )...isdigit..app
-00000b40: 656e 6472 1b00 0000 7220 0000 00da 0945  endr....r .....E
-00000b50: 7863 6570 7469 6f6e 7206 0000 0029 0972  xceptionr....).r
-00000b60: 2800 0000 7229 0000 0072 2a00 0000 722b  (...r)...r*...r+
-00000b70: 0000 0072 2c00 0000 da04 7461 736b da05  ...r,.....task..
-00000b80: 6578 7472 615a 0974 6173 6b5f 6e61 6d65  extraZ.task_name
-00000b90: da01 6572 2500 0000 7225 0000 0072 2600  ..er%...r%...r&.
-00000ba0: 0000 da0d 6765 745f 7461 736b 5f6e 616d  ....get_task_nam
-00000bb0: 6566 0000 0073 4200 0000 0810 0801 0a01  ef...sB.........
-00000bc0: 0a01 0201 0c01 0801 0401 0c01 06ff 0405  ................
-00000bd0: 0c01 06ff 0812 02e9 0817 0ef1 0401 0801  ................
-00000be0: 0401 0c01 06ff 0405 0c01 0eff 0807 0af4  ................
-00000bf0: 080c 0880 02f1 040c 0401 0802 7234 0000  ............r4..
-00000c00: 00da 1670 726f 6a65 6374 735f 7769 7468  ...projects_with
-00000c10: 5f6e 6f5f 7461 736b 73da 0c61 6c6c 5f70  _no_tasks..all_p
-00000c20: 726f 6a65 6374 7363 0300 0000 0000 0000  rojectsc........
-00000c30: 0000 0000 0600 0000 0900 0000 4300 0000  ............C...
-00000c40: 7356 0000 0074 007d 0364 017d 047c 0264  sV...t.}.d.}.|.d
-00000c50: 0175 0172 277c 0244 005d 1c7d 047c 04a0  .u.r'|.D.].}.|..
-00000c60: 0164 02a1 016a 027d 0374 0364 0369 0069  .d...j.}.t.d.i.i
-00000c70: 0067 007c 047c 037c 0183 077d 057c 007c  .g.|.|.|...}.|.|
-00000c80: 0576 0072 267c 037c 0466 0202 0001 0053  .v.r&|.|.f.....S
-00000c90: 0071 0a7c 037c 0466 0253 0029 0461 4b01  .q.|.|.f.S.).aK.
-00000ca0: 0000 0a20 2020 2046 696e 6420 7468 6520  ...    Find the 
-00000cb0: 5072 6f6a 6563 7420 6265 6c6f 6e67 696e  Project belongin
-00000cc0: 6720 746f 2074 6865 2054 6173 6b20 6964  g to the Task id
-00000cd0: 2070 6173 7365 6420 696e 0a20 2020 2020   passed in.     
-00000ce0: 2020 203a 7061 7261 6d20 7468 655f 7461     :param the_ta
-00000cf0: 736b 5f69 643a 2074 6865 2049 4420 6f66  sk_id: the ID of
-00000d00: 2074 6865 2054 6173 6b0a 2020 2020 2020   the Task.      
-00000d10: 2020 3a70 6172 616d 2070 726f 6a65 6374    :param project
-00000d20: 735f 7769 7468 5f6e 6f5f 7461 736b 733a  s_with_no_tasks:
-00000d30: 206c 6973 7420 6f66 2050 726f 6a65 6374   list of Project
-00000d40: 7320 7468 6174 2064 6f20 6e6f 7420 6861  s that do not ha
-00000d50: 7665 2061 6e79 2054 6173 6b73 0a20 2020  ve any Tasks.   
-00000d60: 2020 2020 203a 7061 7261 6d20 616c 6c5f       :param all_
-00000d70: 7072 6f6a 6563 7473 3a20 616c 6c20 5461  projects: all Ta
-00000d80: 736b 6572 2050 726f 6a65 6374 730a 2020  sker Projects.  
-00000d90: 2020 2020 2020 3a72 6574 7572 6e3a 206e        :return: n
-00000da0: 616d 6520 6f66 2074 6865 2050 726f 6a65  ame of the Proje
-00000db0: 6374 2074 6861 7420 6265 6c6f 6e67 7320  ct that belongs 
-00000dc0: 746f 2074 6869 7320 7461 736b 2061 6e64  to this task and
-00000dd0: 2074 6865 2050 726f 6a65 6374 2078 6d6c   the Project xml
-00000de0: 2065 6c65 6d65 6e74 0a20 2020 204e da04   element.    N..
-00000df0: 6e61 6d65 4629 0472 0700 0000 721b 0000  nameF).r....r...
-00000e00: 0072 2000 0000 7205 0000 0029 0672 2800  .r ...r....).r(.
-00000e10: 0000 7235 0000 0072 3600 0000 5a09 7072  ..r5...r6...Z.pr
-00000e20: 6f6a 5f6e 616d 65da 0770 726f 6a65 6374  oj_name..project
-00000e30: da08 7461 736b 5f69 6473 7225 0000 0072  ..task_idsr%...r
-00000e40: 2500 0000 7226 0000 00da 1967 6574 5f70  %...r&.....get_p
-00000e50: 726f 6a65 6374 5f66 6f72 5f73 6f6c 6f5f  roject_for_solo_
-00000e60: 7461 736b 9a00 0000 7318 0000 0004 0a04  task....s.......
-00000e70: 0108 0108 020c 0102 010e 0104 ff08 030c  ................
-00000e80: 0102 ff08 0272 3a00 0000 da0a 616c 6c5f  .....r:.....all_
-00000e90: 7363 656e 6573 6302 0000 0000 0000 0000  scenesc.........
-00000ea0: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
-00000eb0: 6000 0000 7c01 a000 a100 4400 5d29 7d02  `...|.....D.])}.
-00000ec0: 7c02 4400 5d24 7d03 7401 7c03 6a02 6401  |.D.]$}.t.|.j.d.
-00000ed0: 8302 722c 7c03 4400 5d19 7d04 7401 7c04  ..r,|.D.].}.t.|.
-00000ee0: 6a02 6402 8302 7224 7c00 7c04 6a03 6b02  j.d...r$|.|.j.k.
-00000ef0: 7224 0100 0100 0100 6401 5300 7c03 6a02  r$......d.S.|.j.
-00000f00: 6403 6b02 722b 0100 6e01 7112 7108 7104  d.k.r+..n.q.q.q.
-00000f10: 6402 5300 2904 6118 0100 000a 2020 2020  d.S.).a.....    
-00000f20: 4964 656e 7469 6679 2077 6865 7468 6572  Identify whether
-00000f30: 2074 6865 2054 6173 6b20 7061 7373 6564   the Task passed
-00000f40: 2069 6e20 6973 2070 6172 7420 6f66 2061   in is part of a
-00000f50: 2053 6365 6e65 3a20 5472 7565 203d 2079   Scene: True = y
-00000f60: 6573 2c20 4661 6c73 6520 3d20 6e6f 0a20  es, False = no. 
-00000f70: 2020 2020 2020 203a 7061 7261 6d20 7468         :param th
-00000f80: 655f 7461 736b 5f69 643a 2074 6865 2069  e_task_id: the i
-00000f90: 6420 6f66 2074 6865 2054 6173 6b20 746f  d of the Task to
-00000fa0: 2063 6865 636b 2061 6761 696e 7374 0a20   check against. 
-00000fb0: 2020 2020 2020 203a 7061 7261 6d20 616c         :param al
-00000fc0: 6c5f 7363 656e 6573 3a20 616c 6c20 5363  l_scenes: all Sc
-00000fd0: 656e 6573 2069 6e20 5461 736b 6572 2063  enes in Tasker c
-00000fe0: 6f6e 6669 6775 7261 7469 6f6e 0a20 2020  onfiguration.   
-00000ff0: 2020 2020 203a 7265 7475 726e 3a20 5472       :return: Tr
-00001000: 7565 2069 6620 5461 736b 2069 7320 7061  ue if Task is pa
-00001010: 7274 206f 6620 6120 5363 656e 652c 2046  rt of a Scene, F
-00001020: 616c 7365 206f 7468 6572 7769 7365 0a20  alse otherwise. 
-00001030: 2020 2054 46da 0353 7472 2904 da06 7661     TF..Str)...va
-00001040: 6c75 6573 7202 0000 00da 0374 6167 7220  luesr......tagr 
-00001050: 0000 0029 0572 2800 0000 723b 0000 00da  ...).r(...r;....
-00001060: 0576 616c 7565 7224 0000 005a 0873 7562  .valuer$...Z.sub
-00001070: 6368 696c 6472 2500 0000 7225 0000 0072  childr%...r%...r
-00001080: 2600 0000 da0d 7461 736b 5f69 6e5f 7363  &.....task_in_sc
-00001090: 656e 65b5 0000 0073 1c00 0000 0c08 0801  ene....s........
-000010a0: 0c01 0801 0a03 02ff 0a02 0a02 0a01 0401  ................
-000010b0: 0202 0280 02f4 040d 7240 0000 00da 0d6f  ........r@.....o
-000010c0: 7572 5f74 6173 6b5f 6e61 6d65 da0b 6f75  ur_task_name..ou
-000010d0: 7470 7574 5f6c 6973 74da 0c70 726f 6a65  tput_list..proje
-000010e0: 6374 5f6e 616d 65da 0c70 726f 6669 6c65  ct_name..profile
-000010f0: 5f6e 616d 65da 0768 6561 6469 6e67 da0b  _name..heading..
-00001100: 666f 756e 645f 6974 656d 73da 0974 6173  found_items..tas
-00001110: 6b5f 6c69 7374 da10 6f75 725f 7461 736b  k_list..our_task
-00001120: 5f65 6c65 6d65 6e74 da13 6c69 7374 5f6f  _element..list_o
-00001130: 665f 666f 756e 645f 7461 736b 73da 1061  f_found_tasks..a
-00001140: 6c6c 5f74 6173 6b65 725f 6974 656d 73da  ll_tasker_items.
-00001150: 0c70 726f 6772 616d 5f61 7267 7363 0c00  .program_argsc..
-00001160: 0000 0000 0000 0000 0000 1100 0000 0a00  ................
-00001170: 0000 4300 0000 730a 0100 0064 0164 026c  ..C...s....d.d.l
-00001180: 006d 017d 0c01 0074 02a0 0364 037c 0b64  .m.}...t...d.|.d
-00001190: 0419 009b 0064 057c 009b 009d 04a1 0101  .....d.|........
-000011a0: 007c 0b64 0419 007c 006b 0272 5664 067c  .|.d...|.k.rVd.|
-000011b0: 0564 073c 0074 04a0 0564 067c 017c 027c  .d.<.t...d.|.|.|
-000011c0: 037c 047c 0a7c 0ba1 0701 0067 007d 0d74  .|.|.|.....g.}.t
-000011d0: 067c 0683 0164 086b 0472 4774 067c 0083  .|...d.k.rGt.|..
-000011e0: 017d 0e7c 0644 005d 0f7d 0f7c 007c 0f64  .}.|.D.].}.|.|.d
-000011f0: 097c 0e85 0219 006b 0272 457c 0f67 017d  .|.....k.rE|.g.}
-00001200: 0d01 006e 0171 366e 027c 067d 0d7c 0c64  ...n.q6n.|.}.|.d
-00001210: 0a7c 017c 0d7c 077c 087c 0b7c 0a7c 0983  .|.|.|.|.|.|.|..
-00001220: 0801 0064 0953 0074 067c 0683 0164 086b  ...d.S.t.|...d.k
-00001230: 0472 817c 0644 005d 247d 107c 0b64 0419  .r.|.D.]$}.|.d..
-00001240: 007c 1076 0072 8074 04a0 077c 0a7c 0b7c  .|.v.r.t...|.|.|
-00001250: 0164 0864 0ba1 0501 007c 1067 017d 067c  .d.d.....|.g.}.|
-00001260: 0c64 0a7c 017c 067c 077c 087c 0b7c 0a7c  .d.|.|.|.|.|.|.|
-00001270: 0983 0801 0001 0064 0953 0071 5e64 0953  .......d.S.q^d.S
-00001280: 0064 0953 0029 0c61 db02 0000 0a20 2020  .d.S.).a.....   
-00001290: 2050 726f 6365 7373 2061 2073 696e 676c   Process a singl
-000012a0: 6520 5461 736b 206f 6e6c 790a 2020 2020  e Task only.    
-000012b0: 2020 2020 3a70 6172 616d 206f 7572 5f74      :param our_t
-000012c0: 6173 6b5f 6e61 6d65 3a20 6e61 6d65 206f  ask_name: name o
-000012d0: 6620 7468 6520 5461 736b 2074 6f20 7072  f the Task to pr
-000012e0: 6f63 6573 730a 2020 2020 2020 2020 3a70  ocess.        :p
-000012f0: 6172 616d 206f 7574 7075 745f 6c69 7374  aram output_list
-00001300: 3a20 7768 6572 6520 7468 6520 6f75 7470  : where the outp
-00001310: 7574 206c 696e 6520 676f 6573 2066 6f72  ut line goes for
-00001320: 2054 6173 6b0a 2020 2020 2020 2020 3a70   Task.        :p
-00001330: 6172 616d 2070 726f 6a65 6374 5f6e 616d  aram project_nam
-00001340: 653a 206e 616d 6520 6f66 2074 6865 2050  e: name of the P
-00001350: 726f 6a65 6374 2054 6173 6b20 6265 6c6f  roject Task belo
-00001360: 6e67 7320 746f 0a20 2020 2020 2020 203a  ngs to.        :
-00001370: 7061 7261 6d20 7072 6f66 696c 655f 6e61  param profile_na
-00001380: 6d65 3a20 6e61 6d65 206f 6620 7468 6520  me: name of the 
-00001390: 5072 6f66 696c 6520 7468 6520 5461 736b  Profile the Task
-000013a0: 2062 656c 6f6e 6773 2074 6f0a 2020 2020   belongs to.    
-000013b0: 2020 2020 3a70 6172 616d 2068 6561 6469      :param headi
-000013c0: 6e67 3a20 7468 6520 6865 6164 696e 672c  ng: the heading,
-000013d0: 2069 6620 616e 790a 2020 2020 2020 2020   if any.        
-000013e0: 3a70 6172 616d 2066 6f75 6e64 5f69 7465  :param found_ite
-000013f0: 6d73 3a20 7369 6e67 6c65 206e 616d 6520  ms: single name 
-00001400: 666f 7220 5072 6f6a 6563 742f 5072 6f66  for Project/Prof
-00001410: 696c 652f 5461 736b 0a20 2020 2020 2020  ile/Task.       
-00001420: 203a 7061 7261 6d20 7461 736b 5f6c 6973   :param task_lis
-00001430: 743a 206c 6973 7420 6f66 2054 6173 6b73  t: list of Tasks
-00001440: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001450: 6f75 725f 7461 736b 5f65 6c65 6d65 6e74  our_task_element
-00001460: 3a20 7468 6520 786d 6c20 656c 656d 656e  : the xml elemen
-00001470: 7420 666f 7220 7468 6973 2054 6173 6b0a  t for this Task.
-00001480: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
-00001490: 6973 745f 6f66 5f66 6f75 6e64 5f74 6173  ist_of_found_tas
-000014a0: 6b73 3a20 616c 6c20 5461 736b 7320 7072  ks: all Tasks pr
-000014b0: 6f63 6573 7365 6420 736f 2066 6172 0a20  ocessed so far. 
-000014c0: 2020 2020 2020 203a 7061 7261 6d20 616c         :param al
-000014d0: 6c5f 7461 736b 6572 5f69 7465 6d73 3a20  l_tasker_items: 
-000014e0: 616c 6c20 5072 6f6a 6563 7473 2f50 726f  all Projects/Pro
-000014f0: 6669 6c65 732f 5461 736b 732f 5363 656e  files/Tasks/Scen
-00001500: 6573 0a20 2020 2020 2020 203a 7061 7261  es.        :para
-00001510: 6d20 636f 6c6f 726d 6170 3a20 636f 6c6f  m colormap: colo
-00001520: 7273 2074 6f20 7573 6520 696e 206f 7574  rs to use in out
-00001530: 7075 740a 2020 2020 2020 2020 3a70 6172  put.        :par
-00001540: 616d 2070 726f 6772 616d 5f61 7267 733a  am program_args:
-00001550: 2072 756e 7469 6d65 2061 7267 756d 656e   runtime argumen
-00001560: 7473 0a20 2020 2072 0100 0000 a901 da0c  ts.    r........
-00001570: 7072 6f63 6573 735f 6c69 7374 7a17 7461  process_listz.ta
-00001580: 736b 7320 7369 6e67 6c65 2074 6173 6b20  sks single task 
-00001590: 6e61 6d65 3ada 1073 696e 676c 655f 7461  name:..single_ta
-000015a0: 736b 5f6e 616d 657a 0f20 6f75 7220 5461  sk_namez. our Ta
-000015b0: 736b 206e 616d 653a 54da 1173 696e 676c  sk name:T..singl
-000015c0: 655f 7461 736b 5f66 6f75 6e64 7213 0000  e_task_foundr...
-000015d0: 004e fa05 5461 736b 3a72 0f00 0000 2908  .N..Task:r....).
-000015e0: da16 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
-000015f0: 7072 6f63 6c69 7374 724d 0000 0072 0800  proclistrM...r..
-00001600: 0000 7219 0000 00da 0c62 7569 6c64 5f6f  ..r......build_o
-00001610: 7574 7075 74da 1272 6566 7265 7368 5f6f  utput..refresh_o
-00001620: 7572 5f6f 7574 7075 7472 1a00 0000 da09  ur_outputr......
-00001630: 6d79 5f6f 7574 7075 7429 1172 4100 0000  my_output).rA...
-00001640: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
-00001650: 4500 0000 7246 0000 0072 4700 0000 7248  E...rF...rG...rH
-00001660: 0000 0072 4900 0000 724a 0000 0072 0b00  ...rI...rJ...r..
-00001670: 0000 724b 0000 0072 4d00 0000 5a13 7465  ..rK...rM...Z.te
-00001680: 6d70 6f72 6172 795f 7461 736b 5f6c 6973  mporary_task_lis
-00001690: 745a 1474 6865 5f74 6173 6b5f 6e61 6d65  tZ.the_task_name
-000016a0: 5f6c 656e 6774 68da 0469 7465 6d5a 0974  _length..itemZ.t
-000016b0: 6173 6b5f 6974 656d 7225 0000 0072 2500  ask_itemr%...r%.
-000016c0: 0000 7226 0000 00da 0e64 6f5f 7369 6e67  ..r&.....do_sing
-000016d0: 6c65 5f74 6173 6bd1 0000 0073 7400 0000  le_task....st...
-000016e0: 0c1e 0402 0c01 0201 04ff 04ff 0c04 0802  ................
-000016f0: 0403 0201 0201 0201 0201 0201 0201 0201  ................
-00001700: 04f9 040b 0c01 0801 0801 1001 0601 0401  ................
-00001710: 02fe 0280 0404 0202 0201 0201 0201 0201  ................
-00001720: 0201 0201 0201 0201 08f8 0c0b 0802 0c01  ................
-00001730: 0401 0a01 04ff 0603 0201 0201 0201 0201  ................
-00001740: 0201 0201 0201 0201 0201 04f8 060d 02ee  ................
-00001750: 04fd 0402 7256 0000 00da 0864 6f5f 6578  ....rV.....do_ex
-00001760: 7472 6163 0d00 0000 0000 0000 0000 0000  trac............
-00001770: 1000 0000 0d00 0000 4300 0000 73d6 0000  ........C...s...
-00001780: 0064 0164 026c 006d 017d 0d01 007c 0c72  .d.d.l.m.}...|.r
-00001790: 317c 0964 0319 0064 046b 0272 3174 027c  1|.d...d.k.r1t.|
-000017a0: 0283 0104 007d 0e72 1f7c 0364 0119 009b  .....}.r.|.d....
-000017b0: 0064 057c 0e9b 009d 037c 0364 013c 0074  .d.|.....|.d.<.t
-000017c0: 037c 0264 0683 0204 007d 0f72 317c 0364  .|.d.....}.r1|.d
-000017d0: 0119 009b 0064 057c 0f9b 009d 037c 0364  .....d.|.....|.d
-000017e0: 013c 007c 0164 076b 0372 4a7c 0964 0819  .<.|.d.k.rJ|.d..
-000017f0: 0072 4a74 047c 017c 007c 047c 057c 077c  .rJt.|.|.|.|.|.|
-00001800: 0b7c 037c 027c 067c 0a7c 087c 0983 0c01  .|.|.|.|.|.|....
-00001810: 0064 0953 007c 0372 6974 05a0 067c 087c  .d.S.|.rit...|.|
-00001820: 097c 0064 0a64 07a1 0501 007c 0d64 0b7c  .|.d.d.....|.d.|
-00001830: 007c 037c 027c 067c 097c 087c 0a83 0801  .|.|.|.|.|.|....
-00001840: 0074 05a0 067c 087c 097c 0064 0464 07a1  .t...|.|.|.d.d..
-00001850: 0501 0064 0653 0029 0c61 5c03 0000 0a20  ...d.S.).a\.... 
-00001860: 2020 2057 6520 6861 7665 2061 2073 696e     We have a sin
-00001870: 676c 6520 5461 736b 206f 7220 6120 6c69  gle Task or a li
-00001880: 7374 206f 6620 5461 736b 732e 2020 4f75  st of Tasks.  Ou
-00001890: 7470 7574 2069 742f 7468 656d 2e0a 2020  tput it/them..  
-000018a0: 2020 2020 2020 3a70 6172 616d 206f 7574        :param out
-000018b0: 7075 745f 6c69 7374 3a20 6c69 7374 206f  put_list: list o
-000018c0: 6620 6f75 7470 7574 206c 696e 6573 2067  f output lines g
-000018d0: 656e 6572 6174 6564 2074 6875 7320 6661  enerated thus fa
-000018e0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
-000018f0: 206f 7572 5f74 6173 6b5f 6e61 6d65 3a20   our_task_name: 
-00001900: 6e61 6d65 206f 6620 5461 736b 0a20 2020  name of Task.   
-00001910: 2020 2020 203a 7061 7261 6d20 6f75 725f       :param our_
-00001920: 7461 736b 5f65 6c65 6d65 6e74 3a20 5461  task_element: Ta
-00001930: 736b 2078 6d6c 2065 6c65 6d65 6e74 0a20  sk xml element. 
-00001940: 2020 2020 2020 203a 7061 7261 6d20 7461         :param ta
-00001950: 736b 5f6c 6973 743a 2054 6173 6b20 6c69  sk_list: Task li
-00001960: 7374 0a20 2020 2020 2020 203a 7061 7261  st.        :para
-00001970: 6d20 7072 6f6a 6563 745f 6e61 6d65 3a20  m project_name: 
-00001980: 6e61 6d65 206f 6620 6375 7272 656e 7420  name of current 
-00001990: 5072 6f6a 6563 740a 2020 2020 2020 2020  Project.        
-000019a0: 3a70 6172 616d 2070 726f 6669 6c65 5f6e  :param profile_n
-000019b0: 616d 653a 206e 616d 6520 6f66 2063 7572  ame: name of cur
-000019c0: 7265 6e74 2050 726f 6669 6c65 0a20 2020  rent Profile.   
-000019d0: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
-000019e0: 5f6f 665f 666f 756e 645f 7461 736b 733a  _of_found_tasks:
-000019f0: 206c 6973 7420 6f66 2054 6173 6b73 2066   list of Tasks f
-00001a00: 6f75 6e64 2073 6f20 6661 720a 2020 2020  ound so far.    
-00001a10: 2020 2020 3a70 6172 616d 2068 6561 6469      :param headi
-00001a20: 6e67 3a20 6375 7272 656e 7420 6865 6164  ng: current head
-00001a30: 696e 670a 2020 2020 2020 2020 3a70 6172  ing.        :par
-00001a40: 616d 2063 6f6c 6f72 6d61 703a 2063 6f6c  am colormap: col
-00001a50: 6f72 7320 746f 2075 7365 2069 6e20 6f75  ors to use in ou
-00001a60: 7470 7574 0a20 2020 2020 2020 203a 7061  tput.        :pa
-00001a70: 7261 6d20 7072 6f67 7261 6d5f 6172 6773  ram program_args
-00001a80: 3a20 7275 6e74 696d 6520 6172 6775 6d65  : runtime argume
-00001a90: 6e74 730a 2020 2020 2020 2020 3a70 6172  nts.        :par
-00001aa0: 616d 2061 6c6c 5f74 6173 6b65 725f 6974  am all_tasker_it
-00001ab0: 656d 733a 2061 6c6c 2050 726f 6a65 6374  ems: all Project
-00001ac0: 732f 5072 6f66 696c 6573 2f54 6173 6b73  s/Profiles/Tasks
-00001ad0: 2f53 6365 6e65 730a 2020 2020 2020 2020  /Scenes.        
-00001ae0: 3a70 6172 616d 2066 6f75 6e64 5f69 7465  :param found_ite
-00001af0: 6d73 3a20 7369 6e67 6c65 2050 726f 6a65  ms: single Proje
-00001b00: 6374 2f50 726f 6669 6c65 2f54 6173 6b20  ct/Profile/Task 
-00001b10: 746f 2073 6561 7263 6820 666f 720a 2020  to search for.  
-00001b20: 2020 2020 2020 3a70 6172 616d 2064 6f5f        :param do_
-00001b30: 6578 7472 613a 2066 6c61 6720 746f 2064  extra: flag to d
-00001b40: 6f2f 6f75 7470 7574 2065 7874 7261 2054  o/output extra T
-00001b50: 6173 6b20 7374 7566 660a 2020 2020 2020  ask stuff.      
-00001b60: 2020 3a72 6574 7572 6e3a 2054 7275 6520    :return: True 
-00001b70: 6966 2077 6520 6172 6520 7365 6172 6368  if we are search
-00001b80: 696e 6720 666f 7220 6120 7369 6e67 6c65  ing for a single
-00001b90: 2054 6173 6b20 616e 6420 666f 756e 6420   Task and found 
-00001ba0: 6974 2e20 204f 7468 6572 7769 7365 2c20  it.  Otherwise, 
-00001bb0: 4661 6c73 650a 2020 2020 7201 0000 0072  False.    r....r
-00001bc0: 4c00 0000 da14 6469 7370 6c61 795f 6465  L.....display_de
-00001bd0: 7461 696c 5f6c 6576 656c e903 0000 00fa  tail_level......
-00001be0: 0120 4672 0f00 0000 724e 0000 0054 7213  . Fr....rN...Tr.
-00001bf0: 0000 0072 5000 0000 2907 7251 0000 0072  ...rP...).rQ...r
-00001c00: 4d00 0000 7203 0000 0072 0400 0000 7256  M...r....r....rV
-00001c10: 0000 0072 5200 0000 7254 0000 0029 1072  ...rR...rT...).r
-00001c20: 4200 0000 7241 0000 0072 4800 0000 7247  B...rA...rH...rG
-00001c30: 0000 0072 4300 0000 7244 0000 0072 4900  ...rC...rD...rI.
-00001c40: 0000 7245 0000 0072 0b00 0000 724b 0000  ..rE...r....rK..
-00001c50: 0072 4a00 0000 7246 0000 0072 5700 0000  .rJ...rF...rW...
-00001c60: 724d 0000 00da 0c6b 6964 5f61 7070 5f69  rM.....kid_app_i
-00001c70: 6e66 6fda 0870 7269 6f72 6974 7972 2500  nfo..priorityr%.
-00001c80: 0000 7225 0000 0072 2600 0000 da0b 6f75  ..r%...r&.....ou
-00001c90: 7470 7574 5f74 6173 6b35 0100 0073 4800  tput_task5...sH.
-00001ca0: 0000 0c21 1003 0c01 1601 0e01 1601 1003  ...!............
-00001cb0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001cc0: 0201 0201 0201 0201 0201 04f4 040e 0401  ................
-00001cd0: 1202 0202 0201 0201 0201 0201 0201 0201  ................
-00001ce0: 0201 0201 04f8 120b 0402 725d 0000 0029  ..........r]...)
-00001cf0: 24da 1664 6566 7573 6564 786d 6c2e 456c  $..defusedxml.El
-00001d00: 656d 656e 7454 7265 6572 1600 0000 da15  ementTreer......
-00001d10: 6d61 7074 6173 6b65 722e 7372 632e 6163  maptasker.src.ac
-00001d20: 7469 6f6e 65da 0373 7263 da07 6163 7469  tione..src..acti
-00001d30: 6f6e 6572 1c00 0000 da15 6d61 7074 6173  oner......maptas
-00001d40: 6b65 722e 7372 632e 6f75 7470 7574 6cda  ker.src.outputl.
-00001d50: 076f 7574 7075 746c 7252 0000 00da 156d  .outputlrR.....m
-00001d60: 6170 7461 736b 6572 2e73 7263 2e78 6d6c  aptasker.src.xml
-00001d70: 6461 7461 7202 0000 00da 146d 6170 7461  datar......mapta
-00001d80: 736b 6572 2e73 7263 2e6b 6964 6170 7072  sker.src.kidappr
-00001d90: 0300 0000 da16 6d61 7074 6173 6b65 722e  ......maptasker.
-00001da0: 7372 632e 7072 696f 7269 7479 7204 0000  src.priorityr...
-00001db0: 00da 146d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
-00001dc0: 2e67 6574 6964 7372 0500 0000 da16 6d61  .getidsr......ma
-00001dd0: 7074 6173 6b65 722e 7372 632e 7379 7363  ptasker.src.sysc
-00001de0: 6f6e 7374 7206 0000 0072 0700 0000 7208  onstr....r....r.
-00001df0: 0000 00da 176d 6170 7461 736b 6572 2e73  .....maptasker.s
-00001e00: 7263 2e73 6865 6c6c 736f 7274 7209 0000  rc.shellsortr...
-00001e10: 00da 0b45 6c65 6d65 6e74 5472 6565 da03  ...ElementTree..
-00001e20: 584d 4cda 0464 6963 74da 046c 6973 7472  XML..dict..listr
-00001e30: 2700 0000 721e 0000 00da 0574 7570 6c65  '...r......tuple
-00001e40: 7234 0000 0072 3a00 0000 da04 626f 6f6c  r4...r:.....bool
-00001e50: 7240 0000 0072 5600 0000 725d 0000 0072  r@...rV...r]...r
-00001e60: 2500 0000 7225 0000 0072 2500 0000 7226  %...r%...r%...r&
-00001e70: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001e80: 0073 c600 0000 080d 1201 1202 0c01 0c01  .s..............
-00001e90: 0c01 0c01 0c01 0c01 0c01 0c02 0207 0601  ................
-00001ea0: 02ff 0201 02ff 0201 02ff 0202 0afe 0245  ...............E
-00001eb0: 0201 02ff 0202 02fe 0203 02fd 0204 02fc  ................
-00001ec0: 0205 02fb 0e06 0afa 0234 0201 02ff 0201  .........4......
-00001ed0: 02ff 0201 02ff 0c02 0afe 161b 021c 0201  ................
-00001ee0: 02ff 0202 02fe 0203 02fd 0204 02fc 0205  ................
-00001ef0: 02fb 0206 02fa 0207 02f9 0608 02f8 0209  ................
-00001f00: 02f7 020a 02f6 020b 02f5 020c 02f4 020d  ................
-00001f10: 0af3 0264 0201 02ff 0202 02fe 0603 02fd  ...d............
-00001f20: 0204 02fc 0205 02fb 0206 02fa 0207 02f9  ................
-00001f30: 0208 02f8 0209 02f7 020a 02f6 020b 02f5  ................
-00001f40: 020c 02f4 020d 02f3 020e 0ef2            ............
+000000b0: 6409 6c15 6d16 5a16 0100 6400 640a 6c17  d.l.m.Z...d.d.l.
+000000c0: 6d18 5a18 0100 6400 640b 6c19 6d1a 5a1a  m.Z...d.d.l.m.Z.
+000000d0: 0100 640c 6501 6a1b 6a1c 640d 651d 640e  ..d.e.j.j.d.e.d.
+000000e0: 651d 640f 651e 6608 6410 6411 8404 5a1f  e.d.e.f.d.d...Z.
+000000f0: 6412 6520 6413 651e 6414 651e 6415 6520  d.e d.e.d.e.d.e 
+00000100: 6416 651d 640f 6521 6501 6a1b 6a1c 6520  d.e.d.e!e.j.j.e 
+00000110: 6602 1900 660c 6417 6418 8404 5a22 6412  f...f.d.d...Z"d.
+00000120: 6520 6419 651e 641a 651d 640f 6521 6520  e d.e.d.e.d.e!e 
+00000130: 6501 6a1b 6602 1900 6608 641b 641c 8404  e.j.f...f.d.d...
+00000140: 5a23 6412 6520 641d 651d 640f 6524 6606  Z#d.e d.e.d.e$f.
+00000150: 641e 641f 8404 5a25 6420 6520 6421 651e  d.d...Z%d e d!e.
+00000160: 6422 6520 6423 6520 6424 6520 6425 651d  d"e d#e d$e d%e.
+00000170: 6426 651e 6427 6501 6a1b 6a1c 6428 651e  d&e.d'e.j.j.d(e.
+00000180: 6429 651d 640d 651d 642a 651d 640f 6401  d)e.d.e.d*e.d.d.
+00000190: 661a 642b 642c 8404 5a26 6421 651e 6420  f.d+d,..Z&d!e.d 
+000001a0: 6520 6427 6501 6a1b 6a1c 6426 651e 6422  e d'e.j.j.d&e.d"
+000001b0: 6520 6423 6520 6428 651e 6424 6520 640d  e d#e d(e.d$e d.
+000001c0: 651d 642a 651d 6429 651d 6425 651d 642d  e.d*e.d)e.d%e.d-
+000001d0: 6524 640f 6524 661c 642e 642f 8404 5a27  e$d.e$f.d.d/..Z'
+000001e0: 6401 5300 2930 e900 0000 004e 2901 da0b  d.S.)0.....N)...
+000001f0: 7461 675f 696e 5f74 7970 6529 01da 0b67  tag_in_type)...g
+00000200: 6574 5f6b 6964 5f61 7070 2901 da0c 6765  et_kid_app)...ge
+00000210: 745f 7072 696f 7269 7479 2901 da07 6765  t_priority)...ge
+00000220: 745f 6964 7329 01da 1155 4e4b 4e4f 574e  t_ids)...UNKNOWN
+00000230: 5f54 4153 4b5f 4e41 4d45 2901 da0a 4e4f  _TASK_NAME)...NO
+00000240: 5f50 524f 4a45 4354 2901 da06 6c6f 6767  _PROJECT)...logg
+00000250: 6572 2901 da0d 6572 726f 725f 6861 6e64  er)...error_hand
+00000260: 6c65 7229 01da 0b66 6f72 6d61 745f 6874  ler)...format_ht
+00000270: 6d6c 2901 da0a 7368 656c 6c5f 736f 7274  ml)...shell_sort
+00000280: da0c 6375 7272 656e 745f 7461 736b da08  ..current_task..
+00000290: 636f 6c6f 726d 6170 da09 7072 6f67 5f61  colormap..prog_a
+000002a0: 7267 73da 0672 6574 7572 6e63 0300 0000  rgs..returnc....
+000002b0: 0000 0000 0000 0000 0b00 0000 0900 0000  ................
+000002c0: 4300 0000 733a 0100 0067 007d 037a 077c  C...s:...g.}.z.|
+000002d0: 00a0 0064 01a1 017d 0457 006e 1604 0074  ...d...}.W.n...t
+000002e0: 016a 0279 1f01 0001 0001 0074 0364 027c  .j.y.......t.d.|
+000002f0: 0083 0201 0074 0464 0364 0483 0201 0067  .....t.d.d.....g
+00000300: 0006 0059 0053 0077 007c 0472 9b64 057d  ...Y.S.w.|.r.d.}
+00000310: 0564 047d 0674 057c 0483 0164 046b 0472  .d.}.t.|...d.k.r
+00000320: 3274 067c 0464 0664 0783 0301 007c 0444  2t.|.d.d.....|.D
+00000330: 005d 667d 077c 07a0 0764 08a1 017d 0874  .]f}.|...d...}.t
+00000340: 08a0 097c 087c 0764 067c 0164 097c 02a1  ...|.|.d.|.d.|..
+00000350: 067d 0974 0aa0 0b64 0a74 0c7c 076a 0d64  .}.t...d.t.|.j.d
+00000360: 0b19 0083 0117 0064 0c17 007c 086a 0e17  .......d...|.j..
+00000370: 0064 0d17 007c 0917 0064 0e17 0074 0c7c  .d...|...d...t.|
+00000380: 076a 0d83 0117 00a1 0101 0064 0f7c 0976  .j.........d.|.v
+00000390: 0073 6d64 107c 0976 0073 6d64 117c 0976  .smd.|.v.smd.|.v
+000003a0: 0072 7b7c 0664 1238 007d 0674 057c 0583  .r{|.d.8.}.t.|..
+000003b0: 017d 0a7c 0564 137c 0a85 0219 007d 0574  .}.|.d.|.....}.t
+000003c0: 08a0 0f7c 017c 037c 097c 087c 067c 05a1  ...|.|.|.|.|.|..
+000003d0: 067d 0364 147c 0976 0073 9164 107c 0976  .}.d.|.v.s.d.|.v
+000003e0: 0073 9164 157c 0976 0072 9a7c 0664 1237  .s.d.|.v.r.|.d.7
+000003f0: 007d 067c 059b 0064 169d 027d 0571 347c  .}.|...d...}.q4|
+00000400: 0353 0029 1761 1d01 0000 0a20 2020 2052  .S.).a.....    R
+00000410: 6574 7572 6e20 6120 6c69 7374 206f 6620  eturn a list of 
+00000420: 5461 736b 2773 2061 6374 696f 6e73 2066  Task's actions f
+00000430: 6f72 2074 6865 2067 6976 656e 2054 6173  or the given Tas
+00000440: 6b0a 2020 2020 2020 2020 3a70 6172 616d  k.        :param
+00000450: 2063 7572 7265 6e74 5f74 6173 6b3a 2078   current_task: x
+00000460: 6d6c 2065 6c65 6d65 6e74 206f 6620 7468  ml element of th
+00000470: 6520 5461 736b 2077 6520 6172 6520 6765  e Task we are ge
+00000480: 7474 696e 6720 6163 7469 6f6e 7320 666f  tting actions fo
+00000490: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
+000004a0: 2063 6f6c 6f72 6d61 703a 2063 6f6c 6f72   colormap: color
+000004b0: 7320 746f 2075 7365 2069 6e20 6f75 7470  s to use in outp
+000004c0: 7574 0a20 2020 2020 2020 203a 7061 7261  ut.        :para
+000004d0: 6d20 7072 6f67 5f61 7267 733a 2072 756e  m prog_args: run
+000004e0: 7469 6d65 2061 7267 756d 656e 7473 0a20  time arguments. 
+000004f0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00000500: 6c69 7374 206f 6620 5461 736b 2027 6163  list of Task 'ac
+00000510: 7469 6f6e 2720 6f75 7470 7574 206c 696e  tion' output lin
+00000520: 6573 0a20 2020 20da 0641 6374 696f 6e7a  es.    ..Actionz
+00000530: 1674 6173 6b73 2e70 7920 6375 7272 656e  .tasks.py curren
+00000540: 7420 5461 736b 3a7a 1945 7272 6f72 3a20  t Task:z.Error: 
+00000550: 4e6f 2061 6374 696f 6e20 666f 756e 6421  No action found!
+00000560: 2121 7201 0000 00da 0054 46da 0463 6f64  !!r......TF..cod
+00000570: 65da 0174 7a08 5461 736b 2049 443a da02  e..tz.Task ID:..
+00000580: 7372 7a06 2043 6f64 653a 7a0b 2074 6173  srz. Code:z. tas
+00000590: 6b5f 636f 6465 3a7a 0c41 6374 696f 6e20  k_code:z.Action 
+000005a0: 6174 7472 3a7a 073e 456e 6420 4966 7a05  attr:z.>End Ifz.
+000005b0: 3e45 6c73 657a 083e 456e 6420 466f 72e9  >Elsez.>End For.
+000005c0: 0100 0000 e918 0000 007a 033e 4966 7a05  .........z.>Ifz.
+000005d0: 3e46 6f72 3c7a 1826 6e62 7370 3b26 6e62  >For<z.&nbsp;&nb
+000005e0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b29  sp;&nbsp;&nbsp;)
+000005f0: 10da 0766 696e 6461 6c6c da0a 6465 6675  ...findall..defu
+00000600: 7365 6478 6d6c da13 4465 6675 7365 6458  sedxml..DefusedX
+00000610: 6d6c 4578 6365 7074 696f 6eda 0570 7269  mlException..pri
+00000620: 6e74 7209 0000 00da 036c 656e 720b 0000  ntr......lenr...
+00000630: 00da 0466 696e 64da 0f61 6374 696f 6e5f  ...find..action_
+00000640: 6576 616c 7561 7465 da0f 6765 745f 6163  evaluate..get_ac
+00000650: 7469 6f6e 5f63 6f64 6572 0800 0000 da05  tion_coder......
+00000660: 6465 6275 67da 0373 7472 da06 6174 7472  debug..str..attr
+00000670: 6962 da04 7465 7874 da0c 6275 696c 645f  ib..text..build_
+00000680: 6163 7469 6f6e 290b 720c 0000 0072 0d00  action).r....r..
+00000690: 0000 720e 0000 005a 0874 6173 6b6c 6973  ..r....Z.tasklis
+000006a0: 745a 0c74 6173 6b5f 6163 7469 6f6e 735a  tZ.task_actionsZ
+000006b0: 1269 6e64 656e 7461 7469 6f6e 5f61 6d6f  .indentation_amo
+000006c0: 756e 745a 0b69 6e64 656e 7461 7469 6f6e  untZ.indentation
+000006d0: da06 6163 7469 6f6e da05 6368 696c 645a  ..action..childZ
+000006e0: 0974 6173 6b5f 636f 6465 5a0d 6c65 6e67  .task_codeZ.leng
+000006f0: 7468 5f69 6e64 656e 74a9 0072 2600 0000  th_indent..r&...
+00000700: fa74 2f55 7365 7273 2f6d 696b 7275 6269  .t/Users/mikrubi
+00000710: 6e2f 4c69 6272 6172 792f 436c 6f75 6453  n/Library/CloudS
+00000720: 746f 7261 6765 2f47 6f6f 676c 6544 7269  torage/GoogleDri
+00000730: 7665 2d6d 696b 7275 6269 6e40 676d 6169  ve-mikrubin@gmai
+00000740: 6c2e 636f 6d2f 4d79 2044 7269 7665 2f50  l.com/My Drive/P
+00000750: 7974 686f 6e2f 6d61 7074 6173 6b65 722f  ython/maptasker/
+00000760: 6d61 7074 6173 6b65 722f 7372 632f 7461  maptasker/src/ta
+00000770: 736b 732e 7079 da0b 6765 745f 6163 7469  sks.py..get_acti
+00000780: 6f6e 7323 0000 0073 6200 0000 040a 0203  ons#...sb.......
+00000790: 0e01 0e01 0a01 0a01 0801 02fd 0406 0401  ................
+000007a0: 0401 0c03 0c01 0802 0a01 0402 0c01 04ff  ................
+000007b0: 0403 0201 0c01 02ff 0202 02fe 0403 02fd  ................
+000007c0: 0204 02fc 0205 02fb 0206 02fa 0807 02f9  ................
+000007d0: 04ff 080d 0801 0801 0802 0801 0c01 0401  ................
+000007e0: 0c01 04ff 1805 0802 0a01 0280 0402 7228  ..............r(
+000007f0: 0000 00da 0b74 6865 5f74 6173 6b5f 6964  .....the_task_id
+00000800: da1a 7461 736b 735f 7468 6174 5f68 6176  ..tasks_that_hav
+00000810: 655f 6265 656e 5f66 6f75 6e64 da11 7461  e_been_found..ta
+00000820: 736b 5f6f 7574 7075 745f 6c69 6e65 73da  sk_output_lines.
+00000830: 0974 6173 6b5f 7479 7065 da09 616c 6c5f  .task_type..all_
+00000840: 7461 736b 7363 0500 0000 0000 0000 0000  tasksc..........
+00000850: 0000 0800 0000 0800 0000 4300 0000 73e0  ..........C...s.
+00000860: 0000 007c 00a0 00a1 0072 687c 047c 0019  ...|.....rh|.|..
+00000870: 007d 057c 01a0 017c 00a1 0101 0064 017c  .}.|...|.....d.|
+00000880: 009b 009d 027d 067a 297c 05a0 0264 02a1  .....}.z)|...d..
+00000890: 016a 037d 077c 0364 036b 0272 287c 02a0  .j.}.|.d.k.r(|..
+000008a0: 017c 079b 0064 047c 069b 009d 03a1 0101  .|...d.|........
+000008b0: 006e 0f7c 02a0 017c 079b 0064 057c 069b  .n.|...|...d.|..
+000008c0: 009d 03a1 0101 0057 007c 057c 0766 0253  .......W.|.|.f.S
+000008d0: 0057 007c 057c 0766 0253 0004 0074 0479  .W.|.|.f.S...t.y
+000008e0: 6701 0001 0001 0074 057d 077c 0364 036b  g......t.}.|.d.k
+000008f0: 0272 537c 02a0 0174 059b 0064 047c 069b  .rS|...t...d.|..
+00000900: 009d 03a1 0101 006e 0f7c 02a0 0174 059b  .......n.|...t..
+00000910: 0064 057c 069b 009d 03a1 0101 0059 007c  .d.|.........Y.|
+00000920: 057c 0766 0253 0059 007c 057c 0766 0253  .|.f.S.Y.|.|.f.S
+00000930: 0077 0064 067d 0564 077d 077c 057c 0766  .w.d.}.d.}.|.|.f
+00000940: 0253 0029 0861 7801 0000 0a20 2020 2047  .S.).ax....    G
+00000950: 6574 2074 6865 206e 616d 6520 6f66 2074  et the name of t
+00000960: 6865 2074 6173 6b20 6769 7665 6e20 7468  he task given th
+00000970: 6520 5461 736b 2049 440a 2020 2020 2020  e Task ID.      
+00000980: 2020 3a70 6172 616d 2074 6865 5f74 6173    :param the_tas
+00000990: 6b5f 6964 3a20 7468 6520 5461 736b 2773  k_id: the Task's
+000009a0: 2049 4420 2865 2e67 2e20 2734 3727 290a   ID (e.g. '47').
+000009b0: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
+000009c0: 6173 6b73 5f74 6861 745f 6861 7665 5f62  asks_that_have_b
+000009d0: 6565 6e5f 666f 756e 643a 206c 6973 7420  een_found: list 
+000009e0: 6f66 2054 6173 6b73 2066 6f75 6e64 2073  of Tasks found s
+000009f0: 6f20 6661 720a 2020 2020 2020 2020 3a70  o far.        :p
+00000a00: 6172 616d 2074 6173 6b5f 6f75 7470 7574  aram task_output
+00000a10: 5f6c 696e 6573 3a20 6c69 7374 206f 6620  _lines: list of 
+00000a20: 5461 736b 730a 2020 2020 2020 2020 3a70  Tasks.        :p
+00000a30: 6172 616d 2074 6173 6b5f 7479 7065 3a20  aram task_type: 
+00000a40: 5479 7065 206f 6620 5461 736b 2028 456e  Type of Task (En
+00000a50: 7472 792c 2045 7869 742c 2053 6365 6e65  try, Exit, Scene
+00000a60: 290a 2020 2020 2020 2020 3a70 6172 616d  ).        :param
+00000a70: 2061 6c6c 5f74 6173 6b73 3a20 616c 6c20   all_tasks: all 
+00000a80: 5461 736b 7320 696e 2078 6d6c 0a20 2020  Tasks in xml.   
+00000a90: 2020 2020 203a 7265 7475 726e 3a20 5461       :return: Ta
+00000aa0: 736b 2773 2078 6d6c 2065 6c65 6d65 6e74  sk's xml element
+00000ab0: 2c20 5461 736b 2773 206e 616d 650a 2020  , Task's name.  
+00000ac0: 2020 7a15 266e 6273 703b 266e 6273 703b    z.&nbsp;&nbsp;
+00000ad0: 5461 736b 2049 443a 20da 036e 6d65 5a04  Task ID: ..nmeZ.
+00000ae0: 4578 6974 7a25 266e 6273 703b 266e 6273  Exitz%&nbsp;&nbs
+00000af0: 703b 266e 6273 703b 266e 6273 703b 3c3c  p;&nbsp;&nbsp;<<
+00000b00: 3c20 4578 6974 2054 6173 6b7a 2626 6e62  < Exit Taskz&&nb
+00000b10: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
+00000b20: 6e62 7370 3b3c 3c3c 2045 6e74 7279 2054  nbsp;<<< Entry T
+00000b30: 6173 6b4e 7211 0000 0029 06da 0769 7364  askNr....)...isd
+00000b40: 6967 6974 da06 6170 7065 6e64 721c 0000  igit..appendr...
+00000b50: 0072 2200 0000 da0e 4174 7472 6962 7574  .r".....Attribut
+00000b60: 6545 7272 6f72 7206 0000 0029 0872 2900  eErrorr....).r).
+00000b70: 0000 722a 0000 0072 2b00 0000 722c 0000  ..r*...r+...r,..
+00000b80: 0072 2d00 0000 da04 7461 736b da05 6578  .r-.....task..ex
+00000b90: 7472 615a 0974 6173 6b5f 6e61 6d65 7226  traZ.task_namer&
+00000ba0: 0000 0072 2600 0000 7227 0000 00da 0d67  ...r&...r'.....g
+00000bb0: 6574 5f74 6173 6b5f 6e61 6d65 6b00 0000  et_task_namek...
+00000bc0: 7340 0000 0008 1008 010a 010a 0102 020c  s@..............
+00000bd0: 0108 0104 010c 0106 ff04 050c 0106 ff08  ................
+00000be0: 1202 e908 170c f104 0108 0104 010c 0106  ................
+00000bf0: ff04 050c 0106 ff08 0702 f408 0c02 f104  ................
+00000c00: 0c04 0108 0272 3400 0000 da16 7072 6f6a  .....r4.....proj
+00000c10: 6563 7473 5f77 6974 685f 6e6f 5f74 6173  ects_with_no_tas
+00000c20: 6b73 da0c 616c 6c5f 7072 6f6a 6563 7473  ks..all_projects
+00000c30: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
+00000c40: 0009 0000 0043 0000 0073 5600 0000 7400  .....C...sV...t.
+00000c50: 7d03 6401 7d04 7c02 6401 7501 7227 7c02  }.d.}.|.d.u.r'|.
+00000c60: 4400 5d1c 7d04 7c04 a001 6402 a101 6a02  D.].}.|...d...j.
+00000c70: 7d03 7403 6403 6900 6900 6700 7c04 7c03  }.t.d.i.i.g.|.|.
+00000c80: 7c01 8307 7d05 7c00 7c05 7600 7226 7c03  |...}.|.|.v.r&|.
+00000c90: 7c04 6602 0200 0100 5300 710a 7c03 7c04  |.f.....S.q.|.|.
+00000ca0: 6602 5300 2904 614b 0100 000a 2020 2020  f.S.).aK....    
+00000cb0: 4669 6e64 2074 6865 2050 726f 6a65 6374  Find the Project
+00000cc0: 2062 656c 6f6e 6769 6e67 2074 6f20 7468   belonging to th
+00000cd0: 6520 5461 736b 2069 6420 7061 7373 6564  e Task id passed
+00000ce0: 2069 6e0a 2020 2020 2020 2020 3a70 6172   in.        :par
+00000cf0: 616d 2074 6865 5f74 6173 6b5f 6964 3a20  am the_task_id: 
+00000d00: 7468 6520 4944 206f 6620 7468 6520 5461  the ID of the Ta
+00000d10: 736b 0a20 2020 2020 2020 203a 7061 7261  sk.        :para
+00000d20: 6d20 7072 6f6a 6563 7473 5f77 6974 685f  m projects_with_
+00000d30: 6e6f 5f74 6173 6b73 3a20 6c69 7374 206f  no_tasks: list o
+00000d40: 6620 5072 6f6a 6563 7473 2074 6861 7420  f Projects that 
+00000d50: 646f 206e 6f74 2068 6176 6520 616e 7920  do not have any 
+00000d60: 5461 736b 730a 2020 2020 2020 2020 3a70  Tasks.        :p
+00000d70: 6172 616d 2061 6c6c 5f70 726f 6a65 6374  aram all_project
+00000d80: 733a 2061 6c6c 2054 6173 6b65 7220 5072  s: all Tasker Pr
+00000d90: 6f6a 6563 7473 0a20 2020 2020 2020 203a  ojects.        :
+00000da0: 7265 7475 726e 3a20 6e61 6d65 206f 6620  return: name of 
+00000db0: 7468 6520 5072 6f6a 6563 7420 7468 6174  the Project that
+00000dc0: 2062 656c 6f6e 6773 2074 6f20 7468 6973   belongs to this
+00000dd0: 2074 6173 6b20 616e 6420 7468 6520 5072   task and the Pr
+00000de0: 6f6a 6563 7420 786d 6c20 656c 656d 656e  oject xml elemen
+00000df0: 740a 2020 2020 4eda 046e 616d 6546 2904  t.    N..nameF).
+00000e00: 7207 0000 0072 1c00 0000 7222 0000 0072  r....r....r"...r
+00000e10: 0500 0000 2906 7229 0000 0072 3500 0000  ....).r)...r5...
+00000e20: 7236 0000 005a 0970 726f 6a5f 6e61 6d65  r6...Z.proj_name
+00000e30: da07 7072 6f6a 6563 74da 0874 6173 6b5f  ..project..task_
+00000e40: 6964 7372 2600 0000 7226 0000 0072 2700  idsr&...r&...r'.
+00000e50: 0000 da19 6765 745f 7072 6f6a 6563 745f  ....get_project_
+00000e60: 666f 725f 736f 6c6f 5f74 6173 6ba0 0000  for_solo_task...
+00000e70: 0073 1800 0000 040a 0401 0801 0802 0c01  .s..............
+00000e80: 0201 0e01 04ff 0803 0c01 02ff 0802 723a  ..............r:
+00000e90: 0000 00da 0a61 6c6c 5f73 6365 6e65 7363  .....all_scenesc
+00000ea0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00000eb0: 0600 0000 4300 0000 7360 0000 007c 01a0  ....C...s`...|..
+00000ec0: 00a1 0044 005d 297d 027c 0244 005d 247d  ...D.])}.|.D.]$}
+00000ed0: 0374 017c 036a 0264 0183 0272 2c7c 0344  .t.|.j.d...r,|.D
+00000ee0: 005d 197d 0474 017c 046a 0264 0283 0272  .].}.t.|.j.d...r
+00000ef0: 247c 007c 046a 036b 0272 2401 0001 0001  $|.|.j.k.r$.....
+00000f00: 0064 0153 007c 036a 0264 036b 0272 2b01  .d.S.|.j.d.k.r+.
+00000f10: 006e 0171 1271 0871 0464 0253 0029 0461  .n.q.q.q.d.S.).a
+00000f20: 1801 0000 0a20 2020 2049 6465 6e74 6966  .....    Identif
+00000f30: 7920 7768 6574 6865 7220 7468 6520 5461  y whether the Ta
+00000f40: 736b 2070 6173 7365 6420 696e 2069 7320  sk passed in is 
+00000f50: 7061 7274 206f 6620 6120 5363 656e 653a  part of a Scene:
+00000f60: 2054 7275 6520 3d20 7965 732c 2046 616c   True = yes, Fal
+00000f70: 7365 203d 206e 6f0a 2020 2020 2020 2020  se = no.        
+00000f80: 3a70 6172 616d 2074 6865 5f74 6173 6b5f  :param the_task_
+00000f90: 6964 3a20 7468 6520 6964 206f 6620 7468  id: the id of th
+00000fa0: 6520 5461 736b 2074 6f20 6368 6563 6b20  e Task to check 
+00000fb0: 6167 6169 6e73 740a 2020 2020 2020 2020  against.        
+00000fc0: 3a70 6172 616d 2061 6c6c 5f73 6365 6e65  :param all_scene
+00000fd0: 733a 2061 6c6c 2053 6365 6e65 7320 696e  s: all Scenes in
+00000fe0: 2054 6173 6b65 7220 636f 6e66 6967 7572   Tasker configur
+00000ff0: 6174 696f 6e0a 2020 2020 2020 2020 3a72  ation.        :r
+00001000: 6574 7572 6e3a 2054 7275 6520 6966 2054  eturn: True if T
+00001010: 6173 6b20 6973 2070 6172 7420 6f66 2061  ask is part of a
+00001020: 2053 6365 6e65 2c20 4661 6c73 6520 6f74   Scene, False ot
+00001030: 6865 7277 6973 650a 2020 2020 5446 da03  herwise.    TF..
+00001040: 5374 7229 04da 0676 616c 7565 7372 0200  Str)...valuesr..
+00001050: 0000 da03 7461 6772 2200 0000 2905 7229  ....tagr"...).r)
+00001060: 0000 0072 3b00 0000 da05 7661 6c75 6572  ...r;.....valuer
+00001070: 2500 0000 5a08 7375 6263 6869 6c64 7226  %...Z.subchildr&
+00001080: 0000 0072 2600 0000 7227 0000 00da 0d74  ...r&...r'.....t
+00001090: 6173 6b5f 696e 5f73 6365 6e65 bb00 0000  ask_in_scene....
+000010a0: 731c 0000 000c 0808 010c 0108 010a 0302  s...............
+000010b0: ff0a 020a 020a 0104 0102 0202 8002 f404  ................
+000010c0: 0d72 4000 0000 da0d 6f75 725f 7461 736b  .r@.....our_task
+000010d0: 5f6e 616d 65da 0b6f 7574 7075 745f 6c69  _name..output_li
+000010e0: 7374 da0c 7072 6f6a 6563 745f 6e61 6d65  st..project_name
+000010f0: da0c 7072 6f66 696c 655f 6e61 6d65 da07  ..profile_name..
+00001100: 6865 6164 696e 67da 0b66 6f75 6e64 5f69  heading..found_i
+00001110: 7465 6d73 da09 7461 736b 5f6c 6973 74da  tems..task_list.
+00001120: 106f 7572 5f74 6173 6b5f 656c 656d 656e  .our_task_elemen
+00001130: 74da 136c 6973 745f 6f66 5f66 6f75 6e64  t..list_of_found
+00001140: 5f74 6173 6b73 da10 616c 6c5f 7461 736b  _tasks..all_task
+00001150: 6572 5f69 7465 6d73 da0c 7072 6f67 7261  er_items..progra
+00001160: 6d5f 6172 6773 630c 0000 0000 0000 0000  m_argsc.........
+00001170: 0000 0011 0000 000a 0000 0043 0000 0073  ...........C...s
+00001180: 0a01 0000 6401 6402 6c00 6d01 7d0c 0100  ....d.d.l.m.}...
+00001190: 7402 a003 6403 7c0b 6404 1900 9b00 6405  t...d.|.d.....d.
+000011a0: 7c00 9b00 9d04 a101 0100 7c0b 6404 1900  |.........|.d...
+000011b0: 7c00 6b02 7256 6406 7c05 6407 3c00 7404  |.k.rVd.|.d.<.t.
+000011c0: a005 6406 7c01 7c02 7c03 7c04 7c0a 7c0b  ..d.|.|.|.|.|.|.
+000011d0: a107 0100 6700 7d0d 7406 7c06 8301 6408  ....g.}.t.|...d.
+000011e0: 6b04 7247 7406 7c00 8301 7d0e 7c06 4400  k.rGt.|...}.|.D.
+000011f0: 5d0f 7d0f 7c00 7c0f 6409 7c0e 8502 1900  ].}.|.|.d.|.....
+00001200: 6b02 7245 7c0f 6701 7d0d 0100 6e01 7136  k.rE|.g.}...n.q6
+00001210: 6e02 7c06 7d0d 7c0c 640a 7c01 7c0d 7c07  n.|.}.|.d.|.|.|.
+00001220: 7c08 7c0b 7c0a 7c09 8308 0100 6409 5300  |.|.|.|.....d.S.
+00001230: 7406 7c06 8301 6408 6b04 7281 7c06 4400  t.|...d.k.r.|.D.
+00001240: 5d24 7d10 7c0b 6404 1900 7c10 7600 7280  ]$}.|.d...|.v.r.
+00001250: 7404 a007 7c0a 7c0b 7c01 6408 640b a105  t...|.|.|.d.d...
+00001260: 0100 7c10 6701 7d06 7c0c 640a 7c01 7c06  ..|.g.}.|.d.|.|.
+00001270: 7c07 7c08 7c0b 7c0a 7c09 8308 0100 0100  |.|.|.|.|.......
+00001280: 6409 5300 715e 6409 5300 6409 5300 290c  d.S.q^d.S.d.S.).
+00001290: 61db 0200 000a 2020 2020 5072 6f63 6573  a.....    Proces
+000012a0: 7320 6120 7369 6e67 6c65 2054 6173 6b20  s a single Task 
+000012b0: 6f6e 6c79 0a20 2020 2020 2020 203a 7061  only.        :pa
+000012c0: 7261 6d20 6f75 725f 7461 736b 5f6e 616d  ram our_task_nam
+000012d0: 653a 206e 616d 6520 6f66 2074 6865 2054  e: name of the T
+000012e0: 6173 6b20 746f 2070 726f 6365 7373 0a20  ask to process. 
+000012f0: 2020 2020 2020 203a 7061 7261 6d20 6f75         :param ou
+00001300: 7470 7574 5f6c 6973 743a 2077 6865 7265  tput_list: where
+00001310: 2074 6865 206f 7574 7075 7420 6c69 6e65   the output line
+00001320: 2067 6f65 7320 666f 7220 5461 736b 0a20   goes for Task. 
+00001330: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
+00001340: 6f6a 6563 745f 6e61 6d65 3a20 6e61 6d65  oject_name: name
+00001350: 206f 6620 7468 6520 5072 6f6a 6563 7420   of the Project 
+00001360: 5461 736b 2062 656c 6f6e 6773 2074 6f0a  Task belongs to.
+00001370: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+00001380: 726f 6669 6c65 5f6e 616d 653a 206e 616d  rofile_name: nam
+00001390: 6520 6f66 2074 6865 2050 726f 6669 6c65  e of the Profile
+000013a0: 2074 6865 2054 6173 6b20 6265 6c6f 6e67   the Task belong
+000013b0: 7320 746f 0a20 2020 2020 2020 203a 7061  s to.        :pa
+000013c0: 7261 6d20 6865 6164 696e 673a 2074 6865  ram heading: the
+000013d0: 2068 6561 6469 6e67 2c20 6966 2061 6e79   heading, if any
+000013e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000013f0: 666f 756e 645f 6974 656d 733a 2073 696e  found_items: sin
+00001400: 676c 6520 6e61 6d65 2066 6f72 2050 726f  gle name for Pro
+00001410: 6a65 6374 2f50 726f 6669 6c65 2f54 6173  ject/Profile/Tas
+00001420: 6b0a 2020 2020 2020 2020 3a70 6172 616d  k.        :param
+00001430: 2074 6173 6b5f 6c69 7374 3a20 6c69 7374   task_list: list
+00001440: 206f 6620 5461 736b 730a 2020 2020 2020   of Tasks.      
+00001450: 2020 3a70 6172 616d 206f 7572 5f74 6173    :param our_tas
+00001460: 6b5f 656c 656d 656e 743a 2074 6865 2078  k_element: the x
+00001470: 6d6c 2065 6c65 6d65 6e74 2066 6f72 2074  ml element for t
+00001480: 6869 7320 5461 736b 0a20 2020 2020 2020  his Task.       
+00001490: 203a 7061 7261 6d20 6c69 7374 5f6f 665f   :param list_of_
+000014a0: 666f 756e 645f 7461 736b 733a 2061 6c6c  found_tasks: all
+000014b0: 2054 6173 6b73 2070 726f 6365 7373 6564   Tasks processed
+000014c0: 2073 6f20 6661 720a 2020 2020 2020 2020   so far.        
+000014d0: 3a70 6172 616d 2061 6c6c 5f74 6173 6b65  :param all_taske
+000014e0: 725f 6974 656d 733a 2061 6c6c 2050 726f  r_items: all Pro
+000014f0: 6a65 6374 732f 5072 6f66 696c 6573 2f54  jects/Profiles/T
+00001500: 6173 6b73 2f53 6365 6e65 730a 2020 2020  asks/Scenes.    
+00001510: 2020 2020 3a70 6172 616d 2063 6f6c 6f72      :param color
+00001520: 6d61 703a 2063 6f6c 6f72 7320 746f 2075  map: colors to u
+00001530: 7365 2069 6e20 6f75 7470 7574 0a20 2020  se in output.   
+00001540: 2020 2020 203a 7061 7261 6d20 7072 6f67       :param prog
+00001550: 7261 6d5f 6172 6773 3a20 7275 6e74 696d  ram_args: runtim
+00001560: 6520 6172 6775 6d65 6e74 730a 2020 2020  e arguments.    
+00001570: 7201 0000 00a9 01da 0c70 726f 6365 7373  r........process
+00001580: 5f6c 6973 747a 1774 6173 6b73 2073 696e  _listz.tasks sin
+00001590: 676c 6520 7461 736b 206e 616d 653a da10  gle task name:..
+000015a0: 7369 6e67 6c65 5f74 6173 6b5f 6e61 6d65  single_task_name
+000015b0: 7a0f 206f 7572 2054 6173 6b20 6e61 6d65  z. our Task name
+000015c0: 3a54 da11 7369 6e67 6c65 5f74 6173 6b5f  :T..single_task_
+000015d0: 666f 756e 6472 1500 0000 4efa 0554 6173  foundr....N..Tas
+000015e0: 6b3a 7211 0000 0029 08da 166d 6170 7461  k:r....)...mapta
+000015f0: 736b 6572 2e73 7263 2e70 726f 636c 6973  sker.src.proclis
+00001600: 7472 4d00 0000 7208 0000 0072 1f00 0000  trM...r....r....
+00001610: da0c 6275 696c 645f 6f75 7470 7574 da12  ..build_output..
+00001620: 7265 6672 6573 685f 6f75 725f 6f75 7470  refresh_our_outp
+00001630: 7574 721b 0000 00da 096d 795f 6f75 7470  utr......my_outp
+00001640: 7574 2911 7241 0000 0072 4200 0000 7243  ut).rA...rB...rC
+00001650: 0000 0072 4400 0000 7245 0000 0072 4600  ...rD...rE...rF.
+00001660: 0000 7247 0000 0072 4800 0000 7249 0000  ..rG...rH...rI..
+00001670: 0072 4a00 0000 720d 0000 0072 4b00 0000  .rJ...r....rK...
+00001680: 724d 0000 005a 1374 656d 706f 7261 7279  rM...Z.temporary
+00001690: 5f74 6173 6b5f 6c69 7374 5a14 7468 655f  _task_listZ.the_
+000016a0: 7461 736b 5f6e 616d 655f 6c65 6e67 7468  task_name_length
+000016b0: da04 6974 656d 5a09 7461 736b 5f69 7465  ..itemZ.task_ite
+000016c0: 6d72 2600 0000 7226 0000 0072 2700 0000  mr&...r&...r'...
+000016d0: da0e 646f 5f73 696e 676c 655f 7461 736b  ..do_single_task
+000016e0: d700 0000 7374 0000 000c 1e04 020c 0102  ....st..........
+000016f0: 0104 ff04 ff0c 0408 0204 0302 0102 0102  ................
+00001700: 0102 0102 0102 0102 0104 f904 0b0c 0108  ................
+00001710: 0108 0110 0106 0104 0102 fe02 8004 0402  ................
+00001720: 0202 0102 0102 0102 0102 0102 0102 0102  ................
+00001730: 0108 f80c 0b08 020c 0104 010a 0104 ff06  ................
+00001740: 0302 0102 0102 0102 0102 0102 0102 0102  ................
+00001750: 0102 0104 f806 0a02 f104 fd04 0272 5600  .............rV.
+00001760: 0000 da08 646f 5f65 7874 7261 630d 0000  ....do_extrac...
+00001770: 0000 0000 0000 0000 0010 0000 000d 0000  ................
+00001780: 0043 0000 0073 e600 0000 6401 6402 6c00  .C...s....d.d.l.
+00001790: 6d01 7d0d 0100 7c0c 7239 7c09 6403 1900  m.}...|.r9|.d...
+000017a0: 6404 6b02 7239 7402 7c02 8301 0400 7d0e  d.k.r9t.|.....}.
+000017b0: 7227 7403 7c08 6405 6406 7c0e 6407 8305  r't.|.d.d.|.d...
+000017c0: 7d0e 7c03 6401 1900 9b00 6408 7c0e 9b00  }.|.d.....d.|...
+000017d0: 9d03 7c03 6401 3c00 7404 7c02 6409 8302  ..|.d.<.t.|.d...
+000017e0: 0400 7d0f 7239 7c03 6401 1900 9b00 6408  ..}.r9|.d.....d.
+000017f0: 7c0f 9b00 9d03 7c03 6401 3c00 7c01 6406  |.....|.d.<.|.d.
+00001800: 6b03 7252 7c09 640a 1900 7252 7405 7c01  k.rR|.d...rRt.|.
+00001810: 7c00 7c04 7c05 7c07 7c0b 7c03 7c02 7c06  |.|.|.|.|.|.|.|.
+00001820: 7c0a 7c08 7c09 830c 0100 6407 5300 7c03  |.|.|.....d.S.|.
+00001830: 7271 7406 a007 7c08 7c09 7c00 640b 6406  rqt...|.|.|.d.d.
+00001840: a105 0100 7c0d 640c 7c00 7c03 7c02 7c06  ....|.d.|.|.|.|.
+00001850: 7c09 7c08 7c0a 8308 0100 7406 a007 7c08  |.|.|.....t...|.
+00001860: 7c09 7c00 6404 6406 a105 0100 6409 5300  |.|.d.d.....d.S.
+00001870: 290d 615c 0300 000a 2020 2020 5765 2068  ).a\....    We h
+00001880: 6176 6520 6120 7369 6e67 6c65 2054 6173  ave a single Tas
+00001890: 6b20 6f72 2061 206c 6973 7420 6f66 2054  k or a list of T
+000018a0: 6173 6b73 2e20 204f 7574 7075 7420 6974  asks.  Output it
+000018b0: 2f74 6865 6d2e 0a20 2020 2020 2020 203a  /them..        :
+000018c0: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
+000018d0: 743a 206c 6973 7420 6f66 206f 7574 7075  t: list of outpu
+000018e0: 7420 6c69 6e65 7320 6765 6e65 7261 7465  t lines generate
+000018f0: 6420 7468 7573 2066 6172 0a20 2020 2020  d thus far.     
+00001900: 2020 203a 7061 7261 6d20 6f75 725f 7461     :param our_ta
+00001910: 736b 5f6e 616d 653a 206e 616d 6520 6f66  sk_name: name of
+00001920: 2054 6173 6b0a 2020 2020 2020 2020 3a70   Task.        :p
+00001930: 6172 616d 206f 7572 5f74 6173 6b5f 656c  aram our_task_el
+00001940: 656d 656e 743a 2054 6173 6b20 786d 6c20  ement: Task xml 
+00001950: 656c 656d 656e 740a 2020 2020 2020 2020  element.        
+00001960: 3a70 6172 616d 2074 6173 6b5f 6c69 7374  :param task_list
+00001970: 3a20 5461 736b 206c 6973 740a 2020 2020  : Task list.    
+00001980: 2020 2020 3a70 6172 616d 2070 726f 6a65      :param proje
+00001990: 6374 5f6e 616d 653a 206e 616d 6520 6f66  ct_name: name of
+000019a0: 2063 7572 7265 6e74 2050 726f 6a65 6374   current Project
+000019b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000019c0: 7072 6f66 696c 655f 6e61 6d65 3a20 6e61  profile_name: na
+000019d0: 6d65 206f 6620 6375 7272 656e 7420 5072  me of current Pr
+000019e0: 6f66 696c 650a 2020 2020 2020 2020 3a70  ofile.        :p
+000019f0: 6172 616d 206c 6973 745f 6f66 5f66 6f75  aram list_of_fou
+00001a00: 6e64 5f74 6173 6b73 3a20 6c69 7374 206f  nd_tasks: list o
+00001a10: 6620 5461 736b 7320 666f 756e 6420 736f  f Tasks found so
+00001a20: 2066 6172 0a20 2020 2020 2020 203a 7061   far.        :pa
+00001a30: 7261 6d20 6865 6164 696e 673a 2063 7572  ram heading: cur
+00001a40: 7265 6e74 2068 6561 6469 6e67 0a20 2020  rent heading.   
+00001a50: 2020 2020 203a 7061 7261 6d20 636f 6c6f       :param colo
+00001a60: 726d 6170 3a20 636f 6c6f 7273 2074 6f20  rmap: colors to 
+00001a70: 7573 6520 696e 206f 7574 7075 740a 2020  use in output.  
+00001a80: 2020 2020 2020 3a70 6172 616d 2070 726f        :param pro
+00001a90: 6772 616d 5f61 7267 733a 2072 756e 7469  gram_args: runti
+00001aa0: 6d65 2061 7267 756d 656e 7473 0a20 2020  me arguments.   
+00001ab0: 2020 2020 203a 7061 7261 6d20 616c 6c5f       :param all_
+00001ac0: 7461 736b 6572 5f69 7465 6d73 3a20 616c  tasker_items: al
+00001ad0: 6c20 5072 6f6a 6563 7473 2f50 726f 6669  l Projects/Profi
+00001ae0: 6c65 732f 5461 736b 732f 5363 656e 6573  les/Tasks/Scenes
+00001af0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001b00: 666f 756e 645f 6974 656d 733a 2073 696e  found_items: sin
+00001b10: 676c 6520 5072 6f6a 6563 742f 5072 6f66  gle Project/Prof
+00001b20: 696c 652f 5461 736b 2074 6f20 7365 6172  ile/Task to sear
+00001b30: 6368 2066 6f72 0a20 2020 2020 2020 203a  ch for.        :
+00001b40: 7061 7261 6d20 646f 5f65 7874 7261 3a20  param do_extra: 
+00001b50: 666c 6167 2074 6f20 646f 2f6f 7574 7075  flag to do/outpu
+00001b60: 7420 6578 7472 6120 5461 736b 2073 7475  t extra Task stu
+00001b70: 6666 0a20 2020 2020 2020 203a 7265 7475  ff.        :retu
+00001b80: 726e 3a20 5472 7565 2069 6620 7765 2061  rn: True if we a
+00001b90: 7265 2073 6561 7263 6869 6e67 2066 6f72  re searching for
+00001ba0: 2061 2073 696e 676c 6520 5461 736b 2061   a single Task a
+00001bb0: 6e64 2066 6f75 6e64 2069 742e 2020 4f74  nd found it.  Ot
+00001bc0: 6865 7277 6973 652c 2046 616c 7365 0a20  herwise, False. 
+00001bd0: 2020 2072 0100 0000 724c 0000 00da 1464     r....rL.....d
+00001be0: 6973 706c 6179 5f64 6574 6169 6c5f 6c65  isplay_detail_le
+00001bf0: 7665 6ce9 0300 0000 da0a 7461 736b 5f63  vel.......task_c
+00001c00: 6f6c 6f72 7211 0000 0054 da01 2046 724e  olorr....T.. FrN
+00001c10: 0000 0072 1500 0000 7250 0000 0029 0872  ...r....rP...).r
+00001c20: 5100 0000 724d 0000 0072 0300 0000 720a  Q...rM...r....r.
+00001c30: 0000 0072 0400 0000 7256 0000 0072 5200  ...r....rV...rR.
+00001c40: 0000 7254 0000 0029 1072 4200 0000 7241  ..rT...).rB...rA
+00001c50: 0000 0072 4800 0000 7247 0000 0072 4300  ...rH...rG...rC.
+00001c60: 0000 7244 0000 0072 4900 0000 7245 0000  ..rD...rI...rE..
+00001c70: 0072 0d00 0000 724b 0000 0072 4a00 0000  .r....rK...rJ...
+00001c80: 7246 0000 0072 5700 0000 724d 0000 00da  rF...rW...rM....
+00001c90: 0c6b 6964 5f61 7070 5f69 6e66 6fda 0870  .kid_app_info..p
+00001ca0: 7269 6f72 6974 7972 2600 0000 7226 0000  riorityr&...r&..
+00001cb0: 0072 2700 0000 da0b 6f75 7470 7574 5f74  .r'.....output_t
+00001cc0: 6173 6b38 0100 0073 4a00 0000 0c21 1003  ask8...sJ....!..
+00001cd0: 0c01 1001 1601 0e01 1601 1003 0201 0201  ................
+00001ce0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001cf0: 0201 0201 0201 04f4 040e 0401 1202 0202  ................
+00001d00: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001d10: 04f8 120b 0402 725e 0000 0029 28da 1664  ......r^...)(..d
+00001d20: 6566 7573 6564 786d 6c2e 456c 656d 656e  efusedxml.Elemen
+00001d30: 7454 7265 6572 1800 0000 da15 6d61 7074  tTreer......mapt
+00001d40: 6173 6b65 722e 7372 632e 6163 7469 6f6e  asker.src.action
+00001d50: 65da 0373 7263 da07 6163 7469 6f6e 6572  e..src..actioner
+00001d60: 1d00 0000 da15 6d61 7074 6173 6b65 722e  ......maptasker.
+00001d70: 7372 632e 6f75 7470 7574 6cda 076f 7574  src.outputl..out
+00001d80: 7075 746c 7252 0000 00da 156d 6170 7461  putlrR.....mapta
+00001d90: 736b 6572 2e73 7263 2e78 6d6c 6461 7461  sker.src.xmldata
+00001da0: 7202 0000 00da 146d 6170 7461 736b 6572  r......maptasker
+00001db0: 2e73 7263 2e6b 6964 6170 7072 0300 0000  .src.kidappr....
+00001dc0: da16 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
+00001dd0: 7072 696f 7269 7479 7204 0000 00da 146d  priorityr......m
+00001de0: 6170 7461 736b 6572 2e73 7263 2e67 6574  aptasker.src.get
+00001df0: 6964 7372 0500 0000 da16 6d61 7074 6173  idsr......maptas
+00001e00: 6b65 722e 7372 632e 7379 7363 6f6e 7374  ker.src.sysconst
+00001e10: 7206 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
+00001e20: 136d 6170 7461 736b 6572 2e73 7263 2e65  .maptasker.src.e
+00001e30: 7272 6f72 7209 0000 00da 166d 6170 7461  rrorr......mapta
+00001e40: 736b 6572 2e73 7263 2e66 726d 7468 746d  sker.src.frmthtm
+00001e50: 6c72 0a00 0000 da17 6d61 7074 6173 6b65  lr......maptaske
+00001e60: 722e 7372 632e 7368 656c 6c73 6f72 7472  r.src.shellsortr
+00001e70: 0b00 0000 da0b 456c 656d 656e 7454 7265  ......ElementTre
+00001e80: 65da 0358 4d4c da04 6469 6374 da04 6c69  e..XML..dict..li
+00001e90: 7374 7228 0000 0072 2000 0000 da05 7475  str(...r .....tu
+00001ea0: 706c 6572 3400 0000 723a 0000 00da 0462  pler4...r:.....b
+00001eb0: 6f6f 6c72 4000 0000 7256 0000 0072 5e00  oolr@...rV...r^.
+00001ec0: 0000 7226 0000 0072 2600 0000 7226 0000  ..r&...r&...r&..
+00001ed0: 0072 2700 0000 da08 3c6d 6f64 756c 653e  .r'.....<module>
+00001ee0: 0100 0000 73ca 0000 0008 0d12 0112 020c  ....s...........
+00001ef0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001f00: 010c 0202 0706 0102 ff02 0102 ff02 0102  ................
+00001f10: ff02 020a fe02 4802 0102 ff02 0202 fe02  ......H.........
+00001f20: 0302 fd02 0402 fc02 0502 fb0e 060a fa02  ................
+00001f30: 3502 0102 ff02 0102 ff02 0102 ff0c 020a  5...............
+00001f40: fe16 1b02 1c02 0102 ff02 0202 fe02 0302  ................
+00001f50: fd02 0402 fc02 0502 fb02 0602 fa02 0702  ................
+00001f60: f906 0802 f802 0902 f702 0a02 f602 0b02  ................
+00001f70: f502 0c02 f402 0d0a f302 6102 0102 ff02  ..........a.....
+00001f80: 0202 fe06 0302 fd02 0402 fc02 0502 fb02  ................
+00001f90: 0602 fa02 0702 f902 0802 f802 0902 f702  ................
+00001fa0: 0a02 f602 0b02 f502 0c02 f402 0d02 f302  ................
+00001fb0: 0e0e f2                                  ...
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/taskuniq.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/taskuniq.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 16 16:23:58 2023 UTC, .py size: 9713 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,212 +1,210 @@
-00000000: 6f0d 0d0a 0000 0000 1e21 3c64 f125 0000  o........!<d.%..
+00000000: 6f0d 0d0a 0000 0000 855a 4164 c225 0000  o........ZAd.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 e600 0000 6400  .....@...s....d.
+00000020: 0012 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 0200 0100 6d05 5a06 0100  d.l.m.....m.Z...
 00000050: 6400 6402 6c07 6d04 0200 0100 6d08 5a08  d.d.l.m.....m.Z.
 00000060: 0100 6400 6403 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c0b 6d0c 5a0c 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
-00000080: 6d0d 5a0d 0100 6400 6406 6c0b 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000090: 0100 6407 6501 650f 1900 6408 6502 6501  ..d.e.e...d.e.e.
-000000a0: 650f 1900 6501 6602 1900 6409 6501 650f  e...e.f...d.e.e.
-000000b0: 1900 640a 6510 640b 6510 640c 6510 640d  ..d.e.d.e.d.e.d.
-000000c0: 6402 660e 640e 640f 8404 5a11 6410 6512  d.f.d.d...Z.d.e.
-000000d0: 6602 6411 6412 8404 5a13 6407 6501 650f  f.d.d...Z.d.e.e.
-000000e0: 1900 6408 6501 6413 6501 650f 1900 640c  ..d.e.d.e.e...d.
-000000f0: 6510 640a 6510 6414 650f 640b 6510 6415  e.d.e.d.e.d.e.d.
-00000100: 6510 640d 6402 6612 6416 6417 8404 5a14  e.d.d.f.d.d...Z.
-00000110: 6402 5300 2918 e900 0000 0029 02da 044c  d.S.)......)...L
-00000120: 6973 74da 0555 6e69 6f6e 4e29 01da 0b66  ist..UnionN)...f
-00000130: 6f72 6d61 745f 6874 6d6c 2901 da0b 464f  ormat_html)...FO
-00000140: 4e54 5f54 4f5f 5553 4529 01da 1155 4e4b  NT_TO_USE)...UNK
-00000150: 4e4f 574e 5f54 4153 4b5f 4e41 4d45 2901  NOWN_TASK_NAME).
-00000160: da0a 4e4f 5f50 524f 4a45 4354 da0b 6f75  ..NO_PROJECT..ou
-00000170: 7470 7574 5f6c 6973 74da 1670 726f 6a65  tput_list..proje
-00000180: 6374 735f 7769 7468 5f6e 6f5f 7461 736b  cts_with_no_task
-00000190: 73da 1970 726f 6a65 6374 735f 7769 7468  s..projects_with
-000001a0: 6f75 745f 7072 6f66 696c 6573 da0b 666f  out_profiles..fo
-000001b0: 756e 645f 6974 656d 73da 0863 6f6c 6f72  und_items..color
-000001c0: 6d61 70da 0c70 726f 6772 616d 5f61 7267  map..program_arg
-000001d0: 73da 0672 6574 7572 6e63 0600 0000 0000  s..returnc......
-000001e0: 0000 0000 0000 0700 0000 0e00 0000 4300  ..............C.
-000001f0: 0000 73b8 0000 0074 007c 0183 0164 016b  ..s....t.|...d.k
-00000200: 0472 317c 0364 0219 0073 3174 01a0 027c  .r1|.d...s1t...|
-00000210: 047c 057c 0064 0174 037c 0464 0364 0464  .|.|.d.t.|.d.d.d
-00000220: 0564 0683 05a1 0501 007c 0144 005d 157d  .d.......|.D.].}
-00000230: 0674 01a0 027c 047c 057c 0064 0774 037c  .t...|.|.|.d.t.|
-00000240: 0464 0364 0464 087c 069b 0064 099d 0364  .d.d.d.|...d...d
-00000250: 0683 05a1 0501 0071 1b7c 0272 5a74 01a0  .......q.|.rZt..
-00000260: 027c 047c 057c 0064 0174 037c 0464 0364  .|.|.|.d.t.|.d.d
-00000270: 0a64 0b64 0683 05a1 0501 007c 0244 005d  .d.d.......|.D.]
-00000280: 157d 0674 01a0 027c 047c 057c 0064 0774  .}.t...|.|.|.d.t
-00000290: 037c 0464 0364 0464 0c7c 069b 0064 0d9d  .|.d.d.d.|...d..
-000002a0: 0364 0683 05a1 0501 0071 4464 0053 0029  .d.......qDd.S.)
-000002b0: 0e4e 7201 0000 00da 1173 696e 676c 655f  .Nr......single_
-000002c0: 7461 736b 5f66 6f75 6e64 da17 7472 6169  task_found..trai
-000002d0: 6c69 6e67 5f63 6f6d 6d65 6e74 735f 636f  ling_comments_co
-000002e0: 6c6f 72da 007a 263c 6872 3e3c 656d 3e50  lor..z&<hr><em>P
-000002f0: 726f 6a65 6374 7320 5769 7468 6f75 7420  rojects Without 
-00000300: 5461 736b 732e 2e2e 3c2f 656d 3e54 e904  Tasks...</em>T..
-00000310: 0000 007a 0850 726f 6a65 6374 207a 1c20  ...z.Project z. 
-00000320: 6861 7320 6e6f 203c 656d 3e4e 616d 6564  has no <em>Named
-00000330: 3c2f 656d 3e20 5461 736b 737a 043c 6272  </em> Tasksz.<br
-00000340: 3e7a 253c 656d 3e50 726f 6a65 6374 7320  >z%<em>Projects 
-00000350: 5769 7468 6f75 7420 5072 6f66 696c 6573  Without Profiles
-00000360: 2e2e 2e3c 2f65 6d3e 7a09 3e50 726f 6a65  ...</em>z.>Proje
-00000370: 6374 207a 1020 6861 7320 6e6f 2050 726f  ct z. has no Pro
-00000380: 6669 6c65 7329 04da 036c 656e da0c 6275  files)...len..bu
-00000390: 696c 645f 6f75 7470 7574 da09 6d79 5f6f  ild_output..my_o
-000003a0: 7574 7075 7472 0400 0000 2907 7208 0000  utputr....).r...
-000003b0: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-000003c0: 720c 0000 0072 0d00 0000 da04 6974 656d  r....r......item
-000003d0: a900 7217 0000 00fa 772f 5573 6572 732f  ..r.....w/Users/
-000003e0: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
-000003f0: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
-00000400: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
-00000410: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
-00000420: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
-00000430: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
-00000440: 2f73 7263 2f74 6173 6b75 6e69 712e 7079  /src/taskuniq.py
-00000450: da22 7072 6f63 6573 735f 6d69 7373 696e  ."process_missin
-00000460: 675f 7461 736b 735f 616e 645f 7072 6f66  g_tasks_and_prof
-00000470: 696c 6573 1b00 0000 7372 0000 0014 0904  iles....sr......
-00000480: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000490: 0102 0102 0102 fb04 fb08 0e04 0102 0102  ................
-000004a0: 0102 0102 0102 0102 0102 0102 010a 0102  ................
-000004b0: 0102 fb06 fb04 0f04 0102 0102 0102 0102  ................
-000004c0: 0102 0102 0102 0102 0102 0102 0102 fb04  ................
-000004d0: fb08 0d04 0102 0102 0102 0102 0102 0102  ................
-000004e0: 0102 0102 010a 0102 0102 fb06 fb04 0d72  ...............r
-000004f0: 1900 0000 da0c 6861 7665 5f68 6561 6469  ......have_headi
-00000500: 6e67 630b 0000 0000 0000 0000 0000 0013  ngc.............
-00000510: 0000 000f 0000 0043 0000 0073 4601 0000  .......C...sF...
-00000520: 6401 7d0b 6402 5c02 7d0c 7d0d 7400 a001  d.}.d.\.}.}.t...
-00000530: 7c01 7c07 7c0a 6403 1900 a103 5c02 7d0e  |.|.|.d.....\.}.
-00000540: 7d0f 7400 a002 7c01 7c02 6700 6401 7c0a  }.t...|.|.g.d.|.
-00000550: 6404 1900 a105 5c02 7d10 7d11 7c11 7403  d.....\.}.}.|.t.
-00000560: 6b02 7239 7403 9b00 6405 7c01 9b00 9d03  k.r9t...d.|.....
-00000570: 7d11 7400 a004 7c01 7c0a 6406 1900 a102  }.t...|.|.d.....
-00000580: 7236 7c06 7c0d 7c05 6603 5300 6407 7d0c  r6|.|.|.f.S.d.}.
-00000590: 6e02 7c11 7d0b 7c05 6408 3700 7d05 7c06  n.|.}.|.d.7.}.|.
-000005a0: 7364 7405 a006 7c09 7c03 7c00 6409 640a  sdt...|.|.|.d.d.
-000005b0: a105 0100 7405 a006 7c09 7c03 7c00 6409  ....t...|.|.|.d.
-000005c0: 7407 7c09 640b 6401 640c 6407 8305 a105  t.|.d.d.d.d.....
-000005d0: 0100 7405 a006 7c09 7c03 7c00 6408 6401  ..t...|.|.|.d.d.
-000005e0: a105 0100 6407 7d06 7c0c 7382 7c0e 7408  ....d.}.|.s.|.t.
-000005f0: 6b03 7282 7c03 640d 1900 727a 7c11 640e  k.r.|.d...rz|.d.
-00000600: 7c01 9b00 640f 7c0e 9b00 6410 9d05 3700  |...d.|...d...7.
-00000610: 7d11 6e08 7c11 640f 7c0e 9b00 6410 9d03  }.n.|.d.|...d...
-00000620: 3700 7d11 7c0c 728a 7c03 6411 1900 6412  7.}.|.r.|.d...d.
-00000630: 6b02 729e 7c11 6701 7d12 7400 a009 7c00  k.r.|.g.}.t...|.
-00000640: 7c0b 7c10 7c12 7c0e 6413 6700 7c08 7c09  |.|.|.|.d.g.|.|.
-00000650: 7c03 7c0a 7c04 6414 a10d 7d0d 7c06 7c0d  |.|.|.d...}.|.|.
-00000660: 7c05 6603 5300 2915 4e72 1100 0000 2902  |.f.S.).Nr....).
-00000670: 4646 da0c 616c 6c5f 7072 6f6a 6563 7473  FF..all_projects
-00000680: da09 616c 6c5f 7461 736b 737a 1526 6e62  ..all_tasksz.&nb
-00000690: 7370 3b26 6e62 7370 3b54 6173 6b20 4944  sp;&nbsp;Task ID
-000006a0: 3a20 da0a 616c 6c5f 7363 656e 6573 54e9  : ..all_scenesT.
-000006b0: 0100 0000 7201 0000 007a 043c 6872 3e72  ....r....z.<hr>r
-000006c0: 1000 0000 7a2b 5461 736b 7320 7468 6174  ....z+Tasks that
-000006d0: 2061 7265 206e 6f74 2063 616c 6c65 6420   are not called 
-000006e0: 6279 2061 6e79 2050 726f 6669 6c65 2e2e  by any Profile..
-000006f0: 2eda 0564 6562 7567 7a0f 2077 6974 6820  ...debugz. with 
-00000700: 5461 736b 2049 443a 207a 0f20 2e2e 2e69  Task ID: z. ...i
-00000710: 6e20 5072 6f6a 6563 7420 7a14 203c 656d  n Project z. <em
-00000720: 3e4e 6f20 5072 6f66 696c 653c 2f65 6d3e  >No Profile</em>
-00000730: da14 6469 7370 6c61 795f 6465 7461 696c  ..display_detail
-00000740: 5f6c 6576 656c e903 0000 00da 044e 6f6e  _level.......Non
-00000750: 6546 290a da05 7461 736b 73da 1967 6574  eF)...tasks..get
-00000760: 5f70 726f 6a65 6374 5f66 6f72 5f73 6f6c  _project_for_sol
-00000770: 6f5f 7461 736b da0d 6765 745f 7461 736b  o_task..get_task
-00000780: 5f6e 616d 6572 0600 0000 da0d 7461 736b  _namer......task
-00000790: 5f69 6e5f 7363 656e 6572 1400 0000 7215  _in_scener....r.
-000007a0: 0000 0072 0400 0000 7207 0000 00da 0b6f  ...r....r......o
-000007b0: 7574 7075 745f 7461 736b 2913 7208 0000  utput_task).r...
-000007c0: 00da 0774 6173 6b5f 6964 da0b 666f 756e  ...task_id..foun
-000007d0: 645f 7461 736b 7372 0d00 0000 720b 0000  d_tasksr....r...
-000007e0: 00da 1275 6e6e 616d 6564 5f74 6173 6b5f  ...unnamed_task_
-000007f0: 636f 756e 7472 1a00 0000 7209 0000 00da  countr....r.....
-00000800: 0768 6561 6469 6e67 720c 0000 00da 1061  .headingr......a
-00000810: 6c6c 5f74 6173 6b65 725f 6974 656d 73da  ll_tasker_items.
-00000820: 0d74 6865 5f74 6173 6b5f 6e61 6d65 5a0c  .the_task_nameZ.
-00000830: 756e 6b6e 6f77 6e5f 7461 736b da0d 7370  unknown_task..sp
-00000840: 6563 6966 6963 5f74 6173 6bda 0c70 726f  ecific_task..pro
-00000850: 6a65 6374 5f6e 616d 655a 0b74 6865 5f70  ject_nameZ.the_p
-00000860: 726f 6a65 6374 da0c 7461 736b 5f65 6c65  roject..task_ele
-00000870: 6d65 6e74 da09 7461 736b 5f6e 616d 65da  ment..task_name.
-00000880: 0974 6173 6b5f 6c69 7374 7217 0000 0072  .task_listr....r
-00000890: 1700 0000 7218 0000 00da 2170 726f 6365  ....r.....!proce
-000008a0: 7373 5f73 6f6c 6f5f 7461 736b 5f77 6974  ss_solo_task_wit
-000008b0: 685f 6e6f 5f70 726f 6669 6c65 6500 0000  h_no_profilee...
-000008c0: 737a 0000 0004 0d08 0104 030a 0108 ff04  sz..............
-000008d0: 050e 0108 ff08 030e 0110 020a 0106 0104  ................
-000008e0: 0208 0104 0304 010a 0104 ff04 0302 0102  ................
-000008f0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000900: 0102 fb04 fb04 0d0a 0104 ff04 030c 0208  ................
-00000910: 0102 0110 0106 ff10 0504 030c 0106 0204  ................
-00000920: 0302 0102 0102 0102 0102 0102 0102 0102  ................
-00000930: 0102 0102 0102 0102 0102 0104 f30a 0f72  ...............r
-00000940: 3300 0000 da10 666f 756e 645f 7461 736b  3.....found_task
-00000950: 735f 6c69 7374 722b 0000 0072 2c00 0000  s_listr+...r,...
-00000960: 6308 0000 0000 0000 0000 0000 000d 0000  c...............
-00000970: 000d 0000 0043 0000 0073 fa00 0000 6401  .....C...s....d.
-00000980: 7d08 6402 7d09 6403 7d0a 7c07 6404 1900  }.d.}.d.}.|.d...
-00000990: 4400 5d21 7d0b 7c04 6405 1900 7212 0100  D.]!}.|.d...r...
-000009a0: 6e1a 7c0b 7c02 7601 722b 7400 7c00 7c0b  n.|.|.v.r+t.|.|.
-000009b0: 7c02 7c03 7c04 7c08 7c0a 7c01 7c05 7c06  |.|.|.|.|.|.|.|.
-000009c0: 7c07 830b 5c03 7d0a 7d0c 7d08 7c0c 722b  |...\.}.}.}.|.r+
-000009d0: 0100 6e01 710a 7c08 6401 6b04 7265 7c03  ..n.q.|.d.k.re|.
-000009e0: 6406 1900 6401 6b04 723f 7401 a002 7c06  d...d.k.r?t...|.
-000009f0: 7c03 7c00 6401 6402 a105 0100 7401 a002  |.|.d.d.....t...
-00000a00: 7c06 7c03 7c00 6407 6402 a105 0100 7c04  |.|.|.d.d.....|.
-00000a10: 6405 1900 7365 7c03 6406 1900 6401 6b03  d...se|.d...d.k.
-00000a20: 7265 7401 a002 7c06 7c03 7c00 6401 7403  ret...|.|.|.d.t.
-00000a30: 7c06 6408 6402 6409 7c08 9b00 640a 9d03  |.d.d.d.|...d...
-00000a40: 640b 8305 a105 0100 7c09 640b 7500 7272  d.......|.d.u.rr
-00000a50: 7401 a002 7c06 7c03 7c00 6407 6402 a105  t...|.|.|.d.d...
-00000a60: 0100 7401 a002 7c06 7c03 7c00 6407 6402  ..t...|.|.|.d.d.
-00000a70: a105 0100 6400 5300 290c 4e72 0100 0000  ....d.S.).Nr....
-00000a80: 7211 0000 0046 721c 0000 0072 0f00 0000  r....Fr....r....
-00000a90: 7220 0000 0072 2100 0000 da12 756e 6b6e  r ...r!.....unkn
-00000aa0: 6f77 6e5f 7461 736b 5f63 6f6c 6f72 7a15  own_task_colorz.
-00000ab0: 5468 6572 6520 6172 6520 6120 746f 7461  There are a tota
-00000ac0: 6c20 6f66 207a 2d20 756e 6e61 6d65 6420  l of z- unnamed 
-00000ad0: 5461 736b 7320 6e6f 7420 6173 736f 6369  Tasks not associ
-00000ae0: 6174 6564 2077 6974 6820 6120 5072 6f66  ated with a Prof
-00000af0: 696c 6521 5429 0472 3300 0000 7214 0000  ile!T).r3...r...
-00000b00: 0072 1500 0000 7204 0000 0029 0d72 0800  .r....r....).r..
-00000b10: 0000 7209 0000 0072 3400 0000 720d 0000  ..r....r4...r...
-00000b20: 0072 0b00 0000 722b 0000 0072 0c00 0000  .r....r+...r....
-00000b30: 722c 0000 0072 2a00 0000 7231 0000 0072  r,...r*...r1...r
-00000b40: 1a00 0000 7228 0000 0072 2e00 0000 7217  ....r(...r....r.
-00000b50: 0000 0072 1700 0000 7218 0000 00da 2370  ...r....r.....#p
-00000b60: 726f 6365 7373 5f74 6173 6b73 5f6e 6f74  rocess_tasks_not
-00000b70: 5f63 616c 6c65 645f 6279 5f70 726f 6669  _called_by_profi
-00000b80: 6c65 c400 0000 7370 0000 0004 0a04 0104  le....sp........
-00000b90: 010c 0302 0102 0104 ff04 0308 0602 0202  ................
-00000ba0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000bb0: 0102 0102 0102 f508 ff04 0f04 0102 8008  ................
-00000bc0: 030c 0112 0104 010a 0104 ff06 0502 ff0c  ................
-00000bd0: 0204 0202 0102 0102 0102 0102 0102 0102  ................
-00000be0: 0102 010a 0202 0302 f804 fb08 1104 010a  ................
-00000bf0: 0104 ff04 040a 0104 ff04 0372 3600 0000  ...........r6...
-00000c00: 2915 da06 7479 7069 6e67 7202 0000 0072  )...typingr....r
-00000c10: 0300 0000 da15 6d61 7074 6173 6b65 722e  ......maptasker.
-00000c20: 7372 632e 6f75 7470 7574 6cda 0373 7263  src.outputl..src
-00000c30: da07 6f75 7470 7574 6c72 1400 0000 da13  ..outputlr......
-00000c40: 6d61 7074 6173 6b65 722e 7372 632e 7461  maptasker.src.ta
-00000c50: 736b 7372 2300 0000 da16 6d61 7074 6173  sksr#.....maptas
-00000c60: 6b65 722e 7372 632e 6672 6d74 6874 6d6c  ker.src.frmthtml
-00000c70: 7204 0000 00da 166d 6170 7461 736b 6572  r......maptasker
-00000c80: 2e73 7263 2e73 7973 636f 6e73 7472 0500  .src.sysconstr..
-00000c90: 0000 7206 0000 0072 0700 0000 da03 7374  ..r....r......st
-00000ca0: 72da 0464 6963 7472 1900 0000 da04 626f  r..dictr......bo
-00000cb0: 6f6c 7233 0000 0072 3600 0000 7217 0000  olr3...r6...r...
-00000cc0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000cd0: da08 3c6d 6f64 756c 653e 0100 0000 7358  ..<module>....sX
-00000ce0: 0000 0010 0d12 0212 010c 010c 010c 010c  ................
-00000cf0: 0102 0606 0102 ff0e 0202 fe06 0302 fd02  ................
-00000d00: 0402 fc02 0502 fb02 0602 fa02 070a f902  ................
-00000d10: 4a02 070a f902 5f06 0102 ff02 0202 fe06  J....._.........
-00000d20: 0302 fd02 0402 fc02 0502 fb02 0602 fa02  ................
-00000d30: 0702 f902 0802 f802 090e f7              ...........
+00000080: 6d0d 5a0d 0100 6406 6501 650e 1900 6407  m.Z...d.e.e...d.
+00000090: 6502 6501 650e 1900 6501 6602 1900 6408  e.e.e...e.f...d.
+000000a0: 6501 650e 1900 6409 650f 640a 650f 640b  e.e...d.e.d.e.d.
+000000b0: 650f 640c 6402 660e 640d 640e 8404 5a10  e.d.d.f.d.d...Z.
+000000c0: 640f 6511 6602 6410 6411 8404 5a12 6406  d.e.f.d.d...Z.d.
+000000d0: 6501 650e 1900 6407 6501 6412 6501 650e  e.e...d.e.d.e.e.
+000000e0: 1900 640b 650f 6409 650f 6413 650e 640a  ..d.e.d.e.d.e.d.
+000000f0: 650f 6414 650f 640c 6402 6612 6415 6416  e.d.e.d.d.f.d.d.
+00000100: 8404 5a13 6402 5300 2917 e900 0000 0029  ..Z.d.S.)......)
+00000110: 02da 044c 6973 74da 0555 6e69 6f6e 4e29  ...List..UnionN)
+00000120: 01da 0b66 6f72 6d61 745f 6874 6d6c 2901  ...format_html).
+00000130: da0a 4e4f 5f50 524f 4a45 4354 2901 da11  ..NO_PROJECT)...
+00000140: 554e 4b4e 4f57 4e5f 5441 534b 5f4e 414d  UNKNOWN_TASK_NAM
+00000150: 45da 0b6f 7574 7075 745f 6c69 7374 da16  E..output_list..
+00000160: 7072 6f6a 6563 7473 5f77 6974 685f 6e6f  projects_with_no
+00000170: 5f74 6173 6b73 da19 7072 6f6a 6563 7473  _tasks..projects
+00000180: 5f77 6974 686f 7574 5f70 726f 6669 6c65  _without_profile
+00000190: 73da 0b66 6f75 6e64 5f69 7465 6d73 da08  s..found_items..
+000001a0: 636f 6c6f 726d 6170 da0c 7072 6f67 7261  colormap..progra
+000001b0: 6d5f 6172 6773 da06 7265 7475 726e 6306  m_args..returnc.
+000001c0: 0000 0000 0000 0000 0000 0007 0000 000e  ................
+000001d0: 0000 0043 0000 0073 b800 0000 7400 7c01  ...C...s....t.|.
+000001e0: 8301 6401 6b04 7231 7c03 6402 1900 7331  ..d.k.r1|.d...s1
+000001f0: 7401 a002 7c04 7c05 7c00 6401 7403 7c04  t...|.|.|.d.t.|.
+00000200: 6403 6404 6405 6406 8305 a105 0100 7c01  d.d.d.d.......|.
+00000210: 4400 5d15 7d06 7401 a002 7c04 7c05 7c00  D.].}.t...|.|.|.
+00000220: 6407 7403 7c04 6403 6404 6408 7c06 9b00  d.t.|.d.d.d.|...
+00000230: 6409 9d03 6406 8305 a105 0100 711b 7c02  d...d.......q.|.
+00000240: 725a 7401 a002 7c04 7c05 7c00 6401 7403  rZt...|.|.|.d.t.
+00000250: 7c04 6403 640a 640b 6406 8305 a105 0100  |.d.d.d.d.......
+00000260: 7c02 4400 5d15 7d06 7401 a002 7c04 7c05  |.D.].}.t...|.|.
+00000270: 7c00 6407 7403 7c04 6403 6404 640c 7c06  |.d.t.|.d.d.d.|.
+00000280: 9b00 640d 9d03 6406 8305 a105 0100 7144  ..d...d.......qD
+00000290: 6400 5300 290e 4e72 0100 0000 da11 7369  d.S.).Nr......si
+000002a0: 6e67 6c65 5f74 6173 6b5f 666f 756e 64da  ngle_task_found.
+000002b0: 1774 7261 696c 696e 675f 636f 6d6d 656e  .trailing_commen
+000002c0: 7473 5f63 6f6c 6f72 da00 7a26 3c68 723e  ts_color..z&<hr>
+000002d0: 3c65 6d3e 5072 6f6a 6563 7473 2057 6974  <em>Projects Wit
+000002e0: 686f 7574 2054 6173 6b73 2e2e 2e3c 2f65  hout Tasks...</e
+000002f0: 6d3e 54e9 0400 0000 7a08 5072 6f6a 6563  m>T.....z.Projec
+00000300: 7420 7a1c 2068 6173 206e 6f20 3c65 6d3e  t z. has no <em>
+00000310: 4e61 6d65 643c 2f65 6d3e 2054 6173 6b73  Named</em> Tasks
+00000320: 7a04 3c62 723e 7a25 3c65 6d3e 5072 6f6a  z.<br>z%<em>Proj
+00000330: 6563 7473 2057 6974 686f 7574 2050 726f  ects Without Pro
+00000340: 6669 6c65 732e 2e2e 3c2f 656d 3e7a 093e  files...</em>z.>
+00000350: 5072 6f6a 6563 7420 7a10 2068 6173 206e  Project z. has n
+00000360: 6f20 5072 6f66 696c 6573 2904 da03 6c65  o Profiles)...le
+00000370: 6eda 0c62 7569 6c64 5f6f 7574 7075 74da  n..build_output.
+00000380: 096d 795f 6f75 7470 7574 7204 0000 0029  .my_outputr....)
+00000390: 0772 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
+000003a0: 720a 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+000003b0: 0469 7465 6da9 0072 1600 0000 fa77 2f55  .item..r.....w/U
+000003c0: 7365 7273 2f6d 696b 7275 6269 6e2f 4c69  sers/mikrubin/Li
+000003d0: 6272 6172 792f 436c 6f75 6453 746f 7261  brary/CloudStora
+000003e0: 6765 2f47 6f6f 676c 6544 7269 7665 2d6d  ge/GoogleDrive-m
+000003f0: 696b 7275 6269 6e40 676d 6169 6c2e 636f  ikrubin@gmail.co
+00000400: 6d2f 4d79 2044 7269 7665 2f50 7974 686f  m/My Drive/Pytho
+00000410: 6e2f 6d61 7074 6173 6b65 722f 6d61 7074  n/maptasker/mapt
+00000420: 6173 6b65 722f 7372 632f 7461 736b 756e  asker/src/taskun
+00000430: 6971 2e70 79da 2270 726f 6365 7373 5f6d  iq.py."process_m
+00000440: 6973 7369 6e67 5f74 6173 6b73 5f61 6e64  issing_tasks_and
+00000450: 5f70 726f 6669 6c65 731a 0000 0073 7200  _profiles....sr.
+00000460: 0000 1409 0401 0201 0201 0201 0201 0201  ................
+00000470: 0201 0201 0201 0201 0201 02fb 04fb 080e  ................
+00000480: 0401 0201 0201 0201 0201 0201 0201 0201  ................
+00000490: 0201 0a01 0201 02fb 06fb 040f 0401 0201  ................
+000004a0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+000004b0: 0201 02fb 04fb 080d 0401 0201 0201 0201  ................
+000004c0: 0201 0201 0201 0201 0201 0a01 0201 02fb  ................
+000004d0: 06fb 040d 7218 0000 00da 0c68 6176 655f  ....r......have_
+000004e0: 6865 6164 696e 6763 0b00 0000 0000 0000  headingc........
+000004f0: 0000 0000 1300 0000 0f00 0000 4300 0000  ............C...
+00000500: 7346 0100 0064 017d 0b64 025c 027d 0c7d  sF...d.}.d.\.}.}
+00000510: 0d74 00a0 017c 017c 077c 0a64 0319 00a1  .t...|.|.|.d....
+00000520: 035c 027d 0e7d 0f74 00a0 027c 017c 0267  .\.}.}.t...|.|.g
+00000530: 0064 017c 0a64 0419 00a1 055c 027d 107d  .d.|.d.....\.}.}
+00000540: 117c 1174 036b 0272 3974 039b 0064 057c  .|.t.k.r9t...d.|
+00000550: 019b 009d 037d 1174 00a0 047c 017c 0a64  .....}.t...|.|.d
+00000560: 0619 00a1 0272 367c 067c 0d7c 0566 0353  .....r6|.|.|.f.S
+00000570: 0064 077d 0c6e 027c 117d 0b7c 0564 0837  .d.}.n.|.}.|.d.7
+00000580: 007d 057c 0673 6474 05a0 067c 097c 037c  .}.|.sdt...|.|.|
+00000590: 0064 0964 0aa1 0501 0074 05a0 067c 097c  .d.d.....t...|.|
+000005a0: 037c 0064 0974 077c 0964 0b64 0164 0c64  .|.d.t.|.d.d.d.d
+000005b0: 0783 05a1 0501 0074 05a0 067c 097c 037c  .......t...|.|.|
+000005c0: 0064 0864 01a1 0501 0064 077d 067c 0c73  .d.d.....d.}.|.s
+000005d0: 827c 0e74 086b 0372 827c 0364 0d19 0072  .|.t.k.r.|.d...r
+000005e0: 7a7c 1164 0e7c 019b 0064 0f7c 0e9b 0064  z|.d.|...d.|...d
+000005f0: 109d 0537 007d 116e 087c 1164 0f7c 0e9b  ...7.}.n.|.d.|..
+00000600: 0064 109d 0337 007d 117c 0c72 8a7c 0364  .d...7.}.|.r.|.d
+00000610: 1119 0064 126b 0272 9e7c 1167 017d 1274  ...d.k.r.|.g.}.t
+00000620: 00a0 097c 007c 0b7c 107c 127c 0e64 1367  ...|.|.|.|.|.d.g
+00000630: 007c 087c 097c 037c 0a7c 0464 14a1 0d7d  .|.|.|.|.|.d...}
+00000640: 0d7c 067c 0d7c 0566 0353 0029 154e 7210  .|.|.|.f.S.).Nr.
+00000650: 0000 0029 0246 46da 0c61 6c6c 5f70 726f  ...).FF..all_pro
+00000660: 6a65 6374 73da 0961 6c6c 5f74 6173 6b73  jects..all_tasks
+00000670: 7a15 266e 6273 703b 266e 6273 703b 5461  z.&nbsp;&nbsp;Ta
+00000680: 736b 2049 443a 20da 0a61 6c6c 5f73 6365  sk ID: ..all_sce
+00000690: 6e65 7354 e901 0000 0072 0100 0000 7a04  nesT.....r....z.
+000006a0: 3c68 723e 720f 0000 007a 2b54 6173 6b73  <hr>r....z+Tasks
+000006b0: 2074 6861 7420 6172 6520 6e6f 7420 6361   that are not ca
+000006c0: 6c6c 6564 2062 7920 616e 7920 5072 6f66  lled by any Prof
+000006d0: 696c 652e 2e2e da05 6465 6275 677a 0f20  ile.....debugz. 
+000006e0: 7769 7468 2054 6173 6b20 4944 3a20 7a0f  with Task ID: z.
+000006f0: 202e 2e2e 696e 2050 726f 6a65 6374 207a   ...in Project z
+00000700: 1420 3c65 6d3e 4e6f 2050 726f 6669 6c65  . <em>No Profile
+00000710: 3c2f 656d 3eda 1464 6973 706c 6179 5f64  </em>..display_d
+00000720: 6574 6169 6c5f 6c65 7665 6ce9 0300 0000  etail_level.....
+00000730: da04 4e6f 6e65 4629 0ada 0574 6173 6b73  ..NoneF)...tasks
+00000740: da19 6765 745f 7072 6f6a 6563 745f 666f  ..get_project_fo
+00000750: 725f 736f 6c6f 5f74 6173 6bda 0d67 6574  r_solo_task..get
+00000760: 5f74 6173 6b5f 6e61 6d65 7206 0000 00da  _task_namer.....
+00000770: 0d74 6173 6b5f 696e 5f73 6365 6e65 7213  .task_in_scener.
+00000780: 0000 0072 1400 0000 7204 0000 0072 0500  ...r....r....r..
+00000790: 0000 da0b 6f75 7470 7574 5f74 6173 6b29  ....output_task)
+000007a0: 1372 0700 0000 da07 7461 736b 5f69 64da  .r......task_id.
+000007b0: 0b66 6f75 6e64 5f74 6173 6b73 720c 0000  .found_tasksr...
+000007c0: 0072 0a00 0000 da12 756e 6e61 6d65 645f  .r......unnamed_
+000007d0: 7461 736b 5f63 6f75 6e74 7219 0000 0072  task_countr....r
+000007e0: 0800 0000 da07 6865 6164 696e 6772 0b00  ......headingr..
+000007f0: 0000 da10 616c 6c5f 7461 736b 6572 5f69  ....all_tasker_i
+00000800: 7465 6d73 da0d 7468 655f 7461 736b 5f6e  tems..the_task_n
+00000810: 616d 655a 0c75 6e6b 6e6f 776e 5f74 6173  ameZ.unknown_tas
+00000820: 6bda 0d73 7065 6369 6669 635f 7461 736b  k..specific_task
+00000830: da0c 7072 6f6a 6563 745f 6e61 6d65 5a0b  ..project_nameZ.
+00000840: 7468 655f 7072 6f6a 6563 74da 0c74 6173  the_project..tas
+00000850: 6b5f 656c 656d 656e 74da 0974 6173 6b5f  k_element..task_
+00000860: 6e61 6d65 da09 7461 736b 5f6c 6973 7472  name..task_listr
+00000870: 1600 0000 7216 0000 0072 1700 0000 da21  ....r....r.....!
+00000880: 7072 6f63 6573 735f 736f 6c6f 5f74 6173  process_solo_tas
+00000890: 6b5f 7769 7468 5f6e 6f5f 7072 6f66 696c  k_with_no_profil
+000008a0: 6564 0000 0073 7a00 0000 040d 0801 0403  ed...sz.........
+000008b0: 0a01 08ff 0405 0e01 08ff 0803 0e01 1002  ................
+000008c0: 0a01 0601 0402 0801 0403 0401 0a01 04ff  ................
+000008d0: 0403 0201 0201 0201 0201 0201 0201 0201  ................
+000008e0: 0201 0201 0201 02fb 04fb 040d 0a01 04ff  ................
+000008f0: 0403 0c02 0801 0201 1001 06ff 1005 0403  ................
+00000900: 0c01 0602 0403 0201 0201 0201 0201 0201  ................
+00000910: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000920: 04f3 0a0f 7232 0000 00da 1066 6f75 6e64  ....r2.....found
+00000930: 5f74 6173 6b73 5f6c 6973 7472 2a00 0000  _tasks_listr*...
+00000940: 722b 0000 0063 0800 0000 0000 0000 0000  r+...c..........
+00000950: 0000 0d00 0000 0d00 0000 4300 0000 73fa  ..........C...s.
+00000960: 0000 0064 017d 0864 027d 0964 037d 0a7c  ...d.}.d.}.d.}.|
+00000970: 0764 0419 0044 005d 217d 0b7c 0464 0519  .d...D.]!}.|.d..
+00000980: 0072 1201 006e 1a7c 0b7c 0276 0172 2b74  .r...n.|.|.v.r+t
+00000990: 007c 007c 0b7c 027c 037c 047c 087c 0a7c  .|.|.|.|.|.|.|.|
+000009a0: 017c 057c 067c 0783 0b5c 037d 0a7d 0c7d  .|.|.|...\.}.}.}
+000009b0: 087c 0c72 2b01 006e 0171 0a7c 0864 016b  .|.r+..n.q.|.d.k
+000009c0: 0472 657c 0364 0619 0064 016b 0472 3f74  .re|.d...d.k.r?t
+000009d0: 01a0 027c 067c 037c 0064 0164 02a1 0501  ...|.|.|.d.d....
+000009e0: 0074 01a0 027c 067c 037c 0064 0764 02a1  .t...|.|.|.d.d..
+000009f0: 0501 007c 0464 0519 0073 657c 0364 0619  ...|.d...se|.d..
+00000a00: 0064 016b 0372 6574 01a0 027c 067c 037c  .d.k.ret...|.|.|
+00000a10: 0064 0174 037c 0664 0864 0264 097c 089b  .d.t.|.d.d.d.|..
+00000a20: 0064 0a9d 0364 0b83 05a1 0501 007c 0964  .d...d.......|.d
+00000a30: 0b75 0072 7274 01a0 027c 067c 037c 0064  .u.rrt...|.|.|.d
+00000a40: 0764 02a1 0501 0074 01a0 027c 067c 037c  .d.....t...|.|.|
+00000a50: 0064 0764 02a1 0501 0064 0053 0029 0c4e  .d.d.....d.S.).N
+00000a60: 7201 0000 0072 1000 0000 4672 1b00 0000  r....r....Fr....
+00000a70: 720e 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+00000a80: 1275 6e6b 6e6f 776e 5f74 6173 6b5f 636f  .unknown_task_co
+00000a90: 6c6f 727a 1554 6865 7265 2061 7265 2061  lorz.There are a
+00000aa0: 2074 6f74 616c 206f 6620 7a2d 2075 6e6e   total of z- unn
+00000ab0: 616d 6564 2054 6173 6b73 206e 6f74 2061  amed Tasks not a
+00000ac0: 7373 6f63 6961 7465 6420 7769 7468 2061  ssociated with a
+00000ad0: 2050 726f 6669 6c65 2154 2904 7232 0000   Profile!T).r2..
+00000ae0: 0072 1300 0000 7214 0000 0072 0400 0000  .r....r....r....
+00000af0: 290d 7207 0000 0072 0800 0000 7233 0000  ).r....r....r3..
+00000b00: 0072 0c00 0000 720a 0000 0072 2a00 0000  .r....r....r*...
+00000b10: 720b 0000 0072 2b00 0000 7229 0000 0072  r....r+...r)...r
+00000b20: 3000 0000 7219 0000 0072 2700 0000 722d  0...r....r'...r-
+00000b30: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000b40: 0000 da23 7072 6f63 6573 735f 7461 736b  ...#process_task
+00000b50: 735f 6e6f 745f 6361 6c6c 6564 5f62 795f  s_not_called_by_
+00000b60: 7072 6f66 696c 65c3 0000 0073 7000 0000  profile....sp...
+00000b70: 040a 0401 0401 0c03 0201 0201 04ff 0403  ................
+00000b80: 0806 0202 0201 0201 0201 0201 0201 0201  ................
+00000b90: 0201 0201 0201 0201 0201 02f5 08ff 040f  ................
+00000ba0: 0401 0280 0803 0c01 1201 0401 0a01 04ff  ................
+00000bb0: 0605 02ff 0c02 0402 0201 0201 0201 0201  ................
+00000bc0: 0201 0201 0201 0201 0a02 0203 02f8 04fb  ................
+00000bd0: 0811 0401 0a01 04ff 0404 0a01 04ff 0403  ................
+00000be0: 7235 0000 0029 14da 0674 7970 696e 6772  r5...)...typingr
+00000bf0: 0200 0000 7203 0000 00da 156d 6170 7461  ....r......mapta
+00000c00: 736b 6572 2e73 7263 2e6f 7574 7075 746c  sker.src.outputl
+00000c10: da03 7372 63da 076f 7574 7075 746c 7213  ..src..outputlr.
+00000c20: 0000 00da 136d 6170 7461 736b 6572 2e73  .....maptasker.s
+00000c30: 7263 2e74 6173 6b73 7222 0000 00da 166d  rc.tasksr".....m
+00000c40: 6170 7461 736b 6572 2e73 7263 2e66 726d  aptasker.src.frm
+00000c50: 7468 746d 6c72 0400 0000 da16 6d61 7074  thtmlr......mapt
+00000c60: 6173 6b65 722e 7372 632e 7379 7363 6f6e  asker.src.syscon
+00000c70: 7374 7205 0000 0072 0600 0000 da03 7374  str....r......st
+00000c80: 72da 0464 6963 7472 1800 0000 da04 626f  r..dictr......bo
+00000c90: 6f6c 7232 0000 0072 3500 0000 7216 0000  olr2...r5...r...
+00000ca0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000cb0: da08 3c6d 6f64 756c 653e 0100 0000 7356  ..<module>....sV
+00000cc0: 0000 0010 0d12 0212 010c 010c 010c 0102  ................
+00000cd0: 0606 0102 ff0e 0202 fe06 0302 fd02 0402  ................
+00000ce0: fc02 0502 fb02 0602 fa02 070a f902 4a02  ..............J.
+00000cf0: 070a f902 5f06 0102 ff02 0202 fe06 0302  ...._...........
+00000d00: fd02 0402 fc02 0502 fb02 0602 fa02 0702  ................
+00000d10: f902 0802 f802 090e f7                   .........
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/userintr.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/userintr.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 10 14:44:20 2023 UTC, .py size: 30601 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-00000000: 6f0d 0d0a 0000 0000 c420 3464 8977 0000  o........ 4d.w..
+00000000: 6f0d 0d0a 0000 0000 a390 4164 047c 0000  o.........Ad.|..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6501  ..d.d.l.m.Z...e.
 00000070: a00a 6406 a101 0100 6501 a00b 6407 a101  ..d.....e...d...
 00000080: 0100 6408 5a0c 4700 6409 640a 8400 640a  ..d.Z.G.d.d...d.
 00000090: 6501 6a0d 8303 5a0e 6401 5300 290b e900  e.j...Z.d.S.)...
 000000a0: 0000 004e 2901 da04 5061 7468 2901 da08  ...N)...Path)...
 000000b0: 4173 6b43 6f6c 6f72 2901 da11 7361 7665  AskColor)...save
 000000c0: 5f72 6573 746f 7265 5f61 7267 7329 01da  _restore_args)..
 000000d0: 1454 5950 4553 5f4f 465f 434f 4c4f 525f  .TYPES_OF_COLOR_
 000000e0: 4e41 4d45 53da 0653 7973 7465 6d5a 0462  NAMES..SystemZ.b
-000000f0: 6c75 6561 6706 0000 4d61 7054 6173 6b65  lueag...MapTaske
+000000f0: 6c75 6561 9e06 0000 4d61 7054 6173 6b65  luea....MapTaske
 00000100: 7220 6469 7370 6c61 7973 2079 6f75 7220  r displays your 
 00000110: 416e 6472 6f69 6420 5461 736b 6572 2063  Android Tasker c
 00000120: 6f6e 6669 6775 7261 7469 6f6e 2062 6173  onfiguration bas
 00000130: 6564 206f 6e20 796f 7572 2075 706c 6f61  ed on your uploa
 00000140: 6465 6420 5461 736b 6572 2062 6163 6b75  ded Tasker backu
 00000150: 7020 6669 6c65 2028 652e 672e 2022 6261  p file (e.g. "ba
 00000160: 636b 7570 2e78 6d6c 2229 2e20 2054 6865  ckup.xml").  The
@@ -78,810 +78,859 @@
 000004d0: 7465 6d20 6465 6661 756c 742e 0a0a 2a20  tem default...* 
 000004e0: 5265 7365 7420 4f70 7469 6f6e 733a 2043  Reset Options: C
 000004f0: 6c65 6172 2065 7665 7279 7468 696e 6720  lear everything 
 00000500: 616e 6420 7374 6172 7420 616e 6577 2e0a  and start anew..
 00000510: 0a2a 2052 756e 3a20 5275 6e20 7468 6520  .* Run: Run the 
 00000520: 7072 6f67 7261 6d20 7769 7468 2074 6865  program with the
 00000530: 2073 6574 7469 6e67 7320 7072 6f76 6964   settings provid
-00000540: 6564 2e0a 0a2a 2053 7065 6369 6669 6320  ed...* Specific 
-00000550: 4e61 6d65 2074 6162 3a20 656e 7465 7220  Name tab: enter 
-00000560: 6120 7369 6e67 6c65 2c20 7370 6563 6966  a single, specif
-00000570: 6963 206e 616d 6564 2069 7465 6d20 746f  ic named item to
-00000580: 2064 6973 706c 6179 2e2e 2e0a 2020 202d   display....   -
-00000590: 2050 726f 6a65 6374 204e 616d 653a 2065   Project Name: e
-000005a0: 6e74 6572 2061 2073 7065 6369 6669 6320  nter a specific 
-000005b0: 5072 6f6a 6563 7420 746f 2064 6973 706c  Project to displ
-000005c0: 6179 0a20 2020 2d20 5072 6f66 696c 6520  ay.   - Profile 
+00000540: 6564 2e0a 2a20 5265 5275 6e3a 2052 756e  ed..* ReRun: Run
+00000550: 206d 756c 7469 706c 6520 7469 6d65 7320   multiple times 
+00000560: 2877 6974 6820 6469 6666 6572 656e 7420  (with different 
+00000570: 7365 7474 696e 6773 292e 0a0a 2a20 5370  settings)...* Sp
+00000580: 6563 6966 6963 204e 616d 6520 7461 623a  ecific Name tab:
+00000590: 2065 6e74 6572 2061 2073 696e 676c 652c   enter a single,
+000005a0: 2073 7065 6369 6669 6320 6e61 6d65 6420   specific named 
+000005b0: 6974 656d 2074 6f20 6469 7370 6c61 792e  item to display.
+000005c0: 2e2e 0a20 2020 2d20 5072 6f6a 6563 7420  ...   - Project 
 000005d0: 4e61 6d65 3a20 656e 7465 7220 6120 7370  Name: enter a sp
-000005e0: 6563 6966 6963 2050 726f 6669 6c65 2074  ecific Profile t
-000005f0: 6f20 6469 7370 6c61 790a 2020 202d 2054  o display.   - T
-00000600: 6173 6b20 4e61 6d65 3a20 656e 7465 7220  ask Name: enter 
-00000610: 6120 7370 6563 6966 6963 2054 6173 6b20  a specific Task 
-00000620: 746f 2064 6973 706c 6179 0a20 2020 2854  to display.   (T
-00000630: 6865 7365 2074 6872 6565 2061 7265 2065  hese three are e
-00000640: 7863 6c75 7369 7665 3a20 656e 7465 7220  xclusive: enter 
-00000650: 6f6e 6520 6f6e 6c79 290a 0a2a 2043 6f6c  one only)..* Col
-00000660: 6f72 7320 7461 623a 2073 656c 6563 7420  ors tab: select 
-00000670: 636f 6c6f 7273 2066 6f72 2076 6172 696f  colors for vario
-00000680: 7573 2065 6c65 6d65 6e74 7320 6f66 2074  us elements of t
-00000690: 6865 2064 6973 706c 6179 0a20 2020 2020  he display.     
-000006a0: 2020 2020 2020 2020 2028 652e 672e 2063           (e.g. c
-000006b0: 6f6c 6f72 2066 6f72 2050 726f 6a65 6374  olor for Project
-000006c0: 732c 2050 726f 6669 6c65 732c 2054 6173  s, Profiles, Tas
-000006d0: 6b73 2c20 6574 632e 290a 0a2a 2045 7869  ks, etc.)..* Exi
-000006e0: 743a 2045 7869 7420 7468 6520 7072 6f67  t: Exit the prog
-000006f0: 7261 6d20 2871 7569 7429 2e0a 0a4e 6f74  ram (quit)...Not
-00000700: 653a 2059 6f75 2077 696c 6c20 6265 2070  e: You will be p
-00000710: 726f 6d70 7465 6420 746f 2069 6465 6e74  rompted to ident
-00000720: 6966 7920 796f 7572 2054 6173 6b65 7220  ify your Tasker 
-00000730: 6261 636b 7570 2066 696c 6520 6f6e 6365  backup file once
-00000740: 0a20 2020 2020 2079 6f75 2068 6974 2074  .      you hit t
-00000750: 6865 2027 5275 6e27 2062 7574 746f 6e63  he 'Run' buttonc
-00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000770: 0300 0000 0000 0000 73dc 0000 0065 005a  ........s....e.Z
-00000780: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
-00000790: 0364 0365 0466 0264 0464 0584 045a 0564  .d.e.f.d.d...Z.d
-000007a0: 0664 0784 005a 0664 0864 0984 005a 0764  .d...Z.d.d...Z.d
-000007b0: 0a64 0b84 005a 0864 0c64 0d84 005a 0964  .d...Z.d.d...Z.d
-000007c0: 0e64 0f84 005a 0a64 1064 1184 005a 0b64  .d...Z.d.d...Z.d
-000007d0: 1265 0c66 0264 1364 1484 045a 0d64 1565  .e.f.d.d...Z.d.e
-000007e0: 0c66 0264 1664 1784 045a 0e64 1865 0c66  .f.d.d...Z.d.e.f
-000007f0: 0264 1964 1a84 045a 0f64 1b64 1c84 005a  .d.d...Z.d.d...Z
-00000800: 1064 1d64 1e84 005a 1164 1f64 2084 005a  .d.d...Z.d.d ..Z
-00000810: 1264 2164 2284 005a 1364 2364 2484 005a  .d!d"..Z.d#d$..Z
-00000820: 1464 2564 2684 005a 1564 2764 2884 005a  .d%d&..Z.d'd(..Z
-00000830: 1664 2964 2a84 005a 1764 2b64 2c84 005a  .d)d*..Z.d+d,..Z
-00000840: 1864 2d64 2e84 005a 1964 2f64 3084 005a  .d-d...Z.d/d0..Z
-00000850: 1a87 0004 005a 1b53 0029 31da 054d 7947  .....Z.S.)1..MyG
-00000860: 7569 6301 0000 0000 0000 0000 0000 0001  uic.............
-00000870: 0000 0008 0000 0003 0000 0073 0205 0000  ...........s....
-00000880: 7400 8300 a001 a100 0100 7c00 a002 6401  t.........|...d.
-00000890: a101 0100 7c00 a003 6402 a101 0100 7c00  ....|...d.....|.
-000008a0: 6a04 6403 6403 6404 8d02 0100 7c00 6a04  j.d.d.d.....|.j.
-000008b0: 6405 6406 6404 8d02 0100 7c00 6a05 6406  d.d.d.....|.j.d.
-000008c0: 6403 6404 8d02 0100 7406 6a07 7c00 6407  d.d.....t.j.|.d.
-000008d0: 6406 6408 8d03 7c00 5f08 7c00 6a08 6a09  d.d...|._.|.j.j.
-000008e0: 6406 6406 6409 640a 640b 8d04 0100 7c00  d.d.d.d.d.....|.
-000008f0: 6a08 6a05 640c 6403 6404 8d02 0100 7406  j.j.d.d.d.....t.
-00000900: 6a0a 7c00 6a08 640d 7406 6a0b 640e 640f  j.|.j.d.t.j.d.d.
-00000910: 6410 8d02 6411 8d03 7c00 5f0c 7c00 6a0c  d...d...|._.|.j.
-00000920: 6a09 6406 6406 640e 6412 6413 8d04 0100  j.d.d.d.d.d.....
-00000930: 7406 6a0a 7c00 6a08 6414 6415 6416 8d03  t.j.|.j.d.d.d...
-00000940: 7c00 5f0d 7c00 6a0d 6a09 6403 6406 640e  |._.|.j.j.d.d.d.
-00000950: 6417 6413 8d04 0100 7406 6a0e 7c00 6a08  d.d.....t.j.|.j.
-00000960: 6700 6418 a201 7c00 6a0f 6419 8d03 7c00  g.d...|.j.d...|.
-00000970: 5f10 7c00 6a10 6a09 641a 6406 640e 6417  _.|.j.j.d.d.d.d.
-00000980: 6413 8d04 0100 7406 6a11 7c00 6a08 7c00  d.....t.j.|.j.|.
-00000990: 6a12 641b 641c 641d 641e 8d05 7c00 5f13  j.d.d.d.d...|._.
-000009a0: 7c00 6a13 6a09 641f 6406 640e 6420 6415  |.j.j.d.d.d.d d.
-000009b0: 6421 8d05 0100 7406 6a11 7c00 6a08 7c00  d!....t.j.|.j.|.
-000009c0: 6a14 6422 641c 641d 641e 8d05 7c00 5f15  j.d"d.d.d...|._.
-000009d0: 7c00 6a15 6a09 6423 6406 640e 6420 6415  |.j.j.d#d.d.d d.
-000009e0: 6421 8d05 0100 7406 6a11 7c00 6a08 7c00  d!....t.j.|.j.|.
-000009f0: 6a16 6424 641c 641d 641e 8d05 7c00 5f17  j.d$d.d.d...|._.
-00000a00: 7c00 6a17 6a09 6425 6406 640e 6420 6415  |.j.j.d%d.d.d d.
-00000a10: 6421 8d05 0100 7406 6a18 7c00 6a08 6426  d!....t.j.|.j.d&
-00000a20: 641a 6427 7c00 6a19 6428 8d05 7c00 5f1a  d.d'|.j.d(..|._.
-00000a30: 7c00 6a1a 6a09 6409 6406 6420 640e 6429  |.j.j.d.d.d d.d)
-00000a40: 6421 8d05 0100 7406 6a18 7c00 6a08 6426  d!....t.j.|.j.d&
-00000a50: 641a 642a 7c00 6a1b 6428 8d05 7c00 5f1c  d.d*|.j.d(..|._.
-00000a60: 7c00 6a1c 6a09 642b 6406 6420 6406 642c  |.j.j.d+d.d d.d,
-00000a70: 6421 8d05 0100 7406 6a0a 7c00 6a08 642d  d!....t.j.|.j.d-
-00000a80: 6415 6416 8d03 7c00 5f1d 7c00 6a1d 6a09  d.d...|._.|.j.j.
-00000a90: 642e 6406 640e 6420 6413 8d04 0100 7406  d.d.d.d d.....t.
-00000aa0: 6a0e 7c00 6a08 6700 642f a201 7c00 6a1e  j.|.j.g.d/..|.j.
-00000ab0: 6419 8d03 7c00 5f1f 7c00 6a1f 6a09 640c  d...|._.|.j.j.d.
-00000ac0: 6406 6406 642c 6430 8d04 0100 7406 6a18  d.d.d,d0....t.j.
-00000ad0: 7c00 6431 641a 6432 7c00 6a20 6433 8d05  |.d1d.d2|.j d3..
-00000ae0: 7c00 5f21 7c00 6a21 6a09 6409 6406 6434  |._!|.j!j.d.d.d4
-00000af0: 6434 640a 6421 8d05 0100 7406 6a18 7c00  d4d.d!....t.j.|.
-00000b00: 6431 641a 6435 7c00 6a22 6436 6437 8d06  d1d.d5|.j"d6d7..
-00000b10: 7c00 5f23 7c00 6a23 6a09 642b 6406 6434  |._#|.j#j.d+d.d4
-00000b20: 6434 640a 6421 8d05 0100 7406 6a18 7c00  d4d.d!....t.j.|.
-00000b30: 6431 641a 6438 7c00 6a24 6439 6437 8d06  d1d.d8|.j$d9d7..
-00000b40: 7c00 5f25 7c00 6a25 6a09 642b 641a 6434  |._%|.j%j.d+d.d4
-00000b50: 6434 6413 8d04 0100 7406 6a26 7c00 643a  d4d.....t.j&|.d:
-00000b60: 643b 643c 8d03 7c00 5f27 7c00 6a27 6a28  d;d<..|._'|.j'j(
-00000b70: 6426 643d 8d01 0100 7c00 6a27 6a09 6406  d&d=....|.j'j.d.
-00000b80: 6403 643e 643e 640a 6421 8d05 0100 7406  d.d>d>d.d!....t.
-00000b90: 6a29 7c00 643b 6426 643f 8d03 7c00 5f2a  j)|.d;d&d?..|._*
-00000ba0: 7c00 6a2a 6a09 6406 641a 643e 643e 640a  |.j*j.d.d.d>d>d.
-00000bb0: 6421 8d05 0100 7c00 6a2a a02b 6440 a101  d!....|.j*.+d@..
-00000bc0: 0100 7c00 6a2a a02b 6441 a101 0100 7c00  ..|.j*.+dA....|.
-00000bd0: 6a2a a02b 6442 a101 0100 7c00 6a2a a02c  j*.+dB....|.j*.,
-00000be0: 6440 a101 6a04 6406 6403 6404 8d02 0100  d@..j.d.d.d.....
-00000bf0: 7c00 6a2a a02c 6441 a101 6a04 6406 6403  |.j*.,dA..j.d.d.
-00000c00: 6404 8d02 0100 7406 6a2d 7c00 6a2a a02c  d.....t.j-|.j*.,
-00000c10: 6440 a101 6443 7c00 6a2e 6426 6444 6445  d@..dC|.j.d&dDdE
-00000c20: 8d05 7c00 5f2f 7c00 6a2f 6a09 6403 6406  ..|._/|.j/j.d.d.
-00000c30: 640e 6446 640a 6421 8d05 0100 7406 6a2d  d.dFd.d!....t.j-
-00000c40: 7c00 6a2a a02c 6440 a101 6447 7c00 6a30  |.j*.,d@..dG|.j0
-00000c50: 6426 6444 6445 8d05 7c00 5f31 7c00 6a31  d&dDdE..|._1|.j1
-00000c60: 6a09 641a 6406 640e 6446 640a 6421 8d05  j.d.d.d.dFd.d!..
-00000c70: 0100 7406 6a2d 7c00 6a2a a02c 6440 a101  ..t.j-|.j*.,d@..
-00000c80: 6448 7c00 6a32 6426 6444 6445 8d05 7c00  dH|.j2d&dDdE..|.
-00000c90: 5f33 7c00 6a33 6a09 641f 6406 640e 6446  _3|.j3j.d.d.d.dF
-00000ca0: 640a 6421 8d05 0100 7406 6a0a 7c00 6a2a  d.d!....t.j.|.j*
-00000cb0: a02c 6440 a101 6449 6415 6416 8d03 7c00  .,d@..dId.d...|.
-00000cc0: 5f34 7c00 6a34 6a09 6423 6406 640e 6446  _4|.j4j.d#d.d.dF
-00000cd0: 6413 8d04 0100 7406 6a0a 7c00 6a2a a02c  d.....t.j.|.j*.,
-00000ce0: 6441 a101 644a 644b 8d02 7c00 5f35 7c00  dA..dJdK..|._5|.
-00000cf0: 6a35 6a09 6406 6406 6406 6406 6413 8d04  j5j.d.d.d.d.d...
-00000d00: 0100 7406 6a0e 7c00 6a2a a02c 6441 a101  ..t.j.|.j*.,dA..
-00000d10: 6700 644c a201 7c00 6a36 6419 8d03 7c00  g.dL..|.j6d...|.
-00000d20: 5f37 7c00 6a37 6a09 6403 6406 640e 6446  _7|.j7j.d.d.d.dF
-00000d30: 6413 8d04 0100 7406 6a11 7c00 6a2a a02c  d.....t.j.|.j*.,
-00000d40: 6442 a101 644d 7c00 6a38 641c 641d 644e  dB..dM|.j8d.d.dN
-00000d50: 8d05 7c00 5f39 7c00 6a27 6a28 6426 644f  ..|._9|.j'j(d&dO
-00000d60: 8d01 0100 7c00 6a39 6a3a 640e 6420 6450  ....|.j9j:d.d dP
-00000d70: 8d02 0100 7c00 a03b 641c a101 0100 6400  ....|..;d.....d.
-00000d80: 5300 2951 4e7a 194d 6170 5461 736b 6572  S.)QNz.MapTasker
-00000d90: 2052 756e 7469 6d65 204f 7074 696f 6e73   Runtime Options
-00000da0: 5a08 3131 3030 7836 3030 e901 0000 0029  Z.1100x600.....)
-00000db0: 01da 0677 6569 6768 7429 02e9 0200 0000  ...weight)......
-00000dc0: e903 0000 0072 0100 0000 e98c 0000 0029  .....r.........)
-00000dd0: 02da 0577 6964 7468 5a0d 636f 726e 6572  ...widthZ.corner
-00000de0: 5f72 6164 6975 73e9 0600 0000 da04 6e73  _radius.......ns
-00000df0: 6577 2904 da03 726f 77da 0663 6f6c 756d  ew)...row..colum
-00000e00: 6e5a 0772 6f77 7370 616e da06 7374 6963  nZ.rowspan..stic
-00000e10: 6b79 e909 0000 00da 094d 6170 5461 736b  ky.......MapTask
-00000e20: 6572 e914 0000 005a 0462 6f6c 6429 02da  er.....Z.bold)..
-00000e30: 0473 697a 6572 0900 0000 2902 da04 7465  .sizer....)...te
-00000e40: 7874 da04 666f 6e74 2902 7215 0000 00e9  xt..font).r.....
-00000e50: 0a00 0000 a904 7210 0000 0072 1100 0000  ......r....r....
-00000e60: da04 7061 6478 da04 7061 6479 7a15 4469  ..padx..padyz.Di
-00000e70: 7370 6c61 7920 4465 7461 696c 204c 6576  splay Detail Lev
-00000e80: 656c 3ada 0177 2902 7217 0000 00da 0661  el:..w).r......a
-00000e90: 6e63 686f 7229 0272 1900 0000 7201 0000  nchor).r....r...
-00000ea0: 00a9 04da 0130 da01 31da 0132 da01 3329  .....0..1..2..3)
-00000eb0: 02da 0676 616c 7565 73da 0763 6f6d 6d61  ...values..comma
-00000ec0: 6e64 720a 0000 007a 1244 6973 706c 6179  ndr....z.Display
-00000ed0: 2043 6f6e 6469 7469 6f6e 7354 4629 0472   ConditionsTF).r
-00000ee0: 2500 0000 7217 0000 00da 076f 6e76 616c  %...r......onval
-00000ef0: 7565 da08 6f66 6676 616c 7565 720b 0000  ue..offvaluer...
-00000f00: 0072 1900 0000 2905 7210 0000 0072 1100  .r....).r....r..
-00000f10: 0000 721b 0000 0072 1c00 0000 7212 0000  ..r....r....r...
-00000f20: 007a 1644 6973 706c 6179 2054 6173 6b65  .z.Display Taske
-00000f30: 724e 6574 2049 6e66 6fe9 0400 0000 7a1a  rNet Info.....z.
-00000f40: 4469 7370 6c61 7920 5461 736b 6572 2050  Display Tasker P
-00000f50: 7265 6665 7265 6e63 6573 e905 0000 007a  references.....z
-00000f60: 0723 3635 3633 6666 7a0d 5361 7665 2053  .#6563ffz.Save S
-00000f70: 6574 7469 6e67 7329 04da 0c62 6f72 6465  ettings)...borde
-00000f80: 725f 636f 6c6f 72da 0c62 6f72 6465 725f  r_color..border_
-00000f90: 7769 6474 6872 1700 0000 7225 0000 00da  widthr....r%....
-00000fa0: 0173 7a10 5265 7374 6f72 6520 5365 7474  .sz.Restore Sett
-00000fb0: 696e 6773 e907 0000 00da 016e 7a14 4755  ings.......nz.GU
-00000fc0: 4920 4170 7065 6172 616e 6365 204d 6f64  I Appearance Mod
-00000fd0: 653a e908 0000 0029 03da 054c 6967 6874  e:.....)...Light
-00000fe0: da04 4461 726b 7206 0000 0029 0472 1000  ..Darkr....).r..
-00000ff0: 0000 7211 0000 0072 1b00 0000 7212 0000  ..r....r....r...
-00001000: 007a 0723 3234 3646 4236 7a0d 5265 7365  .z.#246FB6z.Rese
-00001010: 7420 4f70 7469 6f6e 7329 05da 066d 6173  t Options)...mas
-00001020: 7465 72da 0866 675f 636f 6c6f 7272 2b00  ter..fg_colorr+.
-00001030: 0000 7217 0000 0072 2500 0000 2902 7215  ..r....r%...).r.
-00001040: 0000 0072 1500 0000 5a03 5275 6e29 027a  ...r....Z.Run).z
-00001050: 0723 3042 4630 3735 7a07 2331 4144 3633  .#0BF075z.#1AD63
-00001060: 4429 0672 3200 0000 7233 0000 0072 2b00  D).r2...r3...r+.
-00001070: 0000 7217 0000 0072 2500 0000 da0a 7465  ..r....r%.....te
-00001080: 7874 5f63 6f6c 6f72 5a04 4578 6974 da03  xt_colorZ.Exit..
-00001090: 5265 64e9 6400 0000 e9fa 0000 0029 02da  Red.d........)..
-000010a0: 0668 6569 6768 7472 0d00 0000 2901 5a16  .heightr....).Z.
-000010b0: 7363 726f 6c6c 6261 725f 6275 7474 6f6e  scrollbar_button
-000010c0: 5f63 6f6c 6f72 2902 7215 0000 0072 0100  _color).r....r..
-000010d0: 0000 2902 720d 0000 005a 1973 6567 6d65  ..).r....Z.segme
-000010e0: 6e74 6564 5f62 7574 746f 6e5f 6667 5f63  nted_button_fg_c
-000010f0: 6f6c 6f72 7a0d 5370 6563 6966 6963 204e  olorz.Specific N
-00001100: 616d 65da 0643 6f6c 6f72 735a 0544 6562  ame..ColorsZ.Deb
-00001110: 7567 7a0c 5072 6f6a 6563 7420 4e61 6d65  ugz.Project Name
-00001120: 7a07 2331 6263 3966 6629 0472 1700 0000  z.#1bc9ff).r....
-00001130: 7225 0000 0072 3300 0000 722a 0000 0029  r%...r3...r*...)
-00001140: 0272 1900 0000 7219 0000 007a 0c50 726f  .r....r....z.Pro
-00001150: 6669 6c65 204e 616d 657a 0954 6173 6b20  file Namez.Task 
-00001160: 4e61 6d65 7a0f 2850 6963 6b20 4f4e 4c59  Namez.(Pick ONLY
-00001170: 204f 6e65 297a 1f53 6574 2056 6172 696f   One)z.Set Vario
-00001180: 7573 2044 6973 706c 6179 2043 6f6c 6f72  us Display Color
-00001190: 7320 4865 7265 a901 7217 0000 0029 0fda  s Here..r....)..
-000011a0: 0850 726f 6a65 6374 73da 0850 726f 6669  .Projects..Profi
-000011b0: 6c65 737a 1144 6973 6162 6c65 6420 5072  lesz.Disabled Pr
-000011c0: 6f66 696c 6573 7a0d 4c61 756e 6368 6572  ofilesz.Launcher
-000011d0: 2054 6173 6bfa 1250 726f 6669 6c65 2043   Task..Profile C
-000011e0: 6f6e 6469 7469 6f6e 73da 0554 6173 6b73  onditions..Tasks
-000011f0: 7a0e 2854 6173 6b29 2041 6374 696f 6e73  z.(Task) Actions
-00001200: fa11 4163 7469 6f6e 2043 6f6e 6469 7469  ..Action Conditi
-00001210: 6f6e 737a 0d41 6374 696f 6e20 4c61 6265  onsz.Action Labe
-00001220: 6c73 7a0c 4163 7469 6f6e 204e 616d 6573  lsz.Action Names
-00001230: da06 5363 656e 6573 da0a 4261 636b 6772  ..Scenes..Backgr
-00001240: 6f75 6e64 da07 4275 6c6c 6574 73fa 1554  ound..Bullets..T
-00001250: 6173 6b65 724e 6574 2049 6e66 6f72 6d61  askerNet Informa
-00001260: 7469 6f6e fa12 5461 736b 6572 2050 7265  tion..Tasker Pre
-00001270: 6665 7265 6e63 6573 7a0a 4465 6275 6720  ferencesz.Debug 
-00001280: 4d6f 6465 2904 7217 0000 0072 2500 0000  Mode).r....r%...
-00001290: 7226 0000 0072 2700 0000 2901 722a 0000  r&...r'...).r*..
-000012a0: 0029 0272 1b00 0000 721c 0000 0029 3cda  .).r....r....)<.
-000012b0: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
-000012c0: da05 7469 746c 65da 0867 656f 6d65 7472  ..title..geometr
-000012d0: 79da 1467 7269 645f 636f 6c75 6d6e 636f  y..grid_columnco
-000012e0: 6e66 6967 7572 65da 1167 7269 645f 726f  nfigure..grid_ro
-000012f0: 7763 6f6e 6669 6775 7265 da0d 6375 7374  wconfigure..cust
-00001300: 6f6d 746b 696e 7465 725a 0843 546b 4672  omtkinterZ.CTkFr
-00001310: 616d 655a 0d73 6964 6562 6172 5f66 7261  ameZ.sidebar_fra
-00001320: 6d65 da04 6772 6964 da08 4354 6b4c 6162  me..grid..CTkLab
-00001330: 656c 5a07 4354 6b46 6f6e 745a 0a6c 6f67  elZ.CTkFontZ.log
-00001340: 6f5f 6c61 6265 6c5a 0c64 6574 6169 6c5f  o_labelZ.detail_
-00001350: 6c61 6265 6c5a 0d43 546b 4f70 7469 6f6e  labelZ.CTkOption
-00001360: 4d65 6e75 da15 6465 7461 696c 5f73 656c  Menu..detail_sel
-00001370: 6563 7465 645f 6576 656e 74da 1573 6964  ected_event..sid
-00001380: 6562 6172 5f64 6574 6169 6c5f 6f70 7469  ebar_detail_opti
-00001390: 6f6e 5a0b 4354 6b43 6865 636b 426f 78da  onZ.CTkCheckBox.
-000013a0: 0f63 6f6e 6469 7469 6f6e 5f65 7665 6e74  .condition_event
-000013b0: da10 636f 6e64 6974 696f 6e5f 6275 7474  ..condition_butt
-000013c0: 6f6e da17 6469 7370 6c61 795f 7461 736b  on..display_task
-000013d0: 6572 6e65 745f 6576 656e 74da 1864 6973  ernet_event..dis
-000013e0: 706c 6179 5f74 6173 6b65 726e 6574 5f62  play_taskernet_b
-000013f0: 7574 746f 6eda 1964 6973 706c 6179 5f70  utton..display_p
-00001400: 7265 6665 7265 6e63 6573 5f65 7665 6e74  references_event
-00001410: da1a 6469 7370 6c61 795f 7072 6566 6572  ..display_prefer
-00001420: 656e 6365 735f 6275 7474 6f6e 5a09 4354  ences_buttonZ.CT
-00001430: 6b42 7574 746f 6eda 1373 6176 655f 7365  kButton..save_se
-00001440: 7474 696e 6773 5f65 7665 6e74 5a14 7361  ttings_eventZ.sa
-00001450: 7665 5f73 6574 7469 6e67 735f 6275 7474  ve_settings_butt
-00001460: 6f6e da16 7265 7374 6f72 655f 7365 7474  on..restore_sett
-00001470: 696e 6773 5f65 7665 6e74 5a17 7265 7374  ings_eventZ.rest
-00001480: 6f72 655f 7365 7474 696e 6773 5f62 7574  ore_settings_but
-00001490: 746f 6e5a 1561 7070 6561 7261 6e63 655f  tonZ.appearance_
-000014a0: 6d6f 6465 5f6c 6162 656c da1c 6368 616e  mode_label..chan
-000014b0: 6765 5f61 7070 6561 7261 6e63 655f 6d6f  ge_appearance_mo
-000014c0: 6465 5f65 7665 6e74 da1b 6170 7065 6172  de_event..appear
-000014d0: 616e 6365 5f6d 6f64 655f 6f70 7469 6f6e  ance_mode_option
-000014e0: 656d 656e 75da 1472 6573 6574 5f73 6574  emenu..reset_set
-000014f0: 7469 6e67 735f 6576 656e 745a 0c72 6573  tings_eventZ.res
-00001500: 6574 5f62 7574 746f 6eda 0b72 756e 5f70  et_button..run_p
-00001510: 726f 6772 616d 5a0a 7275 6e5f 6275 7474  rogramZ.run_butt
-00001520: 6f6e da0c 6578 6974 5f70 726f 6772 616d  on..exit_program
-00001530: 5a0b 6578 6974 5f62 7574 746f 6eda 0a43  Z.exit_button..C
-00001540: 546b 5465 7874 626f 78da 0774 6578 7462  TkTextbox..textb
-00001550: 6f78 da09 636f 6e66 6967 7572 655a 0a43  ox..configureZ.C
-00001560: 546b 5461 6276 6965 77da 0774 6162 7669  TkTabview..tabvi
-00001570: 6577 da03 6164 64da 0374 6162 5a0e 4354  ew..add..tabZ.CT
-00001580: 6b52 6164 696f 4275 7474 6f6e da19 7369  kRadioButton..si
-00001590: 6e67 6c65 5f70 726f 6a65 6374 5f6e 616d  ngle_project_nam
-000015a0: 655f 6576 656e 74da 1473 7472 696e 675f  e_event..string_
-000015b0: 696e 7075 745f 6275 7474 6f6e 31da 1973  input_button1..s
-000015c0: 696e 676c 655f 7072 6f66 696c 655f 6e61  ingle_profile_na
-000015d0: 6d65 5f65 7665 6e74 da14 7374 7269 6e67  me_event..string
-000015e0: 5f69 6e70 7574 5f62 7574 746f 6e32 da16  _input_button2..
-000015f0: 7369 6e67 6c65 5f74 6173 6b5f 6e61 6d65  single_task_name
-00001600: 5f65 7665 6e74 da14 7374 7269 6e67 5f69  _event..string_i
-00001610: 6e70 7574 5f62 7574 746f 6e33 5a0a 6e61  nput_button3Z.na
-00001620: 6d65 5f6c 6162 656c 5a0b 6c61 6265 6c5f  me_labelZ.label_
-00001630: 7461 625f 32da 0c63 6f6c 6f72 735f 6576  tab_2..colors_ev
-00001640: 656e 745a 1263 6f6c 6f72 735f 6f70 7469  entZ.colors_opti
-00001650: 6f6e 656d 656e 75da 1464 6562 7567 5f63  onemenu..debug_c
-00001660: 6865 636b 626f 785f 6576 656e 74da 0e64  heckbox_event..d
-00001670: 6562 7567 5f63 6865 636b 626f 78da 0470  ebug_checkbox..p
-00001680: 6163 6bda 0c73 6574 5f64 6566 6175 6c74  ack..set_default
-00001690: 73a9 01da 0473 656c 66a9 01da 095f 5f63  s....self....__c
-000016a0: 6c61 7373 5f5f a900 fa77 2f55 7365 7273  lass__...w/Users
-000016b0: 2f6d 696b 7275 6269 6e2f 4c69 6272 6172  /mikrubin/Librar
-000016c0: 792f 436c 6f75 6453 746f 7261 6765 2f47  y/CloudStorage/G
-000016d0: 6f6f 676c 6544 7269 7665 2d6d 696b 7275  oogleDrive-mikru
-000016e0: 6269 6e40 676d 6169 6c2e 636f 6d2f 4d79  bin@gmail.com/My
-000016f0: 2044 7269 7665 2f50 7974 686f 6e2f 6d61   Drive/Python/ma
-00001700: 7074 6173 6b65 722f 6d61 7074 6173 6b65  ptasker/maptaske
-00001710: 722f 7372 632f 7573 6572 696e 7472 2e70  r/src/userintr.p
-00001720: 7972 4600 0000 3d00 0000 7362 0100 000a  yrF...=...sb....
-00001730: 010a 030a 010e 030e 010e 0112 0314 0110  ................
-00001740: 0204 0104 0102 010c 0108 fd14 0504 0308  ................
-00001750: 0108 ff14 0304 0104 0106 0104 0108 fd14  ................
-00001760: 0504 0304 0104 0102 0102 0102 0108 fb16  ................
-00001770: 0704 0304 0104 0102 0102 0102 0108 fb06  ................
-00001780: 070a 0106 ff04 0504 0104 0102 0102 0102  ................
-00001790: 0108 fb06 070a 0106 ff04 0504 0102 0102  ................
-000017a0: 0102 0104 0108 fb16 0704 0304 0102 0102  ................
-000017b0: 0102 0104 0108 fb16 0704 0308 0108 ff14  ................
-000017c0: 0304 0104 0106 0104 0108 fd14 0504 0302  ................
-000017d0: 0102 0102 0102 0104 0108 fb06 070a 0106  ................
-000017e0: ff04 0502 0102 0102 0102 0104 0102 0108  ................
-000017f0: fa06 080a 0106 ff04 0502 0102 0102 0102  ................
-00001800: 0104 0102 0108 fa14 0812 030e 0116 0104  ................
-00001810: 0306 0108 ff16 030c 010c 010c 010c 0104  ................
-00001820: 0106 ff16 0304 030a 0102 0104 0102 0102  ................
-00001830: 0108 fb06 070a 0106 ff04 050a 0102 0104  ................
-00001840: 0102 0102 0108 fb06 070a 0106 ff04 050a  ................
-00001850: 0102 0104 0102 0102 0108 fb06 070a 0106  ................
-00001860: ff04 050e 0108 ff14 0304 030c 0108 ff14  ................
-00001870: 0304 010a 0106 0104 1108 ed14 1504 030a  ................
-00001880: 0102 0104 0102 0102 0108 fb0e 0710 010e  ................
-00001890: 037a 0e4d 7947 7569 2e5f 5f69 6e69 745f  .z.MyGui.__init_
-000018a0: 5fda 0a66 6972 7374 5f74 696d 6563 0200  _..first_timec..
-000018b0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-000018c0: 0000 4300 0000 73a4 0000 007c 006a 006a  ..C...s....|.j.j
-000018d0: 0167 0064 01a2 0164 028d 0101 007c 006a  .g.d...d.....|.j
-000018e0: 00a0 0264 03a1 0101 0064 047c 005f 0364  ...d.....d.|._.d
-000018f0: 0504 007c 005f 0404 007c 005f 0504 007c  ...|._...|._...|
-00001900: 005f 0604 007c 005f 0704 007c 005f 0804  ._...|._...|._..
-00001910: 007c 005f 0904 007c 005f 0a7c 005f 0b64  .|._...|._.|._.d
-00001920: 0604 007c 005f 0c04 007c 005f 0d7c 005f  ...|._...|._.|._
-00001930: 0e64 077c 005f 0f7c 006a 10a0 0264 08a1  .d.|._.|.j...d..
-00001940: 0101 0067 007c 005f 1164 087c 005f 127c  ...g.|._.d.|._.|
-00001950: 0172 4d7c 006a 13a0 1464 0964 0a74 1517  .rM|.j...d.d.t..
-00001960: 00a1 0201 0069 007c 005f 1664 0053 0029  .....i.|._.d.S.)
-00001970: 0b4e 721f 0000 0029 0172 2400 0000 7221  .Nr....).r$...r!
-00001980: 0000 0072 0800 0000 46da 0072 0a00 0000  ...r....F..r....
-00001990: 7206 0000 00fa 0330 2e30 7a10 4d61 7054  r......0.0z.MapT
-000019a0: 6173 6b65 7220 4865 6c70 0a0a 2917 724f  asker Help..).rO
-000019b0: 0000 0072 5f00 0000 da03 7365 74da 1464  ...r_.....set..d
-000019c0: 6973 706c 6179 5f64 6574 6169 6c5f 6c65  isplay_detail_le
-000019d0: 7665 6cda 1a64 6973 706c 6179 5f70 726f  vel..display_pro
-000019e0: 6669 6c65 5f63 6f6e 6469 7469 6f6e 73da  file_conditions.
-000019f0: 1364 6973 706c 6179 5f70 7265 6665 7265  .display_prefere
-00001a00: 6e63 6573 da11 6469 7370 6c61 795f 7461  nces..display_ta
-00001a10: 736b 6572 6e65 74da 0564 6562 7567 5a0e  skernet..debugZ.
-00001a20: 636c 6561 725f 7365 7474 696e 6773 da05  clear_settings..
-00001a30: 7265 7365 74da 0465 7869 74da 0a67 6f5f  reset..exit..go_
-00001a40: 7072 6f67 7261 6dda 1373 696e 676c 655f  program..single_
-00001a50: 7072 6f6a 6563 745f 6e61 6d65 da13 7369  project_name..si
-00001a60: 6e67 6c65 5f70 726f 6669 6c65 5f6e 616d  ngle_profile_nam
-00001a70: 65da 1073 696e 676c 655f 7461 736b 5f6e  e..single_task_n
-00001a80: 616d 65da 0e63 6f6c 6f72 5f74 6578 745f  ame..color_text_
-00001a90: 726f 7772 5900 0000 da0c 636f 6c6f 725f  rowrY.....color_
-00001aa0: 6c61 6265 6c73 da0f 6170 7065 6172 616e  labels..appearan
-00001ab0: 6365 5f6d 6f64 6572 5e00 0000 da06 696e  ce_moder^.....in
-00001ac0: 7365 7274 da09 494e 464f 5f54 4558 54da  sert..INFO_TEXT.
-00001ad0: 0c63 6f6c 6f72 5f6c 6f6f 6b75 7029 0272  .color_lookup).r
-00001ae0: 6f00 0000 7274 0000 0072 7200 0000 7272  o...rt...rr...rr
-00001af0: 0000 0072 7300 0000 726d 0000 0030 0100  ...rs...rm...0..
-00001b00: 0073 3000 0000 1201 0c01 0601 0207 08fa  .s0.............
-00001b10: 0401 02ff 0403 02fd 0405 02fb 0406 02fa  ................
-00001b20: 0406 02fa 0806 1201 0601 0c01 0601 0601  ................
-00001b30: 0401 1201 0a01 7a12 4d79 4775 692e 7365  ......z.MyGui.se
-00001b40: 745f 6465 6661 756c 7473 6302 0000 0000  t_defaultsc.....
-00001b50: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
-00001b60: 0000 0073 5000 0000 7400 6a01 7c00 6401  ...sP...t.j.|.d.
-00001b70: 6402 8d02 7c00 5f02 7c00 6a02 6a03 6403  d...|._.|.j.j.d.
-00001b80: 6404 6405 6405 6406 8d04 0100 7c00 6a02  d.d.d.d.....|.j.
-00001b90: a004 6407 7c01 a102 0100 7c00 6a02 6a05  ..d.|.....|.j.j.
-00001ba0: 6408 6409 640a 8d02 0100 7c00 6a02 a006  d.d.d.....|.j...
-00001bb0: a100 0100 6400 5300 290b 4e72 3700 0000  ....d.S.).Nr7...
-00001bc0: a901 720d 0000 0072 2800 0000 720a 0000  ..r....r(...r...
-00001bd0: 0072 1500 0000 721a 0000 0072 7600 0000  .r....r....rv...
-00001be0: da08 6469 7361 626c 6564 7235 0000 00a9  ..disabledr5....
-00001bf0: 02da 0573 7461 7465 7234 0000 00a9 0772  ...stater4.....r
-00001c00: 4b00 0000 725d 0000 0072 5e00 0000 724c  K...r]...r^...rL
-00001c10: 0000 0072 8600 0000 725f 0000 00da 0966  ...r....r_.....f
-00001c20: 6f63 7573 5f73 6574 2902 726f 0000 00da  ocus_set).ro....
-00001c30: 0d65 7272 6f72 5f6d 6573 7361 6765 7272  .error_messagerr
-00001c40: 0000 0072 7200 0000 7273 0000 00da 1164  ...rr...rs.....d
-00001c50: 6973 706c 6179 5f65 7272 6f72 5f62 6f78  isplay_error_box
-00001c60: 4701 0000 730e 0000 0010 0114 010e 0106  G...s...........
-00001c70: 0104 0106 ff0e 037a 174d 7947 7569 2e64  .......z.MyGui.d
-00001c80: 6973 706c 6179 5f65 7272 6f72 5f62 6f78  isplay_error_box
-00001c90: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00001ca0: 0006 0000 0043 0000 0073 6200 0000 7c02  .....C...sb...|.
-00001cb0: 7204 6401 6e01 6402 7d03 7400 6a01 7c00  r.d.n.d.}.t.j.|.
-00001cc0: 6403 6404 8d02 7c00 5f02 7c00 6a02 6a03  d.d...|._.|.j.j.
-00001cd0: 6405 6406 6407 6407 6408 8d04 0100 7c00  d.d.d.d.d.....|.
-00001ce0: 6a02 a004 6409 7c01 9b00 640a 9d02 a102  j...d.|...d.....
-00001cf0: 0100 7c00 6a02 6a05 640b 7c03 640c 8d02  ..|.j.j.d.|.d...
-00001d00: 0100 7c00 6a02 a006 a100 0100 6400 5300  ..|.j.......d.S.
-00001d10: 290d 4eda 0547 7265 656e 7235 0000 0069  ).N..Greenr5...i
-00001d20: 5802 0000 7289 0000 0072 2800 0000 7208  X...r....r(...r.
-00001d30: 0000 0072 1500 0000 721a 0000 0072 7600  ...r....r....rv.
-00001d40: 0000 da01 0a72 8a00 0000 728b 0000 0072  .....r....r....r
-00001d50: 8d00 0000 2904 726f 0000 00da 076d 6573  ....).ro.....mes
-00001d60: 7361 6765 5a04 676f 6f64 da05 636f 6c6f  sageZ.good..colo
-00001d70: 7272 7200 0000 7272 0000 0072 7300 0000  rrr...rr...rs...
-00001d80: da13 6469 7370 6c61 795f 6d65 7373 6167  ..display_messag
-00001d90: 655f 626f 7853 0100 0073 1000 0000 0c01  e_boxS...s......
-00001da0: 1001 1401 1401 0601 0401 06ff 0e03 7a19  ..............z.
-00001db0: 4d79 4775 692e 6469 7370 6c61 795f 6d65  MyGui.display_me
-00001dc0: 7373 6167 655f 626f 7863 0300 0000 0000  ssage_boxc......
-00001dd0: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
-00001de0: 0000 738c 0000 0064 017d 037c 0173 0d64  ..s....d.}.|.s.d
-00001df0: 027c 0217 0064 0317 007d 0364 047c 005f  .|...d...}.d.|._
-00001e00: 007c 006a 0172 167c 006a 0272 1664 057d  .|.j.r.|.j.r.d.}
-00001e10: 036e 117c 006a 0172 1f7c 006a 0372 1f64  .n.|.j.r.|.j.r.d
-00001e20: 067d 036e 087c 006a 0272 277c 006a 0372  .}.n.|.j.r'|.j.r
-00001e30: 2764 077d 037c 0372 387c 00a0 047c 03a1  'd.}.|.r8|...|..
-00001e40: 0101 0064 085c 037c 005f 017c 005f 027c  ...d.\.|._.|._.|
-00001e50: 005f 0364 0053 007c 00a0 0564 097c 019b  ._.d.S.|...d.|..
-00001e60: 0064 0a7c 029b 009d 0464 0ba1 0201 0064  .d.|.....d.....d
-00001e70: 0053 0029 0c4e 7275 0000 007a 2145 7272  .S.).Nru...z!Err
-00001e80: 6f72 3a0a 0a54 6865 206e 616d 6520 656e  or:..The name en
-00001e90: 7465 7265 6420 666f 7220 7468 6520 7a16  tered for the z.
-00001ea0: 2069 7320 626c 616e 6b21 0a0a 5472 7920   is blank!..Try 
-00001eb0: 6167 6169 6e2e 467a 5b45 7272 6f72 3a0a  again.Fz[Error:.
-00001ec0: 0a59 6f75 2068 6176 6520 656e 7465 7265  .You have entere
-00001ed0: 6420 626f 7468 2061 2050 726f 6a65 6374  d both a Project
-00001ee0: 2061 6e64 2061 2050 726f 6669 6c65 206e   and a Profile n
-00001ef0: 616d 6521 0a0a 5472 7920 6167 6169 6e20  ame!..Try again 
-00001f00: 616e 6420 6f6e 6c79 2073 656c 6563 7420  and only select 
-00001f10: 6f6e 652e 7a58 4572 726f 723a 0a0a 596f  one.zXError:..Yo
-00001f20: 7520 6861 7665 2065 6e74 6572 6564 2062  u have entered b
-00001f30: 6f74 6820 6120 5072 6f6a 6563 7420 616e  oth a Project an
-00001f40: 6420 6120 5461 736b 206e 616d 6521 0a0a  d a Task name!..
-00001f50: 5472 7920 6167 6169 6e20 616e 6420 6f6e  Try again and on
-00001f60: 6c79 2073 656c 6563 7420 6f6e 652e 7a58  ly select one.zX
-00001f70: 4572 726f 723a 0a0a 596f 7520 6861 7665  Error:..You have
-00001f80: 2065 6e74 6572 6564 2062 6f74 6820 6120   entered both a 
-00001f90: 5072 6f66 696c 6520 616e 6420 6120 5461  Profile and a Ta
-00001fa0: 736b 206e 616d 6521 0a0a 5472 7920 6167  sk name!..Try ag
-00001fb0: 6169 6e20 616e 6420 6f6e 6c79 2073 656c  ain and only sel
-00001fc0: 6563 7420 6f6e 652e 2903 7275 0000 0072  ect one.).ru...r
-00001fd0: 7500 0000 7275 0000 007a 1244 6973 706c  u...ru...z.Displ
-00001fe0: 6179 206f 6e6c 7920 7468 6520 277a 0227  ay only the 'z.'
-00001ff0: 2054 2906 5a0a 6e61 6d65 645f 6974 656d   T).Z.named_item
-00002000: 7280 0000 0072 8100 0000 7282 0000 0072  r....r....r....r
-00002010: 9000 0000 7295 0000 0029 0472 6f00 0000  ....r....).ro...
-00002020: da08 7468 655f 6e61 6d65 5a0c 656c 656d  ..the_nameZ.elem
-00002030: 656e 745f 6e61 6d65 728f 0000 0072 7200  ent_namer....rr.
-00002040: 0000 7272 0000 0072 7300 0000 da0a 6368  ..rr...rs.....ch
-00002050: 6563 6b5f 6e61 6d65 6001 0000 7338 0000  eck_name`...s8..
-00002060: 0004 0104 0102 0202 0102 ff02 0202 fe02  ................
-00002070: ff06 050c 0102 0204 ff0c 0402 0204 ff0c  ................
-00002080: 0402 0202 ff04 050a 0102 0502 fc04 0104  ................
-00002090: 0108 0104 0310 0108 ff7a 104d 7947 7569  .........z.MyGui
-000020a0: 2e63 6865 636b 5f6e 616d 6563 0100 0000  .check_namec....
-000020b0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-000020c0: 4300 0000 f34c 0000 0064 017d 017c 00a0  C....L...d.}.|..
-000020d0: 007c 01a1 0101 007c 006a 01a0 02a1 0001  .|.....|.j......
-000020e0: 007c 006a 03a0 02a1 0001 0074 046a 0564  .|.j.......t.j.d
-000020f0: 0264 0364 048d 027d 027c 02a0 06a1 007c  .d.d...}.|.....|
-00002100: 005f 077c 00a0 087c 006a 0764 05a1 0201  ._.|...|.j.d....
-00002110: 0064 0053 0029 064e 7275 0000 007a 1345  .d.S.).Nru...z.E
-00002120: 6e74 6572 2050 726f 6a65 6374 206e 616d  nter Project nam
-00002130: 653a 7a18 4469 7370 6c61 7920 5370 6563  e:z.Display Spec
-00002140: 6966 6963 2050 726f 6a65 6374 a902 7217  ific Project..r.
-00002150: 0000 0072 4700 0000 da07 5072 6f6a 6563  ...rG.....Projec
-00002160: 7429 0972 9000 0000 7266 0000 00da 0864  t).r....rf.....d
-00002170: 6573 656c 6563 7472 6800 0000 724b 0000  eselectrh...rK..
-00002180: 00da 0e43 546b 496e 7075 7444 6961 6c6f  ...CTkInputDialo
-00002190: 67da 0967 6574 5f69 6e70 7574 7280 0000  g..get_inputr...
-000021a0: 0072 9700 0000 a903 726f 0000 0072 8f00  .r......ro...r..
-000021b0: 0000 da06 6469 616c 6f67 7272 0000 0072  ....dialogrr...r
-000021c0: 7200 0000 7273 0000 0072 6300 0000 8801  r...rs...rc.....
-000021d0: 0000 f312 0000 0004 020a 010a 020a 0104  ................
-000021e0: 0204 0106 ff0a 0412 027a 1f4d 7947 7569  .........z.MyGui
-000021f0: 2e73 696e 676c 655f 7072 6f6a 6563 745f  .single_project_
-00002200: 6e61 6d65 5f65 7665 6e74 6301 0000 0000  name_eventc.....
-00002210: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00002220: 0000 0072 9800 0000 2906 4e72 7500 0000  ...r....).Nru...
-00002230: 7a13 456e 7465 7220 5072 6f66 696c 6520  z.Enter Profile 
-00002240: 6e61 6d65 3a7a 1844 6973 706c 6179 2053  name:z.Display S
-00002250: 7065 6369 6669 6320 5072 6f66 696c 6572  pecific Profiler
-00002260: 9900 0000 da07 5072 6f66 696c 6529 0972  ......Profile).r
-00002270: 9000 0000 7264 0000 0072 9b00 0000 7268  ....rd...r....rh
-00002280: 0000 0072 4b00 0000 729c 0000 0072 9d00  ...rK...r....r..
-00002290: 0000 7281 0000 0072 9700 0000 729e 0000  ..r....r....r...
-000022a0: 0072 7200 0000 7272 0000 0072 7300 0000  .rr...rr...rs...
-000022b0: 7265 0000 009b 0100 0072 a000 0000 7a1f  re.......r....z.
-000022c0: 4d79 4775 692e 7369 6e67 6c65 5f70 726f  MyGui.single_pro
-000022d0: 6669 6c65 5f6e 616d 655f 6576 656e 7463  file_name_eventc
-000022e0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-000022f0: 0400 0000 4300 0000 7298 0000 0029 064e  ....C...r....).N
-00002300: 7275 0000 007a 1045 6e74 6572 2054 6173  ru...z.Enter Tas
-00002310: 6b20 6e61 6d65 3a7a 1544 6973 706c 6179  k name:z.Display
-00002320: 2053 7065 6369 6669 6320 5461 736b 7299   Specific Taskr.
-00002330: 0000 00da 0454 6173 6b29 0972 9000 0000  .....Task).r....
-00002340: 7264 0000 0072 9b00 0000 7266 0000 0072  rd...r....rf...r
-00002350: 4b00 0000 729c 0000 0072 9d00 0000 7282  K...r....r....r.
-00002360: 0000 0072 9700 0000 729e 0000 0072 7200  ...r....r....rr.
-00002370: 0000 7272 0000 0072 7300 0000 7267 0000  ..rr...rs...rg..
-00002380: 00ae 0100 0072 a000 0000 7a1c 4d79 4775  .....r....z.MyGu
-00002390: 692e 7369 6e67 6c65 5f74 6173 6b5f 6e61  i.single_task_na
-000023a0: 6d65 5f65 7665 6e74 da13 6e65 775f 6170  me_event..new_ap
-000023b0: 7065 6172 616e 6365 5f6d 6f64 6563 0200  pearance_modec..
-000023c0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000023d0: 0000 4300 0000 7314 0000 0074 00a0 017c  ..C...s....t...|
-000023e0: 01a1 0101 007c 017c 005f 0264 0053 00a9  .....|.|._.d.S..
-000023f0: 014e 2903 724b 0000 00da 1373 6574 5f61  .N).rK.....set_a
-00002400: 7070 6561 7261 6e63 655f 6d6f 6465 7285  ppearance_moder.
-00002410: 0000 0029 0272 6f00 0000 72a3 0000 0072  ...).ro...r....r
-00002420: 7200 0000 7272 0000 0072 7300 0000 7258  r...rr...rs...rX
-00002430: 0000 00c1 0100 0073 0400 0000 0a01 0a01  .......s........
-00002440: 7a22 4d79 4775 692e 6368 616e 6765 5f61  z"MyGui.change_a
-00002450: 7070 6561 7261 6e63 655f 6d6f 6465 5f65  ppearance_mode_e
-00002460: 7665 6e74 da0e 6469 7370 6c61 795f 6465  vent..display_de
-00002470: 7461 696c 6302 0000 0000 0000 0000 0000  tailc...........
-00002480: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00002490: 0000 7c01 7c00 5f00 6400 5300 72a4 0000  ..|.|._.d.S.r...
-000024a0: 0029 0172 7800 0000 2902 726f 0000 0072  .).rx...).ro...r
-000024b0: a600 0000 7272 0000 0072 7200 0000 7273  ....rr...rr...rs
-000024c0: 0000 0072 4e00 0000 c801 0000 7302 0000  ...rN.......s...
-000024d0: 000a 017a 1b4d 7947 7569 2e64 6574 6169  ...z.MyGui.detai
-000024e0: 6c5f 7365 6c65 6374 6564 5f65 7665 6e74  l_selected_event
-000024f0: da13 636f 6c6f 725f 7365 6c65 6374 6564  ..color_selected
-00002500: 5f69 7465 6d63 0200 0000 0000 0000 0000  _itemc..........
-00002510: 0000 0800 0000 0800 0000 4300 0000 73d6  ..........C...s.
-00002520: 0000 0067 0064 01a2 017d 027c 006a 007c  ...g.d...}.|.j.|
-00002530: 006a 007c 006a 017c 006a 0267 047d 0374  .j.|.j.|.j.g.}.t
-00002540: 03a0 0474 05a1 018f 3001 007c 02a0 067c  ...t....0..|...|
-00002550: 01a1 017d 047c 037c 0419 0073 3c7c 01a0  ...}.|.|...s<|..
-00002560: 0764 0264 03a1 027d 057c 05a0 0764 0464  .d.d...}.|...d.d
-00002570: 03a1 027d 057c 00a0 0864 057c 059b 0064  ...}.|...d.|...d
-00002580: 069d 0364 07a1 0201 0009 0057 0064 0004  ...d.......W.d..
-00002590: 0004 0083 0301 0064 0053 0057 0064 0004  .......d.S.W.d..
-000025a0: 0004 0083 0301 006e 0831 0073 4677 0101  .......n.1.sFw..
-000025b0: 0001 0001 0059 0001 0074 0983 007d 067c  .....Y...t...}.|
-000025c0: 06a0 0aa1 007d 077c 0764 0075 0172 697c  .....}.|.d.u.ri|
-000025d0: 00a0 087c 019b 0064 087c 079b 009d 0364  ...|...d.|.....d
-000025e0: 07a1 0201 007c 00a0 0b7c 077c 01a1 0201  .....|...|.|....
-000025f0: 0064 0053 0064 0053 0029 094e 2904 723d  .d.S.d.S.).N).r=
-00002600: 0000 0072 3f00 0000 7243 0000 0072 4400  ...r?...rC...rD.
-00002610: 0000 7a08 5072 6f66 696c 6520 7275 0000  ..z.Profile ru..
-00002620: 007a 0741 6374 696f 6e20 7a08 4469 7370  .z.Action z.Disp
-00002630: 6c61 7920 7a17 2069 7320 6e6f 7420 7365  lay z. is not se
-00002640: 7420 746f 2064 6973 706c 6179 2146 fa12  t to display!F..
-00002650: 2063 6f6c 6f72 2063 6861 6e67 6564 2074   color changed t
-00002660: 6f20 290c 7279 0000 0072 7b00 0000 727a  o ).ry...r{...rz
-00002670: 0000 00da 0a63 6f6e 7465 7874 6c69 62da  .....contextlib.
-00002680: 0873 7570 7072 6573 73da 0945 7863 6570  .suppress..Excep
-00002690: 7469 6f6e da05 696e 6465 78da 0772 6570  tion..index..rep
-000026a0: 6c61 6365 7295 0000 0072 0300 0000 da03  lacer....r......
-000026b0: 6765 74da 1865 7874 7261 6374 5f63 6f6c  get..extract_col
-000026c0: 6f72 5f66 726f 6d5f 6576 656e 7429 0872  or_from_event).r
-000026d0: 6f00 0000 72a7 0000 005a 0d77 6172 6e69  o...r....Z.warni
-000026e0: 6e67 5f63 6865 636b 5a0d 6368 6563 6b5f  ng_checkZ.check_
-000026f0: 6167 6169 6e73 745a 0974 6865 5f69 6e64  againstZ.the_ind
-00002700: 6578 5a12 7468 655f 6f75 7470 7574 5f6d  exZ.the_output_m
-00002710: 6573 7361 6765 5a0a 7069 636b 5f63 6f6c  essageZ.pick_col
-00002720: 6f72 7294 0000 0072 7200 0000 7272 0000  orr....rr...rr..
-00002730: 0072 7300 0000 7269 0000 00ce 0100 0073  .rs...ri.......s
-00002740: 3400 0000 0801 0407 0401 0401 0401 04fc  4...............
-00002750: 0c09 0a01 0801 0c01 0c01 0401 0c01 04ff  ................
-00002760: 0203 10f8 0202 1cfe 060a 0801 0801 0401  ................
-00002770: 0e01 04ff 1005 04fa 7a12 4d79 4775 692e  ........z.MyGui.
-00002780: 636f 6c6f 7273 5f65 7665 6e74 6303 0000  colors_eventc...
-00002790: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-000027a0: 0043 0000 0073 7c00 0000 7c00 6a00 7d03  .C...s|...|.j.}.
-000027b0: 7c01 7c00 6a01 7402 7c02 1900 3c00 7c00  |.|.j.t.|...<.|.
-000027c0: 6a03 a004 7405 6a06 7c00 6a07 a008 6401  j...t.j.|.j...d.
-000027d0: a101 7c02 9b00 6402 9d02 7c01 6403 8d03  ..|...d...|.d...
-000027e0: a101 0100 7c00 6a03 6404 1900 6a09 7c00  ....|.j.d...j.|.
-000027f0: 6a00 6405 6405 6405 6406 8d04 0100 7c00  j.d.d.d.d.....|.
-00002800: 0400 6a00 6407 3700 0200 5f00 7c00 a00a  ..j.d.7..._.|...
-00002810: 7c02 9b00 6408 7c01 9b00 9d03 6409 a102  |...d.|.....d...
-00002820: 0100 6400 5300 290a 4e72 3900 0000 7a09  ..d.S.).Nr9...z.
-00002830: 203c 3c20 636f 6c6f 7229 0272 1700 0000   << color).r....
-00002840: 7234 0000 00e9 ffff ffff 7201 0000 0072  r4........r....r
-00002850: 1a00 0000 7208 0000 0072 a800 0000 5429  ....r....r....T)
-00002860: 0b72 8300 0000 7288 0000 0072 0500 0000  .r....r....r....
-00002870: 7284 0000 00da 0661 7070 656e 6472 4b00  r......appendrK.
-00002880: 0000 724d 0000 0072 6000 0000 7262 0000  ..rM...r`...rb..
-00002890: 0072 4c00 0000 7295 0000 0029 0472 6f00  .rL...r....).ro.
-000028a0: 0000 7294 0000 0072 a700 0000 7210 0000  ..r....r....r...
-000028b0: 0072 7200 0000 7272 0000 0072 7300 0000  .rr...rr...rs...
-000028c0: 72af 0000 00f2 0100 0073 1e00 0000 0601  r........s......
-000028d0: 0202 0cff 0603 0401 0a01 0801 0201 04fd  ................
-000028e0: 04ff 1a07 0e01 0401 0e01 08ff 7a1e 4d79  ............z.My
-000028f0: 4775 692e 6578 7472 6163 745f 636f 6c6f  Gui.extract_colo
-00002900: 725f 6672 6f6d 5f65 7665 6e74 6301 0000  r_from_eventc...
-00002910: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00002920: 0043 0000 00f3 1000 0000 7c00 6a00 a001  .C........|.j...
-00002930: a100 7c00 5f02 6400 5300 72a4 0000 0029  ..|._.d.S.r....)
-00002940: 0372 5100 0000 72ae 0000 0072 7900 0000  .rQ...r....ry...
-00002950: 726e 0000 0072 7200 0000 7272 0000 0072  rn...rr...rr...r
-00002960: 7300 0000 7250 0000 0007 0200 00f3 0200  s...rP..........
-00002970: 0000 1001 7a15 4d79 4775 692e 636f 6e64  ....z.MyGui.cond
-00002980: 6974 696f 6e5f 6576 656e 7463 0100 0000  ition_eventc....
-00002990: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-000029a0: 4300 0000 72b2 0000 0072 a400 0000 2903  C...r....r....).
-000029b0: 7255 0000 0072 ae00 0000 727a 0000 0072  rU...r....rz...r
-000029c0: 6e00 0000 7272 0000 0072 7200 0000 7273  n...rr...rr...rs
-000029d0: 0000 0072 5400 0000 0d02 0000 72b3 0000  ...rT.......r...
-000029e0: 007a 1f4d 7947 7569 2e64 6973 706c 6179  .z.MyGui.display
-000029f0: 5f70 7265 6665 7265 6e63 6573 5f65 7665  _preferences_eve
-00002a00: 6e74 6301 0000 0000 0000 0000 0000 0001  ntc.............
-00002a10: 0000 0002 0000 0043 0000 0072 b200 0000  .......C...r....
-00002a20: 72a4 0000 0029 0372 5300 0000 72ae 0000  r....).rS...r...
-00002a30: 0072 7b00 0000 726e 0000 0072 7200 0000  .r{...rn...rr...
-00002a40: 7272 0000 0072 7300 0000 7252 0000 0013  rr...rs...rR....
-00002a50: 0200 0072 b300 0000 7a1d 4d79 4775 692e  ...r....z.MyGui.
-00002a60: 6469 7370 6c61 795f 7461 736b 6572 6e65  display_taskerne
-00002a70: 745f 6576 656e 7463 0100 0000 0000 0000  t_eventc........
-00002a80: 0000 0000 0200 0000 0900 0000 4300 0000  ............C...
-00002a90: 734a 0000 007c 006a 007c 006a 017c 006a  sJ...|.j.|.j.|.j
-00002aa0: 027c 006a 037c 006a 047c 006a 057c 006a  .|.j.|.j.|.j.|.j
-00002ab0: 067c 006a 0764 019c 087d 0174 0864 027c  .|.j.d...}.t.d.|
-00002ac0: 006a 097c 0183 035c 027d 017c 005f 097c  .j.|...\.}.|._.|
-00002ad0: 00a0 0a64 0364 02a1 0201 0064 0053 0029  ...d.d.....d.S.)
-00002ae0: 044e 2908 7278 0000 0072 7900 0000 727a  .N).rx...ry...rz
-00002af0: 0000 0072 7b00 0000 7280 0000 0072 8100  ...r{...r....r..
-00002b00: 0000 7282 0000 0072 7c00 0000 547a 0f53  ..r....r|...Tz.S
-00002b10: 6574 7469 6e67 7320 7361 7665 642e 290b  ettings saved.).
-00002b20: 7278 0000 0072 7900 0000 727a 0000 0072  rx...ry...rz...r
-00002b30: 7b00 0000 7280 0000 0072 8100 0000 7282  {...r....r....r.
-00002b40: 0000 0072 7c00 0000 7204 0000 0072 8800  ...r|...r....r..
-00002b50: 0000 7295 0000 0029 0272 6f00 0000 da09  ..r....).ro.....
-00002b60: 7465 6d70 5f61 7267 7372 7200 0000 7272  temp_argsrr...rr
-00002b70: 0000 0072 7300 0000 7256 0000 0019 0200  ...rs...rV......
-00002b80: 0073 1a00 0000 0402 0401 0401 0401 0401  .s..............
-00002b90: 0401 0401 0401 06f8 020a 0801 0aff 1003  ................
-00002ba0: 7a19 4d79 4775 692e 7361 7665 5f73 6574  z.MyGui.save_set
-00002bb0: 7469 6e67 735f 6576 656e 7463 0300 0000  tings_eventc....
-00002bc0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
-00002bd0: 4300 0000 7346 0100 0064 017d 037c 0104  C...sF...d.}.|..
-00002be0: 0064 026b 0272 1801 007c 0272 117c 006a  .d.k.r...|.r.|.j
-00002bf0: 00a0 01a1 0001 007c 0353 007c 006a 00a0  .......|.S.|.j..
-00002c00: 02a1 0001 007c 0353 0004 0064 036b 0272  .....|.S...d.k.r
-00002c10: 2701 007c 006a 03a0 0474 057c 0283 01a1  '..|.j...t.|....
-00002c20: 0101 007c 0353 0004 0064 046b 0272 3c01  ...|.S...d.k.r<.
-00002c30: 007c 0272 357c 006a 06a0 01a1 0001 007c  .|.r5|.j.......|
-00002c40: 0353 007c 006a 06a0 02a1 0001 007c 0353  .S.|.j.......|.S
-00002c50: 0004 0064 056b 0272 5101 007c 0272 4a7c  ...d.k.rQ..|.rJ|
-00002c60: 006a 07a0 01a1 0001 007c 0353 007c 006a  .j.......|.S.|.j
-00002c70: 07a0 02a1 0001 007c 0353 0004 0064 066b  .......|.S...d.k
-00002c80: 0272 6601 007c 0272 5f7c 006a 08a0 01a1  .rf..|.r_|.j....
-00002c90: 0001 007c 0353 007c 006a 08a0 02a1 0001  ...|.S.|.j......
-00002ca0: 007c 0353 0004 0064 076b 0272 7701 007c  .|.S...d.k.rw..|
-00002cb0: 0272 757c 039b 0064 087c 029b 0064 099d  .ru|...d.|...d..
-00002cc0: 047d 037c 0353 0004 0064 0a6b 0272 8801  .}.|.S...d.k.r..
-00002cd0: 007c 0272 867c 039b 0064 0b7c 029b 0064  .|.r.|...d.|...d
-00002ce0: 099d 047d 037c 0353 0064 0c6b 0272 977c  ...}.|.S.d.k.r.|
-00002cf0: 0272 957c 039b 0064 0d7c 029b 0064 099d  .r.|...d.|...d..
-00002d00: 047d 037c 0353 0009 007c 00a0 0964 0e7c  .}.|.S...|...d.|
-00002d10: 029b 009d 0264 0fa1 0201 007c 0353 0029  .....d.....|.S.)
-00002d20: 104e 7275 0000 0072 7c00 0000 7278 0000  .Nru...r|...rx..
-00002d30: 0072 7900 0000 727a 0000 0072 7b00 0000  .ry...rz...r{...
-00002d40: 7280 0000 007a 0f50 726f 6a65 6374 2073  r....z.Project s
-00002d50: 6574 2074 6f20 7a02 2e0a 7281 0000 007a  et to z...r....z
-00002d60: 0f50 726f 6669 6c65 2073 6574 2074 6f20  .Profile set to 
-00002d70: 7282 0000 007a 0c54 6173 6b20 7365 7420  r....z.Task set 
-00002d80: 746f 207a 1d52 7574 726f 6821 2020 556e  to z.Rutroh!  Un
-00002d90: 6465 6669 6e65 6420 6172 6775 6d65 6e74  defined argument
-00002da0: 3a20 4629 0a72 6b00 0000 da06 7365 6c65  : F).rk.....sele
-00002db0: 6374 729b 0000 0072 4f00 0000 7277 0000  ctr....rO...rw..
-00002dc0: 00da 0373 7472 7251 0000 0072 5500 0000  ...strrQ...rU...
-00002dd0: 7253 0000 0072 9500 0000 2904 726f 0000  rS...r....).ro..
-00002de0: 00da 036b 6579 da05 7661 6c75 6572 9300  ...key..valuer..
-00002df0: 0000 7272 0000 0072 7200 0000 7273 0000  ..rr...rr...rs..
-00002e00: 00da 0f72 6573 746f 7265 5f64 6973 706c  ...restore_displ
-00002e10: 6179 2c02 0000 7358 0000 0004 0102 010a  ay,...sX........
-00002e20: 0104 010a 0104 1f0a e304 1d0a e410 0104  ................
-00002e30: 1b0a e604 010a 0104 180a ea04 160a eb04  ................
-00002e40: 010a 0104 130a ef04 110a f004 010a 0104  ................
-00002e50: 0e0a f404 0c0a f504 0110 0104 090a f804  ................
-00002e60: 0110 0104 0606 fb04 0110 0104 0302 fe12  ................
-00002e70: 0104 017a 154d 7947 7569 2e72 6573 746f  ...z.MyGui.resto
-00002e80: 7265 5f64 6973 706c 6179 6301 0000 0000  re_displayc.....
-00002e90: 0000 0000 0000 0007 0000 0008 0000 0043  ...............C
-00002ea0: 0000 0073 1601 0000 7c00 a000 6401 a101  ...s....|...d...
-00002eb0: 0100 6900 7d01 7401 6401 7c00 6a02 7c01  ..i.}.t.d.|.j.|.
-00002ec0: 8303 5c02 7d01 7c00 5f02 7a11 7c01 6402  ..\.}.|._.z.|.d.
-00002ed0: 1900 7221 7c00 a003 7c01 6402 1900 6401  ..r!|...|.d...d.
-00002ee0: a102 0100 5700 6400 5300 5700 6e09 0400  ....W.d.S.W.n...
-00002ef0: 7404 792b 0100 0100 0100 5900 6e01 7700  t.y+......Y.n.w.
-00002f00: 7c01 7331 7c00 6a02 7283 6403 5c02 7d02  |.s1|.j.r.d.\.}.
-00002f10: 7d03 7c01 a005 a100 4400 5d1a 5c02 7d04  }.|.....D.].\.}.
-00002f20: 7d05 7c04 6400 7501 7253 7406 7c00 7c04  }.|.d.u.rSt.|.|.
-00002f30: 7c05 8303 0100 7c00 a007 7c04 7c05 a102  |.....|...|.|...
-00002f40: 0400 7d03 7253 7c02 7c03 1700 7d02 7139  ..}.rS|.|...}.q9
-00002f50: 6404 6405 8400 7408 a005 a100 4400 8301  d.d...t.....D...
-00002f60: 7d06 7c00 6a02 a005 a100 4400 5d15 5c02  }.|.j.....D.].\.
-00002f70: 7d04 7d05 7c04 6400 7501 7277 7c02 9b00  }.}.|.d.u.rw|...
-00002f80: 6406 7c06 7c04 1900 9b00 6407 7c05 9b00  d.|.|.....d.|...
-00002f90: 6408 9d06 7d02 7162 7c00 a003 7c02 9b00  d...}.qb|...|...
-00002fa0: 6409 9d02 640a a102 0100 6400 5300 7c00  d...d.....d.S.|.
-00002fb0: a003 640b 6401 a102 0100 6400 5300 290c  ..d.d.....d.S.).
-00002fc0: 4e46 da03 6d73 6729 0272 7500 0000 7275  NF..msg).ru...ru
-00002fd0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00002fe0: 0300 0000 0400 0000 5300 0000 7316 0000  ........S...s...
-00002ff0: 0069 007c 005d 075c 027d 017d 027c 027c  .i.|.].\.}.}.|.|
-00003000: 0193 0271 0253 0072 7200 0000 7272 0000  ...q.S.rr...rr..
-00003010: 0029 03da 022e 30da 016b da01 7672 7200  .)....0..k..vrr.
-00003020: 0000 7272 0000 0072 7300 0000 da0a 3c64  ..rr...rs.....<d
-00003030: 6963 7463 6f6d 703e 6d02 0000 7302 0000  ictcomp>m...s...
-00003040: 0016 007a 304d 7947 7569 2e72 6573 746f  ...z0MyGui.resto
-00003050: 7265 5f73 6574 7469 6e67 735f 6576 656e  re_settings_even
-00003060: 742e 3c6c 6f63 616c 733e 2e3c 6469 6374  t.<locals>.<dict
-00003070: 636f 6d70 3efa 0120 7a0e 2063 6f6c 6f72  comp>.. z. color
-00003080: 2073 6574 2074 6f20 7292 0000 007a 130a   set to r....z..
-00003090: 5365 7474 696e 6773 2072 6573 746f 7265  Settings restore
-000030a0: 642e 547a 174e 6f20 7365 7474 696e 6773  d.Tz.No settings
-000030b0: 2066 696c 6520 666f 756e 642e 2909 726d   file found.).rm
-000030c0: 0000 0072 0400 0000 7288 0000 0072 9500  ...r....r....r..
-000030d0: 0000 da08 4b65 7945 7272 6f72 da05 6974  ....KeyError..it
-000030e0: 656d 73da 0773 6574 6174 7472 72b9 0000  ems..setattrr...
-000030f0: 0072 0500 0000 2907 726f 0000 0072 b400  .r....).ro...r..
-00003100: 0000 5a0c 616c 6c5f 6d65 7373 6167 6573  ..Z.all_messages
-00003110: 5a0b 6e65 775f 6d65 7373 6167 6572 b700  Z.new_messager..
-00003120: 0000 72b8 0000 005a 0f69 6e76 5f63 6f6c  ..r....Z.inv_col
-00003130: 6f72 5f6e 616d 6573 7272 0000 0072 7200  or_namesrr...rr.
-00003140: 0000 7273 0000 0072 5700 0000 5502 0000  ..rs...rW...U...
-00003150: 733a 0000 000a 0104 0102 0208 010a ff02  s:..............
-00003160: 0408 0110 0106 0104 fe0c 0304 0102 ff0a  ................
-00003170: 0408 0110 0108 010c 0110 0108 0102 8012  ................
-00003180: 0212 0108 0118 0202 ff02 8016 0410 037a  ...............z
-00003190: 1c4d 7947 7569 2e72 6573 746f 7265 5f73  .MyGui.restore_s
-000031a0: 6574 7469 6e67 735f 6576 656e 7463 0100  ettings_eventc..
-000031b0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000031c0: 0000 4300 0000 738c 0000 007c 006a 00a0  ..C...s....|.j..
-000031d0: 0164 01a1 0101 007c 006a 02a0 03a1 0001  .d.....|.j......
-000031e0: 007c 006a 04a0 03a1 0001 007c 006a 05a0  .|.j.......|.j..
-000031f0: 03a1 0001 007c 006a 06a0 0164 02a1 0101  .....|.j...d....
-00003200: 0074 07a0 0864 02a1 0101 007c 006a 09a0  .t...d.....|.j..
-00003210: 03a1 0001 007c 00a0 0a64 0364 04a1 0201  .....|...d.d....
-00003220: 007c 00a0 0b64 05a1 0101 007c 006a 0c72  .|...d.....|.j.r
-00003230: 3f7c 006a 0c44 005d 087d 017c 016a 0d64  ?|.j.D.].}.|.j.d
-00003240: 0564 068d 0101 0071 367c 00a0 0e64 07a1  .d.....q6|...d..
-00003250: 0101 0064 0053 0029 084e 7221 0000 0072  ...d.S.).Nr!...r
-00003260: 0600 0000 7a0f 5365 7474 696e 6773 2072  ....z.Settings r
-00003270: 6573 6574 2e54 7275 0000 0072 3a00 0000  eset.Tru...r:...
-00003280: 4629 0f72 4f00 0000 7277 0000 0072 5100  F).rO...rw...rQ.
-00003290: 0000 729b 0000 0072 5500 0000 7253 0000  ..r....rU...rS..
-000032a0: 0072 5900 0000 724b 0000 0072 a500 0000  .rY...rK...r....
-000032b0: 726b 0000 0072 9500 0000 7290 0000 0072  rk...r....r....r
-000032c0: 8400 0000 725f 0000 0072 6d00 0000 2902  ....r_...rm...).
-000032d0: 726f 0000 00da 056c 6162 656c 7272 0000  ro.....labelrr..
-000032e0: 0072 7200 0000 7273 0000 0072 5a00 0000  .rr...rs...rZ...
-000032f0: 7c02 0000 731a 0000 000c 010a 010a 010a  |...s...........
-00003300: 010c 010a 010a 010c 010a 0106 010a 010e  ................
-00003310: 010e 017a 1a4d 7947 7569 2e72 6573 6574  ...z.MyGui.reset
-00003320: 5f73 6574 7469 6e67 735f 6576 656e 7463  _settings_eventc
-00003330: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00003340: 0400 0000 4300 0000 734e 0000 007c 006a  ....C...sN...|.j
-00003350: 00a0 01a1 007c 005f 027c 006a 0272 1f74  .....|._.|.j.r.t
-00003360: 0364 0183 01a0 04a1 0072 177c 00a0 0564  .d.......r.|...d
-00003370: 0264 03a1 0201 0064 0053 007c 00a0 0564  .d.....d.S.|...d
-00003380: 0464 05a1 0201 0064 0053 007c 00a0 0564  .d.....d.S.|...d
-00003390: 0664 03a1 0201 0064 0053 0029 074e 7a0a  .d.....d.S.).Nz.
-000033a0: 6261 636b 7570 2e78 6d6c 7a13 4465 6275  backup.xmlz.Debu
-000033b0: 6720 6d6f 6465 2065 6e61 626c 6564 2e54  g mode enabled.T
-000033c0: 7a53 4465 6275 6720 6d6f 6465 2072 6571  zSDebug mode req
-000033d0: 7569 7265 7320 5461 736b 6572 2062 6163  uires Tasker bac
-000033e0: 6b75 7020 6669 6c65 2074 6f20 6265 206e  kup file to be n
-000033f0: 616d 6564 3a20 2762 6163 6b75 702e 786d  amed: 'backup.xm
-00003400: 6c27 2c20 7768 6963 6820 6973 206d 6973  l', which is mis
-00003410: 7369 6e67 2146 7a14 4465 6275 6720 6d6f  sing!Fz.Debug mo
-00003420: 6465 2064 6973 6162 6c65 642e 2906 726b  de disabled.).rk
-00003430: 0000 0072 ae00 0000 727c 0000 0072 0200  ...r....r|...r..
-00003440: 0000 da07 6973 5f66 696c 6572 9500 0000  ....is_filer....
-00003450: 726e 0000 0072 7200 0000 7272 0000 0072  rn...rr...rr...r
-00003460: 7300 0000 726a 0000 008e 0200 0073 1200  s...rj.......s..
-00003470: 0000 0c01 0601 0c01 1001 0402 0202 0203  ................
-00003480: 08fb 1008 7a1a 4d79 4775 692e 6465 6275  ....z.MyGui.debu
-00003490: 675f 6368 6563 6b62 6f78 5f65 7665 6e74  g_checkbox_event
-000034a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000034b0: 0002 0000 0043 0000 00f3 1200 0000 6401  .....C........d.
-000034c0: 7c00 5f00 7c00 a001 a100 0100 6400 5300  |._.|.......d.S.
-000034d0: a902 4e54 2902 727f 0000 00da 0471 7569  ..NT).r......qui
-000034e0: 7472 6e00 0000 7272 0000 0072 7200 0000  trn...rr...rr...
-000034f0: 7273 0000 0072 5b00 0000 a102 0000 f304  rs...r[.........
-00003500: 0000 0006 010c 017a 114d 7947 7569 2e72  .......z.MyGui.r
-00003510: 756e 5f70 726f 6772 616d 6301 0000 0000  un_programc.....
-00003520: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00003530: 0000 0072 c500 0000 72c6 0000 0029 0272  ...r....r....).r
-00003540: 7e00 0000 72c7 0000 0072 6e00 0000 7272  ~...r....rn...rr
-00003550: 0000 0072 7200 0000 7273 0000 0072 5c00  ...rr...rs...r\.
-00003560: 0000 a802 0000 72c8 0000 007a 124d 7947  ......r....z.MyG
-00003570: 7569 2e65 7869 745f 7072 6f67 7261 6d29  ui.exit_program)
-00003580: 1cda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00003590: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000035a0: 616d 655f 5f72 4600 0000 da04 626f 6f6c  ame__rF.....bool
-000035b0: 726d 0000 0072 9000 0000 7295 0000 0072  rm...r....r....r
-000035c0: 9700 0000 7263 0000 0072 6500 0000 7267  ....rc...re...rg
-000035d0: 0000 0072 b600 0000 7258 0000 0072 4e00  ...r....rX...rN.
-000035e0: 0000 7269 0000 0072 af00 0000 7250 0000  ..ri...r....rP..
-000035f0: 0072 5400 0000 7252 0000 0072 5600 0000  .rT...rR...rV...
-00003600: 72b9 0000 0072 5700 0000 725a 0000 0072  r....rW...rZ...r
-00003610: 6a00 0000 725b 0000 0072 5c00 0000 da0d  j...r[...r\.....
-00003620: 5f5f 636c 6173 7363 656c 6c5f 5f72 7200  __classcell__rr.
-00003630: 0000 7272 0000 0072 7000 0000 7273 0000  ..rr...rp...rs..
-00003640: 0072 0700 0000 3c00 0000 7330 0000 0008  .r....<...s0....
-00003650: 000c 0100 7f0e 7408 1708 0c08 0d08 2808  ......t.......(.
-00003660: 1308 130e 130e 070e 0608 2408 1508 0608  ..........$.....
-00003670: 0608 0608 1308 2908 2708 1208 1310 0772  ......).'......r
-00003680: 0700 0000 290f 72a9 0000 0072 4b00 0000  ....).r....rK...
-00003690: da07 7061 7468 6c69 6272 0200 0000 5a1f  ..pathlibr....Z.
-000036a0: 4354 6b43 6f6c 6f72 5069 636b 6572 2e63  CTkColorPicker.c
-000036b0: 746b 5f63 6f6c 6f72 5f70 6963 6b65 7272  tk_color_pickerr
-000036c0: 0300 0000 da17 6d61 7074 6173 6b65 722e  ......maptasker.
-000036d0: 7372 632e 6765 7470 7574 6172 6772 0400  src.getputargr..
-000036e0: 0000 da16 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
-000036f0: 632e 7379 7363 6f6e 7374 7205 0000 0072  c.sysconstr....r
-00003700: a500 0000 5a17 7365 745f 6465 6661 756c  ....Z.set_defaul
-00003710: 745f 636f 6c6f 725f 7468 656d 6572 8700  t_color_themer..
-00003720: 0000 5a03 4354 6b72 0700 0000 7272 0000  ..Z.CTkr....rr..
-00003730: 0072 7200 0000 7272 0000 0072 7300 0000  .rr...rr...rs...
-00003740: da08 3c6d 6f64 756c 653e 0100 0000 7316  ..<module>....s.
-00003750: 0000 0008 1208 010c 010c 010c 010c 010a  ................
-00003760: 030a 0202 0302 ff16 1d                   .........
+000005e0: 6563 6966 6963 2050 726f 6a65 6374 2074  ecific Project t
+000005f0: 6f20 6469 7370 6c61 790a 2020 202d 2050  o display.   - P
+00000600: 726f 6669 6c65 204e 616d 653a 2065 6e74  rofile Name: ent
+00000610: 6572 2061 2073 7065 6369 6669 6320 5072  er a specific Pr
+00000620: 6f66 696c 6520 746f 2064 6973 706c 6179  ofile to display
+00000630: 0a20 2020 2d20 5461 736b 204e 616d 653a  .   - Task Name:
+00000640: 2065 6e74 6572 2061 2073 7065 6369 6669   enter a specifi
+00000650: 6320 5461 736b 2074 6f20 6469 7370 6c61  c Task to displa
+00000660: 790a 2020 2028 5468 6573 6520 7468 7265  y.   (These thre
+00000670: 6520 6172 6520 6578 636c 7573 6976 653a  e are exclusive:
+00000680: 2065 6e74 6572 206f 6e65 206f 6e6c 7929   enter one only)
+00000690: 0a0a 2a20 436f 6c6f 7273 2074 6162 3a20  ..* Colors tab: 
+000006a0: 7365 6c65 6374 2063 6f6c 6f72 7320 666f  select colors fo
+000006b0: 7220 7661 7269 6f75 7320 656c 656d 656e  r various elemen
+000006c0: 7473 206f 6620 7468 6520 6469 7370 6c61  ts of the displa
+000006d0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+000006e0: 2865 2e67 2e20 636f 6c6f 7220 666f 7220  (e.g. color for 
+000006f0: 5072 6f6a 6563 7473 2c20 5072 6f66 696c  Projects, Profil
+00000700: 6573 2c20 5461 736b 732c 2065 7463 2e29  es, Tasks, etc.)
+00000710: 0a0a 2a20 4578 6974 3a20 4578 6974 2074  ..* Exit: Exit t
+00000720: 6865 2070 726f 6772 616d 2028 7175 6974  he program (quit
+00000730: 292e 0a0a 4e6f 7465 3a20 596f 7520 7769  )...Note: You wi
+00000740: 6c6c 2062 6520 7072 6f6d 7074 6564 2074  ll be prompted t
+00000750: 6f20 6964 656e 7469 6679 2079 6f75 7220  o identify your 
+00000760: 5461 736b 6572 2062 6163 6b75 7020 6669  Tasker backup fi
+00000770: 6c65 206f 6e63 650a 2020 2020 2020 796f  le once.      yo
+00000780: 7520 6869 7420 7468 6520 2752 756e 2720  u hit the 'Run' 
+00000790: 6275 7474 6f6e 6300 0000 0000 0000 0000  buttonc.........
+000007a0: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
+000007b0: fe00 0000 6500 5a01 6400 5a02 8700 6601  ....e.Z.d.Z...f.
+000007c0: 6401 6402 8408 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
+000007d0: 6405 6505 6602 6406 6407 8404 5a06 6408  d.e.f.d.d...Z.d.
+000007e0: 6409 8400 5a07 640a 640b 8400 5a08 640c  d...Z.d.d...Z.d.
+000007f0: 640d 8400 5a09 640e 640f 8400 5a0a 6410  d...Z.d.d...Z.d.
+00000800: 6411 8400 5a0b 6412 6413 8400 5a0c 6414  d...Z.d.d...Z.d.
+00000810: 650d 6602 6415 6416 8404 5a0e 6417 650d  e.f.d.d...Z.d.e.
+00000820: 6602 6418 6419 8404 5a0f 641a 650d 6602  f.d.d...Z.d.e.f.
+00000830: 641b 641c 8404 5a10 641d 641e 8400 5a11  d.d...Z.d.d...Z.
+00000840: 641f 6420 8400 5a12 6421 6422 8400 5a13  d.d ..Z.d!d"..Z.
+00000850: 6423 6424 8400 5a14 6425 6426 8400 5a15  d#d$..Z.d%d&..Z.
+00000860: 6427 6428 8400 5a16 6429 642a 8400 5a17  d'd(..Z.d)d*..Z.
+00000870: 642b 6518 642c 642d 6604 642e 642f 8404  d+e.d,d-f.d.d/..
+00000880: 5a19 6430 6431 8400 5a1a 6432 6433 8400  Z.d0d1..Z.d2d3..
+00000890: 5a1b 6434 6435 8400 5a1c 6436 6437 8400  Z.d4d5..Z.d6d7..
+000008a0: 5a1d 6438 6439 8400 5a1e 8700 0400 5a1f  Z.d8d9..Z.....Z.
+000008b0: 5300 293a da05 4d79 4775 6963 0100 0000  S.):..MyGuic....
+000008c0: 0000 0000 0000 0000 0100 0000 0800 0000  ................
+000008d0: 0300 0000 7332 0500 0074 0083 00a0 01a1  ....s2...t......
+000008e0: 0001 007c 00a0 0264 01a1 0101 007c 00a0  ...|...d.....|..
+000008f0: 0364 02a1 0101 007c 006a 0464 0364 0364  .d.....|.j.d.d.d
+00000900: 048d 0201 007c 006a 0464 0564 0664 048d  .....|.j.d.d.d..
+00000910: 0201 007c 006a 0564 0664 0364 048d 0201  ...|.j.d.d.d....
+00000920: 0074 066a 077c 0064 0764 0664 088d 037c  .t.j.|.d.d.d...|
+00000930: 005f 087c 006a 086a 0964 0664 0664 0964  ._.|.j.j.d.d.d.d
+00000940: 0a64 0b8d 0401 007c 006a 086a 0564 0c64  .d.....|.j.j.d.d
+00000950: 0364 048d 0201 0074 066a 0a7c 006a 0864  .d.....t.j.|.j.d
+00000960: 0d74 066a 0b64 0e64 0f64 108d 0264 118d  .t.j.d.d.d...d..
+00000970: 037c 005f 0c7c 006a 0c6a 0964 0664 0664  .|._.|.j.j.d.d.d
+00000980: 0e64 1264 138d 0401 0074 066a 0a7c 006a  .d.d.....t.j.|.j
+00000990: 0864 1464 1564 168d 037c 005f 0d7c 006a  .d.d.d...|._.|.j
+000009a0: 0d6a 0964 0364 0664 0e64 1764 138d 0401  .j.d.d.d.d.d....
+000009b0: 0074 066a 0e7c 006a 0867 0064 18a2 017c  .t.j.|.j.g.d...|
+000009c0: 006a 0f64 198d 037c 005f 107c 006a 106a  .j.d...|._.|.j.j
+000009d0: 0964 1a64 0664 0e64 1764 138d 0401 0074  .d.d.d.d.d.....t
+000009e0: 066a 117c 006a 087c 006a 1264 1b64 1c64  .j.|.j.|.j.d.d.d
+000009f0: 1d64 1e8d 057c 005f 137c 006a 136a 0964  .d...|._.|.j.j.d
+00000a00: 1f64 0664 0e64 2064 1564 218d 0501 0074  .d.d.d d.d!....t
+00000a10: 066a 117c 006a 087c 006a 1464 2264 1c64  .j.|.j.|.j.d"d.d
+00000a20: 1d64 1e8d 057c 005f 157c 006a 156a 0964  .d...|._.|.j.j.d
+00000a30: 2364 0664 0e64 2064 1564 218d 0501 0074  #d.d.d d.d!....t
+00000a40: 066a 117c 006a 087c 006a 1664 2464 1c64  .j.|.j.|.j.d$d.d
+00000a50: 1d64 1e8d 057c 005f 177c 006a 176a 0964  .d...|._.|.j.j.d
+00000a60: 2564 0664 0e64 2064 1564 218d 0501 0074  %d.d.d d.d!....t
+00000a70: 066a 187c 006a 0864 2664 1a64 277c 006a  .j.|.j.d&d.d'|.j
+00000a80: 1964 288d 057c 005f 1a7c 006a 1a6a 0964  .d(..|._.|.j.j.d
+00000a90: 0964 0664 2064 0e64 2964 218d 0501 0074  .d.d d.d)d!....t
+00000aa0: 066a 187c 006a 0864 2664 1a64 2a7c 006a  .j.|.j.d&d.d*|.j
+00000ab0: 1b64 288d 057c 005f 1c7c 006a 1c6a 0964  .d(..|._.|.j.j.d
+00000ac0: 2b64 0664 2064 0664 2c64 218d 0501 0074  +d.d d.d,d!....t
+00000ad0: 066a 0a7c 006a 0864 2d64 1564 168d 037c  .j.|.j.d-d.d...|
+00000ae0: 005f 1d7c 006a 1d6a 0964 2e64 0664 0e64  ._.|.j.j.d.d.d.d
+00000af0: 2064 138d 0401 0074 066a 0e7c 006a 0867   d.....t.j.|.j.g
+00000b00: 0064 2fa2 017c 006a 1e64 198d 037c 005f  .d/..|.j.d...|._
+00000b10: 1f7c 006a 1f6a 0964 0c64 0664 0664 2c64  .|.j.j.d.d.d.d,d
+00000b20: 308d 0401 0074 066a 187c 0064 3164 1a64  0....t.j.|.d1d.d
+00000b30: 327c 006a 2064 338d 057c 005f 217c 006a  2|.j d3..|._!|.j
+00000b40: 216a 0964 0964 0664 3464 3464 0a64 218d  !j.d.d.d4d4d.d!.
+00000b50: 0501 0074 066a 187c 0064 3164 1a64 357c  ...t.j.|.d1d.d5|
+00000b60: 006a 2264 3664 378d 067c 005f 237c 006a  .j"d6d7..|._#|.j
+00000b70: 236a 0964 0964 0364 3864 3464 0a64 218d  #j.d.d.d8d4d.d!.
+00000b80: 0501 0074 066a 187c 0064 3164 1a64 397c  ...t.j.|.d1d.d9|
+00000b90: 006a 2464 3664 378d 067c 005f 257c 006a  .j$d6d7..|._%|.j
+00000ba0: 256a 0964 2b64 0364 3864 3464 0a64 218d  %j.d+d.d8d4d.d!.
+00000bb0: 0501 0074 066a 187c 0064 3164 1a64 3a7c  ...t.j.|.d1d.d:|
+00000bc0: 006a 2664 3b64 378d 067c 005f 277c 006a  .j&d;d7..|._'|.j
+00000bd0: 276a 0964 2b64 1a64 3464 3464 138d 0401  'j.d+d.d4d4d....
+00000be0: 0074 066a 287c 0064 3c64 3d64 3e8d 037c  .t.j(|.d<d=d>..|
+00000bf0: 005f 297c 006a 296a 2a64 2664 3f8d 0101  ._)|.j)j*d&d?...
+00000c00: 007c 006a 296a 0964 0664 0364 4064 4064  .|.j)j.d.d.d@d@d
+00000c10: 0a64 218d 0501 0074 066a 2b7c 0064 3d64  .d!....t.j+|.d=d
+00000c20: 2664 418d 037c 005f 2c7c 006a 2c6a 0964  &dA..|._,|.j,j.d
+00000c30: 0664 1a64 4064 4064 0a64 218d 0501 007c  .d.d@d@d.d!....|
+00000c40: 006a 2ca0 2d64 42a1 0101 007c 006a 2ca0  .j,.-dB....|.j,.
+00000c50: 2d64 43a1 0101 007c 006a 2ca0 2d64 44a1  -dC....|.j,.-dD.
+00000c60: 0101 007c 006a 2ca0 2e64 42a1 016a 0464  ...|.j,..dB..j.d
+00000c70: 0664 0364 048d 0201 007c 006a 2ca0 2e64  .d.d.....|.j,..d
+00000c80: 43a1 016a 0464 0664 0364 048d 0201 0074  C..j.d.d.d.....t
+00000c90: 066a 2f7c 006a 2ca0 2e64 42a1 0164 457c  .j/|.j,..dB..dE|
+00000ca0: 006a 3064 2664 4664 478d 057c 005f 317c  .j0d&dFdG..|._1|
+00000cb0: 006a 316a 0964 0364 0664 0e64 4864 0a64  .j1j.d.d.d.dHd.d
+00000cc0: 218d 0501 0074 066a 2f7c 006a 2ca0 2e64  !....t.j/|.j,..d
+00000cd0: 42a1 0164 497c 006a 3264 2664 4664 478d  B..dI|.j2d&dFdG.
+00000ce0: 057c 005f 337c 006a 336a 0964 1a64 0664  .|._3|.j3j.d.d.d
+00000cf0: 0e64 4864 0a64 218d 0501 0074 066a 2f7c  .dHd.d!....t.j/|
+00000d00: 006a 2ca0 2e64 42a1 0164 4a7c 006a 3464  .j,..dB..dJ|.j4d
+00000d10: 2664 4664 478d 057c 005f 357c 006a 356a  &dFdG..|._5|.j5j
+00000d20: 0964 1f64 0664 0e64 4864 0a64 218d 0501  .d.d.d.dHd.d!...
+00000d30: 0074 066a 0a7c 006a 2ca0 2e64 42a1 0164  .t.j.|.j,..dB..d
+00000d40: 4b64 1564 168d 037c 005f 367c 006a 366a  Kd.d...|._6|.j6j
+00000d50: 0964 2364 0664 0e64 4864 138d 0401 0074  .d#d.d.dHd.....t
+00000d60: 066a 0a7c 006a 2ca0 2e64 43a1 0164 4c64  .j.|.j,..dC..dLd
+00000d70: 4d8d 027c 005f 377c 006a 376a 0964 0664  M..|._7|.j7j.d.d
+00000d80: 0664 0664 0664 138d 0401 0074 066a 0e7c  .d.d.d.....t.j.|
+00000d90: 006a 2ca0 2e64 43a1 0167 0064 4ea2 017c  .j,..dC..g.dN..|
+00000da0: 006a 3864 198d 037c 005f 397c 006a 396a  .j8d...|._9|.j9j
+00000db0: 0964 0364 0664 0e64 4864 138d 0401 0074  .d.d.d.dHd.....t
+00000dc0: 066a 117c 006a 2ca0 2e64 44a1 0164 4f7c  .j.|.j,..dD..dO|
+00000dd0: 006a 3a64 1c64 1d64 508d 057c 005f 3b7c  .j:d.d.dP..|._;|
+00000de0: 006a 296a 2a64 2664 518d 0101 007c 006a  .j)j*d&dQ....|.j
+00000df0: 3b6a 3c64 0e64 2064 528d 0201 007c 00a0  ;j<d.d dR....|..
+00000e00: 3d64 1ca1 0101 0064 0053 0029 534e 7a19  =d.....d.S.)SNz.
+00000e10: 4d61 7054 6173 6b65 7220 5275 6e74 696d  MapTasker Runtim
+00000e20: 6520 4f70 7469 6f6e 735a 0831 3130 3078  e OptionsZ.1100x
+00000e30: 3630 30e9 0100 0000 2901 da06 7765 6967  600.....)...weig
+00000e40: 6874 2902 e902 0000 00e9 0300 0000 7201  ht)...........r.
+00000e50: 0000 00e9 8c00 0000 2902 da05 7769 6474  ........)...widt
+00000e60: 685a 0d63 6f72 6e65 725f 7261 6469 7573  hZ.corner_radius
+00000e70: e906 0000 00da 046e 7365 7729 04da 0372  .......nsew)...r
+00000e80: 6f77 da06 636f 6c75 6d6e 5a07 726f 7773  ow..columnZ.rows
+00000e90: 7061 6eda 0673 7469 636b 79e9 0900 0000  pan..sticky.....
+00000ea0: da09 4d61 7054 6173 6b65 72e9 1400 0000  ..MapTasker.....
+00000eb0: 5a04 626f 6c64 2902 da04 7369 7a65 7209  Z.bold)...sizer.
+00000ec0: 0000 0029 02da 0474 6578 74da 0466 6f6e  ...)...text..fon
+00000ed0: 7429 0272 1500 0000 e90a 0000 00a9 0472  t).r...........r
+00000ee0: 1000 0000 7211 0000 00da 0470 6164 78da  ....r......padx.
+00000ef0: 0470 6164 797a 1544 6973 706c 6179 2044  .padyz.Display D
+00000f00: 6574 6169 6c20 4c65 7665 6c3a da01 7729  etail Level:..w)
+00000f10: 0272 1700 0000 da06 616e 6368 6f72 2902  .r......anchor).
+00000f20: 7219 0000 0072 0100 0000 a904 da01 30da  r....r........0.
+00000f30: 0131 da01 32da 0133 2902 da06 7661 6c75  .1..2..3)...valu
+00000f40: 6573 da07 636f 6d6d 616e 6472 0a00 0000  es..commandr....
+00000f50: 7a12 4469 7370 6c61 7920 436f 6e64 6974  z.Display Condit
+00000f60: 696f 6e73 5446 2904 7225 0000 0072 1700  ionsTF).r%...r..
+00000f70: 0000 da07 6f6e 7661 6c75 65da 086f 6666  ....onvalue..off
+00000f80: 7661 6c75 6572 0b00 0000 7219 0000 0029  valuer....r....)
+00000f90: 0572 1000 0000 7211 0000 0072 1b00 0000  .r....r....r....
+00000fa0: 721c 0000 0072 1200 0000 7a16 4469 7370  r....r....z.Disp
+00000fb0: 6c61 7920 5461 736b 6572 4e65 7420 496e  lay TaskerNet In
+00000fc0: 666f e904 0000 007a 1a44 6973 706c 6179  fo.....z.Display
+00000fd0: 2054 6173 6b65 7220 5072 6566 6572 656e   Tasker Preferen
+00000fe0: 6365 73e9 0500 0000 7a07 2336 3536 3366  ces.....z.#6563f
+00000ff0: 667a 0d53 6176 6520 5365 7474 696e 6773  fz.Save Settings
+00001000: 2904 da0c 626f 7264 6572 5f63 6f6c 6f72  )...border_color
+00001010: da0c 626f 7264 6572 5f77 6964 7468 7217  ..border_widthr.
+00001020: 0000 0072 2500 0000 da01 737a 1052 6573  ...r%.....sz.Res
+00001030: 746f 7265 2053 6574 7469 6e67 73e9 0700  tore Settings...
+00001040: 0000 da01 6e7a 1447 5549 2041 7070 6561  ....nz.GUI Appea
+00001050: 7261 6e63 6520 4d6f 6465 3ae9 0800 0000  rance Mode:.....
+00001060: 2903 da05 4c69 6768 74da 0444 6172 6b72  )...Light..Darkr
+00001070: 0600 0000 2904 7210 0000 0072 1100 0000  ....).r....r....
+00001080: 721b 0000 0072 1200 0000 7a07 2332 3436  r....r....z.#246
+00001090: 4642 367a 0d52 6573 6574 204f 7074 696f  FB6z.Reset Optio
+000010a0: 6e73 2905 da06 6d61 7374 6572 da08 6667  ns)...master..fg
+000010b0: 5f63 6f6c 6f72 722b 0000 0072 1700 0000  _colorr+...r....
+000010c0: 7225 0000 0029 0272 1500 0000 7215 0000  r%...).r....r...
+000010d0: 005a 0352 756e 2902 7a07 2330 4246 3037  .Z.Run).z.#0BF07
+000010e0: 357a 0723 3141 4436 3344 2906 7232 0000  5z.#1AD63D).r2..
+000010f0: 0072 3300 0000 722b 0000 0072 1700 0000  .r3...r+...r....
+00001100: 7225 0000 00da 0a74 6578 745f 636f 6c6f  r%.....text_colo
+00001110: 7229 02e9 c800 0000 7235 0000 005a 0552  r)......r5...Z.R
+00001120: 6552 756e da04 4578 6974 da03 5265 64e9  eRun..Exit..Red.
+00001130: 6400 0000 e9fa 0000 0029 02da 0668 6569  d........)...hei
+00001140: 6768 7472 0d00 0000 2901 5a16 7363 726f  ghtr....).Z.scro
+00001150: 6c6c 6261 725f 6275 7474 6f6e 5f63 6f6c  llbar_button_col
+00001160: 6f72 2902 7215 0000 0072 0100 0000 2902  or).r....r....).
+00001170: 720d 0000 005a 1973 6567 6d65 6e74 6564  r....Z.segmented
+00001180: 5f62 7574 746f 6e5f 6667 5f63 6f6c 6f72  _button_fg_color
+00001190: 7a0d 5370 6563 6966 6963 204e 616d 65da  z.Specific Name.
+000011a0: 0643 6f6c 6f72 735a 0544 6562 7567 7a0c  .ColorsZ.Debugz.
+000011b0: 5072 6f6a 6563 7420 4e61 6d65 7a07 2331  Project Namez.#1
+000011c0: 6263 3966 6629 0472 1700 0000 7225 0000  bc9ff).r....r%..
+000011d0: 0072 3300 0000 722a 0000 0029 0272 1900  .r3...r*...).r..
+000011e0: 0000 7219 0000 007a 0c50 726f 6669 6c65  ..r....z.Profile
+000011f0: 204e 616d 657a 0954 6173 6b20 4e61 6d65   Namez.Task Name
+00001200: 7a0f 2850 6963 6b20 4f4e 4c59 204f 6e65  z.(Pick ONLY One
+00001210: 297a 1f53 6574 2056 6172 696f 7573 2044  )z.Set Various D
+00001220: 6973 706c 6179 2043 6f6c 6f72 7320 4865  isplay Colors He
+00001230: 7265 a901 7217 0000 0029 0fda 0850 726f  re..r....)...Pro
+00001240: 6a65 6374 73da 0850 726f 6669 6c65 737a  jects..Profilesz
+00001250: 1144 6973 6162 6c65 6420 5072 6f66 696c  .Disabled Profil
+00001260: 6573 7a0d 4c61 756e 6368 6572 2054 6173  esz.Launcher Tas
+00001270: 6bfa 1250 726f 6669 6c65 2043 6f6e 6469  k..Profile Condi
+00001280: 7469 6f6e 73da 0554 6173 6b73 7a0e 2854  tions..Tasksz.(T
+00001290: 6173 6b29 2041 6374 696f 6e73 fa11 4163  ask) Actions..Ac
+000012a0: 7469 6f6e 2043 6f6e 6469 7469 6f6e 737a  tion Conditionsz
+000012b0: 0d41 6374 696f 6e20 4c61 6265 6c73 7a0c  .Action Labelsz.
+000012c0: 4163 7469 6f6e 204e 616d 6573 da06 5363  Action Names..Sc
+000012d0: 656e 6573 da0a 4261 636b 6772 6f75 6e64  enes..Background
+000012e0: da07 4275 6c6c 6574 73fa 1554 6173 6b65  ..Bullets..Taske
+000012f0: 724e 6574 2049 6e66 6f72 6d61 7469 6f6e  rNet Information
+00001300: fa12 5461 736b 6572 2050 7265 6665 7265  ..Tasker Prefere
+00001310: 6e63 6573 7a0a 4465 6275 6720 4d6f 6465  ncesz.Debug Mode
+00001320: 2904 7217 0000 0072 2500 0000 7226 0000  ).r....r%...r&..
+00001330: 0072 2700 0000 2901 722a 0000 0029 0272  .r'...).r*...).r
+00001340: 1b00 0000 721c 0000 0029 3eda 0573 7570  ....r....)>..sup
+00001350: 6572 da08 5f5f 696e 6974 5f5f da05 7469  er..__init__..ti
+00001360: 746c 65da 0867 656f 6d65 7472 79da 1467  tle..geometry..g
+00001370: 7269 645f 636f 6c75 6d6e 636f 6e66 6967  rid_columnconfig
+00001380: 7572 65da 1167 7269 645f 726f 7763 6f6e  ure..grid_rowcon
+00001390: 6669 6775 7265 da0d 6375 7374 6f6d 746b  figure..customtk
+000013a0: 696e 7465 725a 0843 546b 4672 616d 655a  interZ.CTkFrameZ
+000013b0: 0d73 6964 6562 6172 5f66 7261 6d65 da04  .sidebar_frame..
+000013c0: 6772 6964 da08 4354 6b4c 6162 656c 5a07  grid..CTkLabelZ.
+000013d0: 4354 6b46 6f6e 745a 0a6c 6f67 6f5f 6c61  CTkFontZ.logo_la
+000013e0: 6265 6c5a 0c64 6574 6169 6c5f 6c61 6265  belZ.detail_labe
+000013f0: 6c5a 0d43 546b 4f70 7469 6f6e 4d65 6e75  lZ.CTkOptionMenu
+00001400: da15 6465 7461 696c 5f73 656c 6563 7465  ..detail_selecte
+00001410: 645f 6576 656e 74da 1573 6964 6562 6172  d_event..sidebar
+00001420: 5f64 6574 6169 6c5f 6f70 7469 6f6e 5a0b  _detail_optionZ.
+00001430: 4354 6b43 6865 636b 426f 78da 0f63 6f6e  CTkCheckBox..con
+00001440: 6469 7469 6f6e 5f65 7665 6e74 da10 636f  dition_event..co
+00001450: 6e64 6974 696f 6e5f 6275 7474 6f6e da17  ndition_button..
+00001460: 6469 7370 6c61 795f 7461 736b 6572 6e65  display_taskerne
+00001470: 745f 6576 656e 74da 1864 6973 706c 6179  t_event..display
+00001480: 5f74 6173 6b65 726e 6574 5f62 7574 746f  _taskernet_butto
+00001490: 6eda 1964 6973 706c 6179 5f70 7265 6665  n..display_prefe
+000014a0: 7265 6e63 6573 5f65 7665 6e74 da1a 6469  rences_event..di
+000014b0: 7370 6c61 795f 7072 6566 6572 656e 6365  splay_preference
+000014c0: 735f 6275 7474 6f6e 5a09 4354 6b42 7574  s_buttonZ.CTkBut
+000014d0: 746f 6eda 1373 6176 655f 7365 7474 696e  ton..save_settin
+000014e0: 6773 5f65 7665 6e74 5a14 7361 7665 5f73  gs_eventZ.save_s
+000014f0: 6574 7469 6e67 735f 6275 7474 6f6e da16  ettings_button..
+00001500: 7265 7374 6f72 655f 7365 7474 696e 6773  restore_settings
+00001510: 5f65 7665 6e74 5a17 7265 7374 6f72 655f  _eventZ.restore_
+00001520: 7365 7474 696e 6773 5f62 7574 746f 6e5a  settings_buttonZ
+00001530: 1561 7070 6561 7261 6e63 655f 6d6f 6465  .appearance_mode
+00001540: 5f6c 6162 656c da1c 6368 616e 6765 5f61  _label..change_a
+00001550: 7070 6561 7261 6e63 655f 6d6f 6465 5f65  ppearance_mode_e
+00001560: 7665 6e74 da1b 6170 7065 6172 616e 6365  vent..appearance
+00001570: 5f6d 6f64 655f 6f70 7469 6f6e 656d 656e  _mode_optionemen
+00001580: 75da 1472 6573 6574 5f73 6574 7469 6e67  u..reset_setting
+00001590: 735f 6576 656e 745a 0c72 6573 6574 5f62  s_eventZ.reset_b
+000015a0: 7574 746f 6eda 0b72 756e 5f70 726f 6772  utton..run_progr
+000015b0: 616d 5a0a 7275 6e5f 6275 7474 6f6e da0d  amZ.run_button..
+000015c0: 7265 7275 6e5f 7072 6f67 7261 6d5a 0c72  rerun_programZ.r
+000015d0: 6572 756e 5f62 7574 746f 6eda 0c65 7869  erun_button..exi
+000015e0: 745f 7072 6f67 7261 6d5a 0b65 7869 745f  t_programZ.exit_
+000015f0: 6275 7474 6f6e da0a 4354 6b54 6578 7462  button..CTkTextb
+00001600: 6f78 da07 7465 7874 626f 78da 0963 6f6e  ox..textbox..con
+00001610: 6669 6775 7265 5a0a 4354 6b54 6162 7669  figureZ.CTkTabvi
+00001620: 6577 da07 7461 6276 6965 77da 0361 6464  ew..tabview..add
+00001630: da03 7461 625a 0e43 546b 5261 6469 6f42  ..tabZ.CTkRadioB
+00001640: 7574 746f 6eda 1973 696e 676c 655f 7072  utton..single_pr
+00001650: 6f6a 6563 745f 6e61 6d65 5f65 7665 6e74  oject_name_event
+00001660: da14 7374 7269 6e67 5f69 6e70 7574 5f62  ..string_input_b
+00001670: 7574 746f 6e31 da19 7369 6e67 6c65 5f70  utton1..single_p
+00001680: 726f 6669 6c65 5f6e 616d 655f 6576 656e  rofile_name_even
+00001690: 74da 1473 7472 696e 675f 696e 7075 745f  t..string_input_
+000016a0: 6275 7474 6f6e 32da 1673 696e 676c 655f  button2..single_
+000016b0: 7461 736b 5f6e 616d 655f 6576 656e 74da  task_name_event.
+000016c0: 1473 7472 696e 675f 696e 7075 745f 6275  .string_input_bu
+000016d0: 7474 6f6e 335a 0a6e 616d 655f 6c61 6265  tton3Z.name_labe
+000016e0: 6c5a 0b6c 6162 656c 5f74 6162 5f32 da0c  lZ.label_tab_2..
+000016f0: 636f 6c6f 7273 5f65 7665 6e74 5a12 636f  colors_eventZ.co
+00001700: 6c6f 7273 5f6f 7074 696f 6e65 6d65 6e75  lors_optionemenu
+00001710: da14 6465 6275 675f 6368 6563 6b62 6f78  ..debug_checkbox
+00001720: 5f65 7665 6e74 da0e 6465 6275 675f 6368  _event..debug_ch
+00001730: 6563 6b62 6f78 da04 7061 636b da0c 7365  eckbox..pack..se
+00001740: 745f 6465 6661 756c 7473 a901 da04 7365  t_defaults....se
+00001750: 6c66 a901 da09 5f5f 636c 6173 735f 5fa9  lf....__class__.
+00001760: 00fa 772f 5573 6572 732f 6d69 6b72 7562  ..w/Users/mikrub
+00001770: 696e 2f4c 6962 7261 7279 2f43 6c6f 7564  in/Library/Cloud
+00001780: 5374 6f72 6167 652f 476f 6f67 6c65 4472  Storage/GoogleDr
+00001790: 6976 652d 6d69 6b72 7562 696e 4067 6d61  ive-mikrubin@gma
+000017a0: 696c 2e63 6f6d 2f4d 7920 4472 6976 652f  il.com/My Drive/
+000017b0: 5079 7468 6f6e 2f6d 6170 7461 736b 6572  Python/maptasker
+000017c0: 2f6d 6170 7461 736b 6572 2f73 7263 2f75  /maptasker/src/u
+000017d0: 7365 7269 6e74 722e 7079 7248 0000 003e  serintr.pyrH...>
+000017e0: 0000 0073 7801 0000 0a01 0a03 0a01 0e03  ...sx...........
+000017f0: 0e01 0e01 1203 1401 1002 0401 0401 0201  ................
+00001800: 0c01 08fd 1405 0403 0801 08ff 1403 0401  ................
+00001810: 0401 0601 0401 08fd 1405 0403 0401 0401  ................
+00001820: 0201 0201 0201 08fb 1607 0403 0401 0401  ................
+00001830: 0201 0201 0201 08fb 0607 0a01 06ff 0405  ................
+00001840: 0401 0401 0201 0201 0201 08fb 0607 0a01  ................
+00001850: 06ff 0405 0401 0201 0201 0201 0401 08fb  ................
+00001860: 1607 0403 0401 0201 0201 0201 0401 08fb  ................
+00001870: 1607 0403 0801 08ff 1403 0401 0401 0601  ................
+00001880: 0401 08fd 1405 0403 0201 0201 0201 0201  ................
+00001890: 0401 08fb 0607 0a01 06ff 0405 0201 0201  ................
+000018a0: 0201 0201 0401 0201 08fa 0608 0a01 06ff  ................
+000018b0: 0405 0201 0201 0201 0201 0401 0201 08fa  ................
+000018c0: 0608 0a01 06ff 0405 0201 0201 0201 0201  ................
+000018d0: 0401 0201 08fa 1408 1203 0e01 1601 0403  ................
+000018e0: 0601 08ff 1603 0c01 0c01 0c01 0c01 0401  ................
+000018f0: 06ff 1603 0403 0a01 0201 0401 0201 0201  ................
+00001900: 08fb 0607 0a01 06ff 0405 0a01 0201 0401  ................
+00001910: 0201 0201 08fb 0607 0a01 06ff 0405 0a01  ................
+00001920: 0201 0401 0201 0201 08fb 0607 0a01 06ff  ................
+00001930: 0405 0e01 08ff 1403 0403 0c01 08ff 1403  ................
+00001940: 0401 0a01 0601 0411 08ed 1415 0403 0a01  ................
+00001950: 0201 0401 0201 0201 08fb 0e07 1001 0e03  ................
+00001960: 7a0e 4d79 4775 692e 5f5f 696e 6974 5f5f  z.MyGui.__init__
+00001970: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001980: 0002 0000 0043 0000 0073 2a00 0000 7c00  .....C...s*...|.
+00001990: a000 a100 0100 7401 6401 8301 0100 7c00  ......t.d.....|.
+000019a0: 6a02 6400 7501 7213 7c00 a002 a100 0100  j.d.u.r.|.......
+000019b0: 6400 5300 6400 5300 2902 4e5a 0964 6573  d.S.d.S.).NZ.des
+000019c0: 7472 6f79 6564 2903 da07 6465 7374 726f  troyed)...destro
+000019d0: 79da 0570 7269 6e74 5a0d 636c 6f73 696e  y..printZ.closin
+000019e0: 675f 6576 656e 7472 7100 0000 7275 0000  g_eventrq...ru..
+000019f0: 0072 7500 0000 7276 0000 00da 0763 6c6f  .ru...rv.....clo
+00001a00: 7369 6e67 3e01 0000 730a 0000 0008 0108  sing>...s.......
+00001a10: 010a 010c 0104 ff7a 0d4d 7947 7569 2e63  .......z.MyGui.c
+00001a20: 6c6f 7369 6e67 da0a 6669 7273 745f 7469  losing..first_ti
+00001a30: 6d65 6302 0000 0000 0000 0000 0000 0002  mec.............
+00001a40: 0000 0005 0000 0043 0000 0073 aa00 0000  .......C...s....
+00001a50: 7c00 6a00 6a01 6700 6401 a201 6402 8d01  |.j.j.g.d...d...
+00001a60: 0100 7c00 6a00 a002 6403 a101 0100 6404  ..|.j...d.....d.
+00001a70: 7c00 5f03 6405 0400 7c00 5f04 0400 7c00  |._.d...|._...|.
+00001a80: 5f05 0400 7c00 5f06 0400 7c00 5f07 0400  _...|._...|._...
+00001a90: 7c00 5f08 0400 7c00 5f09 0400 7c00 5f0a  |._...|._...|._.
+00001aa0: 0400 7c00 5f0b 7c00 5f0c 6406 0400 7c00  ..|._.|._.d...|.
+00001ab0: 5f0d 0400 7c00 5f0e 7c00 5f0f 6407 7c00  _...|._.|._.d.|.
+00001ac0: 5f10 7c00 6a11 a002 6408 a101 0100 6700  _.|.j...d.....g.
+00001ad0: 7c00 5f12 6408 7c00 5f13 7c01 7250 7c00  |._.d.|._.|.rP|.
+00001ae0: 6a14 a015 6409 640a 7416 1700 a102 0100  j...d.d.t.......
+00001af0: 6900 7c00 5f17 6400 5300 290b 4e72 1f00  i.|._.d.S.).Nr..
+00001b00: 0000 2901 7224 0000 0072 2100 0000 7208  ..).r$...r!...r.
+00001b10: 0000 0046 da00 720a 0000 0072 0600 0000  ...F..r....r....
+00001b20: fa03 302e 307a 104d 6170 5461 736b 6572  ..0.0z.MapTasker
+00001b30: 2048 656c 700a 0a29 1872 5100 0000 7262   Help..).rQ...rb
+00001b40: 0000 00da 0373 6574 da14 6469 7370 6c61  .....set..displa
+00001b50: 795f 6465 7461 696c 5f6c 6576 656c da1a  y_detail_level..
+00001b60: 6469 7370 6c61 795f 7072 6f66 696c 655f  display_profile_
+00001b70: 636f 6e64 6974 696f 6e73 da13 6469 7370  conditions..disp
+00001b80: 6c61 795f 7072 6566 6572 656e 6365 73da  lay_preferences.
+00001b90: 1164 6973 706c 6179 5f74 6173 6b65 726e  .display_taskern
+00001ba0: 6574 da05 6465 6275 675a 0e63 6c65 6172  et..debugZ.clear
+00001bb0: 5f73 6574 7469 6e67 73da 0572 6573 6574  _settings..reset
+00001bc0: da04 6578 6974 da0a 676f 5f70 726f 6772  ..exit..go_progr
+00001bd0: 616d 725e 0000 00da 1373 696e 676c 655f  amr^.....single_
+00001be0: 7072 6f6a 6563 745f 6e61 6d65 da13 7369  project_name..si
+00001bf0: 6e67 6c65 5f70 726f 6669 6c65 5f6e 616d  ngle_profile_nam
+00001c00: 65da 1073 696e 676c 655f 7461 736b 5f6e  e..single_task_n
+00001c10: 616d 65da 0e63 6f6c 6f72 5f74 6578 745f  ame..color_text_
+00001c20: 726f 7772 5b00 0000 da0c 636f 6c6f 725f  rowr[.....color_
+00001c30: 6c61 6265 6c73 da0f 6170 7065 6172 616e  labels..appearan
+00001c40: 6365 5f6d 6f64 6572 6100 0000 da06 696e  ce_modera.....in
+00001c50: 7365 7274 da09 494e 464f 5f54 4558 54da  sert..INFO_TEXT.
+00001c60: 0c63 6f6c 6f72 5f6c 6f6f 6b75 7029 0272  .color_lookup).r
+00001c70: 7200 0000 727a 0000 0072 7500 0000 7275  r...rz...ru...ru
+00001c80: 0000 0072 7600 0000 7270 0000 0044 0100  ...rv...rp...D..
+00001c90: 0073 3400 0000 1201 0c01 0601 0209 08f8  .s4.............
+00001ca0: 0401 02ff 0403 02fd 0405 02fb 0407 02f9  ................
+00001cb0: 0408 02f8 0408 02f8 0808 1201 0601 0c01  ................
+00001cc0: 0601 0601 0401 1201 0a01 7a12 4d79 4775  ..........z.MyGu
+00001cd0: 692e 7365 745f 6465 6661 756c 7473 6302  i.set_defaultsc.
+00001ce0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00001cf0: 0000 0043 0000 0073 5000 0000 7400 6a01  ...C...sP...t.j.
+00001d00: 7c00 6401 6402 8d02 7c00 5f02 7c00 6a02  |.d.d...|._.|.j.
+00001d10: 6a03 6403 6404 6405 6405 6406 8d04 0100  j.d.d.d.d.d.....
+00001d20: 7c00 6a02 a004 6407 7c01 a102 0100 7c00  |.j...d.|.....|.
+00001d30: 6a02 6a05 6408 6409 640a 8d02 0100 7c00  j.j.d.d.d.....|.
+00001d40: 6a02 a006 a100 0100 6400 5300 290b 4e72  j.......d.S.).Nr
+00001d50: 3900 0000 a901 720d 0000 0072 2800 0000  9.....r....r(...
+00001d60: 720a 0000 0072 1500 0000 721a 0000 0072  r....r....r....r
+00001d70: 7c00 0000 da08 6469 7361 626c 6564 7237  |.....disabledr7
+00001d80: 0000 00a9 02da 0573 7461 7465 7234 0000  .......stater4..
+00001d90: 00a9 0772 4d00 0000 7260 0000 0072 6100  ...rM...r`...ra.
+00001da0: 0000 724e 0000 0072 8c00 0000 7262 0000  ..rN...r....rb..
+00001db0: 00da 0966 6f63 7573 5f73 6574 2902 7272  ...focus_set).rr
+00001dc0: 0000 00da 0d65 7272 6f72 5f6d 6573 7361  .....error_messa
+00001dd0: 6765 7275 0000 0072 7500 0000 7276 0000  geru...ru...rv..
+00001de0: 00da 1164 6973 706c 6179 5f65 7272 6f72  ...display_error
+00001df0: 5f62 6f78 5d01 0000 730e 0000 0010 0114  _box]...s.......
+00001e00: 010e 0106 0104 0106 ff0e 037a 174d 7947  ...........z.MyG
+00001e10: 7569 2e64 6973 706c 6179 5f65 7272 6f72  ui.display_error
+00001e20: 5f62 6f78 6303 0000 0000 0000 0000 0000  _boxc...........
+00001e30: 0004 0000 0006 0000 0043 0000 0073 6200  .........C...sb.
+00001e40: 0000 7c02 7204 6401 6e01 6402 7d03 7400  ..|.r.d.n.d.}.t.
+00001e50: 6a01 7c00 6403 6404 8d02 7c00 5f02 7c00  j.|.d.d...|._.|.
+00001e60: 6a02 6a03 6405 6406 6407 6407 6408 8d04  j.j.d.d.d.d.d...
+00001e70: 0100 7c00 6a02 a004 6409 7c01 9b00 640a  ..|.j...d.|...d.
+00001e80: 9d02 a102 0100 7c00 6a02 6a05 640b 7c03  ......|.j.j.d.|.
+00001e90: 640c 8d02 0100 7c00 6a02 a006 a100 0100  d.....|.j.......
+00001ea0: 6400 5300 290d 4eda 0547 7265 656e 7237  d.S.).N..Greenr7
+00001eb0: 0000 0069 5802 0000 728f 0000 0072 2800  ...iX...r....r(.
+00001ec0: 0000 7208 0000 0072 1500 0000 721a 0000  ..r....r....r...
+00001ed0: 0072 7c00 0000 da01 0a72 9000 0000 7291  .r|......r....r.
+00001ee0: 0000 0072 9300 0000 2904 7272 0000 00da  ...r....).rr....
+00001ef0: 076d 6573 7361 6765 5a04 676f 6f64 da05  .messageZ.good..
+00001f00: 636f 6c6f 7272 7500 0000 7275 0000 0072  colorru...ru...r
+00001f10: 7600 0000 da13 6469 7370 6c61 795f 6d65  v.....display_me
+00001f20: 7373 6167 655f 626f 7869 0100 0073 1000  ssage_boxi...s..
+00001f30: 0000 0c01 1001 1401 1401 0601 0401 06ff  ................
+00001f40: 0e03 7a19 4d79 4775 692e 6469 7370 6c61  ..z.MyGui.displa
+00001f50: 795f 6d65 7373 6167 655f 626f 7863 0300  y_message_boxc..
+00001f60: 0000 0000 0000 0000 0000 0400 0000 0600  ................
+00001f70: 0000 4300 0000 738c 0000 0064 017d 037c  ..C...s....d.}.|
+00001f80: 0173 0d64 027c 0217 0064 0317 007d 0364  .s.d.|...d...}.d
+00001f90: 047c 005f 007c 006a 0172 167c 006a 0272  .|._.|.j.r.|.j.r
+00001fa0: 1664 057d 036e 117c 006a 0172 1f7c 006a  .d.}.n.|.j.r.|.j
+00001fb0: 0372 1f64 067d 036e 087c 006a 0272 277c  .r.d.}.n.|.j.r'|
+00001fc0: 006a 0372 2764 077d 037c 0372 387c 00a0  .j.r'd.}.|.r8|..
+00001fd0: 047c 03a1 0101 0064 085c 037c 005f 017c  .|.....d.\.|._.|
+00001fe0: 005f 027c 005f 0364 0053 007c 00a0 0564  ._.|._.d.S.|...d
+00001ff0: 097c 019b 0064 0a7c 029b 009d 0464 0ba1  .|...d.|.....d..
+00002000: 0201 0064 0053 0029 0c4e 727b 0000 007a  ...d.S.).Nr{...z
+00002010: 2145 7272 6f72 3a0a 0a54 6865 206e 616d  !Error:..The nam
+00002020: 6520 656e 7465 7265 6420 666f 7220 7468  e entered for th
+00002030: 6520 7a16 2069 7320 626c 616e 6b21 0a0a  e z. is blank!..
+00002040: 5472 7920 6167 6169 6e2e 467a 5b45 7272  Try again.Fz[Err
+00002050: 6f72 3a0a 0a59 6f75 2068 6176 6520 656e  or:..You have en
+00002060: 7465 7265 6420 626f 7468 2061 2050 726f  tered both a Pro
+00002070: 6a65 6374 2061 6e64 2061 2050 726f 6669  ject and a Profi
+00002080: 6c65 206e 616d 6521 0a0a 5472 7920 6167  le name!..Try ag
+00002090: 6169 6e20 616e 6420 6f6e 6c79 2073 656c  ain and only sel
+000020a0: 6563 7420 6f6e 652e 7a58 4572 726f 723a  ect one.zXError:
+000020b0: 0a0a 596f 7520 6861 7665 2065 6e74 6572  ..You have enter
+000020c0: 6564 2062 6f74 6820 6120 5072 6f6a 6563  ed both a Projec
+000020d0: 7420 616e 6420 6120 5461 736b 206e 616d  t and a Task nam
+000020e0: 6521 0a0a 5472 7920 6167 6169 6e20 616e  e!..Try again an
+000020f0: 6420 6f6e 6c79 2073 656c 6563 7420 6f6e  d only select on
+00002100: 652e 7a58 4572 726f 723a 0a0a 596f 7520  e.zXError:..You 
+00002110: 6861 7665 2065 6e74 6572 6564 2062 6f74  have entered bot
+00002120: 6820 6120 5072 6f66 696c 6520 616e 6420  h a Profile and 
+00002130: 6120 5461 736b 206e 616d 6521 0a0a 5472  a Task name!..Tr
+00002140: 7920 6167 6169 6e20 616e 6420 6f6e 6c79  y again and only
+00002150: 2073 656c 6563 7420 6f6e 652e 2903 727b   select one.).r{
+00002160: 0000 0072 7b00 0000 727b 0000 007a 1244  ...r{...r{...z.D
+00002170: 6973 706c 6179 206f 6e6c 7920 7468 6520  isplay only the 
+00002180: 277a 0227 2054 2906 5a0a 6e61 6d65 645f  'z.' T).Z.named_
+00002190: 6974 656d 7286 0000 0072 8700 0000 7288  itemr....r....r.
+000021a0: 0000 0072 9600 0000 729b 0000 0029 0472  ...r....r....).r
+000021b0: 7200 0000 da08 7468 655f 6e61 6d65 da0c  r.....the_name..
+000021c0: 656c 656d 656e 745f 6e61 6d65 7295 0000  element_namer...
+000021d0: 0072 7500 0000 7275 0000 0072 7600 0000  .ru...ru...rv...
+000021e0: da0a 6368 6563 6b5f 6e61 6d65 7601 0000  ..check_namev...
+000021f0: 7338 0000 0004 0104 0102 0202 0102 ff02  s8..............
+00002200: 0202 fe02 ff06 050c 0102 0204 ff0c 0402  ................
+00002210: 0204 ff0c 0402 0202 ff04 050a 0102 0502  ................
+00002220: fc04 0104 0108 0104 0310 0108 ff7a 104d  .............z.M
+00002230: 7947 7569 2e63 6865 636b 5f6e 616d 6563  yGui.check_namec
+00002240: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00002250: 0400 0000 4300 0000 f34c 0000 0064 017d  ....C....L...d.}
+00002260: 017c 00a0 007c 01a1 0101 007c 006a 01a0  .|...|.....|.j..
+00002270: 02a1 0001 007c 006a 03a0 02a1 0001 0074  .....|.j.......t
+00002280: 046a 0564 0264 0364 048d 027d 027c 02a0  .j.d.d.d...}.|..
+00002290: 06a1 007c 005f 077c 00a0 087c 006a 0764  ...|._.|...|.j.d
+000022a0: 05a1 0201 0064 0053 0029 064e 727b 0000  .....d.S.).Nr{..
+000022b0: 007a 1345 6e74 6572 2050 726f 6a65 6374  .z.Enter Project
+000022c0: 206e 616d 653a 7a18 4469 7370 6c61 7920   name:z.Display 
+000022d0: 5370 6563 6966 6963 2050 726f 6a65 6374  Specific Project
+000022e0: a902 7217 0000 0072 4900 0000 da07 5072  ..r....rI.....Pr
+000022f0: 6f6a 6563 7429 0972 9600 0000 7269 0000  oject).r....ri..
+00002300: 00da 0864 6573 656c 6563 7472 6b00 0000  ...deselectrk...
+00002310: 724d 0000 00da 0e43 546b 496e 7075 7444  rM.....CTkInputD
+00002320: 6961 6c6f 67da 0967 6574 5f69 6e70 7574  ialog..get_input
+00002330: 7286 0000 0072 9e00 0000 a903 7272 0000  r....r......rr..
+00002340: 0072 9500 0000 da06 6469 616c 6f67 7275  .r......dialogru
+00002350: 0000 0072 7500 0000 7276 0000 0072 6600  ...ru...rv...rf.
+00002360: 0000 9e01 0000 f312 0000 0004 020a 010a  ................
+00002370: 020a 0104 0204 0106 ff0a 0412 027a 1f4d  .............z.M
+00002380: 7947 7569 2e73 696e 676c 655f 7072 6f6a  yGui.single_proj
+00002390: 6563 745f 6e61 6d65 5f65 7665 6e74 6301  ect_name_eventc.
+000023a0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+000023b0: 0000 0043 0000 0072 9f00 0000 2906 4e72  ...C...r....).Nr
+000023c0: 7b00 0000 7a13 456e 7465 7220 5072 6f66  {...z.Enter Prof
+000023d0: 696c 6520 6e61 6d65 3a7a 1844 6973 706c  ile name:z.Displ
+000023e0: 6179 2053 7065 6369 6669 6320 5072 6f66  ay Specific Prof
+000023f0: 696c 6572 a000 0000 da07 5072 6f66 696c  iler......Profil
+00002400: 6529 0972 9600 0000 7267 0000 0072 a200  e).r....rg...r..
+00002410: 0000 726b 0000 0072 4d00 0000 72a3 0000  ..rk...rM...r...
+00002420: 0072 a400 0000 7287 0000 0072 9e00 0000  .r....r....r....
+00002430: 72a5 0000 0072 7500 0000 7275 0000 0072  r....ru...ru...r
+00002440: 7600 0000 7268 0000 00b1 0100 0072 a700  v...rh.......r..
+00002450: 0000 7a1f 4d79 4775 692e 7369 6e67 6c65  ..z.MyGui.single
+00002460: 5f70 726f 6669 6c65 5f6e 616d 655f 6576  _profile_name_ev
+00002470: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
+00002480: 0300 0000 0400 0000 4300 0000 729f 0000  ........C...r...
+00002490: 0029 064e 727b 0000 007a 1045 6e74 6572  .).Nr{...z.Enter
+000024a0: 2054 6173 6b20 6e61 6d65 3a7a 1544 6973   Task name:z.Dis
+000024b0: 706c 6179 2053 7065 6369 6669 6320 5461  play Specific Ta
+000024c0: 736b 72a0 0000 00da 0454 6173 6b29 0972  skr......Task).r
+000024d0: 9600 0000 7267 0000 0072 a200 0000 7269  ....rg...r....ri
+000024e0: 0000 0072 4d00 0000 72a3 0000 0072 a400  ...rM...r....r..
+000024f0: 0000 7288 0000 0072 9e00 0000 72a5 0000  ..r....r....r...
+00002500: 0072 7500 0000 7275 0000 0072 7600 0000  .ru...ru...rv...
+00002510: 726a 0000 00c4 0100 0072 a700 0000 7a1c  rj.......r....z.
+00002520: 4d79 4775 692e 7369 6e67 6c65 5f74 6173  MyGui.single_tas
+00002530: 6b5f 6e61 6d65 5f65 7665 6e74 da13 6e65  k_name_event..ne
+00002540: 775f 6170 7065 6172 616e 6365 5f6d 6f64  w_appearance_mod
+00002550: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+00002560: 0000 0300 0000 4300 0000 7314 0000 0074  ......C...s....t
+00002570: 00a0 017c 01a1 0101 007c 017c 005f 0264  ...|.....|.|._.d
+00002580: 0053 00a9 014e 2903 724d 0000 00da 1373  .S...N).rM.....s
+00002590: 6574 5f61 7070 6561 7261 6e63 655f 6d6f  et_appearance_mo
+000025a0: 6465 728b 0000 0029 0272 7200 0000 72aa  der....).rr...r.
+000025b0: 0000 0072 7500 0000 7275 0000 0072 7600  ...ru...ru...rv.
+000025c0: 0000 725a 0000 00d7 0100 0073 0400 0000  ..rZ.......s....
+000025d0: 0a01 0a01 7a22 4d79 4775 692e 6368 616e  ....z"MyGui.chan
+000025e0: 6765 5f61 7070 6561 7261 6e63 655f 6d6f  ge_appearance_mo
+000025f0: 6465 5f65 7665 6e74 da0e 6469 7370 6c61  de_event..displa
+00002600: 795f 6465 7461 696c 6302 0000 0000 0000  y_detailc.......
+00002610: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00002620: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00002630: 72ab 0000 0029 0172 7e00 0000 2902 7272  r....).r~...).rr
+00002640: 0000 0072 ad00 0000 7275 0000 0072 7500  ...r....ru...ru.
+00002650: 0000 7276 0000 0072 5000 0000 de01 0000  ..rv...rP.......
+00002660: 7302 0000 000a 017a 1b4d 7947 7569 2e64  s......z.MyGui.d
+00002670: 6574 6169 6c5f 7365 6c65 6374 6564 5f65  etail_selected_e
+00002680: 7665 6e74 da13 636f 6c6f 725f 7365 6c65  vent..color_sele
+00002690: 6374 6564 5f69 7465 6d63 0200 0000 0000  cted_itemc......
+000026a0: 0000 0000 0000 0800 0000 0800 0000 4300  ..............C.
+000026b0: 0000 73d6 0000 0067 0064 01a2 017d 027c  ..s....g.d...}.|
+000026c0: 006a 007c 006a 007c 006a 017c 006a 0267  .j.|.j.|.j.|.j.g
+000026d0: 047d 0374 03a0 0474 05a1 018f 3001 007c  .}.t...t....0..|
+000026e0: 02a0 067c 01a1 017d 047c 037c 0419 0073  ...|...}.|.|...s
+000026f0: 3c7c 01a0 0764 0264 03a1 027d 057c 05a0  <|...d.d...}.|..
+00002700: 0764 0464 03a1 027d 057c 00a0 0864 057c  .d.d...}.|...d.|
+00002710: 059b 0064 069d 0364 07a1 0201 0009 0057  ...d...d.......W
+00002720: 0064 0004 0004 0083 0301 0064 0053 0057  .d.........d.S.W
+00002730: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00002740: 4677 0101 0001 0001 0059 0001 0074 0983  Fw.......Y...t..
+00002750: 007d 067c 06a0 0aa1 007d 077c 0764 0075  .}.|.....}.|.d.u
+00002760: 0172 697c 00a0 087c 019b 0064 087c 079b  .ri|...|...d.|..
+00002770: 009d 0364 07a1 0201 007c 00a0 0b7c 077c  ...d.....|...|.|
+00002780: 01a1 0201 0064 0053 0064 0053 0029 094e  .....d.S.d.S.).N
+00002790: 2904 723f 0000 0072 4100 0000 7245 0000  ).r?...rA...rE..
+000027a0: 0072 4600 0000 7a08 5072 6f66 696c 6520  .rF...z.Profile 
+000027b0: 727b 0000 007a 0741 6374 696f 6e20 7a08  r{...z.Action z.
+000027c0: 4469 7370 6c61 7920 7a17 2069 7320 6e6f  Display z. is no
+000027d0: 7420 7365 7420 746f 2064 6973 706c 6179  t set to display
+000027e0: 2146 fa12 2063 6f6c 6f72 2063 6861 6e67  !F.. color chang
+000027f0: 6564 2074 6f20 290c 727f 0000 0072 8100  ed to ).r....r..
+00002800: 0000 7280 0000 00da 0a63 6f6e 7465 7874  ..r......context
+00002810: 6c69 62da 0873 7570 7072 6573 73da 0945  lib..suppress..E
+00002820: 7863 6570 7469 6f6e da05 696e 6465 78da  xception..index.
+00002830: 0772 6570 6c61 6365 729b 0000 0072 0300  .replacer....r..
+00002840: 0000 da03 6765 74da 1865 7874 7261 6374  ....get..extract
+00002850: 5f63 6f6c 6f72 5f66 726f 6d5f 6576 656e  _color_from_even
+00002860: 7429 0872 7200 0000 72ae 0000 005a 0d77  t).rr...r....Z.w
+00002870: 6172 6e69 6e67 5f63 6865 636b 5a0d 6368  arning_checkZ.ch
+00002880: 6563 6b5f 6167 6169 6e73 745a 0974 6865  eck_againstZ.the
+00002890: 5f69 6e64 6578 5a12 7468 655f 6f75 7470  _indexZ.the_outp
+000028a0: 7574 5f6d 6573 7361 6765 5a0a 7069 636b  ut_messageZ.pick
+000028b0: 5f63 6f6c 6f72 729a 0000 0072 7500 0000  _colorr....ru...
+000028c0: 7275 0000 0072 7600 0000 726c 0000 00e4  ru...rv...rl....
+000028d0: 0100 0073 3400 0000 0801 0407 0401 0401  ...s4...........
+000028e0: 0401 04fc 0c09 0a01 0801 0c01 0c01 0401  ................
+000028f0: 0c01 04ff 0203 10f8 0202 1cfe 060a 0801  ................
+00002900: 0801 0401 0e01 04ff 1005 04fa 7a12 4d79  ............z.My
+00002910: 4775 692e 636f 6c6f 7273 5f65 7665 6e74  Gui.colors_event
+00002920: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00002930: 0007 0000 0043 0000 0073 7600 0000 7c01  .....C...sv...|.
+00002940: 7c00 6a00 7401 7c02 1900 3c00 7c00 6a02  |.j.t.|...<.|.j.
+00002950: a003 7404 6a05 7c00 6a06 a007 6401 a101  ..t.j.|.j...d...
+00002960: 7c02 9b00 6402 9d02 7c01 6403 8d03 a101  |...d...|.d.....
+00002970: 0100 7c00 6a02 6404 1900 6a08 7c00 6a09  ..|.j.d...j.|.j.
+00002980: 6405 6405 6405 6406 8d04 0100 7c00 0400  d.d.d.d.....|...
+00002990: 6a09 6407 3700 0200 5f09 7c00 a00a 7c02  j.d.7..._.|...|.
+000029a0: 9b00 6408 7c01 9b00 9d03 6409 a102 0100  ..d.|.....d.....
+000029b0: 6400 5300 290a 4e72 3b00 0000 7a09 203c  d.S.).Nr;...z. <
+000029c0: 3c20 636f 6c6f 7229 0272 1700 0000 7234  < color).r....r4
+000029d0: 0000 00e9 ffff ffff 7201 0000 0072 1a00  ........r....r..
+000029e0: 0000 7208 0000 0072 af00 0000 5429 0b72  ..r....r....T).r
+000029f0: 8e00 0000 7205 0000 0072 8a00 0000 da06  ....r....r......
+00002a00: 6170 7065 6e64 724d 0000 0072 4f00 0000  appendrM...rO...
+00002a10: 7263 0000 0072 6500 0000 724e 0000 0072  rc...re...rN...r
+00002a20: 8900 0000 729b 0000 0029 0372 7200 0000  ....r....).rr...
+00002a30: 729a 0000 0072 ae00 0000 7275 0000 0072  r....r....ru...r
+00002a40: 7500 0000 7276 0000 0072 b600 0000 0802  u...rv...r......
+00002a50: 0000 731c 0000 0002 030c ff06 0304 010a  ..s.............
+00002a60: 0108 0102 0104 fd04 ff1a 070e 0104 010e  ................
+00002a70: 0108 ff7a 1e4d 7947 7569 2e65 7874 7261  ...z.MyGui.extra
+00002a80: 6374 5f63 6f6c 6f72 5f66 726f 6d5f 6576  ct_color_from_ev
+00002a90: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
+00002aa0: 0100 0000 0200 0000 4300 0000 f310 0000  ........C.......
+00002ab0: 007c 006a 00a0 01a1 007c 005f 0264 0053  .|.j.....|._.d.S
+00002ac0: 0072 ab00 0000 2903 7253 0000 0072 b500  .r....).rS...r..
+00002ad0: 0000 727f 0000 0072 7100 0000 7275 0000  ..r....rq...ru..
+00002ae0: 0072 7500 0000 7276 0000 0072 5200 0000  .ru...rv...rR...
+00002af0: 1d02 0000 f302 0000 0010 017a 154d 7947  ...........z.MyG
+00002b00: 7569 2e63 6f6e 6469 7469 6f6e 5f65 7665  ui.condition_eve
+00002b10: 6e74 6301 0000 0000 0000 0000 0000 0001  ntc.............
+00002b20: 0000 0002 0000 0043 0000 0072 b900 0000  .......C...r....
+00002b30: 72ab 0000 0029 0372 5700 0000 72b5 0000  r....).rW...r...
+00002b40: 0072 8000 0000 7271 0000 0072 7500 0000  .r....rq...ru...
+00002b50: 7275 0000 0072 7600 0000 7256 0000 0023  ru...rv...rV...#
+00002b60: 0200 0072 ba00 0000 7a1f 4d79 4775 692e  ...r....z.MyGui.
+00002b70: 6469 7370 6c61 795f 7072 6566 6572 656e  display_preferen
+00002b80: 6365 735f 6576 656e 7463 0100 0000 0000  ces_eventc......
+00002b90: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00002ba0: 0000 72b9 0000 0072 ab00 0000 2903 7255  ..r....r....).rU
+00002bb0: 0000 0072 b500 0000 7281 0000 0072 7100  ...r....r....rq.
+00002bc0: 0000 7275 0000 0072 7500 0000 7276 0000  ..ru...ru...rv..
+00002bd0: 0072 5400 0000 2902 0000 72ba 0000 007a  .rT...)...r....z
+00002be0: 1d4d 7947 7569 2e64 6973 706c 6179 5f74  .MyGui.display_t
+00002bf0: 6173 6b65 726e 6574 5f65 7665 6e74 6301  askernet_eventc.
+00002c00: 0000 0000 0000 0000 0000 0002 0000 0009  ................
+00002c10: 0000 0043 0000 0073 4a00 0000 7c00 6a00  ...C...sJ...|.j.
+00002c20: 7c00 6a01 7c00 6a02 7c00 6a03 7c00 6a04  |.j.|.j.|.j.|.j.
+00002c30: 7c00 6a05 7c00 6a06 7c00 6a07 6401 9c08  |.j.|.j.|.j.d...
+00002c40: 7d01 7408 6402 7c00 6a09 7c01 8303 5c02  }.t.d.|.j.|...\.
+00002c50: 7d01 7c00 5f09 7c00 a00a 6403 6402 a102  }.|._.|...d.d...
+00002c60: 0100 6400 5300 2904 4e29 0872 7e00 0000  ..d.S.).N).r~...
+00002c70: 727f 0000 0072 8000 0000 7281 0000 0072  r....r....r....r
+00002c80: 8600 0000 7287 0000 0072 8800 0000 7282  ....r....r....r.
+00002c90: 0000 0054 7a0f 5365 7474 696e 6773 2073  ...Tz.Settings s
+00002ca0: 6176 6564 2e29 0b72 7e00 0000 727f 0000  aved.).r~...r...
+00002cb0: 0072 8000 0000 7281 0000 0072 8600 0000  .r....r....r....
+00002cc0: 7287 0000 0072 8800 0000 7282 0000 0072  r....r....r....r
+00002cd0: 0400 0000 728e 0000 0072 9b00 0000 a902  ....r....r......
+00002ce0: 7272 0000 00da 0974 656d 705f 6172 6773  rr.....temp_args
+00002cf0: 7275 0000 0072 7500 0000 7276 0000 0072  ru...ru...rv...r
+00002d00: 5800 0000 2f02 0000 731a 0000 0004 0204  X.../...s.......
+00002d10: 0104 0104 0104 0104 0104 0104 0106 f802  ................
+00002d20: 0a08 010a ff10 037a 194d 7947 7569 2e73  .......z.MyGui.s
+00002d30: 6176 655f 7365 7474 696e 6773 5f65 7665  ave_settings_eve
+00002d40: 6e74 6303 0000 0000 0000 0000 0000 0004  ntc.............
+00002d50: 0000 0004 0000 0043 0000 0073 4601 0000  .......C...sF...
+00002d60: 6401 7d03 7c01 0400 6402 6b02 7218 0100  d.}.|...d.k.r...
+00002d70: 7c02 7211 7c00 6a00 a001 a100 0100 7c03  |.r.|.j.......|.
+00002d80: 5300 7c00 6a00 a002 a100 0100 7c03 5300  S.|.j.......|.S.
+00002d90: 0400 6403 6b02 7227 0100 7c00 6a03 a004  ..d.k.r'..|.j...
+00002da0: 7405 7c02 8301 a101 0100 7c03 5300 0400  t.|.......|.S...
+00002db0: 6404 6b02 723c 0100 7c02 7235 7c00 6a06  d.k.r<..|.r5|.j.
+00002dc0: a001 a100 0100 7c03 5300 7c00 6a06 a002  ......|.S.|.j...
+00002dd0: a100 0100 7c03 5300 0400 6405 6b02 7251  ....|.S...d.k.rQ
+00002de0: 0100 7c02 724a 7c00 6a07 a001 a100 0100  ..|.rJ|.j.......
+00002df0: 7c03 5300 7c00 6a07 a002 a100 0100 7c03  |.S.|.j.......|.
+00002e00: 5300 0400 6406 6b02 7266 0100 7c02 725f  S...d.k.rf..|.r_
+00002e10: 7c00 6a08 a001 a100 0100 7c03 5300 7c00  |.j.......|.S.|.
+00002e20: 6a08 a002 a100 0100 7c03 5300 0400 6407  j.......|.S...d.
+00002e30: 6b02 7277 0100 7c02 7275 7c03 9b00 6408  k.rw..|.ru|...d.
+00002e40: 7c02 9b00 6409 9d04 7d03 7c03 5300 0400  |...d...}.|.S...
+00002e50: 640a 6b02 7288 0100 7c02 7286 7c03 9b00  d.k.r...|.r.|...
+00002e60: 640b 7c02 9b00 6409 9d04 7d03 7c03 5300  d.|...d...}.|.S.
+00002e70: 640c 6b02 7297 7c02 7295 7c03 9b00 640d  d.k.r.|.r.|...d.
+00002e80: 7c02 9b00 6409 9d04 7d03 7c03 5300 0900  |...d...}.|.S...
+00002e90: 7c00 a009 640e 7c02 9b00 9d02 640f a102  |...d.|.....d...
+00002ea0: 0100 7c03 5300 2910 4e72 7b00 0000 7282  ..|.S.).Nr{...r.
+00002eb0: 0000 0072 7e00 0000 727f 0000 0072 8000  ...r~...r....r..
+00002ec0: 0000 7281 0000 0072 8600 0000 7a0f 5072  ..r....r....z.Pr
+00002ed0: 6f6a 6563 7420 7365 7420 746f 207a 022e  oject set to z..
+00002ee0: 0a72 8700 0000 7a0f 5072 6f66 696c 6520  .r....z.Profile 
+00002ef0: 7365 7420 746f 2072 8800 0000 7a0c 5461  set to r....z.Ta
+00002f00: 736b 2073 6574 2074 6f20 7a1d 5275 7472  sk set to z.Rutr
+00002f10: 6f68 2120 2055 6e64 6566 696e 6564 2061  oh!  Undefined a
+00002f20: 7267 756d 656e 743a 2046 290a 726e 0000  rgument: F).rn..
+00002f30: 00da 0673 656c 6563 7472 a200 0000 7251  ...selectr....rQ
+00002f40: 0000 0072 7d00 0000 da03 7374 7272 5300  ...r}.....strrS.
+00002f50: 0000 7257 0000 0072 5500 0000 729b 0000  ..rW...rU...r...
+00002f60: 0029 0472 7200 0000 da03 6b65 79da 0576  .).rr.....key..v
+00002f70: 616c 7565 7299 0000 0072 7500 0000 7275  aluer....ru...ru
+00002f80: 0000 0072 7600 0000 da0f 7265 7374 6f72  ...rv.....restor
+00002f90: 655f 6469 7370 6c61 7942 0200 0073 5800  e_displayB...sX.
+00002fa0: 0000 0401 0201 0a01 0401 0a01 041f 0ae3  ................
+00002fb0: 041d 0ae4 1001 041b 0ae6 0401 0a01 0418  ................
+00002fc0: 0aea 0416 0aeb 0401 0a01 0413 0aef 0411  ................
+00002fd0: 0af0 0401 0a01 040e 0af4 040c 0af5 0401  ................
+00002fe0: 1001 0409 0af8 0401 1001 0406 06fb 0401  ................
+00002ff0: 1001 0403 02fe 1201 0401 7a15 4d79 4775  ..........z.MyGu
+00003000: 692e 7265 7374 6f72 655f 6469 7370 6c61  i.restore_displa
+00003010: 7963 0100 0000 0000 0000 0000 0000 0200  yc..............
+00003020: 0000 0800 0000 4300 0000 739e 0000 007c  ......C...s....|
+00003030: 00a0 0064 01a1 0101 0069 007d 0174 0164  ...d.....i.}.t.d
+00003040: 017c 006a 027c 0183 035c 027d 017c 005f  .|.j.|...\.}.|._
+00003050: 0274 03a0 0474 05a1 018f 1d01 007c 0164  .t...t.......|.d
+00003060: 0219 0072 2c7c 00a0 067c 0164 0219 0064  ...r,|...|.d...d
+00003070: 01a1 0201 0009 0057 0064 0004 0004 0083  .......W.d......
+00003080: 0301 0064 0053 0057 0064 0004 0004 0083  ...d.S.W.d......
+00003090: 0301 006e 0831 0073 3677 0101 0001 0001  ...n.1.s6w......
+000030a0: 0059 0001 007c 0173 407c 006a 0272 477c  .Y...|.s@|.j.rG|
+000030b0: 00a0 077c 01a1 0101 0064 0053 007c 00a0  ...|.....d.S.|..
+000030c0: 0664 0364 01a1 0201 0064 0053 0029 044e  .d.d.....d.S.).N
+000030d0: 46da 036d 7367 7a17 4e6f 2073 6574 7469  F..msgz.No setti
+000030e0: 6e67 7320 6669 6c65 2066 6f75 6e64 2e29  ngs file found.)
+000030f0: 0872 7000 0000 7204 0000 0072 8e00 0000  .rp...r....r....
+00003100: 72b0 0000 0072 b100 0000 da08 4b65 7945  r....r......KeyE
+00003110: 7272 6f72 729b 0000 00da 1065 7874 7261  rrorr......extra
+00003120: 6374 5f73 6574 7469 6e67 7372 bb00 0000  ct_settingsr....
+00003130: 7275 0000 0072 7500 0000 7276 0000 0072  ru...ru...rv...r
+00003140: 5900 0000 6b02 0000 731e 0000 000a 0104  Y...k...s.......
+00003150: 0102 0208 010a ff0c 0408 0110 0102 0110  ................
+00003160: fd02 011c ff0a 050e 0110 027a 1c4d 7947  ...........z.MyG
+00003170: 7569 2e72 6573 746f 7265 5f73 6574 7469  ui.restore_setti
+00003180: 6e67 735f 6576 656e 7472 bc00 0000 da06  ngs_eventr......
+00003190: 7265 7475 726e 4e63 0200 0000 0000 0000  returnNc........
+000031a0: 0000 0000 0700 0000 0700 0000 4300 0000  ............C...
+000031b0: 73b6 0000 0064 015c 027d 027d 037c 01a0  s....d.\.}.}.|..
+000031c0: 00a1 0044 005d 1a5c 027d 047d 057c 0464  ...D.].\.}.}.|.d
+000031d0: 0075 0172 2274 017c 007c 047c 0583 0301  .u.r"t.|.|.|....
+000031e0: 007c 00a0 027c 047c 05a1 0204 007d 0372  .|...|.|.....}.r
+000031f0: 227c 027c 0317 007d 0271 0864 0264 0384  "|.|...}.q.d.d..
+00003200: 0074 03a0 00a1 0044 0083 017d 067c 006a  .t.....D...}.|.j
+00003210: 04a0 00a1 0044 005d 155c 027d 047d 057c  .....D.].\.}.}.|
+00003220: 0464 0075 0172 467c 029b 0064 047c 067c  .d.u.rF|...d.|.|
+00003230: 0419 009b 0064 057c 059b 0064 069d 067d  .....d.|...d...}
+00003240: 0271 317c 00a0 057c 029b 0064 079d 0264  .q1|...|...d...d
+00003250: 08a1 0201 007c 006a 0672 597c 00a0 07a1  .....|.j.rY|....
+00003260: 0001 0064 0053 0064 0053 0029 094e 2902  ...d.S.d.S.).N).
+00003270: 727b 0000 0072 7b00 0000 6301 0000 0000  r{...r{...c.....
+00003280: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
+00003290: 0000 0073 1600 0000 6900 7c00 5d07 5c02  ...s....i.|.].\.
+000032a0: 7d01 7d02 7c02 7c01 9302 7102 5300 7275  }.}.|.|...q.S.ru
+000032b0: 0000 0072 7500 0000 2903 da02 2e30 da01  ...ru...)....0..
+000032c0: 6bda 0176 7275 0000 0072 7500 0000 7276  k..vru...ru...rv
+000032d0: 0000 00da 0a3c 6469 6374 636f 6d70 3e85  .....<dictcomp>.
+000032e0: 0200 0073 0200 0000 1600 7a2a 4d79 4775  ...s......z*MyGu
+000032f0: 692e 6578 7472 6163 745f 7365 7474 696e  i.extract_settin
+00003300: 6773 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  gs.<locals>.<dic
+00003310: 7463 6f6d 703e fa01 207a 0e20 636f 6c6f  tcomp>.. z. colo
+00003320: 7220 7365 7420 746f 2072 9800 0000 7a13  r set to r....z.
+00003330: 0a53 6574 7469 6e67 7320 7265 7374 6f72  .Settings restor
+00003340: 6564 2e54 2908 da05 6974 656d 73da 0773  ed.T)...items..s
+00003350: 6574 6174 7472 72c1 0000 0072 0500 0000  etattrr....r....
+00003360: 728e 0000 0072 9b00 0000 7282 0000 0072  r....r....r....r
+00003370: 6d00 0000 2907 7272 0000 0072 bc00 0000  m...).rr...r....
+00003380: 5a0c 616c 6c5f 6d65 7373 6167 6573 5a0b  Z.all_messagesZ.
+00003390: 6e65 775f 6d65 7373 6167 6572 bf00 0000  new_messager....
+000033a0: 72c0 0000 005a 0f69 6e76 5f63 6f6c 6f72  r....Z.inv_color
+000033b0: 5f6e 616d 6573 7275 0000 0072 7500 0000  _namesru...ru...
+000033c0: 7276 0000 0072 c400 0000 7d02 0000 7322  rv...r....}...s"
+000033d0: 0000 0008 0110 0108 010c 0110 0108 0102  ................
+000033e0: 8012 0212 0108 0118 0202 ff02 8012 0406  ................
+000033f0: 010c 0104 ff7a 164d 7947 7569 2e65 7874  .....z.MyGui.ext
+00003400: 7261 6374 5f73 6574 7469 6e67 7363 0100  ract_settingsc..
+00003410: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00003420: 0000 4300 0000 738c 0000 007c 006a 00a0  ..C...s....|.j..
+00003430: 0164 01a1 0101 007c 006a 02a0 03a1 0001  .d.....|.j......
+00003440: 007c 006a 04a0 03a1 0001 007c 006a 05a0  .|.j.......|.j..
+00003450: 03a1 0001 007c 006a 06a0 0164 02a1 0101  .....|.j...d....
+00003460: 0074 07a0 0864 02a1 0101 007c 006a 09a0  .t...d.....|.j..
+00003470: 03a1 0001 007c 00a0 0a64 0364 04a1 0201  .....|...d.d....
+00003480: 007c 00a0 0b64 05a1 0101 007c 006a 0c72  .|...d.....|.j.r
+00003490: 3f7c 006a 0c44 005d 087d 017c 016a 0d64  ?|.j.D.].}.|.j.d
+000034a0: 0564 068d 0101 0071 367c 00a0 0e64 07a1  .d.....q6|...d..
+000034b0: 0101 0064 0053 0029 084e 7221 0000 0072  ...d.S.).Nr!...r
+000034c0: 0600 0000 7a0f 5365 7474 696e 6773 2072  ....z.Settings r
+000034d0: 6573 6574 2e54 727b 0000 0072 3c00 0000  eset.Tr{...r<...
+000034e0: 4629 0f72 5100 0000 727d 0000 0072 5300  F).rQ...r}...rS.
+000034f0: 0000 72a2 0000 0072 5700 0000 7255 0000  ..r....rW...rU..
+00003500: 0072 5b00 0000 724d 0000 0072 ac00 0000  .r[...rM...r....
+00003510: 726e 0000 0072 9b00 0000 7296 0000 0072  rn...r....r....r
+00003520: 8a00 0000 7262 0000 0072 7000 0000 2902  ....rb...rp...).
+00003530: 7272 0000 00da 056c 6162 656c 7275 0000  rr.....labelru..
+00003540: 0072 7500 0000 7276 0000 0072 5c00 0000  .ru...rv...r\...
+00003550: 9302 0000 731a 0000 000c 010a 010a 010a  ....s...........
+00003560: 010c 010a 010a 010c 010a 0106 010a 010e  ................
+00003570: 010e 017a 1a4d 7947 7569 2e72 6573 6574  ...z.MyGui.reset
+00003580: 5f73 6574 7469 6e67 735f 6576 656e 7463  _settings_eventc
+00003590: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000035a0: 0400 0000 4300 0000 734e 0000 007c 006a  ....C...sN...|.j
+000035b0: 00a0 01a1 007c 005f 027c 006a 0272 1f74  .....|._.|.j.r.t
+000035c0: 0364 0183 01a0 04a1 0072 177c 00a0 0564  .d.......r.|...d
+000035d0: 0264 03a1 0201 0064 0053 007c 00a0 0564  .d.....d.S.|...d
+000035e0: 0464 05a1 0201 0064 0053 007c 00a0 0564  .d.....d.S.|...d
+000035f0: 0664 03a1 0201 0064 0053 0029 074e 7a0a  .d.....d.S.).Nz.
+00003600: 6261 636b 7570 2e78 6d6c 7a13 4465 6275  backup.xmlz.Debu
+00003610: 6720 6d6f 6465 2065 6e61 626c 6564 2e54  g mode enabled.T
+00003620: 7a53 4465 6275 6720 6d6f 6465 2072 6571  zSDebug mode req
+00003630: 7569 7265 7320 5461 736b 6572 2062 6163  uires Tasker bac
+00003640: 6b75 7020 6669 6c65 2074 6f20 6265 206e  kup file to be n
+00003650: 616d 6564 3a20 2762 6163 6b75 702e 786d  amed: 'backup.xm
+00003660: 6c27 2c20 7768 6963 6820 6973 206d 6973  l', which is mis
+00003670: 7369 6e67 2146 7a14 4465 6275 6720 6d6f  sing!Fz.Debug mo
+00003680: 6465 2064 6973 6162 6c65 642e 2906 726e  de disabled.).rn
+00003690: 0000 0072 b500 0000 7282 0000 0072 0200  ...r....r....r..
+000036a0: 0000 da07 6973 5f66 696c 6572 9b00 0000  ....is_filer....
+000036b0: 7271 0000 0072 7500 0000 7275 0000 0072  rq...ru...ru...r
+000036c0: 7600 0000 726d 0000 00a5 0200 0073 1200  v...rm.......s..
+000036d0: 0000 0c01 0601 0c01 1001 0402 0202 0203  ................
+000036e0: 08fb 1008 7a1a 4d79 4775 692e 6465 6275  ....z.MyGui.debu
+000036f0: 675f 6368 6563 6b62 6f78 5f65 7665 6e74  g_checkbox_event
+00003700: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00003710: 0002 0000 0043 0000 00f3 1200 0000 6401  .....C........d.
+00003720: 7c00 5f00 7c00 a001 a100 0100 6400 5300  |._.|.......d.S.
+00003730: a902 4e54 2902 7285 0000 00da 0471 7569  ..NT).r......qui
+00003740: 7472 7100 0000 7275 0000 0072 7500 0000  trq...ru...ru...
+00003750: 7276 0000 0072 5d00 0000 b802 0000 f304  rv...r].........
+00003760: 0000 0006 010c 017a 114d 7947 7569 2e72  .......z.MyGui.r
+00003770: 756e 5f70 726f 6772 616d 6301 0000 0000  un_programc.....
+00003780: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00003790: 0000 0073 1a00 0000 6401 7c00 5f00 7c00  ...s....d.|._.|.
+000037a0: a001 a100 0100 7c00 a002 a100 0100 6400  ......|.......d.
+000037b0: 5300 72d0 0000 0029 0372 5e00 0000 da08  S.r....).r^.....
+000037c0: 7769 7468 6472 6177 72d1 0000 0072 7100  withdrawr....rq.
+000037d0: 0000 7275 0000 0072 7500 0000 7276 0000  ..ru...ru...rv..
+000037e0: 0072 5e00 0000 bf02 0000 7306 0000 0006  .r^.......s.....
+000037f0: 0108 020c 017a 134d 7947 7569 2e72 6572  .....z.MyGui.rer
+00003800: 756e 5f70 726f 6772 616d 6301 0000 0000  un_programc.....
+00003810: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00003820: 0000 0072 cf00 0000 72d0 0000 0029 0272  ...r....r....).r
+00003830: 8400 0000 72d1 0000 0072 7100 0000 7275  ....r....rq...ru
+00003840: 0000 0072 7500 0000 7276 0000 0072 5f00  ...ru...rv...r_.
+00003850: 0000 c802 0000 72d2 0000 007a 124d 7947  ......r....z.MyG
+00003860: 7569 2e65 7869 745f 7072 6f67 7261 6d29  ui.exit_program)
+00003870: 20da 085f 5f6e 616d 655f 5fda 0a5f 5f6d   ..__name__..__m
+00003880: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00003890: 616d 655f 5f72 4800 0000 7279 0000 00da  ame__rH...ry....
+000038a0: 0462 6f6f 6c72 7000 0000 7296 0000 0072  .boolrp...r....r
+000038b0: 9b00 0000 729e 0000 0072 6600 0000 7268  ....r....rf...rh
+000038c0: 0000 0072 6a00 0000 72be 0000 0072 5a00  ...rj...r....rZ.
+000038d0: 0000 7250 0000 0072 6c00 0000 72b6 0000  ..rP...rl...r...
+000038e0: 0072 5200 0000 7256 0000 0072 5400 0000  .rR...rV...rT...
+000038f0: 7258 0000 0072 c100 0000 7259 0000 00da  rX...r....rY....
+00003900: 0464 6963 7472 c400 0000 725c 0000 0072  .dictr....r\...r
+00003910: 6d00 0000 725d 0000 0072 5e00 0000 725f  m...r]...r^...r_
+00003920: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00003930: 5f5f 7275 0000 0072 7500 0000 7273 0000  __ru...ru...rs..
+00003940: 0072 7600 0000 7207 0000 003d 0000 0073  .rv...r....=...s
+00003950: 3800 0000 0800 0c01 007f 007f 0802 0e06  8...............
+00003960: 0819 080c 080d 0828 0813 0813 0e13 0e07  .......(........
+00003970: 0e06 0824 0815 0806 0806 0806 0813 0829  ...$...........)
+00003980: 1212 0816 0812 0813 0807 1009 7207 0000  ............r...
+00003990: 0029 0f72 b000 0000 724d 0000 00da 0770  .).r....rM.....p
+000039a0: 6174 686c 6962 7202 0000 005a 1f43 546b  athlibr....Z.CTk
+000039b0: 436f 6c6f 7250 6963 6b65 722e 6374 6b5f  ColorPicker.ctk_
+000039c0: 636f 6c6f 725f 7069 636b 6572 7203 0000  color_pickerr...
+000039d0: 00da 176d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
+000039e0: 2e67 6574 7075 7461 7267 7204 0000 00da  .getputargr.....
+000039f0: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
+00003a00: 7973 636f 6e73 7472 0500 0000 72ac 0000  ysconstr....r...
+00003a10: 005a 1773 6574 5f64 6566 6175 6c74 5f63  .Z.set_default_c
+00003a20: 6f6c 6f72 5f74 6865 6d65 728d 0000 005a  olor_themer....Z
+00003a30: 0343 546b 7207 0000 0072 7500 0000 7275  .CTkr....ru...ru
+00003a40: 0000 0072 7500 0000 7276 0000 00da 083c  ...ru...rv.....<
+00003a50: 6d6f 6475 6c65 3e01 0000 0073 1600 0000  module>....s....
+00003a60: 0812 0801 0c01 0c01 0c01 0c01 0a03 0a02  ................
+00003a70: 0203 02ff 161e                           ......
```

### Comparing `maptasker-1.3.3/maptasker/src/__pycache__/xmldata.cpython-310.pyc` & `maptasker-1.3.4/maptasker/src/__pycache__/xmldata.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 10 19:04:43 2023 UTC, .py size: 6769 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cb5d 3464 711a 0000  o........]4dq...
+00000000: 6f0d 0d0a 0000 0000 a19c 4a64 711a 0000  o.........Jdq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6500 6401 6501 6402 6501 6606 6403 6404  e.d.e.d.e.f.d.d.
 00000040: 8404 5a02 6405 6406 8400 5a03 6402 6504  ..Z.d.d...Z.d.e.
 00000050: 6602 6407 6408 8404 5a05 6409 6500 640a  f.d.d...Z.d.e.d.
 00000060: 6500 6402 6500 6606 640b 640c 8404 5a06  e.d.e.f.d.d...Z.
 00000070: 640d 5300 290e da03 7461 67da 0466 6c61  d.S.)...tag..fla
@@ -143,17 +143,17 @@
 000008e0: 7265 706c 6163 6520 4854 4d4c 2077 6974  replace HTML wit
 000008f0: 682c 2069 6620 616e 790a 2020 2020 3a72  h, if any.    :r
 00000900: 6574 7572 6e3a 2074 6865 2074 6578 7420  eturn: the text 
 00000910: 7769 7468 2048 544d 4c20 7265 6d6f 7665  with HTML remove
 00000920: 640a 2020 2020 7207 0000 004e 7a05 3c2e  d.    r....Nz.<.
 00000930: 2a3f 3e29 03da 0272 65da 0763 6f6d 7069  *?>)...re..compi
 00000940: 6c65 da03 7375 6229 0472 1500 0000 7225  le..sub).r....r%
-00000950: 0000 0072 2600 0000 5a05 636c 6561 6e72  ...r&...Z.cleanr
+00000950: 0000 0072 2600 0000 da05 636c 6561 6e72  ...r&.....cleanr
 00000960: 0400 0000 7204 0000 0072 0500 0000 da10  ....r....r......
 00000970: 7265 6d6f 7665 5f68 746d 6c5f 7461 6773  remove_html_tags
 00000980: 8e00 0000 7306 0000 0008 060a 020e 0172  ....s..........r
-00000990: 2900 0000 4e29 07da 0373 7472 da04 626f  )...N)...str..bo
+00000990: 2a00 0000 4e29 07da 0373 7472 da04 626f  *...N)...str..bo
 000009a0: 6f6c 7206 0000 0072 2200 0000 7217 0000  olr....r"...r...
-000009b0: 0072 2400 0000 7229 0000 0072 0400 0000  .r$...r)...r....
+000009b0: 0072 2400 0000 722a 0000 0072 0400 0000  .r$...r*...r....
 000009c0: 7204 0000 0072 0400 0000 7205 0000 00da  r....r....r.....
 000009d0: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
 000009e0: 0000 1612 0839 0e30 1a12                 .....9.0..
```

### Comparing `maptasker-1.3.3/maptasker/src/actargs.py` & `maptasker-1.3.4/maptasker/src/actargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python3
 
 # ########################################################################################## #
 #                                                                                            #
-# actarg: process Task "Action" arguments                                                    #
+# actargs: process Task "Action" arguments                                                   #
 #                                                                                            #
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 # ########################################################################################## #
@@ -23,24 +23,24 @@
     argtype: list,
     code_action: defusedxml.ElementTree.XML,
     action_type: defusedxml.ElementTree.XML,
     colormap: dict,
     program_args: dict,
 ) -> dict:
     """
-
-    :param evaluated_results: all the Action argument "types" and "arguments"
-    :param arg: the incoming argument
-    :param argeval: the evaluation argument
-    :param argtype: the argument "type"
-    :param code_action: the Action code
-    :param action_type: the Action type
-    :param colormap: colors to use in output
-    :param program_args: runtime arguments
-    :return: dictionary of results
+    Given an <argn> element, evaluate it's contents based on our Action code dictionary (actionc.py)
+        :param evaluated_results: all the Action argument "types" and "arguments" as a dicitonary
+        :param arg: the incoming argument
+        :param argeval: the evaluation argument
+        :param argtype: the argument "type"
+        :param code_action: the Action code
+        :param action_type: the Action type
+        :param colormap: colors to use in output
+        :param program_args: runtime arguments
+        :return: dictionary of results
     """
     match argtype:
         case "Str":
             evaluated_results["get_xml_flag"] = True
             evaluated_results["strargs"].append(f"arg{str(arg)}")
             evaluated_results["streval"].append(argeval)
             evaluated_results["returning_something"] = True
```

### Comparing `maptasker-1.3.3/maptasker/src/action.py` & `maptasker-1.3.4/maptasker/src/action.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 
-import sys
+import defusedxml.ElementTree
 
 from maptasker.src.shellsort import shell_sort
 from maptasker.src.frmthtml import format_html
 from maptasker.src.xmldata import remove_html_tags
-from maptasker.src.sysconst import logger
+from maptasker.src.error import error_handler
 
 
 # #######################################################################################
 # Given a Task's Action, find all 'arg(n)' xml elements and return as a sorted list
 # Input:
 #   action: list of actions or parameters
 #   ignore_list: xml to ignore (e.g. label, on, etc.
@@ -131,22 +131,43 @@
             results.append("")
         else:
             results.append(item[2])
     return results
 
 
 # ####################################################################################################
-# given a required value logic and its position, evaluate the found integer and add to match_results
+# Given a required value logic and its position, evaluate the found integer and add to match_results
 # code_flag identifies the type of xml data to go after based on the specific code in <code>xxx</code>
 # *args is an undetermined number of lists, each consisting of 3 pairs:
 #   1: True=it is a string, False it is an integer,
 #   2: the value to test
 #   3: the value to plug in if it meets the test
 # ####################################################################################################
-def process_xml_list(names, arg_location, the_int_value, match_results, arguments):
+def process_xml_list(
+    names: list,
+    arg_location: int,
+    the_int_value: str,
+    match_results: list,
+    arguments: defusedxml.ElementTree,
+) -> None:
+    """
+    Given a required value logic and its position, evaluate the found integer and add to match_results
+    # code_flag identifies the type of xml data to go after based on the specific code in <code>xxx</code>
+    # *args is an undetermined number of lists, each consisting of 3 pairs:
+    #   1: True=it is a string, False it is an integer,
+    #   2: the value to test
+    #   3: the value to plug in if it meets the test
+        :param names: list of entries to substitute the argn value against.
+        :param arg_location: the location of the argument in the lookup table
+        :param the_int_value: tha integer value found in the <argn> xml element
+        :param match_results: list in which to return the evaluated values
+        :param arguments: list of Int arguments to look for (e.g. arg1,arg5,arg9)
+        :return: nothing
+    """
+    # list of entries to substitute the argn value against.
     # NOTE: Do NOT move this import statement to avoid recursion
     from maptasker.src.actiont import lookup_values
 
     the_list = names[arg_location]
     the_title = the_list[0]  # Title is first element in the list
     idx = 0
     running = True
@@ -177,61 +198,69 @@
         elif this_element == "l":  # Are we to do a table lookup for the value?
             idx = (idx + 1) % len(the_list)
             # next_element = the_list[idx]  # Second element in pair
             if the_list[idx] in lookup_values:
                 evaluated_value = [lookup_values[the_list[idx]][int(the_int_value)]]
                 evaluated_value = the_list[idx - 2] + evaluated_value[0] + ", "
                 match_results.append(evaluated_value)
+            # Error: the element is not in the lookup table.  OHandle the error and exit.
             else:
-                error_msg = (
-                    f"Program error: {the_list[idx]} is not in actiont (lookup table)"
-                    f" for name:{names}"
+                error_handler(
+                    (
+                        f"{the_list[idx]} is not in actiont"
+                        f" (lookup table) for name:{names}"
+                    ),
+                    1,
                 )
-                logger.debug(error_msg)
-                print(error_msg)
-                sys.exit(1)
+            # Get out of loop
             break
         else:
-            msg = (
+            # Not a valid entry in the lookup table
+            error_handler(
                 (
                     "get_xml_int_argument_to_value failed-"
-                    f" this_element:{this_element} {arguments}"
+                    f" this_element:{this_element} {arguments} for element"
+                    f" {this_element}"
                 ),
-                names,
+                1,
             )
-            logger.debug(msg)
-            exit(8)  # Rutroh...not an even pair of elements
+
     return
 
 
 # ####################################################################################################
 # Get Task's label, disabled flag and any conditions
 # ####################################################################################################
 def get_label_disabled_condition(child, colormap):
     task_label = ""
     task_conditions = ""
     the_action_code = child.find("code").text
+    # Get the label, if any
     if child.find("label") is not None:
         lbl = child.find("label").text
         # Make sure the label doesn't have any HTML crap in it
         task_label = clean_label(lbl, colormap)
-
+    # See if Action is disabled
     action_disabled = (
         format_html(colormap, "disabled_action_color", "", " [DISABLED]", True)
         if child.find("on") is not None
         else ""
     )
+    # Look for any conditions
     if child.find("ConditionList") is not None:  # If condition on Action?
         condition_count = 0
         boolean_to_inject = ""
         booleans = []
+        # Go through <ConditionList> sub-elements
         for children in child.find("ConditionList"):
             if "bool" in children.tag:
                 booleans.append(children.text)
+            # We have a condition and this is not an "If" condition
             elif children.tag == "Condition" and the_action_code != "37":
+                # Evaluate the condition to add to output
                 string1, operator, string2 = evaluate_condition(children)
                 if condition_count != 0:
                     boolean_to_inject = f"{booleans[condition_count - 1].upper()} "
                 task_conditions = format_html(
                     colormap,
                     "action_condition_color",
                     "",
@@ -264,20 +293,34 @@
 
 
 # ####################################################################################################
 # Chase after relevant data after <code> Task action
 # code_flag identifies the type of xml data to go after based on the specific code in <code>xxx</code>
 # Get the: label, whether to continue Task after error, etc.
 # ####################################################################################################
-def get_extra_stuff(code_action, action_type, colormap, program_args):
+def get_extra_stuff(
+    code_action: defusedxml.ElementTree,
+    action_type: bool,
+    colormap: dict,
+    program_args: dict,
+) -> str:
+    """
+    # Chase after relevant data after <code> Task action
+    # code_flag identifies the type of xml data to go after based on the specific code in <code>xxx</code>
+    # Get the: label, whether to continue Task after error, etc.
+        :param code_action: action code (e.g. "543") xml element
+        :param action_type: True if this is a Task Action, otherwise False
+        :param colormap: colors to use in output
+        :param program_args: runtime arguments
+        :return: formatted line of extra details about Task Action
+    """
     # Only get extras if this is a Task action (vs. a Profile condition)
     if action_type:
-        extra_stuff = get_label_disabled_condition(
-            code_action, colormap
-        )  # Look for extra Task stiff: label, disabled, conditions
+        # Look for extra Task stiff: label, disabled, conditions
+        extra_stuff = get_label_disabled_condition(code_action, colormap)
         if (
             "<font" in extra_stuff and "</font>" not in extra_stuff
         ):  # Make sure we terminate any fonts
             extra_stuff = f"{extra_stuff}</font>"
         if (
             "&lt;font" in extra_stuff and "&lt;/font&gt;" not in extra_stuff
         ):  # Make sure we terminate any fonts
@@ -291,22 +334,31 @@
     if (
         program_args["debug"] and action_type
     ):  # Add the code if this is an Action and in debug mode
         extra_stuff = format_html(
             colormap,
             "Yellow",
             "",
-            f'&nbsp;&nbsp;code: {code_action.find("code").text}-',
+            f'{extra_stuff}&nbsp;&nbsp;code: {code_action.find("code").text}-',
             False,
         )
 
     # See if Task action is to be continued after error
     child = code_action.find("se")
     if child is not None and child.text == "false":
-        extra_stuff = f" [Continue Task After Error]{extra_stuff}"
+        extra_stuff = (
+            format_html(
+                colormap,
+                "action_color",
+                "",
+                " [Continue Task After Error]",
+                True,
+            )
+            + f"{extra_stuff}"
+        )
     return f"{extra_stuff}</span>"
 
 
 # ####################################################################################################
 # Get the application specifics for the given code
 # ####################################################################################################
 def get_app_details(code_child, action_type, colormap, program_args):
```

### Comparing `maptasker-1.3.3/maptasker/src/actionc.py` & `maptasker-1.3.4/maptasker/src/actionc.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/actiond.py` & `maptasker-1.3.4/maptasker/src/actiond.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/actione.py` & `maptasker-1.3.4/maptasker/src/actione.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import re
 import defusedxml.ElementTree  # Need for type hints
 
 import maptasker.src.actionr as action_results
 
 from maptasker.src.action import get_extra_stuff
 from maptasker.src.frmthtml import format_html
+from maptasker.src.error import error_handler
 from maptasker.src.actionc import action_codes
 from maptasker.src.sysconst import logger
 from maptasker.src.sysconst import FONT_TO_USE
 
 pattern = re.compile(r",[, ]+")
 
 
@@ -50,32 +51,34 @@
     results = results.replace(", <font", "<font")
     return results
 
 
 # ####################################################################################################
 # For debug purposes, this searches dictionary for missing keys: 'reqargs' and 'display'
 # ####################################################################################################
-def look_for_missing_req():
+def look_for_missing_req() -> None:
+    """
+    For debug purposes, this searches dictionary for missing keys: 'reqargs' and 'display'
+        If found, the error is handled and the program exits
+    """
     flag = False
     for item in action_codes:
         entry = action_codes[item]
         numargs = entry["numargs"]
+        # Required arguments missing?  Exit with program error if so.
         if numargs > 0 and "reqargs" not in entry:
-            error_msg = f"Error: dict_code {item} missing reqargs!  numargs:{numargs}"
-            print(error_msg)
-            logger.debug(f"{error_msg}")
-            flag = True
+            error_handler(
+                f"dict_code {item} missing reqargs!  numargs:{numargs}",
+                1,
+            )
+        # Missing the entry's display name?
         if "display" not in entry:
-            error_msg = f'Error: dict_code {item} missing "display"!'
-            print(error_msg)
-            logger.debug(error_msg)
-            entry["display"] = "unmapped"
-            flag = True
-    if flag:
-        exit(99)
+            error_handler(f'dict_code {item} missing "display"!', 1)
+
+    return
 
 
 # ####################################################################################################
 # See if this Task or Profile code isa deprecated
 # ####################################################################################################
 def check_for_deprecation(dict_code):
     from maptasker.src.depricated import depricated
@@ -215,8 +218,8 @@
                             ),
                             True,
                         )
                     )
                     break
     else:
         alist.append(f"Action {code_element.text}: not yet mapped")
-    return
+    return alist
```

### Comparing `maptasker-1.3.3/maptasker/src/actionr.py` & `maptasker-1.3.4/maptasker/src/actionr.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import maptasker.src.action as get_action
 from maptasker.src.actargs import action_args
 from maptasker.src.actionc import action_codes
 from maptasker.src.frmthtml import format_html
 from maptasker.src.sysconst import logger
 from maptasker.src.xmldata import get_xml_int_argument_to_value
 from maptasker.src.xmldata import get_xml_str_argument_to_value
+from maptasker.src.xmldata import remove_html_tags
 
 
 # ####################################################################################################
 # Given a list of positional items, return a string in the correct order based on position
 # ####################################################################################################
 def get_results_in_arg_order(evaluated_results: dict) -> str:
     return_result = ""
@@ -125,15 +126,14 @@
     evaluated_results = defaultdict(
         lambda: []
     )  # Setup default dictionary as empty list
     two_blanks = "&nbsp;&nbsp;"
     result = ""
 
     # Save the associated data
-    # action_codes[dict_code]['display'] = display_name
     lookup_code_entry[dict_code]["reqargs"] = arg_list
     lookup_code_entry[dict_code]["evalargs"] = evaluate_list
     # If just displaying action names or there are no action details, then just display the name
     if arg_list and program_args["display_detail_level"] != 2:
         # Evaluate the required args per arg_list
         evaluated_results = evaluate_action_args(
             dict_code,
@@ -147,14 +147,18 @@
             evaluated_results,
         )
 
     # If we have results from evaluation, then go put them in their appropriate order
     if evaluated_results["returning_something"]:
         result = get_results_in_arg_order(evaluated_results)
 
+    # Clean up the arguments.  Replace <> so they appear properly and by remove any html
+    result = result.replace("<", "&lt;")
+    result = result.replace(">", "&gt;")
+
     # Return the properly formatted HTML with the Action name and extra stuff
     return format_html(
         colormap, "action_name_color", "", action_codes[dict_code]["display"], True
     ) + format_html(
         colormap,
         "action_color",
         "",
```

### Comparing `maptasker-1.3.3/maptasker/src/actiont.py` & `maptasker-1.3.4/maptasker/src/actiont.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/caveats.py` & `maptasker-1.3.4/maptasker/src/caveats.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/colors.py` & `maptasker-1.3.4/maptasker/src/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 import string
 from maptasker.src.sysconst import TYPES_OF_COLOR_NAMES
 from maptasker.src.sysconst import logger
+from maptasker.src.error import error_handler
 
 
 # #######################################################################################
 # Given a list [x,y,z] , print as x y z
 # #######################################################################################
 def print_list(list_title, the_list):
     line_out = ""
@@ -240,39 +241,28 @@
 # #######################################################################################
 # Get the runtime option for a color change and set it
 # #######################################################################################
 def get_and_set_the_color(the_arg, colormap):
     the_color_option = the_arg[2:].split("=")
     color_type = the_color_option[0]
     if len(the_color_option) < 2:  # Do we have the second parameter?
-        handle_error(
-            f"{the_arg} has an invalid 'color'.  See the help (-ch)!", " Exit code 7", 7
-        )
+        error_handler(f"{the_arg} has an invalid 'color'.  See the help (-ch)!", 7)
     if color_type not in TYPES_OF_COLOR_NAMES:
-        handle_error(
+        error_handler(
             f"{color_type} is an invalid type for 'color'.  See the help (-h)!",
             " Exit code 7",
             7,
         )
     desired_color = the_color_option[1]
     logger.debug(f" desired_color:{desired_color}")
     if validate_color(desired_color):  # If the color provided is valid...
         # match color_type:
         colormap[TYPES_OF_COLOR_NAMES[color_type]] = desired_color
     else:
-        error_msg = (
-            f"Invalid color specified: {desired_color} for 'c{the_color_option[0]}'!"
+        error_handler(
+            (
+                f"MapTasker...invalid color specified: {desired_color} for"
+                f" 'c{the_color_option[0]}'!"
+            ),
+            7,
         )
-        handle_error(error_msg, " exit code 7", 7)
     return
-
-
-def handle_error(error_msg: str, arg1: str, arg2: int) -> None:
-    """
-    Log and print error message, and then exit.
-        :param error_msg: message to output
-        :param arg1: exit code text
-        :param arg2: exit code number as int
-    """
-    logger.debug(f"{error_msg}{arg1}")
-    print(error_msg)
-    exit(arg2)
```

### Comparing `maptasker-1.3.3/maptasker/src/colrmode.py` & `maptasker-1.3.4/maptasker/src/colrmode.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/condition.py` & `maptasker-1.3.4/maptasker/src/condition.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/config.py` & `maptasker-1.3.4/maptasker/src/config.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/debug.py` & `maptasker-1.3.4/maptasker/src/debug.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/frmthtml.py` & `maptasker-1.3.4/maptasker/src/frmthtml.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/getids.py` & `maptasker-1.3.4/maptasker/src/getids.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/getputarg.py` & `maptasker-1.3.4/maptasker/src/getputarg.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 import json
 
 from maptasker.src.sysconst import ARGUMENTS_FILE
-from maptasker.src.sysconst import logger
+from maptasker.src.error import error_handler
 from pathlib import Path
 
 
 # #######################################################################################
 # Save and restore colors to use and program arguments
 # #######################################################################################
 def save_restore_args(
@@ -44,21 +44,24 @@
             with open(the_file, "r") as f:
                 list_to_restore = json.load(f)
                 colormap = list_to_restore[0]
                 temp_args = list_to_restore[1]
                 f.close()
         # Handle file not found condition
         except OSError:
-            error_msg = "'-r' Error: No settings file found to restore!"
-            print(error_msg)
-            logger.debug(error_msg)
+            error_handler("'-r' MapTasker Error: No settings file found to restore!", 0)
             temp_args = colormap = {"msg": "No settings file found to restore!"}
         # Handle file format error
         except json.decoder.JSONDecodeError:  # no saved file
-            error_msg = f"'-r' Error: The settings file,  {ARGUMENTS_FILE} is corrupt!"
-            print(error_msg)
-            logger.debug(error_msg)
+            error_handler(
+                f"'-restore' option... The settings file,  {ARGUMENTS_FILE} is corrupt!"
+                "  The old settings can not be restored.  Re-save your settings."
+            )
+            # Return the error as an entry in our dictionaries for display via te GUI, if needed.
             temp_args = colormap = {
-                "msg": "The settings file is corrupt!  Re-save your settings."
+                "msg": (
+                    "The settings file is corrupt!  The old settings can not be"
+                    " restored.  Re-save your settings."
+                )
             }
 
     return temp_args, colormap
```

### Comparing `maptasker-1.3.3/maptasker/src/initparg.py` & `maptasker-1.3.4/maptasker/src/initparg.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/kidapp.py` & `maptasker-1.3.4/maptasker/src/kidapp.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/mapit.py` & `maptasker-1.3.4/maptasker/src/mapit.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,42 +26,45 @@
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # Reference: https://github.com/Taskomater/Tasker-XML-Info                                   #
 #                                                                                            #
 # ########################################################################################## #
 
+import contextlib
 import sys
 import webbrowser  # To be removed in Python 10.13 (2023?)
 import defusedxml.ElementTree  # Need for type hints
 from os import getcwd
-from typing import List, Dict
+from typing import List
 
 import maptasker.src.outputl as build_output
 import maptasker.src.proginit as initialize
 import maptasker.src.projects as projects
 import maptasker.src.taskuniq as special_tasks
 from maptasker.src.caveats import display_caveats
 from maptasker.src.prefers import get_preferences
+from maptasker.src.error import error_handler
 from maptasker.src.sysconst import logger
+from maptasker.src.sysconst import debug_out
 
 
 # import os
 # print('Path:', os.getcwd())
 # print('__file__={0:<35} | __name__={1:<25} | __package__={2:<25}'.format(__file__,__name__,str(__package__)))
 
 
 # #######################################################################################
 # Clean up our memory hogs
 # #######################################################################################
 def clean_up_memory(
     tree: defusedxml.ElementTree.XML,
     root: defusedxml.ElementTree.XML,
     output_list: List[str],
-    all_tasker_items: Dict[str, List[defusedxml.ElementTree.XML]],
+    all_tasker_items: dict[str, List[defusedxml.ElementTree.XML]],
 ) -> None:
     """
     Clean up our memory hogs
         :param tree: xml tree to empty
         :param root: root xml that was parsed from backup file
         :param output_list: list of output lines to clear
         :param all_tasker_items: All Projects/Profiles/Tasks/Scenes
@@ -89,32 +92,49 @@
         :param output_list: list of all output lines generated
         :param my_output_dir: directory to output to
         :param my_file_name: name of file to use
         :return: nothing
     """
     logger.info(f"Function Entry: write_out_the_file dir:{my_output_dir}")
     with open(my_output_dir + my_file_name, "w") as out_file:
-        for item in output_list:
+        for num, item in enumerate(output_list):
+            # Make sure we don't have three </ul>'s in a row
+            item.rstrip()  # Get rid of trailing blanks
+            if (
+                num > 3
+                and item[:5] == "</ul>"
+                and (
+                    output_list[num - 1][:5] == "</ul>"
+                    and output_list[num - 2][:5] == "</ul>"
+                    and output_list[num + 1][:4] == "<br>"
+                )
+            ):
+                continue
+
             # Change "Action: nn ..." to Action nn: ..." (i.e. move the colon)
             action_position = item.find("Action: ")
             if action_position != -1:
                 action_number_list = item[action_position + 8 :].split(" ")
                 action_number = action_number_list[0]
                 temp = (
                     item[:action_position]
                     + action_number
                     + ":"
                     + item[action_position + 8 + len(action_number) :]
                 )
                 output_line = temp
             else:
                 output_line = item
+            # Get rid of extraneous html code that somehow got in to the output
             output_line = output_line.replace("</span></span>", "</span>")
             output_line = output_line.replace("</p></p>", "</p>")
+            # Write the actual final line out as html
             out_file.write(output_line)
+            if debug_out:
+                logger.debug(f"kaka:{output_line}")
     logger.info("Function Exit: write_out_the_file")
     return
 
 
 # ###############################################################################################
 # Cleanup memory and let user know there was no match found for Task/Profile
 # ###############################################################################################
@@ -134,17 +154,15 @@
         :param root: root of xml parsed from file to clear
         :param output_list: list of output lines to empty
         :param all_tasker_items: all Tasker Projects/Profiles/Tasks/Scenes to clear
         :rtype: colors, runtime arguments,
     """
 
     output_list.clear()
-    error_message = f"{name} {profile_or_task_name} not found!!"
-    print(error_message)
-    logger.debug(error_message)
+    error_handler(f"{name} {profile_or_task_name} not found!!", 0)
     clean_up_memory(tree, root, output_list, all_tasker_items)
     sys.exit(5)
 
 
 ##############################################################################################################
 #                                                                                                            #
 #   Main Program Starts Here                                                                                 #
@@ -189,15 +207,20 @@
 
 - It displays the final output by opening the output file in the default browser.
 
 - It returns the exit code of the program.
 '''
 
 
-def mapit_all() -> int:
+def mapit_all(file_to_get: str) -> int:
+    """
+    The primary code starts here
+        :param file_to_get: file name of input backup.xml file or none
+        :return: return code (zero or error code)
+    """
     # Initialize local variables and other stuff
     found_tasks, output_list, projects_without_profiles, projects_with_no_tasks = (
         [],
         [],
         [],
         [],
     )
@@ -209,15 +232,15 @@
         found_items,
         heading,
         output_list,
         tree,
         root,
         filename,
         all_tasker_items,
-    ) = initialize.start_up(output_list)
+    ) = initialize.start_up(output_list, file_to_get)
 
     # Development only parameters here:
     # program_args["display_detail_level"] = 3
     # program_args["display_profile_conditions"] = True
     # program_args['display_preferences'] = True
     # program_args['display_taskernet'] = True
 
@@ -331,34 +354,34 @@
     build_output.my_output(colormap, program_args, output_list, 0, error_msg)
 
     # Okay, lets generate the actual output file.
     # Store the output in the current  directory
     my_output_dir = getcwd()
     logger.debug(f"output directory:{my_output_dir}")
     if my_output_dir is None:
-        error_msg = "MapTasker cancelled.  An error occurred.  Program cancelled."
-        logger.debug(error_msg)
-        print(error_msg)
+        error_handler("MapTasker cancelled.  An error occurred.  Program cancelled.", 0)
         clean_up_memory(tree, root, output_list, all_tasker_items)
         sys.exit(2)
 
     my_file_name = "/MapTasker.html"
     # Output the generated html
     write_out_the_file(output_list, my_output_dir, my_file_name)
 
     # Clean up memory
     clean_up_memory(tree, root, output_list, all_tasker_items)
 
     # Display final output
     logger.debug("MapTasker program ended normally")
-    my_rc = 0
     try:
         webbrowser.open(f"file://{my_output_dir}{my_file_name}", new=2)
     except webbrowser.Error:
-        error_msg = (
-            "Error: Failed to open output in browser: your browser is not supported."
+        error_handler(
+            "Error: Failed to open output in browser: your browser is not supported.", 1
         )
-        print(error_msg)
-        logger.debug(error_msg)
-        my_rc = 1
+
     print("You can find 'MapTasker.html' in the current folder.  Program end.")
-    return my_rc
+
+    # If in ReRun mode, let's do it all again :o)
+    with contextlib.suppress(KeyError):
+        if program_args["rerun"]:
+            mapit_all(filename.name)
+    return 0
```

### Comparing `maptasker-1.3.3/maptasker/src/migrate.py` & `maptasker-1.3.4/maptasker/src/migrate.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,65 +14,88 @@
 #                                                                                            #
 # ########################################################################################## #
 import pickle
 from os import rename
 from pathlib import Path
 
 from maptasker.src.getputarg import save_restore_args
-from maptasker.src.sysconst import logger
+from maptasker.src.error import error_handler
 
 
 # #######################################################################################
 # Save program arguments
 # #######################################################################################
 def restore_old_args(file_to_check: Path) -> tuple[dict, dict]:
     """
     Save program arguments
         :param file_to_check: file path/object to restore
         :return: program runtime arguments and colors to use in output
     """
+    colormap = program_args = {}
 
     # Restore dictionaries
     try:
         with open(file_to_check, "rb") as f:
             colormap = pickle.load(f)
             program_args = pickle.load(f)
     except OSError:  # no saved file
-        error_msg = (
-            "'-r' Error (Restoring Older Settings File): There are no saved items found"
-            " to migrate!"
+        colormap, program_args = process_error(
+            (
+                "'-r' Error (Restoring Older Settings File): There are no saved items"
+                " found to migrate. Prior settings lost."
+            ),
         )
-        print(error_msg)
-        logger.debug(error_msg)
-        program_args, colormap = {}, {}
+
     except _pickle.UnpicklingError:  # Format error
-        error_msg = (
-            f"'-r' Error (Restoring Older Settings File): File {file_to_check} is"
-            " corrupt. to migrate!"
+        colormap, program_args = process_error(
+            (
+                f"'-r' Error (Restoring Older Settings File): File {file_to_check} is"
+                " corrupt.  Migration ignored.  Prior settings lost."
+            ),
+        )
+    except EOFError:
+        colormap, program_args = process_error(
+            (
+                f"'-r' Error (Restoring Older Settings File): File {file_to_check} is"
+                " corrupt.  Migration ignored."
+            ),
         )
-        print(error_msg)
-        logger.debug(error_msg)
-        program_args, colormap = {}, {}
 
     f.close()
 
     return program_args, colormap
 
 
+def process_error(error_msg: str) -> tuple[dict, dict]:
+    """
+    Disspaly and log error message and reset colors and program args to empty
+        :param error_msg: error to print/log
+        :return: empty colormap and program runtime arguments
+    """
+    error_handler(error_msg, 0)
+    return {}, {}
+
+
 # #######################################################################################
 # Migrate from old filename/format to new for saved runtime arguments
 # #######################################################################################
 def migrate() -> None:
-    OLD_ARGUMENTS_FILE = ".MapTasker_arguments.txt"
-    file_to_check = Path(f"{OLD_ARGUMENTS_FILE}")
+    """
+    Migrate from old filename/format to new for saved runtime arguments
+      We have changed from using the unsecure "pickle" code to using "json"
+      to save the program arguments and colors
+        :return: nothing
+    """
+    old_arguments_file = ".MapTasker_arguments.txt"
+    file_to_check = Path(f"{old_arguments_file}")
 
     dir_path = Path.cwd()
     # If we have an old formatted argument file, convert it to new old name
     with contextlib.suppress(FileNotFoundError):
-        rename(f"{dir_path}/.arguments.txt", f"{dir_path}/{OLD_ARGUMENTS_FILE}")
+        rename(f"{dir_path}/.arguments.txt", f"{dir_path}/{old_arguments_file}")
 
     # Now, if we have the old binary file saved via pickle, convert it to JSON
     if file_to_check.is_file():
         program_args, colormap = restore_old_args(file_to_check)
         # Save as JSON file
         nada, nada = save_restore_args(True, colormap, program_args)
         # Now delete the old file
```

### Comparing `maptasker-1.3.3/maptasker/src/outputl.py` & `maptasker-1.3.4/maptasker/src/outputl.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,17 +113,17 @@
 # #############################################################################################
 def ulify_list_item(
     element: defusedxml.ElementTree.XML, colormap: dict, font_to_use: str
 ) -> str:
     if (
         f'{font_to_use}">Project:' in element or "Project has no Profiles" in element
     ):  # Project ========================
-        return f'<li style=color:{colormap["bullet_color"]}>{element}</span></li>\n'
+        return f'<br><li style=color:{colormap["bullet_color"]}>{element}</li>\n'
     elif f'{font_to_use}">Profile:' in element:  # Profile ========================
-        return f'<li style=color:{colormap["bullet_color"]}>{element}</span></li>\n'
+        return f'<br><li style=color:{colormap["bullet_color"]}>{element}</span></li>\n'
     elif (
         element[:5] == "Task:" or "&#45;&#45;Task:" in element
     ):  # Task or Scene's Task ========================
         return (
             put_style(
                 style_details={
                     "is_list": True,
@@ -162,24 +162,15 @@
                 return ""
             tmp = action_evaluate.cleanup_the_result(
                 element.replace("Action: ...", "&nbsp;&nbsp;continued >>> ")
             )
             element = tmp
         return f'<li style=color:{colormap["bullet_color"]}>{element}</span></li>\n'
     elif "TaskerNet " in element:  # TaskerNet
-        return put_style(
-            style_details={
-                "is_list": False,
-                "color1": colormap['bullet_color'],
-                "color2": colormap["taskernet_color"],
-                "font": font_to_use,
-                "element": element,
-                "is_taskernet": True,
-            }
-        )
+        return f'{element}\n'
     else:  # Must be additional item
         return f"<li {element}" + "</span></li>\n"
 
 
 # #############################################################################################
 # Generate the output string based on the input XML <code> passed in
 # Returns a formatted string for output based on the input codes
@@ -212,30 +203,30 @@
     colormap: dict,
     program_args: dict,
     output_list: list,
     list_level: int,
     out_string: str,
 ) -> None:
     """
-    Add line to the list of output lines
+    Add line to the list of output lines.  The output entry is based on the list_level and the contents of the output_str
         :param colormap: colors to use in the output
         :param program_args: runtime arguments
         :param output_list: list of all output lines thus far
         :param list_level: level we are outputting
         :param out_string: the string to add to the output
         :return: none
     """
     if (
         "Task ID:" in out_string and program_args["debug"] is False
     ):  # Drop ID: nnn since we don't need it anymore
         temp_element = out_string.split("Task ID:")
         out_string = temp_element[0]
+
+    # Go configure the output based on the contents of the element and the list level
     output_list.append(
         ulify(out_string, list_level, colormap, program_args["font_to_use"])
     )
     # Log the generated output if in special debug mode
     if debug_out:
-        debug_msg = "out_string:", ulify(
-            out_string, list_level, colormap, program_args["font_to_use"]
-        )
+        debug_msg = f"out_string: {output_list[-1]}"
         logger.debug(debug_msg)
     return
```

### Comparing `maptasker-1.3.3/maptasker/src/parsearg.py` & `maptasker-1.3.4/maptasker/src/parsearg.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/prefers.py` & `maptasker-1.3.4/maptasker/src/prefers.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/priority.py` & `maptasker-1.3.4/maptasker/src/priority.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 
     priority_element = element.find("pri")
     if priority_element is None:
         return ""
     elif event:
         return f' Priority:{priority_element.text}'
     else:
-        return f'<br>&nbsp;&nbsp;&nbsp;[Priority: {priority_element.text}]'
+        return f'&nbsp;&nbsp;&nbsp;[Priority: {priority_element.text}]'
```

### Comparing `maptasker-1.3.3/maptasker/src/proclist.py` & `maptasker-1.3.4/maptasker/src/proclist.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/profiles.py` & `maptasker-1.3.4/maptasker/src/profiles.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/progargs.py` & `maptasker-1.3.4/maptasker/src/progargs.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/proginit.py` & `maptasker-1.3.4/maptasker/src/proginit.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import atexit
 import datetime
 import sys
 from json import dumps, loads  # For write and read counter
 from pathlib import Path
 
 # importing tkinter and tkinter.ttk and all their functions and classes
-from tkinter import *
+from tkinter import Tk
 from tkinter import messagebox
 
 # importing askopenfile (from class filedialog) and messagebox functions
 # from class filedialog
 from tkinter.filedialog import askopenfile
 from typing import Any
 
@@ -32,46 +32,44 @@
 import maptasker.src.progargs as get_args
 from maptasker.src.frmthtml import format_html
 from maptasker.src.colrmode import set_color_mode
 from maptasker.src.config import DARK_MODE
 from maptasker.src.config import GUI
 from maptasker.src.debug import debug1
 from maptasker.src.sysconst import COUNTER_FILE
-from maptasker.src.sysconst import FONT_TO_USE
 from maptasker.src.sysconst import MY_VERSION
 from maptasker.src.sysconst import logger
 from maptasker.src.sysconst import logging
 from maptasker.src.taskerd import get_the_xml_data
+from maptasker.src.error import error_handler
 
 
 # #############################################################################################
 # Use a counter to determine if this is the first time run.
 #  If first time only, then provide a user prompt to locate the backup file
 # #############################################################################################
 def read_counter():
     """Read the program counter
-
-    Parameters: none
-
-    Returns: the count of the number of times the program has been called
+    Get the count of the number of times MapTasker has been called
+        Parameters: none
+        Returns: the count of the number of times the program has been called
 
     """
     return (
         loads(open(COUNTER_FILE, "r").read()) + 1
         if Path.exists(Path(COUNTER_FILE).resolve())
         else 0
     )
 
 
 def write_counter():
     """Write the program counter
-
-    Parameters: none
-
-    Returns: none
+    Write out the number of times MapTasker has been called
+        Parameters: none
+        Returns: none
 
     """
     with open(COUNTER_FILE, "w") as f:
         f.write(dumps(run_counter))
     return
 
 
@@ -80,14 +78,19 @@
 
 
 # #######################################################################################
 # Open and read the Tasker backup XML file
 # Return the file name for use for
 # #######################################################################################
 def open_and_get_backup_xml_file(program_args: dict) -> object:
+    """
+    Open the Tasker backup file and return the file object
+        :param program_args: runtime arguments
+        :return: Tasker backup file object
+    """
     logger.info("entry")
     file_error = False
     # Initialize tkinter
     tkroot = Tk()
     tkroot.geometry("200x100")
     tkroot.title("Select Tasker backup xml file")
     filename = None
@@ -95,21 +98,26 @@
     # dir_path = path.dirname(path.realpath(__file__))  # Get current directory
     dir_path = Path.cwd()
     logger.info(f"dir_path: {dir_path}")
     if program_args["debug"]:
         try:
             filename = open(f"{dir_path}/backup.xml", "r")
         except OSError:
-            error_msg = (
-                f"Error: The backup.xml file was not found in {dir_path}.  Program"
-                " terminated!"
+            error_handler(
+                (
+                    f"Error: The backup.xml file was not found in {dir_path}.  Program"
+                    " terminated!"
+                ),
+                3,
             )
-            logger.debug(error_msg)
-            print(error_msg)
-            exit(3)
+
+    elif program_args["file"]:
+        # We already have the file name...open it.
+        filename = open(program_args["file"], "r")
+
     else:
         try:
             filename = askopenfile(
                 parent=tkroot,
                 mode="r",
                 title="Select Tasker backup xml file",
                 initialdir=dir_path,
@@ -120,14 +128,16 @@
         if filename is None:
             file_error = True
         if file_error:
             cancel_message = "Backup file selection cancelled.  Program ended."
             print(cancel_message)
             logger.debug(cancel_message)
             sys.exit(6)
+    tkroot.destroy()
+    del tkroot
 
     return filename
 
 
 # #############################################################################################
 # Build color dictionary
 # #############################################################################################
@@ -139,59 +149,69 @@
     colormap = {}
 
     appearance = 'Dark' if DARK_MODE else "Light"
     return set_color_mode(appearance, colormap)
 
 
 # #############################################################################################
-# Setup logging if in debug mode
+# Setup logging
 # #############################################################################################
-def setup_logging():
+def setup_logging() -> None:
+    """
+    Set up the logging: name the file and establish the log type and format
+    """
     logging.basicConfig(
         filename="maptasker.log",
         filemode="w",
         format="%(asctime)s,%(msecs)d %(levelname)s %(name)s %(funcName)s %(message)s",
         datefmt="%H:%M:%S",
         level=logging.DEBUG,
     )
     logger.info(sys.version_info)
 
 
 ##############################################################################################
 # Log the arguments
 # ############################################################################################
 def log_startup_values(program_args: dict, colormap: dict) -> None:
+    """
+    Log the runtime arguments
+        :param program_args: runtrime arguments
+        :param colormap: colors to use in the output
+    """
     setup_logging()  # Get logging going
     logger.info(f"{MY_VERSION} {str(datetime.datetime.now())}")
     logger.info(f"sys.argv:{str(sys.argv)}")
     for key, value in program_args.items():
         logger.info(f"{key}: {value}")
     for key, value in colormap.items():
         logger.info(f"colormap for {key} set to {value}")
 
 
 ##############################################################################################
 # Program setup: initialize key elements
 # ############################################################################################
 def setup(
-    colormap: dict, program_args: dict, output_list: list
+    colormap: dict, program_args: dict, output_list: list, file_to_get: str
 ) -> tuple[Any, Any, object, Any, list, str]:
     """
     Perform basic setup
         :param colormap: colors to use for output
         :param program_args: runtime arguments
         :param output_list: lines of output generated thus far
+        :param file_to_get: file object (if file already defined, don't prompt user), or None
         :return xml tree, xml root, all Tasker Projects/Profiles/Tasks/Scenes, output lines, the heading
     """
 
-    # Prompt user for Tasker's backup.xml file location
-    if run_counter < 1 and not GUI:  # Only display message box on first run
+    program_args["file"] = file_to_get
+
+    # Only display message box if we don't yet have the file name
+    if not file_to_get and run_counter < 1 and not GUI:
         msg = "Locate the Tasker backup xml file to use to map your Tasker environment"
-        title = "MapTasker"
-        messagebox.showinfo(title, msg)
+        messagebox.showinfo("MapTasker", msg)
 
     # Open and read the file...
     filename = open_and_get_backup_xml_file(program_args)
 
     # Go get all the xml data
     tree, root, all_tasker_items = get_the_xml_data(filename)
 
@@ -200,17 +220,16 @@
         error_msg = "You did not select a Tasker backup XML file...exit 2"
         build_output.my_output(colormap, program_args, output_list, 0, error_msg)
         logger.debug(f"{error_msg}exit 3")
         sys.exit(3)
     else:
         # Format the output heading
         heading = (
-            '<html>\n<head>\n<title>MapTasker</title>\n<body style="background-color:'
-            + colormap["background_color"]
-            + '">\n'
+            "<html>\n<head>\n<title>MapTasker</title>\n<body"
+            f" style=\"background-color:{colormap['background_color']}\">\n"
             + format_html(
                 colormap,
                 "LawnGreen",
                 "",
                 (
                     "<b>Tasker Mapping................&nbsp;&nbsp;&nbsp;Tasker version:"
                     f" {root.attrib['tv']}&nbsp;&nbsp;&nbsp;&nbsp;Map-Tasker version:"
@@ -222,42 +241,44 @@
         # Start the output with heading
         build_output.my_output(colormap, program_args, output_list, 0, heading)
 
     # If we are debugging, output the runtime arguments and colors
     if program_args["debug"]:
         debug1(colormap, program_args, output_list)
 
-    # Start Project list
+    # Start a list (<ul>)
     build_output.my_output(colormap, program_args, output_list, 1, "")
 
     return tree, root, filename, all_tasker_items, output_list, heading
 
 
 ##############################################################################################
 # Perform maptasker program initialization functions
 # #############################################################################################
-def start_up(output_list: list) -> tuple:
+def start_up(output_list: list, file_to_get: str) -> tuple:
     """
-    Initialize program variables
-        :type output_list: tuple[
+    Perform maptasker program initialization functions
+        :param output_list: list of output lines to add to.
+        :param file_to_get: file name (fully qualified) if previously defined
+        :return: see "return" statement
     """
     colormap = setup_colors()  # Get our map of colors
 
     # Get any arguments passed to program
     logger.info(f"sys.argv{str(sys.argv)}")
 
     # Rename/convert any old argument file to new name/format for clarity (one time only operation)
     old_to_new.migrate()
 
     # Get runtime arguments
     program_args, colormap = get_args.get_program_arguments(colormap)
 
     # Setup program key elements
     tree, root, filename, all_tasker_items, output_list, heading = setup(
-        colormap, program_args, output_list
+        colormap, program_args, output_list, file_to_get
     )
 
     # If debug mode, log the arguments
     if program_args["debug"]:
         log_startup_values(program_args, colormap)
 
     # Force full detail if we are doing a single Task
```

### Comparing `maptasker-1.3.3/maptasker/src/projects.py` & `maptasker-1.3.4/maptasker/src/projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,18 @@
         :param launcher_task_info: details about (any) launcher Task
         :return: True if we are looking for a single Project and this isn't it.  False otherwise.
     """
     # See if there is a Kid app and get the Project's priority
     kid_app_info = priority = ''
     if program_args["display_detail_level"] == 3:
         kid_app_info = get_kid_app(project)
+        if kid_app_info:
+            kid_app_info = format_html(
+                colormap, "project_color", "", kid_app_info, True
+            )
         priority = get_priority(project, False)
 
     # Get the name in a format with proper HTML code wrapped around it
     project_name_details = format_html(
         colormap, "project_color", "", f"Project: {project_name}", True
     )
 
@@ -303,15 +307,15 @@
             found_items,
             heading,
             output_list,
             launcher_task_info,
         ):
             continue
 
-        # Process any <Share> information from TaskerNet
+        # Process any <Share> information from TaskerNet and output it
         if program_args["display_taskernet"]:
             share(project, colormap, program_args, output_list)
 
         if profile_ids := get_ids(
             True,
             program_args,
             colormap,
@@ -346,15 +350,15 @@
                 output_list,
                 2,
                 format_html(
                     colormap,
                     "profile_color",
                     "",
                     "<em>Project has no Profiles</em>",
-                    False,
+                    True,
                 ),
             )
         my_output(colormap, program_args, output_list, 3, "")  # Close Profile list
 
         # # See if there are Tasks in Project that have no Profile
         if task_ids := get_ids(False, {}, {}, [], project, project_name, []):
             # Process Tasks in Project that are not referenced by a Profile
```

### Comparing `maptasker-1.3.3/maptasker/src/runcli.py` & `maptasker-1.3.4/maptasker/src/runcli.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from maptasker.src.rungui import process_gui
 from maptasker.src.initparg import initialize_runtime_arguments
 
 from maptasker.src.sysconst import MY_LICENSE
 from maptasker.src.sysconst import MY_VERSION
 from maptasker.src.sysconst import TYPES_OF_COLORS
 from maptasker.src.sysconst import logger
+from maptasker.src.error import error_handler
 
 
 # #######################################################################################
 # Get arguments from command line and put them to the proper settings
 # #######################################################################################
 def process_arguments(args: object, prog_args: dict, colormap: dict) -> tuple:
     # Color help?
@@ -102,17 +103,15 @@
                 case "single_profile_name":
                     prog_args["single_profile_name"] = value
                 case "single_project_name":
                     prog_args["single_project_name"] = value
                 case "single_task_name":
                     prog_args["single_task_name"] = value
                 case _:
-                    error_msg = "Error: Invalid argument restored!"
-                    print(error_msg)
-                    logger.debug((error_msg))
+                    error_handler("Invalid argument restored!", 0)
 
     # Map the colormap keys and values restored
     for key, value in temp_colormap.items():
         if key is not None:
             colormap[key] = value
 
     return prog_args, colormap
```

### Comparing `maptasker-1.3.3/maptasker/src/rungui.py` & `maptasker-1.3.4/maptasker/src/rungui.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,23 +13,18 @@
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 
-from maptasker.src.config import GUI
 from maptasker.src.initparg import initialize_runtime_arguments
 from maptasker.src.colrmode import set_color_mode
-from maptasker.src.sysconst import FONT_TO_USE
 from maptasker.src.sysconst import logger
 
-if GUI:
-    from maptasker.src.userintr import MyGui
-
 
 # #######################################################################################
 # Output the provided message and return (then quit)
 # #######################################################################################
 def output_and_quit(arg0):
     out_message = arg0
     print(out_message)
@@ -48,27 +43,27 @@
     user_input = MyGui()
     user_input.mainloop()
 
     if user_input.exit:
         output_and_quit("Program exited. Goodbye.")
         exit()
 
-    # User has either closed the window or hit the 'Run' button
-    if not user_input.go_program:  # Window closed?
+    # User has either closed the window or hit the 'Run' or 'ReRun' button
+    if not user_input.go_program and not user_input.rerun_program:
         output_and_quit("Program cancelled be user (killed GUI)")
         exit(99)
 
     # Convert runtime argument default values to a dictionary
     prog_args = initialize_runtime_arguments()
 
     # 'Run' button hit.  Get all the input from GUI variables
     try:
         prog_args["display_detail_level"] = int(user_input.display_detail_level)
     except TypeError:
-        display_detail_level = 1
+        prog_args["display_detail_level"] = 1
     # Ok, load up the arguments from the GUI
     prog_args["display_profile_conditions"] = user_input.display_profile_conditions
     prog_args["display_preferences"] = user_input.display_preferences
     prog_args["display_taskernet"] = user_input.display_taskernet
     prog_args["single_project_name"] = user_input.single_project_name
     prog_args["single_profile_name"] = user_input.single_profile_name
     prog_args["single_task_name"] = user_input.single_task_name
@@ -77,14 +72,16 @@
     # Process the colors
     if user_input.color_lookup:
         for key, value in user_input.color_lookup.items():
             colormap[key] = value
 
     # Debug flag
     prog_args["debug"] = user_input.debug
+    # Save ReRun button setting
+    prog_args["rerun"] = user_input.rerun_program
 
     # Delete the GUI
     MyGui.quit(user_input)
     del user_input
     del MyGui
 
     return (
```

### Comparing `maptasker-1.3.3/maptasker/src/scenes.py` & `maptasker-1.3.4/maptasker/src/scenes.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/servicec.py` & `maptasker-1.3.4/maptasker/src/servicec.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/share.py` & `maptasker-1.3.4/maptasker/src/share.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,22 +12,30 @@
 #                                                                                            #
 # ########################################################################################## #
 import defusedxml.ElementTree  # Need for type hints
 
 
 from maptasker.src.outputl import my_output
 from maptasker.src.sysconst import FONT_TO_USE
+from maptasker.src.frmthtml import format_html
 
 
 def share(
     root_element: defusedxml.ElementTree.XML,
     colormap: dict,
     program_args: dict,
     output_list: list,
 ) -> None:
+    """
+    Go through xml <Share> elements to grab and output TaskerNet description and search-on lines
+        :param root_element: beginning xml element (e.g. Project or Task)
+        :param colormap: colors to use in output
+        :param program_args: runtime arguments
+        :param output_list: where all output lines are added to
+    """
     # Get the <share> element, if any
     share_element: defusedxml.ElementTree = root_element.find("Share")
     if share_element is not None:
         #  We have a <Share> .  Find the description
         description_element = share_element.find("d")
         # Process the description
         if description_element is not None:
@@ -47,44 +55,59 @@
 def description_element_output(
     description_element: defusedxml.ElementTree,
     colormap: dict,
     program_args: dict,
     output_list: list,
 ) -> None:
     """
-    We have a Taskernet description (<Share>).  Process it
+    We have a Taskernet description (<Share>).  Clean it uip and add it to the output list
         :param description_element: the xml element with the description
         :param colormap: the colors to use for the output
         :param program_args: the runtime arguments
         :param output_list: the output lines thus far
     """
     # We need to properly format this since it has embedded stuff that screws it up
-    out_string = f"TaskerNet description: {description_element.text}"
+    out_string = format_html(
+        colormap,
+        "taskernet_color",
+        "",
+        f"TaskerNet description: {description_element.text}",
+        True,
+    )
     indent_html = (
         '</p><p'
-        f' style="margin-left:20px;margin-right:50px;color:{colormap["taskernet_color"]}{FONT_TO_USE}>'
+        f' style="margin-left:20px;margin-right:50px;color:{colormap["taskernet_color"]}{FONT_TO_USE}">'
     )
 
     # Indent the description and override various embedded HTML attributes
     out_string = out_string.replace("<p>", indent_html)
+    out_string = out_string.replace("<P>", indent_html)
+    out_string = out_string.replace("</p>", "")
+    out_string = out_string.replace("</P>", "")
     out_string = out_string.replace("<br/>", indent_html)
     out_string = out_string.replace("<h1>", indent_html)
     out_string = out_string.replace("\r", indent_html)
     out_string = out_string.replace("<li>", f'{indent_html}')
     out_string = out_string.replace("</li>", "")
     # out_string = remove_html_tags(out_string, indent_html)
 
     # Look for double blanks = line break
     new_line = ""
     if indent_html not in out_string:  # Only if we have not already formatted
         for position, character_index in enumerate(out_string):
             new_line = (
                 f'{new_line}<p style="margin-left:20px;'
-                f'margin-right:50px;color:{colormap["taskernet_color"]}{FONT_TO_USE}>'
+                f'margin-right:50px;color:{colormap["taskernet_color"]}{FONT_TO_USE}">'
                 if (character_index == " " and out_string[position + 1] == " ")
                 or (character_index == "-" and out_string[position + 1] == " ")
                 else new_line + character_index
             )
-        out_string = new_line
-    out_string = f'{out_string}'
+
+        # Make certain we have proper html in front of string
+        # if indent_html not in out_string:
+        if "<span " not in out_string:
+            out_string = format_html(colormap, "taskernet_color", "", new_line, True)
+        else:
+            out_string = new_line
+
     # Output the description line
     my_output(colormap, program_args, output_list, 2, out_string)
```

### Comparing `maptasker-1.3.3/maptasker/src/shellsort.py` & `maptasker-1.3.4/maptasker/src/shellsort.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/maptasker/src/sysconst.py` & `maptasker-1.3.4/maptasker/src/sysconst.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #                                                                                            #
 # ########################################################################################## #
 from maptasker.src.config import OUTPUT_FONT
 import logging
 
 # Global constants
 UNKNOWN_TASK_NAME = "Unnamed/Anonymous."
-MY_VERSION = "MapTasker version 1.3.3"
+MY_VERSION = "MapTasker version 1.3.4"
 MY_LICENSE = "GNU GENERAL PUBLIC LICENSE (Version 3, 29 June 2007)"
 NO_PROJECT = "-none found."
 COUNTER_FILE = ".MapTasker_RunCount.txt"
 ARGUMENTS_FILE = ".MapTasker_arguments.json"
 FONT_TO_USE = f';font-family:{OUTPUT_FONT}'
 NO_PROFILE = "None or unnamed!"
```

### Comparing `maptasker-1.3.3/maptasker/src/taskactn.py` & `maptasker-1.3.4/maptasker/src/taskactn.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 import defusedxml.ElementTree  # Need for type hints
 
 import maptasker.src.tasks as tasks
 from maptasker.src.outputl import my_output
-from maptasker.src.sysconst import logger
 from maptasker.src.sysconst import UNKNOWN_TASK_NAME
 from maptasker.src.frmthtml import format_html
+from maptasker.src.error import error_handler
 
 
 # #######################################################################################
 # For this specific Task, get its Actions and output the Task and Actions
 # #######################################################################################
 def get_task_actions_and_output(
     the_task: defusedxml.ElementTree.XML,
@@ -34,20 +34,22 @@
     all_tasks: dict,
 ) -> None:
     # If Unknown task or displaying more detail, then 'the_task' is not valid, and we have to find it.
     if UNKNOWN_TASK_NAME in the_item or program_args["display_detail_level"] > 0:
         # Get the Task ID so that we can get the Task xml element
         # "--Task:" denotes a Task in a Scene
         temp_id = 'x' if "&#45;&#45;Task:" in list_type else the_item.split("Task ID: ")
+        kaka = ""
         # Get the Task xml element
         if len(temp_id) > 1:
             temp_id[1] = temp_id[1].split(' ', 1)[0]  # ID = 1st word of temp_id[1]
             the_task, kaka = tasks.get_task_name(
                 temp_id[1], tasks_found, [temp_id[1]], "", all_tasks
             )
+
         # Get Task actions
         if the_task:
             if alist := tasks.get_actions(the_task, colormap, program_args):
                 my_output(
                     colormap, program_args, output_list, 1, ""
                 )  # Start Action list
                 action_count = 1
@@ -55,17 +57,16 @@
                     colormap, program_args, output_list, action_count, alist, the_item
                 )
                 # End list if Scene Task
                 if "&#45;&#45;Task:" in list_type:
                     my_output(colormap, program_args, output_list, 3, "")
                     my_output(colormap, program_args, output_list, 3, "")
         else:
-            error_msg = 'Error: No Task found!!!'
-            logger.debug(error_msg)
-            print(error_msg)
+            error_handler('No Task found!!!', 0)
+
     return
 
 
 # #######################################################################################
 # Go through list of actions and output them
 # #######################################################################################
 def output_list_of_actions(
@@ -87,16 +88,14 @@
         :param the_item: the specific Task's detailed line
 
     Returns: the count of the number of times the program has been called
 
     """
     for taction in alist:
         if taction is not None:
-            # if "Label for" in taction:
-            #     my_output(colormap, program_args, output_list, 2, taction)
             if taction[:3] == "...":
                 my_output(
                     colormap,
                     program_args,
                     output_list,
                     2,
                     format_html(
@@ -126,9 +125,10 @@
             ):  # Just show first Task if unknown Task
                 break
             elif (
                 program_args["display_detail_level"] == 1
                 and UNKNOWN_TASK_NAME not in the_item
             ):
                 break
+
     my_output(colormap, program_args, output_list, 3, "")  # Close Action list
     return
```

### Comparing `maptasker-1.3.3/maptasker/src/taskerd.py` & `maptasker-1.3.4/maptasker/src/taskerd.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 from maptasker.src.sysconst import logger
+from maptasker.src.error import error_handler
 
 
 # ###############################################################################################
 # Convert list of xml to dictionary
 # ###############################################################################################
 def move_xml_to_table(all_xml, is_scene: bool):
     new_table = {}
@@ -34,18 +35,15 @@
 # ###############################################################################################
 def get_the_xml_data(filename):
     logger.info("entry")
     # Import xml
     try:
         tree = parse(filename)
     except defusedxml.ElementTree.ParseError:
-        error_msg = f"Error parsing {filename}"
-        print(error_msg)
-        logger.debug(error_msg)
-        exit(1)
+        error_handler(f"Error parsing {filename}", 1)  # Error out and exit
 
     root = tree.getroot()
 
     all_services = root.findall("Setting")
     all_projects = root.findall("Project")
     all_profiles_list = root.findall("Profile")
     all_scenes_list = root.findall("Scene")
```

### Comparing `maptasker-1.3.3/maptasker/src/tasks.py` & `maptasker-1.3.4/maptasker/src/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from maptasker.src.xmldata import tag_in_type
 from maptasker.src.kidapp import get_kid_app
 from maptasker.src.priority import get_priority
 from maptasker.src.getids import get_ids
 from maptasker.src.sysconst import UNKNOWN_TASK_NAME
 from maptasker.src.sysconst import NO_PROJECT
 from maptasker.src.sysconst import logger
+from maptasker.src.error import error_handler
+from maptasker.src.frmthtml import format_html
 
 from maptasker.src.shellsort import shell_sort
 
 
 # #######################################################################################
 # Navigate through Task's Actions and identify each
 # Return a list of Task's actions for the given Task
@@ -38,22 +40,23 @@
         :param current_task: xml element of the Task we are getting actions for
         :param colormap: colors to use in output
         :param prog_args: runtime arguments
         :return: list of Task 'action' output lines
     """
     tasklist = []
 
+    # Get the Task's Actions (<Action> elements)
     try:
         task_actions = current_task.findall("Action")
     except defusedxml.DefusedXmlException:
         print("tasks.py current Task:", current_task)
-        error_msg = "Error: No action found!!!"
-        print(error_msg)
-        logger.debug(error_msg)
+        error_handler("Error: No action found!!!", 0)
         return []
+
+    # Process the Actions
     if task_actions:
         indentation_amount = ""
         indentation = 0
         # Task's Action statements can be out-of-order, and we need them in proper-order/sequence
         # sort the Task's Actions by attrib sr (e.g. sr='act0', act1, act2, etc.) to get them in true order
         if len(task_actions) > 0:
             shell_sort(task_actions, True, False)
@@ -70,28 +73,30 @@
                 + " Code:"
                 + child.text
                 + " task_code:"
                 + task_code
                 + "Action attr:"
                 + str(action.attrib)
             )
+
             # Calculate the amount of indention required
             if (
                 ">End If" in task_code
                 or ">Else" in task_code
                 or ">End For" in task_code
             ):  # Do we un-indent?
                 indentation -= 1
                 length_indent = len(indentation_amount)
                 indentation_amount = indentation_amount[24:length_indent]
-            action_evaluate.build_action(
+            tasklist = action_evaluate.build_action(
                 colormap, tasklist, task_code, child, indentation, indentation_amount
             )
+            #  Indent the line if this is a condition
             if (
-                ">If" in task_code or ">Else" in task_code or ">For" in task_code
+                ">If" in task_code or ">Else" in task_code or ">For<" in task_code
             ):  # Do we indent?
                 indentation += 1
                 indentation_amount = f"{indentation_amount}&nbsp;&nbsp;&nbsp;&nbsp;"
 
     return tasklist
 
 
@@ -115,26 +120,27 @@
         :param all_tasks: all Tasks in xml
         :return: Task's xml element, Task's name
     """
     if the_task_id.isdigit():
         task = all_tasks[the_task_id]
         tasks_that_have_been_found.append(the_task_id)
         extra = f"&nbsp;&nbsp;Task ID: {the_task_id}"
+        # Determine if this is an "Entry" or "Exit" Task
         try:
             task_name = task.find("nme").text
             if task_type == "Exit":
                 task_output_lines.append(
                     f"{task_name}&nbsp;&nbsp;&nbsp;&nbsp;<<< Exit Task{extra}"
                 )
 
             else:
                 task_output_lines.append(
                     f"{task_name}&nbsp;&nbsp;&nbsp;&nbsp;<<< Entry Task{extra}"
                 )
-        except Exception as e:
+        except AttributeError:
             task_name = UNKNOWN_TASK_NAME
             if task_type == "Exit":
                 task_output_lines.append(
                     f"{UNKNOWN_TASK_NAME}&nbsp;&nbsp;&nbsp;&nbsp;<<< Exit Task{extra}"
                 )
 
             else:
@@ -293,17 +299,14 @@
                     task_list,
                     our_task_element,
                     list_of_found_tasks,
                     program_args,
                     colormap,
                     all_tasker_items,
                 )
-                # build_output.my_output(
-                #     colormap, program_args, output_list, 3, ""
-                # )  # End Task list
                 break
 
 
 # #######################################################################################
 # output_task: we have a Task and need to generate the output
 # #######################################################################################
 def output_task(
@@ -340,14 +343,15 @@
     """
     # Do NOT move this import.  Otherwise, will get recursion error
     from maptasker.src.proclist import process_list
 
     # See if there is a Kid app and/or Priority
     if do_extra and program_args["display_detail_level"] == 3:
         if kid_app_info := get_kid_app(our_task_element):
+            kid_app_info = format_html(colormap, "task_color", "", kid_app_info, True)
             task_list[0] = f'{task_list[0]} {kid_app_info}'
         if priority := get_priority(our_task_element, False):
             task_list[0] = f'{task_list[0]} {priority}'
 
     # Looking for a single Task?
     if our_task_name != "" and program_args["single_task_name"]:
         do_single_task(
```

### Comparing `maptasker-1.3.3/maptasker/src/taskuniq.py` & `maptasker-1.3.4/maptasker/src/taskuniq.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 #                                                                                            #
 # ########################################################################################## #
 from typing import List, Union
 
 import maptasker.src.outputl as build_output
 import maptasker.src.tasks as tasks
 from maptasker.src.frmthtml import format_html
-from maptasker.src.sysconst import FONT_TO_USE
-from maptasker.src.sysconst import UNKNOWN_TASK_NAME
 from maptasker.src.sysconst import NO_PROJECT
+from maptasker.src.sysconst import UNKNOWN_TASK_NAME
 
 
 # ###############################################################################################
 # Output Projects Without Tasks and Projects Without Profiles
 # ###############################################################################################
 def process_missing_tasks_and_profiles(
     output_list: List[str],
```

### Comparing `maptasker-1.3.3/maptasker/src/userintr.py` & `maptasker-1.3.4/maptasker/src/userintr.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,22 +39,23 @@
     ' details on every Task with action details\n\n* Display Conditions: Turn on the'
     ' display of Profile and Task conditions.\n\n* Display TaskerNet Info - If'
     ' available, display TaskerNet publishing information\n\n* Display Tasker'
     ' Preferences - display Tasker\'s system Preferences\n\n* Save Settings - Save'
     ' these settings for later use.\n\n* Restore Settings - Restore the settings from a'
     ' previously saved session.\n\n* Appearance Mode: Dark, Light, or System'
     ' default.\n\n* Reset Options: Clear everything and start anew.\n\n* Run: Run the'
-    ' program with the settings provided.\n\n* Specific Name tab: enter a single,'
-    ' specific named item to display...\n   - Project Name: enter a specific Project to'
-    ' display\n   - Profile Name: enter a specific Profile to display\n   - Task Name:'
-    ' enter a specific Task to display\n   (These three are exclusive: enter one'
-    ' only)\n\n* Colors tab: select colors for various elements of the display\n       '
-    '       (e.g. color for Projects, Profiles, Tasks, etc.)\n\n* Exit: Exit the'
-    ' program (quit).\n\nNote: You will be prompted to identify your Tasker backup file'
-    ' once\n      you hit the \'Run\' button'
+    ' program with the settings provided.\n* ReRun: Run multiple times (with different'
+    ' settings).\n\n* Specific Name tab: enter a single, specific named item to'
+    ' display...\n   - Project Name: enter a specific Project to display\n   - Profile'
+    ' Name: enter a specific Profile to display\n   - Task Name: enter a specific Task'
+    ' to display\n   (These three are exclusive: enter one only)\n\n* Colors tab:'
+    ' select colors for various elements of the display\n              (e.g. color for'
+    ' Projects, Profiles, Tasks, etc.)\n\n* Exit: Exit the program (quit).\n\nNote: You'
+    ' will be prompted to identify your Tasker backup file once\n      you hit the'
+    ' \'Run\' button'
 )
 
 
 # #######################################################################################
 # Class to define the GUI configuration
 # #######################################################################################
 class MyGui(customtkinter.CTk):
@@ -64,15 +65,15 @@
         # configure window
         self.title("MapTasker Runtime Options")
         self.geometry("1100x600")
 
         # configure grid layout (4x4)
         self.grid_columnconfigure(1, weight=1)
         self.grid_columnconfigure((2, 3), weight=0)
-        self.grid_rowconfigure((0), weight=1)
+        self.grid_rowconfigure(0, weight=1)
 
         # create sidebar frame with widgets
         self.sidebar_frame = customtkinter.CTkFrame(self, width=140, corner_radius=0)
         self.sidebar_frame.grid(row=0, column=0, rowspan=6, sticky="nsew")
         # Define sidebar background frame
         self.sidebar_frame.grid_rowconfigure(9, weight=1)
         self.logo_label = customtkinter.CTkLabel(
@@ -178,15 +179,28 @@
             fg_color="#246FB6",
             border_width=2,
             text="Run",
             command=self.run_program,
             text_color=("#0BF075", "#1AD63D"),
         )
         self.run_button.grid(
-            row=7, column=0, padx=(20, 20), pady=(20, 20), sticky="nsew"
+            row=6, column=1, padx=(200, 200), pady=(20, 20), sticky="nsew"
+        )
+
+        # 'ReRun' button definition
+        self.rerun_button = customtkinter.CTkButton(
+            master=self,
+            fg_color="#246FB6",
+            border_width=2,
+            text="ReRun",
+            command=self.rerun_program,
+            text_color=("#0BF075", "#1AD63D"),
+        )
+        self.rerun_button.grid(
+            row=7, column=1, padx=(200, 200), pady=(20, 20), sticky="nsew"
         )
 
         # 'Exit' button definition
         self.exit_button = customtkinter.CTkButton(
             master=self,
             fg_color="#246FB6",
             border_width=2,
@@ -295,27 +309,35 @@
         self.textbox.configure(border_color="#6563ff")
         self.debug_checkbox.pack(padx=20, pady=10)
 
         # set default values
         self.set_defaults(True)
 
     # #######################################################################################
-    # Set the value defaults
+    # Close the window
     # #######################################################################################
+    def closing(self):
+        self.destroy()
+        print("destroyed")
+        if self.closing_event is not None:
+            self.closing_event()
+
     def set_defaults(self, first_time: bool):
         self.sidebar_detail_option.configure(values=["0", "1", "2", "3"])
         self.sidebar_detail_option.set("1")
         self.display_detail_level = 1
         self.display_profile_conditions = (
             self.display_preferences
         ) = (
             self.display_taskernet
         ) = (
             self.debug
-        ) = self.clear_settings = self.reset = self.exit = self.go_program = False
+        ) = (
+            self.clear_settings
+        ) = self.reset = self.exit = self.go_program = self.rerun_program = False
         self.single_project_name = self.single_profile_name = self.single_task_name = ""
         self.color_text_row = 2
         self.appearance_mode_optionemenu.set("System")
         self.color_labels = []
         self.appearance_mode = "System"
         if first_time:
             self.textbox.insert("0.0", "MapTasker Help\n\n" + INFO_TEXT)
@@ -492,15 +514,15 @@
                 f"{color_selected_item} color changed to {color}", False
             )
 
             # Okay, plug in the selected color for the selected named item
             self.extract_color_from_event(color, color_selected_item)
 
     def extract_color_from_event(self, color, color_selected_item):
-        row = self.color_text_row
+        # row = self.color_text_row
         self.color_lookup[TYPES_OF_COLOR_NAMES[color_selected_item]] = (
             color  # Add color for the selected item to our dictionary
         )
         self.color_labels.append(
             customtkinter.CTkLabel(
                 self.tabview.tab("Colors"),
                 text=f"{color_selected_item} << color",
@@ -598,42 +620,43 @@
         self.set_defaults(False)  # Reset all values
         temp_args = {}
         # Restore all changes that have been saved
         temp_args, self.color_lookup = save_restore_args(
             False, self.color_lookup, temp_args
         )
         # Check for errors
-        try:
+        with contextlib.suppress(KeyError):
             if temp_args["msg"]:
                 self.display_message_box(temp_args["msg"], False)
                 return
-        except KeyError:  # Ignore if key not found.
-            pass
-
         # Restore progargs values
         if temp_args or self.color_lookup:
-            all_messages, new_message = '', ''
-            for key, value in temp_args.items():
-                if key is not None:
-                    setattr(self, key, value)
-                    if new_message := self.restore_display(key, value):
-                        all_messages = all_messages + new_message
-            # Display the restored color changes
-            inv_color_names = {v: k for k, v in TYPES_OF_COLOR_NAMES.items()}
-            for key, value in self.color_lookup.items():
-                if key is not None:
-                    all_messages = (
-                        f"{all_messages} {inv_color_names[key]} color set to {value}\n"
-                    )
-            # Display the queue of messages
-            self.display_message_box(f"{all_messages}\nSettings restored.", True)
-
+            self.extract_settings(temp_args)
         else:  # Empty?
             self.display_message_box("No settings file found.", False)
 
+    def extract_settings(self, temp_args: dict) -> None:
+        all_messages, new_message = '', ''
+        for key, value in temp_args.items():
+            if key is not None:
+                setattr(self, key, value)
+                if new_message := self.restore_display(key, value):
+                    all_messages = all_messages + new_message
+        # Display the restored color changes
+        inv_color_names = {v: k for k, v in TYPES_OF_COLOR_NAMES.items()}
+        for key, value in self.color_lookup.items():
+            if key is not None:
+                all_messages = (
+                    f"{all_messages} {inv_color_names[key]} color set to {value}\n"
+                )
+        # Display the queue of messages
+        self.display_message_box(f"{all_messages}\nSettings restored.", True)
+        if self.debug:
+            self.debug_checkbox_event()
+
     # #######################################################################################
     # Process the 'Reset Settings' button
     # #######################################################################################
     def reset_settings_event(self):
         self.sidebar_detail_option.set("1")  # display detail level
         self.condition_button.deselect()  # Conditions
         self.display_preferences_button.deselect()  # Tasker Preferences
@@ -671,12 +694,21 @@
     # The 'Run' program button has been pressed.  Set the run flag and close the GUI
     # #######################################################################################
     def run_program(self):
         self.go_program = True
         self.quit()
 
     # #######################################################################################
+    # The 'ReRun' program button has been pressed.  Set the run flag and close the GUI
+    # #######################################################################################
+    def rerun_program(self):
+        self.rerun_program = True
+        # MyGui.destroy(self)
+        self.withdraw()
+        self.quit()
+
+    # #######################################################################################
     # The 'Exit' program button has been pressed.  Call it quits
     # #######################################################################################
     def exit_program(self):
         self.exit = True
         self.quit()
```

### Comparing `maptasker-1.3.3/maptasker/src/xmldata.py` & `maptasker-1.3.4/maptasker/src/xmldata.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.3/pyproject.toml` & `maptasker-1.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maptasker"
-version = "1.3.3"
+version = "1.3.4"
 description = "Utility to display your entire Android 'Tasker' configuration on your MAC."
 authors = ["Michael Rubin <mikrubin@gmail.com>"]
 readme = "README_PyPl.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/mctinker/Map-Tasker"
 keywords = ["tasker", "Tasker", "map tasker"]
 packages = [
```

### Comparing `maptasker-1.3.3/PKG-INFO` & `maptasker-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maptasker
-Version: 1.3.3
+Version: 1.3.4
 Summary: Utility to display your entire Android 'Tasker' configuration on your MAC.
 Home-page: https://github.com/mctinker/Map-Tasker
 License: GPL-3.0-or-later
 Keywords: tasker,Tasker,map tasker
 Author: Michael Rubin
 Author-email: mikrubin@gmail.com
 Requires-Python: >=3.10,<4.0
```

