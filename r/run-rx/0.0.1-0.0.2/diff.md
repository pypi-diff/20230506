# Comparing `tmp/run_rx-0.0.1.tar.gz` & `tmp/run_rx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_rx-0.0.1.tar", max compression
+gzip compressed data, was "run_rx-0.0.2.tar", max compression
```

## Comparing `run_rx-0.0.1.tar` & `run_rx-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-05-04 19:54:40.231125 run_rx-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      860 2023-05-04 19:53:49.663222 run_rx-0.0.1/README.md
--rw-r--r--   0        0        0      721 2023-05-04 20:02:59.025906 run_rx-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      300 2023-05-03 20:39:38.474682 run_rx-0.0.1/rx/__main__.py
--rw-r--r--   0        0        0     2250 2023-05-04 19:56:02.804093 run_rx-0.0.1/rx/client/commands/exec.py
--rw-r--r--   0        0        0      989 2023-04-22 21:27:00.833838 run_rx-0.0.1/rx/client/commands/init.py
--rw-r--r--   0        0        0     1970 2023-04-10 18:30:14.435321 run_rx-0.0.1/rx/client/configuration/config_base.py
--rw-r--r--   0        0        0     6583 2023-05-03 20:19:39.734831 run_rx-0.0.1/rx/client/configuration/local.py
--rw-r--r--   0        0        0      481 2023-03-29 19:30:38.625814 run_rx-0.0.1/rx/client/configuration/remote.py
--rw-r--r--   0        0        0     2815 2023-05-01 19:29:48.336430 run_rx-0.0.1/rx/client/executor.py
--rw-r--r--   0        0        0      256 2023-04-10 18:50:33.017005 run_rx-0.0.1/rx/client/grpc_helper.py
--rw-r--r--   0        0        0     5206 2023-04-23 15:34:21.215904 run_rx-0.0.1/rx/client/init_client.py
--rw-r--r--   0        0        0     9432 2023-05-03 20:09:03.579210 run_rx-0.0.1/rx/client/login.py
--rw-r--r--   0        0        0     2029 2023-03-25 18:11:12.345418 run_rx-0.0.1/rx/client/menu.py
--rw-r--r--   0        0        0     1029 2023-05-03 20:09:57.609097 run_rx-0.0.1/rx/client/output_handler.py
--rw-r--r--   0        0        0     2614 2023-05-03 20:22:23.926114 run_rx-0.0.1/rx/client/rsync.py
--rw-r--r--   0        0        0     1579 2023-03-29 19:53:44.892412 run_rx-0.0.1/rx/client/user.py
--rw-r--r--   0        0        0     5624 2023-04-23 18:22:17.589816 run_rx-0.0.1/rx/proto/rx_pb2.py
--rw-r--r--   0        0        0     7378 2023-04-23 18:22:17.589919 run_rx-0.0.1/rx/proto/rx_pb2.pyi
--rw-r--r--   0        0        0    11070 2023-04-23 18:22:17.590590 run_rx-0.0.1/rx/proto/rx_pb2_grpc.py
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 run_rx-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 19:54:40.231125 run_rx-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      897 2023-05-06 18:24:26.470100 run_rx-0.0.2/README.md
+-rw-r--r--   0        0        0      721 2023-05-05 22:21:30.732209 run_rx-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-05-03 20:39:38.474682 run_rx-0.0.2/rx/__main__.py
+-rw-r--r--   0        0        0     2406 2023-05-06 18:41:24.564694 run_rx-0.0.2/rx/client/commands/exec.py
+-rw-r--r--   0        0        0      989 2023-04-22 21:27:00.833838 run_rx-0.0.2/rx/client/commands/init.py
+-rw-r--r--   0        0        0     1970 2023-04-10 18:30:14.435321 run_rx-0.0.2/rx/client/configuration/config_base.py
+-rw-r--r--   0        0        0     6945 2023-05-06 18:38:30.014044 run_rx-0.0.2/rx/client/configuration/local.py
+-rw-r--r--   0        0        0      481 2023-03-29 19:30:38.625814 run_rx-0.0.2/rx/client/configuration/remote.py
+-rw-r--r--   0        0        0     2811 2023-05-05 22:11:45.982253 run_rx-0.0.2/rx/client/executor.py
+-rw-r--r--   0        0        0      256 2023-04-10 18:50:33.017005 run_rx-0.0.2/rx/client/grpc_helper.py
+-rw-r--r--   0        0        0     5202 2023-05-05 22:12:00.605647 run_rx-0.0.2/rx/client/init_client.py
+-rw-r--r--   0        0        0     9492 2023-05-05 21:12:58.788558 run_rx-0.0.2/rx/client/login.py
+-rw-r--r--   0        0        0     2029 2023-03-25 18:11:12.345418 run_rx-0.0.2/rx/client/menu.py
+-rw-r--r--   0        0        0     1029 2023-05-03 20:09:57.609097 run_rx-0.0.2/rx/client/output_handler.py
+-rw-r--r--   0        0        0     2303 2023-05-05 22:11:20.469353 run_rx-0.0.2/rx/client/rsync.py
+-rw-r--r--   0        0        0     1579 2023-03-29 19:53:44.892412 run_rx-0.0.2/rx/client/user.py
+-rw-r--r--   0        0        0     5624 2023-04-23 18:22:17.589816 run_rx-0.0.2/rx/proto/rx_pb2.py
+-rw-r--r--   0        0        0     7378 2023-04-23 18:22:17.589919 run_rx-0.0.2/rx/proto/rx_pb2.pyi
+-rw-r--r--   0        0        0    11070 2023-04-23 18:22:17.590590 run_rx-0.0.2/rx/proto/rx_pb2_grpc.py
+-rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 run_rx-0.0.2/PKG-INFO
```

### Comparing `run_rx-0.0.1/LICENSE.txt` & `run_rx-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.1/README.md` & `run_rx-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,23 +31,24 @@
 You only have to do this once per project (similar to `git init`).
 
 To execute commands on a remote machine, prefix them with `rx`:
 
 ```
 rx python foo.py
 rx ls
-rx ./scripts/my_script.sh
+rx 'echo $PATH > my-path'
 ```
 
 Check out the [getting-started](https://github.com/run-rx/getting-started) repository for more examples.
 
 ## Feedback
 
 Please file an [issue](https://github.com/run-rx/rx/issues).
 
 ## Testing
 
 To run tests, use:
 
 ```
+pip install -r test_requirements.txt
 PYTHONPATH=. pytest
 ```
```

### Comparing `run_rx-0.0.1/pyproject.toml` & `run_rx-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "run-rx"
-version = "0.0.1"
+version = "0.0.2"
 description = "A tool to simplify remote execution"
 authors = ["Kris Chodorow <k.chodorow@gmail.com>"]
 license = "LICENSE.txt"
 readme = "README.md"
 homepage = "https://www.run-rx.com"
 repository = "https://github.com/run-rx/rx"
 packages = [
```

### Comparing `run_rx-0.0.1/rx/client/commands/exec.py` & `run_rx-0.0.2/rx/client/commands/exec.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,24 +54,33 @@
     try:
       return client.exec(self._argv)
     except KeyboardInterrupt:
       client.maybe_kill()
       return executor.SIGINT_CODE
 
 
+class VersionCommand:
+  """Prints the version."""
+
+  def run(self):
+    print(local.VERSION)
+
+
 def main(argv):
   logging.get_absl_handler().python_handler.use_absl_log_file(
     program_name='rx', log_dir=tempfile.gettempdir())
   if len(argv) == 1:
     app.usage(shorthelp=True)
     return -1
+  cmd_to_run = argv[1]
   try:
-    cmd_to_run = argv[1]
     if cmd_to_run == 'init':
       cmd = init.InitCommand()
+    elif cmd_to_run == 'version':
+      cmd = VersionCommand()
     else:
       if cmd_to_run == 'run':
         # "rx run foo" is generally the same as "rx foo", but the extra "run" can
         # be handy when running a script called "init", say, on the remote
         # machine.
         argv = argv[1:]
       cmd = ExecCommand(argv[1:])
```

### Comparing `run_rx-0.0.1/rx/client/commands/init.py` & `run_rx-0.0.2/rx/client/commands/init.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.1/rx/client/configuration/config_base.py` & `run_rx-0.0.2/rx/client/configuration/config_base.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.1/rx/client/configuration/local.py` & `run_rx-0.0.2/rx/client/configuration/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """All of the info we can get without going to the server."""
 import hashlib
 import json
 import pathlib
 import shutil
-import sys
+import subprocess
 from typing import Optional, Tuple
 import uuid
 
 from absl import flags
 from absl import logging
 import sty
 
 from rx.client.configuration import config_base
 from rx.proto import rx_pb2
 
-CLIENT_VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 IGNORE = pathlib.Path('.rxignore')
 
 _REMOTE = flags.DEFINE_string(
   'remote', 'default',
   'The remote configuration file to use (see .rx/README.md).')
+_RSYNC_PATH = flags.DEFINE_string('rsync_path', None, 'Path to rsync binary')
 
 _REMOTE_DIR = config_base.RX_DIR / 'remotes'
 
 
 class LocalConfigWriter(config_base.ReadWriteConfig):
   """This holds all of the configuration options that can be determined from
   the local machine."""
@@ -60,19 +61,23 @@
 
 
 class LocalConfig(config_base.ReadOnlyConfig):
   """Create the local configuration."""
 
   def __init__(self, working_dir: pathlib.Path):
     super().__init__(working_dir / _get_local_config_file())
-    self.cwd = working_dir
+    self._cwd = working_dir
     self.config_dir = self.cwd / config_base.RX_DIR
     self._color = None
 
   @property
+  def cwd(self) -> pathlib.Path:
+    return self._cwd
+
+  @property
   def rsync_source(self) -> rx_pb2.RsyncSource:
     return rx_pb2.RsyncSource(
       machine_id=uuid.getnode(),
       directory=str(self.cwd),
     )
 
   def _get_source_env(self, docker_image: str) -> rx_pb2.Environment:
@@ -115,45 +120,42 @@
 def create_local_config(cwd: pathlib.Path) -> LocalConfig:
   """Gets or creates .rx directory."""
   config_dir = (cwd / _get_local_config_file()).parent
   config_dir.mkdir(exist_ok=True, parents=True)
   with LocalConfigWriter(cwd) as c:
     c.setup_remote()
     c['project_name'] = _find_project_name(cwd)
+    c['rsync_path'] = _get_rsync_path()
   return LocalConfig(cwd)
 
 
 def find_local_config(working_dir: pathlib.Path) -> Optional[LocalConfig]:
   """Factory to create a config by looking for .rx."""
   cfg_path = working_dir / config_base.get_config_dir()
   for parent in cfg_path.parents:
     if (parent / config_base.get_config_dir()).exists():
       return LocalConfig(parent)
   return None
 
 
-def get_bundle_path() -> pathlib.Path:
+def get_source_path() -> pathlib.Path:
   """Gets the path bundled client files can be found on."""
-  if is_bundled():
-    return pathlib.Path(sys._MEIPASS)
-  else:
-    # We are running in a normal Python environment.
-    # __file__ is ./rx/client/configuration/local.py, so this resolves to ./.
-    return pathlib.Path(__file__).resolve().parent.parent.parent.parent
+  # __file__ is ./rx/client/configuration/local.py, so this resolves to ./.
+  return pathlib.Path(__file__).resolve().parent.parent.parent.parent
 
 
 def get_grpc_metadata() -> Tuple[Tuple[str, str]]:
-  return (('cv', CLIENT_VERSION),)
+  return (('cv', VERSION),)
 
 
 def install_local_files(cwd: pathlib.Path):
   # Output directory.
   (cwd / 'rx-out').mkdir(exist_ok=True)
 
-  install_dir = pathlib.Path(get_bundle_path() / 'install')
+  install_dir = pathlib.Path(get_source_path() / 'install')
 
   _install_file(install_dir, cwd, IGNORE)
 
   config_dir = cwd / config_base.RX_DIR
   config_dir.mkdir(exist_ok=True, parents=True)
   _install_file(install_dir, config_dir, 'README.md')
 
@@ -168,17 +170,26 @@
   if default_config.exists():
     # Don't undo someone else's config.
     return
   # .rx/remote/default -> python-cpu
   default_config.symlink_to('python-cpu')
 
 
-def is_bundled() -> bool:
-  """If this is bundled rx (vs. running from source)."""
-  return getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS')
+def _get_rsync_path() -> str:
+  """Make sure rsync is installed."""
+  if _RSYNC_PATH.value:
+    return _RSYNC_PATH.value
+  try:
+    result = subprocess.run(
+      ['which', 'rsync'], check=True, capture_output=True)
+  except subprocess.CalledProcessError as e:
+    logging.error('Error finding rsync: %s', e)
+    raise ConfigError('Cannot find rsync, is it installed/on your path?')
+  # Use rsync on PATH
+  return result.stdout.decode('utf-8').strip('\n')
 
 
 def _find_project_name(start_dir: pathlib.Path) -> str:
   """Heuristic to find a reasonable name for this project."""
   # Probably the git repo is rooted on a good name.
   if (start_dir / '.git').exists():
     return start_dir.name
```

### Comparing `run_rx-0.0.1/rx/client/executor.py` & `run_rx-0.0.2/rx/client/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
   def __init__(
       self,
       channel: grpc.Channel,
       local_cfg: local.LocalConfig,
       remote_cfg: remote.Remote):
     self._uri = remote_cfg['grpc_addr']
-    self._rsync = rsync.RsyncClient(local_cfg.cwd, remote_cfg)
+    self._rsync = rsync.RsyncClient(local_cfg, remote_cfg)
     self._stub = rx_pb2_grpc.ExecutionServiceStub(channel)
     self._metadata = local.get_grpc_metadata()
     self._local_cfg = local_cfg
     self._remote_cfg = remote_cfg
     self._login = login.LoginManager()
     self._current_execution_id = None
```

### Comparing `run_rx-0.0.1/rx/client/init_client.py` & `run_rx-0.0.2/rx/client/init_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         empty_pb2.Empty(), metadata=self._metadata, timeout=_TIMEOUT)
     except grpc.RpcError as e:
       raise InitError(f'Could not get user from rx: {e.details()}', -1)
     return resp.username
 
   def _run_initial_rsync(self):
     self._rsync = rsync.RsyncClient(
-      self._local_cfg.cwd, remote.Remote(self._local_cfg.cwd))
+      self._local_cfg, remote.Remote(self._local_cfg.cwd))
     return_code = self._rsync.to_remote()
     if return_code == 0:
       logging.info('Copied files to %s', self._rsync.host)
 
   def _install_deps(self, grpc_addr: str, workspace_id: str) -> int:
     channel = grpc_helper.get_channel(grpc_addr)
     stub = rx_pb2_grpc.ExecutionServiceStub(channel)
```

### Comparing `run_rx-0.0.1/rx/client/login.py` & `run_rx-0.0.2/rx/client/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,16 +148,18 @@
     else:
       raise RuntimeError(f'Unsupported system: {system}')
     try:
       subprocess.run(cmd, check=True, capture_output=True)
     except subprocess.CalledProcessError as e:
       if e.stdout:
         print(e.stdout)
+      self._server.shutdown()
       raise AuthError(f'Error opening browser: {e}')
     except FileNotFoundError as e:
+      self._server.shutdown()
       raise AuthError(
         f'Could not find browser-opening program {cmd[0]}, are you in an SSH '
         'session?')
 
   def refresh_access_token(self):
     """Refreshes the access token when it expires."""
     refresh_file = _get_refresh_token_file()
```

### Comparing `run_rx-0.0.1/rx/client/menu.py` & `run_rx-0.0.2/rx/client/menu.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.1/rx/client/output_handler.py` & `run_rx-0.0.2/rx/client/output_handler.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.1/rx/client/rsync.py` & `run_rx-0.0.2/rx/client/rsync.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from collections import abc
 import pathlib
 import subprocess
 from typing import List
 
-from absl import flags
 from absl import logging
 
 from rx.client.configuration import config_base
 from rx.client.configuration import local
 
-_RSYNC_PATH = flags.DEFINE_string('rsync_path', None, 'Path to rsync binary')
-
 
 class RsyncClient:
   """Rsync tools."""
 
   def __init__(
-      self, sync_dir: pathlib.Path, remote_cfg: abc.Mapping):
-    self._sync_dir = sync_dir
+      self, local_cfg: local.LocalConfig, remote_cfg: abc.Mapping):
+    self._sync_dir = local_cfg.cwd
     self._cfg = remote_cfg
