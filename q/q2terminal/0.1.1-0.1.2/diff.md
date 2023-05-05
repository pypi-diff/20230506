# Comparing `tmp/q2terminal-0.1.1.tar.gz` & `tmp/q2terminal-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2terminal-0.1.1.tar", max compression
+gzip compressed data, was "q2terminal-0.1.2.tar", max compression
```

## Comparing `q2terminal-0.1.1.tar` & `q2terminal-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      384 2023-05-05 20:36:41.697481 q2terminal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2561 2023-05-05 12:36:04.692157 q2terminal-0.1.1/q2terminal/q2terminal.py
--rw-r--r--   0        0        0       21 2023-05-05 20:36:43.723233 q2terminal-0.1.1/q2terminal/version.py
--rw-r--r--   0        0        0     2249 2023-05-05 19:42:45.995458 q2terminal-0.1.1/README.md
--rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 q2terminal-0.1.1/setup.py
--rw-r--r--   0        0        0     2566 1970-01-01 00:00:00.000000 q2terminal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      384 2023-05-05 22:00:10.298265 q2terminal-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2092 2023-05-05 21:58:06.837131 q2terminal-0.1.2/q2terminal/q2terminal.py
+-rw-r--r--   0        0        0       21 2023-05-05 22:00:14.039607 q2terminal-0.1.2/q2terminal/version.py
+-rw-r--r--   0        0        0     2249 2023-05-05 19:42:45.995458 q2terminal-0.1.2/README.md
+-rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 q2terminal-0.1.2/setup.py
+-rw-r--r--   0        0        0     2566 1970-01-01 00:00:00.000000 q2terminal-0.1.2/PKG-INFO
```

### Comparing `q2terminal-0.1.1/q2terminal/q2terminal.py` & `q2terminal-0.1.2/q2terminal/q2terminal.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,50 +41,26 @@
                 continue
             if first_line:
                 first_line = False
                 continue
 
             if line.strip() == "q2eoc":
                 if rez:
-                    self.exit_code = rez.pop()
+                    self.exit_code = rez.pop().strip()
+                    if self.exit_code.isdigit():
+                        self.exit_code = int(self.exit_code)
+                    else:
+                        self.exit_code = True if self.exit_code == "True" else False
                 break
             elif line == "":
                 continue
             else:
                 rez.append(line)
                 if echo or self.echo:
                     print(f"{ctime()}: {line}")
                 if callable(_callback):
                     callback(line)
 
         return rez
 
     def close(self):
         self.proc.terminate()
-
-
-if __name__ == "__main__":
-    q2t = Q2Terminal()
-
-    # print(q2t.run("$q2 = 123"))
-    # print(q2t.run("echo $q2"))
-    # print(q2t.run("git status"))
-    # print(q2t.exit_code)
-
-    # print(q2t.run("pwd"))
-    # print(q2t.run("pushd"))
-    # print(q2t.run("cd \\"))
-    # print(q2t.run("pwd"))
-    # print(q2t.run("popd"))
-    print(q2t.run("cd C:/Users/andre/Documents/penta.new.local/"))
-    print(q2t.run("pwd", echo=1))
-
-    def cb(line):
-        print(line)
-        if "tarting as process" in line:
-            sys.exit(100)
-
-    print(q2t.run("cmd /c penta.exe", callback=cb))
-    print(q2t.run("py3 --version", echo=1))
-    print(q2t.exit_code)
-
-    q2t.close()
```

### Comparing `q2terminal-0.1.1/README.md` & `q2terminal-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `q2terminal-0.1.1/setup.py` & `q2terminal-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['q2terminal']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'q2terminal',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '# \n\n**(code less, make more)**  \n**Based on:**  \n    q2db        (https://pypi.org/project/q2db)  \n    q2gui       (https://pypi.org/project/q2gui)  \n    q2report    (https://pypi.org/project/q2report)  \n\n## [Read the docs](docs/index.md) \n## Install & run\n**Linux**\n```bash\nsudo apt install python3-venv python3-pip -y &&\\\n    mkdir -p q2rad && \\\n    cd q2rad && \\\n    python3 -m pip install --upgrade pip && \\\n    python3 -m venv q2rad && \\\n    source q2rad/bin/activate && \\\n    python3 -m pip install --upgrade q2rad && \\\n    q2rad\n```\n**Windows**\n```bash\nmkdir q2rad &&^\ncd q2rad &&^\npy -m pip install --upgrade pip &&^\npy -m venv q2rad &&^\ncall q2rad/scripts/activate &&^\npip install --upgrade q2rad &&^\nq2rad\n```\n**Mac**\n```bash\nmkdir -p q2rad && \\\n    cd q2rad && \\\n    pip3 install --upgrade pip && \\\n    python3 -m venv q2rad && \\\n    source q2rad/bin/activate && \\\n    pip3 -m pip install --upgrade pip && \\\n    pip3 -m pip install --upgrade q2rad && \\\n    q2rad\n```\n**Docker**\n```bash\ncurl -s https://raw.githubusercontent.com/AndreiPuchko/q2rad/main/docker-x11/dockerfile > dockerfile && \\\n    mkdir -p q2rad_storage/Desktop && \\\n    chmod -R 777 q2rad_storage && \\\n    sudo docker build -t q2rad . && \\\n    sudo docker run -it \\\n        -v /tmp/.X11-unix:/tmp/.X11-unix \\\n        -v $(pwd)/q2rad_storage:/home/q2rad \\\n        -e DISPLAY=$DISPLAY \\\n        -u q2rad q2rad python3 -m q2rad\n\n```\n## Concept:\nApplication as a database\n```python\nForms:        #  may have main menu (menubar) definitions\n              #  may be linked to database table\n    \n    Lines:    #  form fields(type of data and type of form control) and \n              #  layout definitions\n              #  when form is linked to database - database columns definitions\n    \n    Actions:  #  applies for database linked forms\n              #  may be standard CRUD-action \n              #  or \n              #  run a script (run reports, forms and etc)\n              #  or\n              #  may have linked subforms (one-to-many)\n\nModules:      #  python scripts\n\nQueries:      #  query development and debugging tool\n\nReports:      #  multiformat (HTML, DOCX, XLSX) reporting tool \n```\n',
     'author': 'Andrei Puchko',
     'author_email': 'andrei.puchko@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `q2terminal-0.1.1/PKG-INFO` & `q2terminal-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2terminal
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

