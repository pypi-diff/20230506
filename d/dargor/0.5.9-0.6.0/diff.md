# Comparing `tmp/dargor-0.5.9-py3-none-any.whl.zip` & `tmp/dargor-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 19348 bytes, number of entries: 23
--rw-r-----  2.0 unx     3603 b- defN 22-May-26 20:05 dargor/Curses.py
+Zip file size: 19420 bytes, number of entries: 23
+-rw-r-----  2.0 unx     3573 b- defN 23-May-06 09:58 dargor/Curses.py
 -rw-r-----  2.0 unx     1624 b- defN 22-May-26 20:05 dargor/DelayedKeyboardInterrupt.py
 -rw-r-----  2.0 unx     1245 b- defN 22-May-26 20:05 dargor/Tk.py
--rw-r-----  2.0 unx      843 b- defN 22-Nov-08 22:32 dargor/__init__.py
+-rw-r-----  2.0 unx      843 b- defN 23-May-06 10:10 dargor/__init__.py
 -rw-r-----  2.0 unx     1030 b- defN 22-May-26 20:05 dargor/argparser.py
 -rw-r-----  2.0 unx     1500 b- defN 22-May-26 20:05 dargor/bench.py
 -rw-r-----  2.0 unx      987 b- defN 22-May-26 20:05 dargor/coalesce.py
 -rw-r-----  2.0 unx     2062 b- defN 22-May-26 20:05 dargor/colored_tracebacks.py
--rw-r-----  2.0 unx     1218 b- defN 22-May-26 20:05 dargor/console.py
+-rw-r-----  2.0 unx     1250 b- defN 23-May-06 10:00 dargor/console.py
 -rw-r-----  2.0 unx     1367 b- defN 22-Nov-08 22:29 dargor/dataclasses_helpers.py
 -rw-r-----  2.0 unx     1955 b- defN 22-May-26 20:05 dargor/deck.py
--rw-r-----  2.0 unx     1309 b- defN 22-May-26 20:05 dargor/files.py
+-rw-r-----  2.0 unx     1341 b- defN 23-May-06 10:01 dargor/files.py
 -rw-r-----  2.0 unx     3798 b- defN 22-Jun-05 19:09 dargor/finance.py
 -rw-r-----  2.0 unx     2030 b- defN 22-May-26 20:05 dargor/nice.py
--rw-r-----  2.0 unx     3698 b- defN 22-May-26 20:05 dargor/plots.py
+-rw-r-----  2.0 unx     3857 b- defN 23-May-06 10:07 dargor/plots.py
 -rw-r-----  2.0 unx      903 b- defN 22-May-26 20:05 dargor/pretty.py
 -rw-r-----  2.0 unx        0 b- defN 22-Feb-10 21:17 dargor/py.typed
 -rw-r-----  2.0 unx     1201 b- defN 22-May-26 20:05 dargor/tuning.py
--rw-r-----  2.0 unx      760 b- defN 22-Nov-08 22:35 dargor-0.5.9.dist-info/LICENSE
--rw-r-----  2.0 unx      989 b- defN 22-Nov-08 22:35 dargor-0.5.9.dist-info/METADATA
--rw-r-----  2.0 unx       92 b- defN 22-Nov-08 22:35 dargor-0.5.9.dist-info/WHEEL
--rw-r-----  2.0 unx        7 b- defN 22-Nov-08 22:35 dargor-0.5.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1726 b- defN 22-Nov-08 22:35 dargor-0.5.9.dist-info/RECORD
-23 files, 33947 bytes uncompressed, 16614 bytes compressed:  51.1%
+-rw-r-----  2.0 unx      760 b- defN 23-May-06 10:13 dargor-0.6.0.dist-info/LICENSE
+-rw-r-----  2.0 unx      989 b- defN 23-May-06 10:13 dargor-0.6.0.dist-info/METADATA
+-rw-r-----  2.0 unx       92 b- defN 23-May-06 10:13 dargor-0.6.0.dist-info/WHEEL
+-rw-r-----  2.0 unx        7 b- defN 23-May-06 10:13 dargor-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1726 b- defN 23-May-06 10:13 dargor-0.6.0.dist-info/RECORD
+23 files, 34140 bytes uncompressed, 16686 bytes compressed:  51.1%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: dargor/py.typed
 Comment: 
 
 Filename: dargor/tuning.py
 Comment: 
 
-Filename: dargor-0.5.9.dist-info/LICENSE
+Filename: dargor-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: dargor-0.5.9.dist-info/METADATA
+Filename: dargor-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: dargor-0.5.9.dist-info/WHEEL
+Filename: dargor-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: dargor-0.5.9.dist-info/top_level.txt
+Filename: dargor-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dargor-0.5.9.dist-info/RECORD
+Filename: dargor-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dargor/Curses.py

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, Gabriel Linder <linder.gabriel@gmail.com>
+# Copyright (c) 2023, Gabriel Linder <linder.gabriel@gmail.com>
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
 # copyright notice and this permission notice appear in all copies.
 #
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
 # REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