-    self._rsync_path = _get_rsync_path()
+    self._rsync_path = local_cfg['rsync_path']
     self._daemon_addr = self._cfg["worker_addr"]
     if config_base.is_local():
       # Remove the port (rsync isn't listening on 50051).
       self._daemon_addr = self._daemon_addr.split(':')[0]
 
   @property
   def host(self) -> str:
@@ -80,18 +77,7 @@
       logging.error('stderr: %s', e.stderr)
     if e.returncode is None:
       return -1
     return e.returncode
   if result.stdout:
     print(f'stdout: {result.stdout}')
   return 0
-
-
-def _get_rsync_path() -> str:
-  if _RSYNC_PATH.value:
-    return _RSYNC_PATH.value
-
-  if local.is_bundled():
-    return str(local.get_bundle_path() / 'bin/rsync')
-
-  # Otherwise, use whatever's on the path.
-  return 'rsync'
```

### Comparing `run_rx-0.0.1/rx/client/user.py` & `run_rx-0.0.2/rx/client/user.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.1/rx/proto/rx_pb2.py` & `run_rx-0.0.2/rx/proto/rx_pb2.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.1/rx/proto/rx_pb2.pyi` & `run_rx-0.0.2/rx/proto/rx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.1/rx/proto/rx_pb2_grpc.py` & `run_rx-0.0.2/rx/proto/rx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.1/PKG-INFO` & `run_rx-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-rx
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to simplify remote execution
 Home-page: https://www.run-rx.com
 License: LICENSE.txt
 Author: Kris Chodorow
 Author-email: k.chodorow@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -56,24 +56,25 @@
 You only have to do this once per project (similar to `git init`).
 
 To execute commands on a remote machine, prefix them with `rx`:
 
 ```
 rx python foo.py
 rx ls
-rx ./scripts/my_script.sh
+rx 'echo $PATH > my-path'
 ```
 
 Check out the [getting-started](https://github.com/run-rx/getting-started) repository for more examples.
 
 ## Feedback
 
 Please file an [issue](https://github.com/run-rx/rx/issues).
 
 ## Testing
 
 To run tests, use:
 
 ```
+pip install -r test_requirements.txt
 PYTHONPATH=. pytest
 ```
```

