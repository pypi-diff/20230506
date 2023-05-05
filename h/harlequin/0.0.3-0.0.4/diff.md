# Comparing `tmp/harlequin-0.0.3.tar.gz` & `tmp/harlequin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin-0.0.3.tar", max compression
+gzip compressed data, was "harlequin-0.0.4.tar", max compression
```

## Comparing `harlequin-0.0.3.tar` & `harlequin-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1068 2023-05-04 21:57:48.643889 harlequin-0.0.3/LICENSE
--rw-r--r--   0        0        0      827 2023-05-04 21:57:48.643889 harlequin-0.0.3/README.md
--rw-r--r--   0        0        0     1312 2023-05-04 21:57:48.643889 harlequin-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       53 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/__init__.py
--rw-r--r--   0        0        0      336 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/cli.py
--rw-r--r--   0        0        0        0 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/tui/__init__.py
--rw-r--r--   0        0        0     2254 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/tui/app.css
--rw-r--r--   0        0        0     5738 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/tui/app.py
--rw-r--r--   0        0        0      476 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/tui/components/__init__.py
--rw-r--r--   0        0        0     2083 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/code_editor.py
--rw-r--r--   0        0        0     1034 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/error_modal.py
--rw-r--r--   0        0        0      672 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/filename_modal.py
--rw-r--r--   0        0        0      148 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/results_viewer.py
--rw-r--r--   0        0        0     3677 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/schema_viewer.py
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 harlequin-0.0.3/setup.py
--rw-r--r--   0        0        0     1541 1970-01-01 00:00:00.000000 harlequin-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-05 22:15:17.773850 harlequin-0.0.4/LICENSE
+-rw-r--r--   0        0        0      827 2023-05-05 22:15:17.773850 harlequin-0.0.4/README.md
+-rw-r--r--   0        0        0     1312 2023-05-05 22:15:17.773850 harlequin-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-05-05 22:15:17.773850 harlequin-0.0.4/src/harlequin/__init__.py
+-rw-r--r--   0        0        0      336 2023-05-05 22:15:17.773850 harlequin-0.0.4/src/harlequin/cli.py
+-rw-r--r--   0        0        0        0 2023-05-05 22:15:17.773850 harlequin-0.0.4/src/harlequin/tui/__init__.py
+-rw-r--r--   0        0        0     2647 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/app.css
+-rw-r--r--   0        0        0     8429 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/app.py
+-rw-r--r--   0        0        0      812 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/__init__.py
+-rw-r--r--   0        0        0      881 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/code_editor.py
+-rw-r--r--   0        0        0     1081 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/error_modal.py
+-rw-r--r--   0        0        0      672 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/filename_modal.py
+-rw-r--r--   0        0        0     2430 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/results_viewer.py
+-rw-r--r--   0        0        0     3677 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/schema_viewer.py
+-rw-r--r--   0        0        0    12090 2023-05-05 22:15:17.777850 harlequin-0.0.4/src/harlequin/tui/components/textarea.py
+-rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 harlequin-0.0.4/setup.py
+-rw-r--r--   0        0        0     1541 1970-01-01 00:00:00.000000 harlequin-0.0.4/PKG-INFO
```

### Comparing `harlequin-0.0.3/LICENSE` & `harlequin-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.3/README.md` & `harlequin-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.3/pyproject.toml` & `harlequin-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Text User Interface for DuckDB"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "harlequin", from = "src" },
 ]