@@ -82,18 +82,16 @@
             curses.endwin()
 
     def show_error(self, e: BaseException) -> None:
 
         y, x = self.stdscr.getmaxyx()
         if e.args:
             msg = e.args[0]
-            try:
+            with suppress(ValueError):
                 msg = msg[:msg.index('\n')]
-            except ValueError:
-                pass
             m = f' {e.__class__.__name__}: {msg} '
         else:
             m = f' {e.__class__.__name__} '
         n = len(m)
 
         y = y // 2
         x = (x - n) // 2
```

## dargor/__init__.py

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, Gabriel Linder <linder.gabriel@gmail.com>
+# Copyright (c) 2023, Gabriel Linder <linder.gabriel@gmail.com>
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
 # copyright notice and this permission notice appear in all copies.
 #
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
 # REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
@@ -12,8 +12,8 @@
 # LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
 # OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
 # PERFORMANCE OF THIS SOFTWARE.
 #
 
 
 # XXX need to be the last line
-__version__ = '0.5.9'
+__version__ = '0.6.0'
```

## dargor/console.py

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, Gabriel Linder <linder.gabriel@gmail.com>
+# Copyright (c) 2023, Gabriel Linder <linder.gabriel@gmail.com>
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
 # copyright notice and this permission notice appear in all copies.
 #
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
 # REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
@@ -20,15 +20,15 @@
 
 
 @contextmanager
 def disable_output() -> Iterator[None]:
     try:
         old_out = sys.stdout
         old_err = sys.stderr
-        sys.stdout = open('/dev/null', 'w')
-        sys.stderr = open('/dev/null', 'w')
+        sys.stdout = open('/dev/null', 'w')  # noqa: SIM115
+        sys.stderr = open('/dev/null', 'w')  # noqa: SIM115
         yield
     finally:
         sys.stdout.close()
         sys.stderr.close()
         sys.stdout = old_out
         sys.stderr = old_err
```

## dargor/files.py

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, Gabriel Linder <linder.gabriel@gmail.com>
+# Copyright (c) 2023, Gabriel Linder <linder.gabriel@gmail.com>
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
 # copyright notice and this permission notice appear in all copies.
 #
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
 # REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
@@ -20,16 +20,16 @@
 
 
 @contextmanager
 def lock_and_open_for_write(fname: str,
                             mode: str = 'w') -> Iterator[IO[AnyStr]]:
     try:
         fd = None
-        lock_fd = open(f'{fname}.lock', 'w')
+        lock_fd = open(f'{fname}.lock', 'w')  # noqa: SIM115
         flock(lock_fd, LOCK_EX | LOCK_NB)
-        fd = open(fname, mode)
+        fd = open(fname, mode)  # noqa: SIM115
         yield fd
     finally:
         if fd is not None:
             fd.flush()
             fd.close()
         lock_fd.close()
```

## dargor/plots.py

```diff
@@ -1,23 +1,24 @@
 #
-# Copyright (c) 2022, Gabriel Linder <linder.gabriel@gmail.com>
+# Copyright (c) 2023, Gabriel Linder <linder.gabriel@gmail.com>
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
 # copyright notice and this permission notice appear in all copies.
 #
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
 # REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
 # AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
 # INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
 # LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
 # OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
 # PERFORMANCE OF THIS SOFTWARE.
 #
 
+import matplotlib.pyplot as plt  # type: ignore[import]
 import numpy as np
 from matplotlib.axes import Axes  # type: ignore[import]
 from matplotlib.backend_bases import LocationEvent  # type: ignore[import]
 from matplotlib.figure import Figure  # type: ignore[import]
 
 
 class CursorLines:
@@ -96,7 +97,14 @@
             canvas.widgetlock.release(self)
 
 
 def maybe_add_legend(ax: Axes, *, loc: str = 'best') -> None:
     handles, labels = ax.get_legend_handles_labels()
     if labels:
         ax.legend(handles, labels, loc=loc)
+
+
+def show() -> None:
+    f = plt.gcf()
+    f.set_tight_layout(True)
+    CursorLines(f)
+    plt.show()
```

