# Comparing `tmp/pypawcli-1.0.0.tar.gz` & `tmp/pypawcli-1.1.0.tar.gz`

## Comparing `pypawcli-1.0.0.tar` & `pypawcli-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pypawcli-1.0.0/setup.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/__main__.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/version.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/__init__.py
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/console.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/file.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/students.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/system.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/task/__init__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/task/alwayson.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/task/params.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/task/scheduled.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/webapp/__init__.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/webapp/app.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/webapp/header.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/webapp/params.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/webapp/ssl.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/commands/webapp/static.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/core/__init__.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/core/callback.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/core/config.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/core/context.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/core/enum.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/core/formatter.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/core/path.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/core/result.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pypawcli-1.0.0/src/pawcli/core/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/conftest.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/test_app.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/test_config.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/test_console.py
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/test_file.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/test_students.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/test_system.py
--rw-r--r--   0        0        0     8667 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/test_task.py
--rw-r--r--   0        0        0    17179 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/cli/test_webapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/core/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/core/conftest.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/core/test_callback.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/core/test_enum.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/core/test_path.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pypawcli-1.0.0/tests/core/test_utils.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pypawcli-1.0.0/.gitignore
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pypawcli-1.0.0/LICENSE
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pypawcli-1.0.0/README.md
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 pypawcli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 pypawcli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pypawcli-1.1.0/setup.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/__init__.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/__main__.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/version.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/__init__.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/console.py
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/file.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/students.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/system.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/task/__init__.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/task/alwayson.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/task/params.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/task/scheduled.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/webapp/__init__.py
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/webapp/app.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/webapp/header.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/webapp/params.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/webapp/ssl.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/commands/webapp/static.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/core/__init__.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/core/callback.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/core/config.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/core/context.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/core/enum.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/core/formatter.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/core/path.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/core/result.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pypawcli-1.1.0/src/pawcli/core/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/conftest.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/test_app.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/test_config.py
+-rw-r--r--   0        0        0     5790 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/test_console.py
+-rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/test_file.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/test_students.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/test_system.py
+-rw-r--r--   0        0        0     8667 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/test_task.py
+-rw-r--r--   0        0        0    17179 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/cli/test_webapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/core/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/core/conftest.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/core/test_callback.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/core/test_enum.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/core/test_path.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pypawcli-1.1.0/tests/core/test_utils.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pypawcli-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pypawcli-1.1.0/LICENSE
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pypawcli-1.1.0/README.md
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 pypawcli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 pypawcli-1.1.0/PKG-INFO
```

### Comparing `pypawcli-1.0.0/src/pawcli/app.py` & `pypawcli-1.1.0/src/pawcli/app.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/src/pawcli/commands/console.py` & `pypawcli-1.1.0/src/pawcli/commands/console.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         result = api.list()
     process_result(result)
 
 
 @console_app.command(short_help="Create a new console")
 def new(
     ctx: Context,
-    # TODO: python
     executable: Shell = Argument(..., help="Console executable"),
     args: Optional[str] = Option(None, help="Additional arguments"),
     working_dir: Optional[str] = Option(
         None,
         "--working-dir",
         "-d",
         metavar="PATH",
@@ -103,20 +102,22 @@
     result = ctx.obj.api.console.create(
         executable=executable,
         arguments=args,
         working_directory=(
             resolve(ctx, working_dir) if working_dir is not None else None
         ),
     )
-    process_result(result, expected_status=201)
+    if result is None:
+        ctx.exit(1)
+    process_result(result)
     if default:
-        ctx.obj.config.set("console", "default_id", str(result.content["id"]))
+        ctx.obj.config.set("console", "default_id", str(result["id"]))
         save_config(ctx)
     if open_frame:
-        frame_path = result.content["console_frame_url"]
+        frame_path = result["console_frame_url"]
         launch(f"https://www.pythonanywhere.com{frame_path}")
 
 
 @console_app.command()
 def info(
     ctx: Context,
     console_id: int = CONSOLE_ID_ARGUMENT,
@@ -130,17 +131,18 @@
 @console_app.command()
 def rm(
     ctx: Context,
     console_id: int = CONSOLE_ID_ARGUMENT,
 ) -> None:
     """Remove the console"""
 
-    result = ctx.obj.api.console.kill(console_id)
-    process_result(result, expected_status=204, print_content=False)
+    if not ctx.obj.api.console.kill(console_id):
+        ctx.exit(1)
 
+    # try to remove default_id from config
     try:
         default_id = ctx.obj.config.getint(
             "console",
             "default_id",
             fallback=None,
         )
     except ValueError:  # pragma: no cover
@@ -154,31 +156,35 @@
 @console_app.command()
 def output(
     ctx: Context,
     console_id: int = CONSOLE_ID_ARGUMENT,
 ) -> None:
     """Get console output"""
 
-    result = ctx.obj.api.console.get_output(console_id)
-    process_result(
-        result,
-        print_content=False,
-        callback=lambda c: print(c.get("output", None)),
-    )
+    print(ctx.obj.api.console.get_output(console_id))
 
 
 @console_app.command()
 def exec(
     ctx: Context,
     command: str = Argument(..., metavar="CMD"),
     console_id: int = CONSOLE_ID_OPTION,
+    get_output: bool = Option(
+        False,
+        "--output",
+        "-o",
+        help="Get console output",
+    ),
 ) -> None:
     """Execute command in console"""
 
     if not command.endswith("\n"):
         command += "\n"
 
     result = ctx.obj.api.console.send_input(
         console_id=console_id,
-        input_=command,
+        command=command,
     )
-    process_result(result, print_content=False)
+    if not result:
+        ctx.exit(1)
+    if get_output:
+        output(ctx, console_id)
```

### Comparing `pypawcli-1.0.0/src/pawcli/commands/file.py` & `pypawcli-1.1.0/src/pawcli/commands/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,16 +99,15 @@
     dest = resolve(ctx, dest)
     output = get_remote_output_path(str(source), dest)
     try:
         data = source.read_bytes()
     except IOError:  # pragma: no cover
         print(f"Can't read {source}")
         ctx.abort()
-    result = ctx.obj.api.file.upload(output, data)
-    process_result(result, expected_status=[200, 201], print_content=False)
+    ctx.obj.api.file.upload(output, data)
 
 
 @file_app.command(short_help="Download file")
 def download(
     ctx: Context,
     source: str = Argument(...),
     dest: Path = Argument(Path.cwd(), show_default=False),
@@ -123,55 +122,62 @@
     """Download remote source to local dest"""
 
     source = resolve(ctx, source)
     dest = get_local_output_path(source, str(dest), force)
     if dest is None:
         print("dest path exist")
         ctx.exit(1)
-    result = ctx.obj.api.file.get_content(source)
-    process_result(result, print_content=False)
-    if not isinstance(result.content, bytes):
+    result = ctx.obj.api.file.get_file_content(source)
+    if result is None:
         print(f"{source} not a file")
         ctx.exit(1)
+
     try:
-        dest.write_bytes(result.content)
+        dest.write_bytes(result)
     except IOError:  # pragma: no cover
         print(f"Can't write in {dest}")
         ctx.exit(1)
 
 
 @file_app.command(short_help="Remove content")
 def rm(ctx: Context, path: str = PATH_REMOTE_ARGUMENT) -> None:
     """Remove files and directories
 
     NOTE: directory will be removed recursively.
     """
 
-    result = ctx.obj.api.file.delete(path)
-    process_result(result, expected_status=204, print_content=False)
+    if not ctx.obj.api.file.delete(path):
+        ctx.exit(1)
 
 
 @file_app.command()
 def ls(
     ctx: Context,
     path: str = PATH_REMOTE_ARGUMENT,
     json: bool = Option(False, "--json", is_flag=True, help="JSON output"),
 ) -> None:
     """List directory contents"""
 
-    result = ctx.obj.api.file.get_content(path)
+    result = ctx.obj.api.file.get_directory_content(path)
+    if result is None:
+        print(f"{path} not a directory")
+        ctx.exit(1)
+
     formatter = DirectoryFormatter() if not json else None
     process_result(result, formatter=formatter)
 
 
 @file_app.command()
 def cat(ctx: Context, path: str = PATH_REMOTE_ARGUMENT) -> None:
     """Show file content"""
 
-    result = ctx.obj.api.file.get_content(path)
+    result = ctx.obj.api.file.get_file_content(path)
+    if result is None:
+        print(f"{path} not a file")
+        ctx.exit(1)
     process_result(result, formatter=ContentFormatter())
 
 
 @file_app.command(short_help="Path sharing status")
 def share(
     ctx: Context,
     path: str = PATH_REMOTE_ARGUMENT,
@@ -183,24 +189,26 @@
     ),
 ) -> None:
     """Get or update current sharing status for a path"""
 
     api = ctx.obj.api.file
     if update is not None:
         if update:
-            result = api.start_sharing(path)
-            status = [200, 201]
+            print(api.start_sharing(path))
         else:
-            result = api.stop_sharing(path)
-            status = 204
+            ctx.exit(int(not api.stop_sharing(path)))
     else:
         result = api.get_sharing_status(path)
-        status = 200
-    process_result(result, expected_status=status)
+        if result is None:
+            ctx.exit(1)
+        print(result)
 
 
 @file_app.command()
 def tree(ctx: Context, path: str = PATH_REMOTE_ARGUMENT) -> None:
     """List directory contents (recursively)"""
 
     result = ctx.obj.api.file.get_tree(path)
+    if result is None:
+        print(f"{path} is not a directory or does not exist")
+        ctx.exit(1)
     process_result(result)
```

### Comparing `pypawcli-1.0.0/src/pawcli/commands/students.py` & `pypawcli-1.1.0/src/pawcli/commands/students.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     process_result(result)
 
 
 @students_app.command()
 def rm(ctx: Context, id_: str = Argument(..., metavar="ID")) -> None:
     """Remove the student"""
 
-    result = ctx.obj.api.students.delete(id_)
-    process_result(result, expected_status=204, print_content=False)
+    if not ctx.obj.api.students.delete(id_):
+        ctx.exit(1)
```

### Comparing `pypawcli-1.0.0/src/pawcli/commands/system.py` & `pypawcli-1.1.0/src/pawcli/commands/system.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/src/pawcli/commands/task/alwayson.py` & `pypawcli-1.1.0/src/pawcli/commands/task/alwayson.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """Create a new task"""
 
     result = ctx.obj.api.alwayson_task.create(
         command=command,
         enabled=enabled,
         description=description,
     )
-    process_result(result, expected_status=201)
+    process_result(result)
 
 
 @alwayson_app.command()
 def update(
     ctx: Context,
     task_id: int = TASK_ID_ARGUMENT,
     enabled: Optional[bool] = ENABLED_OPTION,
@@ -69,16 +69,16 @@
     process_result(result)
 
 
 @alwayson_app.command()
 def rm(ctx: Context, task_id: int = TASK_ID_ARGUMENT) -> None:
     """Delete the task"""
 
-    result = ctx.obj.api.alwayson_task.delete(task_id)
-    process_result(result, expected_status=204, print_content=False)
+    if not ctx.obj.api.alwayson_task.delete(task_id):
+        ctx.exit(1)
 
 
 @alwayson_app.command()
 def log(ctx: Context, task_id: int = TASK_ID_ARGUMENT) -> None:
     """Task log"""
 
     cat(ctx, f"/var/log/alwayson-log-{task_id}.log")
```

### Comparing `pypawcli-1.0.0/src/pawcli/commands/task/params.py` & `pypawcli-1.1.0/src/pawcli/commands/task/params.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/src/pawcli/commands/task/scheduled.py` & `pypawcli-1.1.0/src/pawcli/commands/task/scheduled.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         command=command,
         minute=minute,
         hour=hour,
         enabled=enabled,
         interval=interval,
         description=description,
     )
-    process_result(result, expected_status=201)
+    process_result(result)
 
 
 @scheduled_app.command()
 def update(
     ctx: Context,
     task_id: int = TASK_ID_ARGUMENT,
     command: Optional[str] = COMMAND_OPTION,
@@ -98,16 +98,16 @@
     process_result(result)
 
 
 @scheduled_app.command()
 def rm(ctx: Context, task_id: int = TASK_ID_ARGUMENT) -> None:
     """Delete the task"""
 
-    result = ctx.obj.api.scheduled_task.delete(task_id)
-    process_result(result, expected_status=204, print_content=False)
+    if not ctx.obj.api.scheduled_task.delete(task_id):
+        ctx.exit(1)
 
 
 @scheduled_app.command()
 def log(ctx: Context, task_id: int = TASK_ID_ARGUMENT) -> None:
     """Task log"""
 
     cat(ctx, f"/var/log/schedule-log-{task_id}.log")
```

### Comparing `pypawcli-1.0.0/src/pawcli/commands/webapp/app.py` & `pypawcli-1.1.0/src/pawcli/commands/webapp/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 from pawcli.core.callback import init_api
 from pawcli.core.enum import AppLog
 from pawcli.core.enum import Python3Version
 from pawcli.core.path import resolve
 from pawcli.core.result import process_result
 from pawcli.core.utils import save_config
 
+from .params import APP_HTTPS_OPTION
+from .params import APP_PROTECTION_OPTION
+from .params import APP_PROTECTION_PASSWORD_OPTION
+from .params import APP_PROTECTION_USERNAME_OPTION
+from .params import APP_SRC_OPTION
+from .params import APP_VENV_OPTION
 from .params import DOMAIN_ARGUMENT
 from .params import DOMAIN_OPTION
 from .params import PYTHON_VERSION_OPTION
 
 webapp_app = Typer(help="Manage webapps")
 
 
@@ -84,79 +90,67 @@
 ) -> None:
     """App configuration"""
 
     result = ctx.obj.api.webapp.get_info(domain)
     process_result(result)
 
 
-@webapp_app.command(short_help="Create a new app")
+@webapp_app.command()
 def new(
     ctx: Context,
     domain: str = DOMAIN_ARGUMENT,
     python: Optional[Python3Version] = PYTHON_VERSION_OPTION,
+    src: Optional[str] = APP_SRC_OPTION,
+    venv: Optional[str] = APP_VENV_OPTION,
+    https: Optional[bool] = APP_HTTPS_OPTION,
+    protection: Optional[bool] = APP_PROTECTION_OPTION,
+    username: Optional[str] = APP_PROTECTION_USERNAME_OPTION,
+    password: Optional[str] = APP_PROTECTION_PASSWORD_OPTION,
     default: bool = Option(
         False,
         "--default",
         "-D",
         is_flag=True,
         help="Use app as default for `domain` argument",
     ),
 ) -> None:
-    """ \b
-    Create a new app with minimal configuration.
-    Use `update` command to setup your app.
-    """
+    """Create a new app"""
+
+    if not ctx.obj.api.webapp.create(domain, python.as_external()):
+        ctx.exit(1)
 
     if default:
         ctx.obj.config.set("webapp", "default_domain", domain)
         save_config(ctx)
 
-    result = ctx.obj.api.webapp.create(domain, python.as_external())
-    process_result(result)
+    update(
+        ctx=ctx,
+        python=python,
+        domain=domain,
+        src=src,
+        venv=venv,
+        https=https,
+        protection=protection,
+        username=username,
+        password=password,
+    )
+    reload(ctx, domain=domain)
 
 
 @webapp_app.command(short_help="Modify configuration")
 def update(
     ctx: Context,
     domain: str = DOMAIN_ARGUMENT,
     python: Optional[Python3Version] = PYTHON_VERSION_OPTION,
-    src: Optional[str] = Option(
-        None,
-        metavar="PATH",
-        help="Source directory",
-    ),
-    venv: Optional[str] = Option(
-        None,
-        metavar="PATH",
-        help="Virtualenv path",
-    ),
-    https: Optional[bool] = Option(
-        None,
-        "--https/--http",
-        is_flag=True,
-        help="Enbale/Disable force HTTPS",
-    ),
-    protection: Optional[bool] = Option(
-        None,
-        "--priv/--pub",
-        is_flag=True,
-        help="Enable/Disable password protection",
-    ),
-    username: Optional[str] = Option(
-        None,
-        "--username",
-        "-u",
-        help="Username for password protection",
-    ),
-    password: Optional[str] = Option(
-        None,
-        "--password",
-        "-p",
-        help="Password for password protection",
-    ),
+    src: Optional[str] = APP_SRC_OPTION,
+    venv: Optional[str] = APP_VENV_OPTION,
+    https: Optional[bool] = APP_HTTPS_OPTION,
+    protection: Optional[bool] = APP_PROTECTION_OPTION,
+    username: Optional[str] = APP_PROTECTION_USERNAME_OPTION,
+    password: Optional[str] = APP_PROTECTION_PASSWORD_OPTION,
 ) -> None:
     """Modify configuration
 
     App restart required.
     """
 
     result = ctx.obj.api.webapp.update(
@@ -165,62 +159,62 @@
         source_directory=resolve(ctx, src) if src is not None else None,
         virtualenv_path=resolve(ctx, venv) if venv is not None else None,
         force_https=https,
         protection=protection,
         protection_username=username,
         protection_password=password,
     )
-    process_result(result, expected_status=[201, 200])
+    process_result(result)
 
 
 @webapp_app.command(short_help="Delete the app")
 def rm(
     ctx: Context,
     domain: str = DOMAIN_ARGUMENT,
 ) -> None:
     """Delete the app
 
     WSGI config and your code is not touched.
     """
 
-    result = ctx.obj.api.webapp.delete(domain)
-    process_result(result, expected_status=204)
+    if not ctx.obj.api.webapp.delete(domain):
+        ctx.exit(1)
 
 
 @webapp_app.command()
 def on(
     ctx: Context,
     domain: str = DOMAIN_ARGUMENT,
 ) -> None:
     """Enable the app"""
 
-    result = ctx.obj.api.webapp.enable(domain)
-    process_result(result)
+    if not ctx.obj.api.webapp.enable(domain):
+        ctx.exit(1)
 
 
 @webapp_app.command()
 def off(
     ctx: Context,
     domain: str = DOMAIN_ARGUMENT,
 ) -> None:
     """Disable the app"""
 
-    result = ctx.obj.api.webapp.disable(domain)
-    process_result(result)
+    if not ctx.obj.api.webapp.disable(domain):
+        ctx.exit(1)
 
 
 @webapp_app.command()
 def reload(
     ctx: Context,
     domain: str = DOMAIN_ARGUMENT,
 ) -> None:
     """Reload the app"""
 
-    result = ctx.obj.api.webapp.reload(domain)
-    process_result(result)
+    if not ctx.obj.api.webapp.reload(domain):
+        ctx.exit(1)
 
 
 @webapp_app.command()
 def log(
     ctx: Context,
     log: AppLog,
     domain: str = DOMAIN_OPTION,
```

### Comparing `pypawcli-1.0.0/src/pawcli/commands/webapp/header.py` & `pypawcli-1.1.0/src/pawcli/commands/webapp/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     result = ctx.obj.api.webapp.add_static_header(
         domain_name=domain,
         url=url,
         name=name,
         value=value,
     )
-    process_result(result, expected_status=201)
+    process_result(result)
 
 
 @header_app.command()
 def info(
     ctx: Context,
     header_id: int = HEADER_ID_ARGUMENT,
     domain: str = DOMAIN_OPTION,
@@ -91,9 +91,9 @@
     domain: str = DOMAIN_OPTION,
 ) -> None:
     """Remove app static header
 
     App restart required.
     """
 
-    result = ctx.obj.api.webapp.delete_static_header(domain, header_id)
-    process_result(result, expected_status=204, print_content=False)
+    if not ctx.obj.api.webapp.delete_static_header(domain, header_id):
+        ctx.exit(1)
```

### Comparing `pypawcli-1.0.0/src/pawcli/commands/webapp/static.py` & `pypawcli-1.1.0/src/pawcli/commands/webapp/static.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ) -> None:
     """Add static files
 
     App restart required.
     """
 
     result = ctx.obj.api.webapp.add_static_file(domain, url, path)
-    process_result(result, expected_status=201)
+    process_result(result)
 
 
 @static_app.command()
 def info(
     ctx: Context,
     file_id: int = FILE_ID_ARGUMENT,
     domain: str = DOMAIN_OPTION,
@@ -82,9 +82,9 @@
     domain: str = DOMAIN_OPTION,
 ) -> None:
     """Remove static file
 
     App restart required.
     """
 
-    resutl = ctx.obj.api.webapp.delete_static_file(domain, file_id)
-    process_result(resutl, expected_status=204, print_content=False)
+    if not ctx.obj.api.webapp.delete_static_file(domain, file_id):
+        ctx.exit(1)
```

### Comparing `pypawcli-1.0.0/src/pawcli/core/callback.py` & `pypawcli-1.1.0/src/pawcli/core/callback.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/src/pawcli/core/config.py` & `pypawcli-1.1.0/src/pawcli/core/config.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/src/pawcli/core/context.py` & `pypawcli-1.1.0/src/pawcli/core/context.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/src/pawcli/core/enum.py` & `pypawcli-1.1.0/src/pawcli/core/enum.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/src/pawcli/core/formatter.py` & `pypawcli-1.1.0/src/pawcli/core/formatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,25 +16,21 @@
 class JsonFormatter(AbstractFormatter):  # pragma: no cover
     __slots__ = "indent"
 
     def __init__(self, indent: int = 2) -> None:
         self.indent = indent
 
     def __call__(self, content) -> str:
-        if isinstance(content, (dict, list)):
-            return jsonlib.dumps(content, indent=self.indent)
+        return jsonlib.dumps(content, indent=self.indent)
 
 
 class DirectoryFormatter(AbstractFormatter):  # pragma: no cover
     __slots__ = ()
 
     def __call__(self, content) -> str:
-        if not isinstance(content, dict):
-            return "not a directory"
-
         dirs = []
         files = []
         for k, v in content.items():
             if v["type"] == "file":
                 files.append(k)
             else:
                 dirs.append(f"{k}/")
@@ -50,10 +46,8 @@
         return result
 
 
 class ContentFormatter(AbstractFormatter):  # pragma: no cover
     __slots__ = ()
 
     def __call__(self, content) -> str:
-        if not isinstance(content, bytes):
-            return "not a file"
         return content.decode()
```

### Comparing `pypawcli-1.0.0/src/pawcli/core/path.py` & `pypawcli-1.1.0/src/pawcli/core/path.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/conftest.py` & `pypawcli-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/cli/test_config.py` & `pypawcli-1.1.0/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/cli/test_console.py` & `pypawcli-1.1.0/tests/cli/test_console.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     assert result.exit_code == 0, result.stdout
     mock_api.console.create.assert_called_once_with(**args)
 
 
 def test_new_as_default(monkeypatch, mock_context_object):
     new_console_id = 200100
     resp = mock.Mock()
-    resp.content = {"id": new_console_id}
+    resp = {"id": new_console_id}
     mock_context_object.api.console.create.return_value = resp
     monkeypatch.delitem(mock_context_object.config["console"], "default_id")
     with mock.patch(f"{MODULE}.save_config") as save_config:
         result = runner.invoke(app, ["console", "new", "bash", "--default"])
     assert result.exit_code == 0, result.stdout
     save_config.assert_called()
     mock_context_object.api.console.create.assert_called_once_with(
@@ -88,15 +88,15 @@
         mock_context_object.config["console"]["default_id"]
     ) == new_console_id
 
 
 def test_new_open(mock_context_object):
     resp = mock.Mock()
     url = "/user/username/consoles/1234/frame/"
-    resp.content = {"console_frame_url": url}
+    resp = {"console_frame_url": url}
     mock_context_object.api.console.create.return_value = resp
     with mock.patch(f"{MODULE}.launch") as launch:
         result = runner.invoke(app, ["console", "new", "bash", "--open"])
     assert result.exit_code == 0, result.stdout
     launch.assert_called_once_with(f"https://www.pythonanywhere.com{url}")
     mock_context_object.api.console.create.assert_called_once_with(
         executable=Shell.BASH,
@@ -144,35 +144,38 @@
 def test_output(mock_api):
     result = runner.invoke(app, ["console", "output", str(console_id)])
     assert result.exit_code == 0, result.stdout
     mock_api.console.get_output.assert_called_once_with(console_id)
 
 
 def test_exec(mock_api):
+    mock_api.console.send_input.return_value = True
     result = runner.invoke(
         app, ["console", "exec", "-c", str(console_id), cmd_command]
     )
     assert result.exit_code == 0, result.stdout
     mock_api.console.send_input.assert_called_once_with(
         console_id=console_id,
-        input_=cmd_command_nl,
+        command=cmd_command_nl,
     )
 
 
 def test_exec_default_id(mock_api, config_dict):
+    mock_api.console.send_input.return_value = True
     result = runner.invoke(app, ["console", "exec", cmd_command])
     assert result.exit_code == 0, result.stdout
     mock_api.console.send_input.assert_called_once_with(
         console_id=int(config_dict["console"]["default_id"]),
-        input_=cmd_command_nl,
+        command=cmd_command_nl,
     )
 
 
 def test_exec_nl(mock_api):
+    mock_api.console.send_input.return_value = True
     result = runner.invoke(
         app, ["console", "exec", "-c", str(console_id), cmd_command_nl]
     )
     assert result.exit_code == 0, result.stdout
     mock_api.console.send_input.assert_called_once_with(
         console_id=console_id,
-        input_=cmd_command_nl,
+        command=cmd_command_nl,
     )
```

### Comparing `pypawcli-1.0.0/tests/cli/test_file.py` & `pypawcli-1.1.0/tests/cli/test_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,64 +32,68 @@
     "src,esrc,dest",
     (
         ("~/foo.bar", "/home/{}/foo.bar", ""),
         ("pa:~/foo/bar.py", "/home/{}/foo/bar.py", "/tmp/bar.py"),
         ("pa:~/foo/bar.py", "/home/{}/foo/bar.py", "~/bar.py"),
     )
 )
-@mock.patch(f"{MODULE}.isinstance", new=mock.Mock(return_value=True))
 def test_download(mock_api, username, src, esrc, dest):
     with runner.isolated_filesystem():
         with mock.patch("pathlib.Path.write_bytes"):
             result = runner.invoke(app, ["file", "download", src, dest])
 
     assert result.exit_code == 0, result.stdout
-    mock_api.file.get_content.assert_called_once_with(esrc.format(username))
+    mock_api.file.get_file_content.assert_called_once_with(
+        esrc.format(username)
+    )
 
 
-@mock.patch(f"{MODULE}.isinstance", new=mock.Mock(return_value=True))
 def test_download_exists(mock_api):
     with runner.isolated_filesystem():
         dest = Path.cwd() / "foo"
         dest.write_text("bar")
         with mock.patch("pathlib.Path.write_bytes"):
             result = runner.invoke(
                 app, ["file", "download", "~/bar", str(dest)]
             )
 
     assert result.exit_code != 0
-    mock_api.file.get_content.assert_not_called()
+    mock_api.file.get_file_content.assert_not_called()
     assert "path exist" in result.stdout
 
 
-@mock.patch(f"{MODULE}.isinstance", new=mock.Mock(return_value=True))
 def test_download_exists_force(mock_api, username):
     with runner.isolated_filesystem():
         dest = Path.cwd() / "foo"
         dest.write_text("bar")
         with mock.patch("pathlib.Path.write_bytes"):
             result = runner.invoke(
                 app, ["file", "download", "~/bar", str(dest), "-f"]
             )
 
     assert result.exit_code == 0, result.stdout
-    mock_api.file.get_content.assert_called_once_with(f"/home/{username}/bar")
+    mock_api.file.get_file_content.assert_called_once_with(
+        f"/home/{username}/bar"
+    )
 
 
-@mock.patch(f"{MODULE}.isinstance", new=mock.Mock(return_value=False))
 def test_download_not_a_file(monkeypatch, mock_api, username):
+    mock_api.file.get_file_content.return_value = None
     with runner.isolated_filesystem():
         dest = Path.cwd() / "foo"
         with mock.patch("pathlib.Path.write_bytes"):
             result = runner.invoke(
                 app, ["file", "download", "~/bar", str(dest)]
             )
 
+    mock_api.file.get_file_content.return_value = b""
     assert result.exit_code != 0
-    mock_api.file.get_content.assert_called_once_with(f"/home/{username}/bar")
+    mock_api.file.get_file_content.assert_called_once_with(
+        f"/home/{username}/bar"
+    )
     assert "not a file" in result.stdout
 
 
 @pytest.mark.parametrize(
     "src,dest,edest",
     (
         (".foo.py", "pa:~/foo.py", "/home/{}/foo.py"),
@@ -101,22 +105,21 @@
         Path(src).expanduser().resolve().write_text("baz")
         result = runner.invoke(app, ["file", "upload", src, dest])
 
     assert result.exit_code == 0, result.stdout
     mock_api.file.upload.assert_called_once_with(edest.format(username), b"baz")
 
 
-@mock.patch(f"{MODULE}.isinstance", new=mock.Mock(return_value=True))
 def test_cp_download_dest_empty(mock_api, username):
     with runner.isolated_filesystem():
         with mock.patch("pathlib.Path.write_bytes"):
             result = runner.invoke(app, ["file", "cp", "~/foo.bar"])
 
     assert result.exit_code == 0, result.stdout
-    mock_api.file.get_content.assert_called_once_with(
+    mock_api.file.get_file_content.assert_called_once_with(
         f"/home/{username}/foo.bar"
     )
 
 
 @pytest.mark.parametrize(
     "src,esrc,dest",
     (
@@ -127,15 +130,17 @@
 @mock.patch(f"{MODULE}.isinstance", new=mock.Mock(return_value=True))
 def test_cp_download(mock_api, username, src, esrc, dest):
     with runner.isolated_filesystem():
         with mock.patch("pathlib.Path.write_bytes"):
             result = runner.invoke(app, ["file", "cp", src, dest])
 
     assert result.exit_code == 0, result.stdout
-    mock_api.file.get_content.assert_called_once_with(esrc.format(username))
+    mock_api.file.get_file_content.assert_called_once_with(
+        esrc.format(username)
+    )
 
 
 @pytest.mark.parametrize(
     "src,esrc,dest,edest",
     (
         (
             "./foo.py",
@@ -194,22 +199,24 @@
     mock_api.file.delete.assert_called_once_with(out.format(username))
 
 
 @pytest.mark.parametrize("in_,out", _path)
 def test_cat(mock_api, username, in_, out):
     result = runner.invoke(app, ["file", "cat", in_])
     assert result.exit_code == 0, result.stdout
-    mock_api.file.get_content.assert_called_once_with(out.format(username))
+    mock_api.file.get_file_content.assert_called_once_with(out.format(username))
 
 
 @pytest.mark.parametrize("in_,out", _path)
 def test_ls(mock_api, username, in_, out):
     result = runner.invoke(app, ["file", "ls", in_])
     assert result.exit_code == 0, result.stdout
-    mock_api.file.get_content.assert_called_once_with(out.format(username))
+    mock_api.file.get_directory_content.assert_called_once_with(
+        out.format(username)
+    )
 
 
 @pytest.mark.parametrize("in_,out", _path)
 def test_share_info(mock_api, username, in_, out):
     result = runner.invoke(app, ["file", "share", in_])
     assert result.exit_code == 0, result.stdout
     mock_api.file.get_sharing_status.assert_called_once_with(
```

### Comparing `pypawcli-1.0.0/tests/cli/test_students.py` & `pypawcli-1.1.0/tests/cli/test_students.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/cli/test_system.py` & `pypawcli-1.1.0/tests/cli/test_system.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/cli/test_task.py` & `pypawcli-1.1.0/tests/cli/test_task.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/cli/test_webapp.py` & `pypawcli-1.1.0/tests/cli/test_webapp.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/core/test_callback.py` & `pypawcli-1.1.0/tests/core/test_callback.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/core/test_enum.py` & `pypawcli-1.1.0/tests/core/test_enum.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/core/test_path.py` & `pypawcli-1.1.0/tests/core/test_path.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/tests/core/test_utils.py` & `pypawcli-1.1.0/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/LICENSE` & `pypawcli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypawcli-1.0.0/pyproject.toml` & `pypawcli-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.7"
 dependencies = [
-  "pypawapi >=1.2.0,<2.0.0",
+  "pypawapi >=2.0.0,<3.0.0",
   "typer >=0.6.1,<1.0.0",
 ]
 
 [project.optional-dependencies]
 lint = [
   "flake8 ==5.0.4",
   "flake8-bugbear ==22.6.22",
```

### Comparing `pypawcli-1.0.0/PKG-INFO` & `pypawcli-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypawcli
-Version: 1.0.0
+Version: 1.1.0
 Summary: CLI tool for PythonAnywhere
 Project-URL: Source, https://codeberg.org/maraudeur/pawcli
 Author-email: Maraudeur <maraudeur1@protonmail.ch>
 License:  The MIT License (MIT)
         
          Copyright (c) 2020 Maraudeur <maraudeur1 AT protonmail DOT ch>
         
@@ -34,15 +34,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: pypawapi<2.0.0,>=1.2.0
+Requires-Dist: pypawapi<3.0.0,>=2.0.0
 Requires-Dist: typer<1.0.0,>=0.6.1
 Provides-Extra: dev
 Requires-Dist: pre-commit<3.0.0,>=2.0.0; extra == 'dev'
 Provides-Extra: lint
 Requires-Dist: flake8-bugbear==22.6.22; extra == 'lint'
 Requires-Dist: flake8==5.0.4; extra == 'lint'
 Requires-Dist: isort<6.0.0,>=5.10.1; extra == 'lint'
```