```

### Comparing `harlequin-0.0.3/src/harlequin/tui/app.css` & `harlequin-0.0.4/src/harlequin/tui/app.css`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,41 @@
 $border-title-color-nofocus: $primary-lighten-3;
 $border-color-focus: $accent;
 $border-title-color-focus: $accent;
 /* Main Screen */
 #sql_client {
     layout: grid;
     grid-size: 2 2;
-    grid-columns: 1fr 4fr;
+    grid-columns: 1fr 3fr;
 }
 /* ALL WIDGETS */
 SchemaViewer, CodeEditor, ResultsViewer {
     height: 100%;
     border: round $border-color-nofocus;
     border-title-color: $border-title-color-nofocus;
+    background: $boost;
 }
-SchemaViewer:focus, CodeEditor:focus, ResultsViewer:focus {
-    height: 100%;
+SchemaViewer:focus, CodeEditor:focus-within, ResultsViewer:focus-within {
     border: round $border-color-focus;
     border-title-color: $border-title-color-focus;
 }
 
+SchemaViewer, TextContainer, ResultsTable {
+    scrollbar-background: $surface;
+    scrollbar-background-hover: $surface;
+    scrollbar-background-active: $surface;
+    scrollbar-corner-color: $surface;
+    
+    scrollbar-color: $panel-lighten-1;
+    scrollbar-color-hover: $primary;
+    scrollbar-color-active: $accent;
+}
+
+/* QUERY EDITOR */
+
 /* SCHEMA VIEWER */
 SchemaViewer {
     padding: 0 1;
     row-span: 2;
 }
 SchemaViewer .tree--guides {
     color: $primary;
@@ -33,19 +46,21 @@
     color: $accent;
 }
 SchemaViewer .tree--guides-selected {
     color: $secondary;
 }
 
 /* RESULTS VIEWER */
-ResultsViewer {
-    height: 100%;
+
+ResultsViewer.non-responsive {
+    border: round $panel-lighten-1;
 }
-ResultsViewer .datatable--cursor .datatable--header-cursor {
-    background: $secondary;
+
+ResultsTable.datatable--cursor .datatable--header-cursor {
+    background: $boost;
 }
 ResultsViewer .datatable--hover {
     background: $boost;
 }
 ResultsViewer .datatable--header {
     background: $boost;
 }
```

### Comparing `harlequin-0.0.3/src/harlequin/tui/app.py` & `harlequin-0.0.4/src/harlequin/tui/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from pathlib import Path
-from typing import Type
+from typing import Iterator, Type
 
 import duckdb
-from textual import work
+from textual import log, work
 from textual.app import App, ComposeResult, CSSPathType
 from textual.containers import Container
 from textual.driver import Driver
 from textual.reactive import reactive
 from textual.widgets import Footer, Header, Input
-from textual.worker import Worker, get_current_worker
+from textual.worker import Worker, WorkerFailed, get_current_worker
 
 from harlequin.tui.components import (
     SCHEMAS,
     TABLES,
     CodeEditor,
     ErrorModal,
+    ResultsTable,
     ResultsViewer,
     SchemaViewer,
+    TextInput,
 )
 
 
 class Harlequin(App):
     """
     A Textual App for a SQL client for DuckDB.
     """
 
     CSS_PATH = "app.css"
+    MAX_RESULTS = 50_000
 
