# Comparing `tmp/rnsh-0.0.8.tar.gz` & `tmp/rnsh-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnsh-0.0.8.tar", max compression
+gzip compressed data, was "rnsh-0.0.9.tar", max compression
```

## Comparing `rnsh-0.0.8.tar` & `rnsh-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1105 2023-02-11 05:21:53.643929 rnsh-0.0.8/LICENSE
--rw-r--r--   0        0        0    10326 2023-02-14 21:43:08.818325 rnsh-0.0.8/README.md
--rw-r--r--   0        0        0      677 2023-02-14 21:43:08.818325 rnsh-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1623 2023-02-14 21:43:08.818325 rnsh-0.0.8/rnsh/__init__.py
--rw-r--r--   0        0        0     5517 2023-02-14 21:43:08.818325 rnsh-0.0.8/rnsh/args.py
--rw-r--r--   0        0        0      770 2023-02-11 17:11:58.653338 rnsh-0.0.8/rnsh/exception.py
--rw-r--r--   0        0        0     2195 2023-02-12 04:02:21.606394 rnsh-0.0.8/rnsh/hacks.py
--rw-r--r--   0        0        0    20557 2023-02-14 21:43:08.822326 rnsh-0.0.8/rnsh/process.py
--rw-r--r--   0        0        0     7648 2023-02-14 09:56:18.969763 rnsh-0.0.8/rnsh/retry.py
--rw-r--r--   0        0        0    37306 2023-02-14 21:43:08.822326 rnsh-0.0.8/rnsh/rnsh.py
--rw-r--r--   0        0        0     5221 2023-02-13 21:46:25.558817 rnsh-0.0.8/rnsh/rnslogging.py
--rw-r--r--   0        0        0     1609 2023-02-11 14:06:05.513301 rnsh-0.0.8/rnsh/testlogging.py
--rw-r--r--   0        0        0    11361 1970-01-01 00:00:00.000000 rnsh-0.0.8/setup.py
--rw-r--r--   0        0        0    10940 1970-01-01 00:00:00.000000 rnsh-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-02-11 05:21:53.643929 rnsh-0.0.9/LICENSE
+-rw-r--r--   0        0        0    10326 2023-02-14 21:43:08.818325 rnsh-0.0.9/README.md
+-rw-r--r--   0        0        0      659 2023-02-18 19:12:59.806758 rnsh-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1623 2023-02-14 21:43:08.818325 rnsh-0.0.9/rnsh/__init__.py
+-rw-r--r--   0        0        0     5517 2023-02-14 21:43:08.818325 rnsh-0.0.9/rnsh/args.py
+-rw-r--r--   0        0        0      798 2023-02-17 16:48:38.181439 rnsh-0.0.9/rnsh/exception.py
+-rw-r--r--   0        0        0      210 2023-02-18 06:09:41.069929 rnsh-0.0.9/rnsh/helpers.py
+-rw-r--r--   0        0        0    25592 2023-02-18 14:10:38.940197 rnsh-0.0.9/rnsh/process.py
+-rw-r--r--   0        0        0    11619 2023-02-18 06:09:41.069929 rnsh-0.0.9/rnsh/protocol.py
+-rw-r--r--   0        0        0     7661 2023-02-18 06:09:41.069929 rnsh-0.0.9/rnsh/retry.py
+-rw-r--r--   0        0        0    20447 2023-02-18 13:44:36.361172 rnsh-0.0.9/rnsh/rnsh.py
+-rw-r--r--   0        0        0     5225 2023-02-18 14:10:38.940197 rnsh-0.0.9/rnsh/rnslogging.py
+-rw-r--r--   0        0        0    16291 2023-02-18 06:09:41.069929 rnsh-0.0.9/rnsh/session.py
+-rw-r--r--   0        0        0     1609 2023-02-11 14:06:05.513301 rnsh-0.0.9/rnsh/testlogging.py
+-rw-r--r--   0        0        0    11334 1970-01-01 00:00:00.000000 rnsh-0.0.9/setup.py
+-rw-r--r--   0        0        0    10901 1970-01-01 00:00:00.000000 rnsh-0.0.9/PKG-INFO
```

### Comparing `rnsh-0.0.8/LICENSE` & `rnsh-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.8/README.md` & `rnsh-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.8/pyproject.toml` & `rnsh-0.0.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "rnsh"
-version = "0.0.8"
+version = "0.0.9"
 description = "Shell over Reticulum"
 authors = ["acehoss <acehoss@acehoss.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docopt = "^0.6.2"
-psutil = "^5.9.4"
-rns = "^0.4.8"
+rns = "^0.4.9"
 tomli = "^2.0.1"
 
 [tool.poetry.scripts]
 rnsh = 'rnsh.rnsh:rnsh_cli'
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
```

### Comparing `rnsh-0.0.8/rnsh/__init__.py` & `rnsh-0.0.9/rnsh/__init__.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.8/rnsh/args.py` & `rnsh-0.0.9/rnsh/args.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.8/rnsh/exception.py` & `rnsh-0.0.9/rnsh/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import contextlib
 from contextlib import AbstractContextManager
+import logging
+import sys
 
 
 class permit(AbstractContextManager):
     """Context manager to allow specified exceptions
 
     The specified exceptions will be allowed to bubble up. Other
     exceptions are suppressed.
@@ -20,7 +22,9 @@
         self._exceptions = exceptions
 
     def __enter__(self):
         pass
 
     def __exit__(self, exctype, excinst, exctb):
         return exctype is not None and not issubclass(exctype, self._exceptions)
+
+
```

### Comparing `rnsh-0.0.8/rnsh/process.py` & `rnsh-0.0.9/rnsh/process.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+from __future__ import annotations
 import asyncio
 import contextlib
 import copy
 import errno
 import fcntl
 import functools
 import logging as __logging
@@ -34,15 +35,14 @@
 import struct
 import sys
 import termios
 import threading
 import tty
 import types
 import typing
-import psutil
 
 import rnsh.exception as exception
 
 module_logger = __logging.getLogger(__name__)
 
 CTRL_C = "\x03".encode("utf-8")
 CTRL_D = "\x04".encode("utf-8")
@@ -105,14 +105,43 @@
         return result
     except EOFError:
         raise
     except Exception as ex:
         module_logger.error("tty_read error: {ex}")
 
 
+def tty_read_poll(fd: int) -> bytes:
+    """
+    Read available bytes from a tty file descriptor. When used in a callback added to a file descriptor using
+    tty_add_reader_callback(...), this function creates a solution for non-blocking reads from ttys.
+    :param fd: tty file descriptor
+    :return: bytes read
+    """
+    if fd_is_closed(fd):
+        raise EOFError
+
+    result = bytearray()
+    try:
+        flags = fcntl.fcntl(fd, fcntl.F_GETFL)
+        fcntl.fcntl(fd, fcntl.F_SETFL, flags | os.O_NONBLOCK)
+        try:
+            data = os.read(fd, 4096)
+            result.extend(data or [])
+        except OSError as e:
+            if e.errno != errno.EIO and e.errno != errno.EWOULDBLOCK:
+                raise
+            elif e.errno == errno.EIO:
+                raise EOFError
+    except EOFError:
+        raise
+    except Exception as ex:
+        module_logger.error("tty_read error: {ex}")
+    return result
+
+
 def fd_is_closed(fd: int) -> bool:
     """
     Check if file descriptor is closed
     :param fd: file descriptor
     :return: True if file descriptor is closed
     """
     try:
@@ -319,20 +348,86 @@
     :param timeout: maximum number of seconds to wait.
     :return: True if event was set, False if timeout expired
     """
     await event_wait_any([evt], timeout=timeout)
     return evt.is_set()
 
 
+def _launch_child(cmd_line: list[str], env: dict[str, str], stdin_is_pipe: bool, stdout_is_pipe: bool,
+                  stderr_is_pipe: bool) -> tuple[int, int, int, int]:
+    # Set up PTY and/or pipes
+    child_fd = parent_fd = None
+    if not (stdin_is_pipe and stdout_is_pipe and stderr_is_pipe):
+        parent_fd, child_fd = pty.openpty()
+    child_stdin, parent_stdin = (os.pipe() if stdin_is_pipe else (child_fd, parent_fd))
+    parent_stdout, child_stdout = (os.pipe() if stdout_is_pipe else (parent_fd, child_fd))
+    parent_stderr, child_stderr = (os.pipe() if stderr_is_pipe else (parent_fd, child_fd))
+
+    # Fork
+    pid = os.fork()
+
+    if pid == 0:
+        try:
+            # We are in the child process, so close all open sockets and pipes except for the PTY and/or pipes
+            max_fd = os.sysconf("SC_OPEN_MAX")
+            for fd in range(3, max_fd):
+                if fd not in (child_stdin, child_stdout, child_stderr):
+                    try:
+                        os.close(fd)
+                    except OSError:
+                        pass
+
+            # Set up PTY and/or pipes
+            os.dup2(child_stdin, 0)
+            os.dup2(child_stdout, 1)
+            os.dup2(child_stderr, 2)
+            # Make PTY controlling if necessary
+            if child_fd is not None:
+                os.setsid()
+                try:
+                    tmp_fd = os.open(os.ttyname(0 if not stdin_is_pipe else 1 if not stdout_is_pipe else 2), os.O_RDWR)
+                    os.close(tmp_fd)
+                except:
+                    pass
+                # fcntl.ioctl(0 if not stdin_is_pipe else 1 if not stdout_is_pipe else 2), os.O_RDWR, termios.TIOCSCTTY, 0)
+
+            # Execute the command
+            os.execvpe(cmd_line[0], cmd_line, env)
+        except Exception as err:
+            exc_type, exc_obj, exc_tb = sys.exc_info()
+            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+            print(f"Unable to start {cmd_line[0]}: {err} ({fname}:{exc_tb.tb_lineno})")
+            sys.stdout.flush()
+        # don't let any other modules get in our way, do an immediate silent exit.
+        os._exit(255)
+
+    else:
+        # We are in the parent process, so close the child-side of the PTY and/or pipes
+        if child_fd is not None:
+            os.close(child_fd)
+        if child_stdin != child_fd:
+            os.close(child_stdin)
+        if child_stdout != child_fd:
+            os.close(child_stdout)
+        if child_stderr != child_fd:
+            os.close(child_stderr)
+        # # Close the write end of the pipe if a pipe is used for standard input
+        # if not stdin_is_pipe:
+        #     os.close(parent_stdin)
+        # Return the child PID and the file descriptors for the PTY and/or pipes
+        return pid, parent_stdin, parent_stdout, parent_stderr
+
+
 class CallbackSubprocess:
     # time between checks of child process
     PROCESS_POLL_TIME: float = 0.1
 
     def __init__(self, argv: [str], env: dict, loop: asyncio.AbstractEventLoop, stdout_callback: callable,
-                 terminated_callback: callable):
+                 stderr_callback: callable, terminated_callback: callable, stdin_is_pipe: bool, stdout_is_pipe: bool,
+                 stderr_is_pipe: bool):
         """
         Fork a child process and generate callbacks with output from the process.
         :param argv: the command line, tokenized. The first element must be the absolute path to an executable file.
         :param env: environment variables to override
         :param loop: the asyncio event loop to use
         :param stdout_callback: callback for data, e.g. def callback(data:bytes) -> None
         :param terminated_callback: callback for termination/return code, e.g. def callback(return_code:int) -> None
@@ -343,25 +438,49 @@
 
         self._log = module_logger.getChild(self.__class__.__name__)
         # self._log.debug(f"__init__({argv},{term},...")
         self._command: [str] = argv
         self._env = env or {}
         self._loop = loop
         self._stdout_cb = stdout_callback
+        self._stderr_cb = stderr_callback
         self._terminated_cb = terminated_callback
         self._pid: int = None
-        self._child_fd: int = None
+        self._child_stdin: int = None
+        self._child_stdout: int = None
+        self._child_stderr: int = None
         self._return_code: int = None
-        self._eof: bool = False
+        self._stdout_eof: bool = False
+        self._stderr_eof: bool = False
+        self._stdin_is_pipe = stdin_is_pipe
+        self._stdout_is_pipe = stdout_is_pipe
+        self._stderr_is_pipe = stderr_is_pipe
+
+    def _ensure_pipes_closed(self):
+        self._log.debug("Ensuring pipes are closed")
+        stdin = self._child_stdin
+        stdout = self._child_stdout
+        stderr = self._child_stderr
+        fds = list(filter(lambda x: x is not None, list({stdin, stdout, stderr})))
+        for fd in fds:
+            self._log.debug(f"Closing fd {fd}")
+            with contextlib.suppress(OSError):
+                os.close(self._child_stdin)
+            with contextlib.suppress(OSError):
+                tty_unset_reader_callbacks(fd)
+        self._child_stdin = None
+        self._child_stdout = None
+        self._child_stderr = None
 
     def terminate(self, kill_delay: float = 1.0):
         """
         Terminate child process if running
         :param kill_delay: if after kill_delay seconds the child process has not exited, escalate to SIGHUP and SIGKILL
         """
+
         self._log.debug("terminate()")
         if not self.running:
             return
 
         with exception.permit(SystemExit):
             os.kill(self._pid, signal.SIGTERM)
 
@@ -371,20 +490,25 @@
                 with exception.permit(SystemExit):
                     os.kill(self._pid, signal.SIGHUP)
                     os.kill(self._pid, signal.SIGKILL)
 
         self._loop.call_later(kill_delay, kill)
 
         def wait():
+            self._log.debug("wait()")
             with contextlib.suppress(OSError):
-                self._log.debug("wait()")
                 os.waitpid(self._pid, 0)
-                self._log.debug("wait() finish")
+            self._ensure_pipes_closed()
+            self._log.debug("wait() finish")
+
+        threading.Thread(target=wait, daemon=True).start()
 
-        threading.Thread(target=wait).start()
+    def close_stdin(self):
+        with contextlib.suppress(Exception):
+            os.close(self._child_stdin)
 
     @property
     def started(self) -> bool:
         """
         :return: True if child process has been started
         """
         return self._pid is not None
@@ -398,27 +522,27 @@
 
     def write(self, data: bytes):
         """
         Write bytes to the stdin of the child process.
         :param data: bytes to write
         """
         self._log.debug(f"write({data})")
-        os.write(self._child_fd, data)
+        os.write(self._child_stdin, data)
 
     def set_winsize(self, r: int, c: int, h: int, v: int):
         """
         Set the window size on the tty of the child process.
         :param r: rows visible
         :param c: columns visible
         :param h: horizontal pixels visible
         :param v: vertical pixels visible
         :return:
         """
         self._log.debug(f"set_winsize({r},{c},{h},{v}")
-        tty_set_winsize(self._child_fd, r, c, h, v)
+        tty_set_winsize(self._child_stdout, r, c, h, v)
 
     def copy_winsize(self, fromfd: int):
         """
         Copy window size from one tty to another.
         :param fromfd: source tty file descriptor
         """
         r, c, h, v = tty_get_winsize(fromfd)
@@ -426,25 +550,25 @@
 
     def tcsetattr(self, when: int, attr: list[any]):  # actual type is list[int | list[int | bytes]]
         """
         Set tty attributes.
         :param when: when to apply change: termios.TCSANOW or termios.TCSADRAIN or termios.TCSAFLUSH
         :param attr: attributes to set
         """
-        termios.tcsetattr(self._child_fd, when, attr)
+        termios.tcsetattr(self._child_stdin, when, attr)
 
     def tcgetattr(self) -> list[any]:  # actual type is list[int | list[int | bytes]]
         """
         Get tty attributes.
         :return: tty attributes value
         """
-        return termios.tcgetattr(self._child_fd)
+        return termios.tcgetattr(self._child_stdout)
 
     def ttysetraw(self):
-        tty.setraw(self._child_fd, termios.TCSADRAIN)
+        tty.setraw(self._child_stdout, termios.TCSADRAIN)
 
     def start(self):
         """
         Start the child process.
         """
         self._log.debug("start()")
 
@@ -465,68 +589,73 @@
 
         # match = re.search("^/bin/(.*sh)$", program)
         # if match:
         #     self._command[0] = "-" + match.group(1)
         #     env["SHELL"] = program
         #     self._log.debug(f"set login shell {self._command}")
 
-        self._pid, self._child_fd = pty.fork()
-
-        if self._pid == 0:
-            try:
-                # This may not be strictly necessary, but there is
-                # occasionally some funny business that goes on with
-                # networking after the fork. Anecdotally this fixed
-                # it, but more testing is needed as it might be a
-                # coincidence.
-                p = psutil.Process()
-                for c in p.connections(kind='all'):
-                    with exception.permit(SystemExit):
-                        os.close(c.fd)
-                # TODO: verify that skipping setpgrp fixes Operation not permitted on Manjaro
-                # os.setpgrp()
-                os.execvpe(program, self._command, env)
-            except Exception as err:
-                print(f"Child process error: {err}, command: {self._command}")
-                sys.stdout.flush()
-            # don't let any other modules get in our way.
-            os._exit(0)
+        self._pid, \
+            self._child_stdin, \
+            self._child_stdout, \
+            self._child_stderr = _launch_child(self._command, env, self._stdin_is_pipe, self._stdout_is_pipe,
+                                               self._stderr_is_pipe)
 
         def poll():
             # self.log.debug("poll")
             try:
                 pid, self._return_code = os.waitpid(self._pid, os.WNOHANG)
                 if self._return_code is not None:
                     self._return_code = self._return_code & 0xff
                 if self._return_code is not None and not process_exists(self._pid):
                     self._log.debug(f"polled return code {self._return_code}")
                     self._terminated_cb(self._return_code)
-                self._loop.call_later(CallbackSubprocess.PROCESS_POLL_TIME, poll)
+                if self.running:
+                    self._loop.call_later(CallbackSubprocess.PROCESS_POLL_TIME, poll)
+                else:
+                    self._ensure_pipes_closed()
             except Exception as e:
                 if not hasattr(e, "errno") or e.errno != errno.ECHILD:
                     self._log.debug(f"Error in process poll: {e}")
 
         self._loop.call_later(CallbackSubprocess.PROCESS_POLL_TIME, poll)
 
-        def reader(fd: int, callback: callable):
+        def stdout():
+            try:
+                with exception.permit(SystemExit):
+                    data = tty_read_poll(self._child_stdout)
+                    if data is not None and len(data) > 0:
+                        self._stdout_cb(data)
+            except EOFError:
+                self._stdout_eof = True
+                tty_unset_reader_callbacks(self._child_stdout)
+                self._stdout_cb(bytearray())
+
+        def stderr():
             try:
                 with exception.permit(SystemExit):
-                    data = tty_read(fd)
+                    data = tty_read_poll(self._child_stderr)
                     if data is not None and len(data) > 0:
-                        callback(data)
+                        self._stderr_cb(data)
             except EOFError:
-                self._eof = True
-                tty_unset_reader_callbacks(self._child_fd)
-                callback(bytearray())
+                self._stderr_eof = True
+                tty_unset_reader_callbacks(self._child_stderr)
+                self._stdout_cb(bytearray())
+
+        tty_add_reader_callback(self._child_stdout, stdout, self._loop)
+        if self._child_stderr != self._child_stdout:
+            tty_add_reader_callback(self._child_stderr, stderr, self._loop)
 
-        tty_add_reader_callback(self._child_fd, functools.partial(reader, self._child_fd, self._stdout_cb), self._loop)
+    @property
+    def stdout_eof(self):
+        return self._stdout_eof or not self.running
 
     @property
-    def eof(self):
-        return self._eof or not self.running
+    def stderr_eof(self):
+        return self._stderr_eof or not self.running
+
 
     @property
     def return_code(self) -> int:
         return self._return_code
 
     @property
     def pid(self) -> int:
```

### Comparing `rnsh-0.0.8/rnsh/retry.py` & `rnsh-0.0.9/rnsh/retry.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self._log = module_logger.getChild(self.__class__.__name__)
         self._loop_period = loop_period
         self._statuses: list[RetryStatus] = []
         self._tag_counter = 0
         self._lock = threading.RLock()
         self._run = True
         self._finished: asyncio.Future = None
-        self._thread = threading.Thread(name=name, target=self._thread_run)
+        self._thread = threading.Thread(name=name, target=self._thread_run, daemon=True)
         self._thread.start()
 
     def is_alive(self):
         return self._thread.is_alive()
 
     def close(self, loop: asyncio.AbstractEventLoop = None) -> asyncio.Future:
         self._log.debug("stopping timer thread")
```

### Comparing `rnsh-0.0.8/rnsh/rnslogging.py` & `rnsh-0.0.9/rnsh/rnslogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import asyncio
 import logging
 import sys
 import termios
 import rnsh.process as process
 from logging import Handler, getLevelName
-from types import GenericAlias
+# from types import GenericAlias
 from typing import Any
 
 import RNS
 
 import rnsh.exception as exception
 
 
@@ -97,15 +97,15 @@
         except Exception:
             self.handleError(record)
 
     def __repr__(self):
         level = getLevelName(self.level)
         return '<%s (%s)>' % (self.__class__.__name__, level)
 
-    __class_getitem__ = classmethod(GenericAlias)
+    # __class_getitem__ = classmethod(GenericAlias)
 
 
 log_format = '%(name)-30s %(message)s [%(threadName)s]'
 
 logging.basicConfig(
     level=logging.DEBUG,  # RNS.log will filter it, but some formatting will still be processed before it gets there
     # format='%(asctime)s.%(msecs)03d %(levelname)-6s %(threadName)-15s %(name)-15s %(message)s',
```

### Comparing `rnsh-0.0.8/rnsh/testlogging.py` & `rnsh-0.0.9/rnsh/testlogging.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.0.8/setup.py` & `rnsh-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 packages = \
 ['rnsh']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['docopt>=0.6.2,<0.7.0',
- 'psutil>=5.9.4,<6.0.0',
- 'rns>=0.4.8,<0.5.0',
- 'tomli>=2.0.1,<3.0.0']
+['docopt>=0.6.2,<0.7.0', 'rns>=0.4.9,<0.5.0', 'tomli>=2.0.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['rnsh = rnsh.rnsh:rnsh_cli']}
 
 setup_kwargs = {
     'name': 'rnsh',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Shell over Reticulum',
     'long_description': '# `r n s h` \xa0Shell over Reticulum \n[![CI](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml)\xa0\n[![Release](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml)\xa0\n[![PyPI version](https://badge.fury.io/py/rnsh.svg)](https://badge.fury.io/py/rnsh) \xa0\n![PyPI - Downloads](https://img.shields.io/pypi/dw/rnsh?color=informational&label=Installs&logo=pypi)\n\n`rnsh` is a utility written in Python that facilitates shell \nsessions over [Reticulum](https://reticulum.network) networks. \nIt is based on the `rnx` utility that ships with Reticulum and\naims to provide a similar experience to SSH.\n\n`rnsh` is still a little raw; there are some things that are \nimplemented badly, and many other things that haven\'t been \nbuilt at all (yet). Signals (i.e. Ctrl-C) need some work, so have\nanother terminal handy to send a SIGTERM if things glitch\nout.\n\nAnyway, there\'s a lot of room for improvement.\n\n## Contents\n\n- [Alpha Disclaimer](#reminder--alpha-software)\n- [Recent Changes](#recent-changes)\n- [Quickstart](#quickstart)\n- [Options](#options)\n- [How it works](#how-it-works)\n- [Roadmap](#roadmap)\n- [Active TODO](#todo)\n\n### Reminder: Alpha Software\nThese early versions will be buggy. There will sometimes be major\nbreaking changes to the command line parameters between releases.\nThere will sometimes be breaking changes in the protocol between\nreleases. Use at your own peril!\n\n## Recent Changes\n### v0.0.8\n- Improved test suite exposed several issues with the handling of\ncommand line arguments which are now fixed\n- Fixed a race condition that would cause remote characters to be \n  lost intermittently when running remote commands that finish\n  immediately.\n- Added automated testing that actually spins up a random listener\n  and initiator in a private Reticulum network and passes data\n  between them, uncovering more issues which are now fixed.\n- Fixed (hopefully) an issue where `rnsh` doesn\'t know what\n  version it is.\n\n### v0.0.7\nAdded `-A` command line option. This listener option causes the\nremote command line to be appended to the arguments list of the\nlaunched program. This allows the listener to jail connections\nto a particular executable while still allowing parameters.\n\n### v0.0.6\nMinor improvements in transport efficiency\n\n### v0.0.5\n#### Remote command line and pipe compatibility\nCommand line options have changed somewhat to allow the initiator\nto supply a command line. This allows `rnsh` to function similarly\nto SSH. You can pipe into or out of `rnsh` to send input through\nremote commands or remote command output through other commands.\n\nThis behavior can be blocked on the listener with the `-C` option.\n\nWhen the initiator does not supply a command, the listener uses\na default command specified on its command line. If a default\ncommand is not specified, the listener falls back to the shell\nof the user it is running under.\n\n## Quickstart\n\nTested (thus far) on Python 3.11 macOS 13.1 ARM64. Should\nrun on Python 3.6+ on Linux or Unix. WSL probably works. \nCygwin might work, too.\n\n- Activate a virtualenv\n- `pip3 install rnsh`\n  - Or from a `whl` release, `pip3 install /path/to/rnsh-0.0.1-py3-none-any.whl`\n- Configure Reticulum interfaces, check with `rnstatus`\n- Ready to run `rnsh`. The options are shown below.\n\n### Example: Shell server\n#### Setup\nBefore running the listener or initiator, you\'ll need to get the \nlistener destination hash and the initiator identity hash.\n```shell\n# On listener\nrnsh -l -p\n\n# On initiator\nrnsh -p\n```\nNote: if you are using a non-default identity or service name, be\nsure to supply these options with `-p` as the identity and \ndestination hashes will change depending on these settings.\n\n#### Listener\n- Listening for default service name ("default").\n- Using user\'s default Reticulum config dir (~/.reticulum).\n- Using default identity ($RNSCONFIGDIR/storage/identities/rnsh).\n- Allowing remote identity `6d47805065fa470852cf1b1ef417a1ac` to connect.\n- Launching `/bin/zsh` on authorized connect.\n```shell\nrnsh -l -a 6d47805065fa470852cf1b1ef417a1ac -- /bin/zsh\n```\n#### Initiator\n- Connecting to default service name ("default").\n- Using user\'s default Reticulum config dir (~/.reticulum).\n- Using default identity ($RNSCONFIGDIR/storage/identities/rnsh).\n- Connecting to destination `a5f72aefc2cb3cdba648f73f77c4e887`\n```shell\nrnsh a5f72aefc2cb3cdba648f73f77c4e887\n```\n\n## Options\n```\nUsage:\n    rnsh [--config <configdir>] [-i <identityfile>] [-s <service_name>] [-l] -p\n    rnsh -l [--config <configfile>] [-i <identityfile>] [-s <service_name>] \n         [-v... | -q...] [-b <period>] (-n | -a <identity_hash> [-a <identity_hash>] ...) \n         [-A | -C] [[--] <program> [<arg> ...]]\n    rnsh [--config <configfile>] [-i <identityfile>] [-s <service_name>] \n         [-v... | -q...] [-N] [-m] [-w <timeout>] <destination_hash> \n         [[--] <program> [<arg> ...]]\n    rnsh -h\n    rnsh --version\n\nOptions:\n    --config DIR                 Alternate Reticulum config directory to use\n    -i FILE --identity FILE      Specific identity file to use\n    -s NAME --service NAME       Listen on/connect to specific service name if not default\n    -p --print-identity          Print identity information and exit\n    -l --listen                  Listen (server) mode. If supplied, <program> <arg>...will \n                                   be used as the command line when the initiator does not\n                                   provide one or when remote command is disabled. If\n                                   <program> is not supplied, the default shell of the \n                                   user rnsh is running under will be used.\n    -b --announce PERIOD         Announce on startup and every PERIOD seconds\n                                 Specify 0 for PERIOD to announce on startup only.\n    -a HASH --allowed HASH       Specify identities allowed to connect\n    -n --no-auth                 Disable authentication\n    -N --no-id                   Disable identify on connect\n    -A --remote-command-as-args  Concatenate remote command to argument list of <program>/shell\n    -C --no-remote-command       Disable executing command line from remote\n    -m --mirror                  Client returns with code of remote process\n    -w TIME --timeout TIME       Specify client connect and request timeout in seconds\n    -q --quiet                   Increase quietness (move level up), multiple increases effect\n                                          DEFAULT LOGGING LEVEL\n                                                  CRITICAL (silent)\n                                    Initiator ->  ERROR\n                                                  WARNING\n                                     Listener ->  INFO\n                                                  DEBUG    (insane)\n    -v --verbose                 Increase verbosity (move level down), multiple increases effect\n    --version                    Show version\n    -h --help                    Show this help\n```\n\n## How it works\n### Listeners\nListener instances are the servers. Each listener is configured \nwith an RNS identity, and a service name. Together, RNS makes\nthese into a destination hash that can be used to connect to\nyour listener.\n   \nMultiple listeners can use the same identity. As long as \nthey are given different service names. They will have \ndifferent destination hashes and not conflict.\n\nListeners must be configured with a command line to run (at \nleast at this time). The identity hash string is set in the\nenvironment variable RNS_REMOTE_IDENTITY for use in child\nprograms.\n\nListeners are set up using the `-l` flag.\n   \n### Initiators\nInitiators are the clients. Each initiator has an identity\nhash which is used as an authentication mechanism on Reticulum.\nYou\'ll need this value to configure the listener to allow \nyour connection. It is possible to run the server without \nauthentication, but hopefully it\'s obvious that this is an\nadvanced use case. \n    \nTo get the identity hash, use the `-p` flag.\n    \nWith the initiator identity set up in the listener command\nline, and with the listener identity copied (you\'ll need to\ndo `-p` on the listener side, too), you can run the\ninitiator.\n    \nI recommend staying pretty vanilla to start with and\ntrying `/bin/zsh` or whatever your favorite shell is these \ndays. The shell should start in login mode. Ideally it\nworks just like an `ssh` shell session.\n\n### Protocol\nThe protocol is build on top of the Reticulum `Request` and\n`Packet` APIs.\n\n- After the initiator identifies on the connection, it enters\n  a request loop. \n- When idle, the initiator will periodically \n  poll the listener. \n- When the initiator has data available (i.e the user typed \n  some characters), the initiator will send that data to the\n  listener in a request, and the listener will respond with \n  any data available from the listener. \n- When the listener has new data available, it notifies the \n  initiator using a notification packet. The initiator then \n  makes a request to the listener to fetch the data.\n   \n## Roadmap\n1. Plan a better roadmap\n2. ?\n3. Keep my day job\n\n## TODO\n- [X] ~~Initial version~~\n- [X] ~~Pip package with command-line utility support~~\n- [X] ~~Publish to PyPI~~\n- [X] ~~Improve signal handling~~\n- [X] ~~Make it scriptable (currently requires a tty)~~\n- [X] ~~Protocol improvements (throughput!)~~\n- [X] ~~Documentation improvements~~\n- [ ] Test on several platforms\n- [ ] Fix issues that come up with testing\n- [ ] Fix issues with running `rnsh` in a binary pipeline, i.e. \n  piping the output of `tar` over `rsh`.\n- [ ] Beta release\n- [ ] Test and fix more issues\n- [ ] V1.0\n- [ ] Enhancement Ideas\n  - [ ] `authorized_keys` mode similar to SSH\n  - [ ] Git over `rnsh` (git remote helper)\n  - [ ] Sliding window acknowledgements for improved throughput\n\n## Miscellaneous\n\nBy piping into/out of `rnsh`, it should be possible to transfer\nfiles using the same method discussed in \n[this article](https://cromwell-intl.com/open-source/tar-and-ssh.html).\nI tested it just now and it doesn\'t work right. There\'s probably some\nsubtle garbling of the data at one end of the stream or the other.\n',
     'author': 'acehoss',
     'author_email': 'acehoss@acehoss.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rnsh-0.0.8/PKG-INFO` & `rnsh-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: rnsh
-Version: 0.0.8
+Version: 0.0.9
 Summary: Shell over Reticulum
 License: MIT
 Author: acehoss
 Author-email: acehoss@acehoss.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: rns (>=0.4.8,<0.5.0)
+Requires-Dist: rns (>=0.4.9,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # `r n s h`  Shell over Reticulum 
 [![CI](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml) 
 [![Release](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml) 
 [![PyPI version](https://badge.fury.io/py/rnsh.svg)](https://badge.fury.io/py/rnsh)
```