## Comparing `dargor-0.5.9.dist-info/LICENSE` & `dargor-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dargor-0.5.9.dist-info/METADATA` & `dargor-0.6.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargor
-Version: 0.5.9
+Version: 0.6.0
 Summary: My most common routines
 Home-page: https://github.com/dargor/dargor-py
 Author: Gabriel Linder
 Author-email: linder.gabriel@gmail.com
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `dargor-0.5.9.dist-info/RECORD` & `dargor-0.6.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-dargor/Curses.py,sha256=FSW93zVmjhJgDNXdDOE01ezbj_DuNzuqH_sUkv99XZY,3603
+dargor/Curses.py,sha256=MXBOhs7sI9fqokt_6yfS_ONv4ZVgm7aiBD-rqk7PTWE,3573
 dargor/DelayedKeyboardInterrupt.py,sha256=BB9jjRZN_Ig3C_ti6cqa8eqxBYedPf9rrINbBdu3M3M,1624
 dargor/Tk.py,sha256=L-c2rC2z2EC2Q3mQVCh-H5S_Bi10G3S6ATU5lB-4Ayw,1245
-dargor/__init__.py,sha256=6mHW5C-vPTxno-rC8mXATi7vwO8gZSgoNZb0fDUHdZg,843
+dargor/__init__.py,sha256=85d9NCay9OdRDqS-Uv7PQORcv6S8uDkMZeYHbYHiJ6c,843
 dargor/argparser.py,sha256=fRm0pn9EWIaFSHpR0guiSiKcLqrkIUM3pYg464f8og8,1030
 dargor/bench.py,sha256=0OU3NgtMoqhoeYLHk2NmqzjhhK-fRrB-7krjsKctU9A,1500
 dargor/coalesce.py,sha256=wGM0pSQAUTlZqQbLo8gUTL-xk4WHNUF3Ge-dpxo6lXA,987
 dargor/colored_tracebacks.py,sha256=7BP_hq8fgxuXfD4QodMa40Iw_wHXvYD00EgFU_SukFw,2062
-dargor/console.py,sha256=X6nlSpUWG51_7Uw8jwaIZWi16Lw8WmV76Y8V2EvTpKQ,1218
+dargor/console.py,sha256=62QpPvyiUXd3rBICvk8CZXMIF7Y8CNZhkOCsNcnTbGE,1250
 dargor/dataclasses_helpers.py,sha256=pbBq42tTd5NXE-cRyp9nMaqoH3UgboE0ZvyANpf4vlA,1367
 dargor/deck.py,sha256=vYpEjcF8Rp2L2JdE1dBQ67F_4YbEbjSYxXMz0MYnFOk,1955
-dargor/files.py,sha256=UdTiBJVvLWyUal1Ie6bhk41OpNgNSmGNuWVtmmvKil4,1309
+dargor/files.py,sha256=3eoD-ZYwPooy-irv1z2AcQ1-PGRMQkGLFUkUx-uv1kg,1341
 dargor/finance.py,sha256=LQ_5bL43aWkLzzfD6K-Be3n-3BH5W-H1nDFYCBUiJZ8,3798
 dargor/nice.py,sha256=hG098jf_deCW_zq00kYb7DvmWyLTtkxaJrMb-55eR8s,2030
-dargor/plots.py,sha256=q7Ipd7TIG7ZKcPRPwrdWIlQCFYFp4qlNS69_YSoB_oA,3698
+dargor/plots.py,sha256=5IFHt7r8qOVj04S4ZK4S89FLKohnQgknqreNYHWLzGk,3857
 dargor/pretty.py,sha256=MXuZotma8f6oJRc2ZPMa0O-leHjMqD4isv84-sVoIJc,903
 dargor/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dargor/tuning.py,sha256=uCmGHHHpLwfr7hYYNFkHRhizYPvrTlBOHpMy6gh1Nwk,1201
-dargor-0.5.9.dist-info/LICENSE,sha256=cxPRhnxpxK_QJeJdU4N8Nc9rIJ0Xh7jYCxqiwc-I1aw,760
-dargor-0.5.9.dist-info/METADATA,sha256=LyG1633d9jdnR7wmtAswcE0MMkdA065nALlqdUytCVA,989
-dargor-0.5.9.dist-info/WHEEL,sha256=tIy8_2ZxPExwRKcXlg4jzESby3jB9aLsFLrFCKKh88M,92
-dargor-0.5.9.dist-info/top_level.txt,sha256=rmFkR9H4yRLIr2BxJAjvGqemvJKIbaisgdU0_mo1rGc,7
-dargor-0.5.9.dist-info/RECORD,,
+dargor-0.6.0.dist-info/LICENSE,sha256=cxPRhnxpxK_QJeJdU4N8Nc9rIJ0Xh7jYCxqiwc-I1aw,760
+dargor-0.6.0.dist-info/METADATA,sha256=Qd0W9WrM2sEU_LD3WaVBE2jeYuMZbajYVVMhybYYA2Q,989
+dargor-0.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+dargor-0.6.0.dist-info/top_level.txt,sha256=rmFkR9H4yRLIr2BxJAjvGqemvJKIbaisgdU0_mo1rGc,7
+dargor-0.6.0.dist-info/RECORD,,
```