+    query_text: reactive[str] = reactive(str)
     relation: reactive[duckdb.DuckDBPyRelation | None] = reactive(None)
     data: reactive[list[tuple]] = reactive(list)
 
     def __init__(
         self,
         db_path: Path,
         driver_class: Type[Driver] | None = None,
@@ -42,100 +46,162 @@
         super().__init__(driver_class, css_path, watch_css)
 
     def compose(self) -> ComposeResult:
         """Create child widgets for the app."""
         with Container(id="sql_client"):
             yield Header()
             yield SchemaViewer(self.db_name, connection=self.connection)
-            yield CodeEditor(placeholder="select ...")
+            yield CodeEditor()
             yield ResultsViewer()
             yield Footer()
 
-    def on_mount(self) -> None:
-        editor = self.query_one(CodeEditor)
+    async def on_mount(self) -> None:
+        worker = self.update_schema_data()
+        editor = self.query_one(TextInput)
         self.set_focus(editor)
-        self.update_schema_data()
+        await worker.wait()
+
+    def on_code_editor_submitted(self, message: CodeEditor.Submitted) -> None:
+        self.query_text = "\n".join(message.lines)
 
     def on_input_submitted(self, message: Input.Submitted) -> None:
+        self.app.pop_screen()
+        editor = self.query_one(TextInput)
         if message.input.id == "save_modal":
-            self.app.pop_screen()
             try:
                 with open(message.input.value, "w") as f:
-                    editor = self.query_one(CodeEditor)
-                    f.write(editor.value)
+                    query = "\n".join([line.rstrip() for line in editor.lines])
+                    f.write(query)
             except OSError as e:
                 self.push_screen(
                     ErrorModal(
+                        title="Save File Error",
                         header=(
                             "Harlequin encountered an error when "
                             "attempting to save your file:"
                         ),
                         error=e,
                     )
                 )
         elif message.input.id == "load_modal":
-            self.app.pop_screen()
             try:
                 with open(message.input.value, "r") as f:
-                    editor = self.query_one(CodeEditor)
-                    editor.value = f.read()
-                    editor.action_end()
+                    query = f.read()
             except OSError as e:
                 self.push_screen(
                     ErrorModal(
+                        title="Load File Error",
                         header=(
                             "Harlequin encountered an error when "
                             "attempting to load your file:"
                         ),
                         error=e,
                     )
                 )
-        else:
-            try:
-                self.relation = self.connection.sql(message.value)
-            except duckdb.Error as e:
-                self.push_screen(
-                    ErrorModal(
-                        header=(
-                            "DuckDB raised an error when compiling "
-                            "or running your query:"
-                        ),
-                        error=e,
-                    )
-                )
+            else:
+                editor.move_cursor(0, 0)
+                editor.lines = [f"{line} " for line in query.splitlines()]
 
     def set_data(self, data: list[tuple]) -> None:
+        log(f"set_data {len(data)}")
         self.data = data
 
-    async def watch_relation(self, relation: duckdb.DuckDBPyRelation | None) -> None:
-        table = self.query_one(ResultsViewer)
-        table.clear(columns=True)
-        if relation is not None:  # select query
-            table.add_columns(*relation.columns)
-            worker = self.fetch_relation_data(relation)
+    async def watch_query_text(self, query_text: str) -> None:
+        pane = self.query_one(ResultsViewer)
+        pane.show_loading()
+        pane.set_not_responsive()
+        try:
+            worker = self.build_relation(query_text)
             await worker.wait()
-        else:  # DDL/DML query or an error
-            self.data = []
-        self.update_schema_data()
+        except WorkerFailed as e:
+            pane.show_table()
+            self.push_screen(
+                ErrorModal(
+                    title="DuckDB Error",
+                    header=(
+                        "DuckDB raised an error when compiling "
+                        "or running your query:"
+                    ),
+                    error=e.error,
+                )
+            )
+        else:
+            table = pane.get_table()
+            table.clear(columns=True)
+            relation = worker.result
+            if relation:  # select query
+                self.relation = relation
+            elif bool(query_text.strip()):  # DDL/DML query
+                pane.set_responsive()
+                pane.show_table()
+                self.data = []
+                self.update_schema_data()
+            else:  # blank query
+                pane.set_responsive(did_run=False)
+                pane.show_table()
+                self.data = []
+
+    def watch_relation(self, relation: duckdb.DuckDBPyRelation | None) -> None:
+        """
+        Only runs for select statements, except when first mounted.
+        """
+        # invalidate results so watch_data runs even if the results are the same
+        self.data = []
+        if relation is not None:
+            table = self.query_one(ResultsViewer).get_table()
+            table.add_columns(*relation.columns)
+            self.fetch_relation_data(relation)
 
-    def watch_data(self, data: list[tuple]) -> None:
+    async def watch_data(self, data: list[tuple]) -> None:
         if data:
-            table = self.query_one(ResultsViewer)
-            table.add_rows(data)
+            pane = self.query_one(ResultsViewer)
+            pane.set_not_responsive(max_rows=self.MAX_RESULTS, total_rows=len(data))
+            table = pane.get_table()
+            for i, chunk in self.chunk(data[: self.MAX_RESULTS]):
+                worker = self.add_data_to_table(table, chunk)
+                await worker.wait()
+                pane.increment_progress_bar()
+                if i == 0:
+                    pane.show_table()
+            pane.set_responsive(max_rows=self.MAX_RESULTS, total_rows=len(data))
+
+    @staticmethod
+    def chunk(
+        data: list[tuple], chunksize: int = 2000
+    ) -> Iterator[tuple[int, list[tuple]]]:
+        log(f"chunk {len(data)}")
+        for i in range(len(data) // chunksize + 1):
+            log(f"yielding chunk {i}")
+            yield i, data[i * chunksize : (i + 1) * chunksize]
+
+    @work(exclusive=True, exit_on_error=False)  # type: ignore
+    def build_relation(self, query_text: str) -> duckdb.DuckDBPyRelation | None:
+        relation = self.connection.sql(query_text)
+        return relation
+
+    @work(exclusive=True)
+    def fetch_relation_data(self, relation: duckdb.DuckDBPyRelation) -> None:
+        log(f"fetch_relation_data {hash(relation)}")
+        data = relation.fetchall()
+        log(f"fetch_relation_data FINISHED {hash(relation)}")
+        worker = get_current_worker()
+        if not worker.is_cancelled:
+            self.call_from_thread(self.set_data, data)
 
     @work(exclusive=False)
-    def fetch_relation_data(self, relation: duckdb.DuckDBPyRelation) -> Worker:
-        data = relation.fetchall()
+    def add_data_to_table(self, table: ResultsTable, data: list[tuple]) -> Worker:
+        log(f"add_data_to_table {len(data)}")
         worker = get_current_worker()
         if not worker.is_cancelled:
-            self.set_data(data)
+            self.call_from_thread(table.add_rows, data)
         return worker
 
-    @work(exclusive=False)
+    @work(exclusive=True)
     def update_schema_data(self) -> None:
+        log("update_schema_data")
         data: SCHEMAS = []
         schemas = self.connection.execute(
             "select distinct table_schema "
             "from information_schema.tables "
             "order by 1"
         ).fetchall()
         for (schema,) in schemas:
@@ -161,9 +227,9 @@
         schema_viewer = self.query_one(SchemaViewer)
         worker = get_current_worker()
         if not worker.is_cancelled:
             self.call_from_thread(schema_viewer.update_tree, data)
 
 
 if __name__ == "__main__":
-    app = Harlequin(Path("dev.db"))
+    app = Harlequin(Path("f1.db"))
     app.run()
```

### Comparing `harlequin-0.0.3/src/harlequin/tui/components/error_modal.py` & `harlequin-0.0.4/src/harlequin/tui/components/error_modal.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 from textual.screen import ModalScreen
 from textual.widgets import Static
 
 
 class ErrorModal(ModalScreen):
     def __init__(
         self,
+        title: str,
         header: str,
-        error: Exception,
+        error: BaseException,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
     ) -> None:
+        self.title = title
         self.header = header
         self.error = error
         super().__init__(name, id, classes)
 
     def compose(self) -> ComposeResult:
         with Vertical(id="outer"):
             yield Static(self.header, id="error_header")
             with Vertical(id="inner"):
                 with VerticalScroll():
                     yield Static(str(self.error), id="error_info")
             yield Static("Press any key to continue.", id="error_footer")
 
     def on_mount(self) -> None:
         container = self.query_one("#outer")
-        container.border_title = "DuckDB Error"
+        container.border_title = self.title
 
     def on_key(self) -> None:
         self.app.pop_screen()
```

### Comparing `harlequin-0.0.3/src/harlequin/tui/components/filename_modal.py` & `harlequin-0.0.4/src/harlequin/tui/components/filename_modal.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.3/src/harlequin/tui/components/schema_viewer.py` & `harlequin-0.0.4/src/harlequin/tui/components/schema_viewer.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.3/setup.py` & `harlequin-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'textual>=0.22.3,<0.23.0']
 
 entry_points = \
 {'console_scripts': ['harlequin = harlequin.cli:harlequin']}
 
 setup_kwargs = {
     'name': 'harlequin',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'A Text User Interface for DuckDB',
     'long_description': '# harlequin\nA Text User Interface for DuckDB.\n\n(A Harlequin is a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)\n\n![harlequin](harlequin.jpg)\n\n## Installing Harlequin\n\nUse `pip` or `pipx`:\n\n```bash\npipx install harlequin\n```\n\n## Using Harlequin\n\nTo open a DuckDB database file:\n\n```bash\nharlequin "path/to/duck.db"\n```\n\nTo open an in-memory DuckDB session, run Harlequin with no arguments:\n\n```bash\nharlequin\n```\n\nWhen Harlequin is open, you can view the schema of your DuckDB database in the left sidebar.\n\nTo run a query, enter your code in the main text input, then press Ctrl+Enter. You should see the data appear in the pane below.\n\nYou can press Tab or use your mouse to change the focus between the panes.\n\nWhen the focus is on the data pane, you can use your arrow keys or mouse to select different cells.',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `harlequin-0.0.3/PKG-INFO` & `harlequin-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlequin
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Text User Interface for DuckDB
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

