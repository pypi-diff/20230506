# Comparing `tmp/zoomaker-0.3.1.tar.gz` & `tmp/zoomaker-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomaker-0.3.1.tar", max compression
+gzip compressed data, was "zoomaker-0.4.0.tar", max compression
```

## Comparing `zoomaker-0.3.1.tar` & `zoomaker-0.4.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     5252 2023-04-28 12:07:13.807392 zoomaker-0.3.1/README.md
--rw-r--r--   0        0        0      587 2023-04-28 13:10:44.197861 zoomaker-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6645 2023-04-28 13:10:48.598419 zoomaker-0.3.1/zoomaker.py
--rw-r--r--   0        0        0     5959 1970-01-01 00:00:00.000000 zoomaker-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     5402 2023-05-01 14:39:32.383238 zoomaker-0.4.0/README.md
+-rw-r--r--   0        0        0      587 2023-05-06 08:07:46.152788 zoomaker-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6538 2023-05-06 08:07:37.811516 zoomaker-0.4.0/zoomaker.py
+-rw-r--r--   0        0        0     6109 1970-01-01 00:00:00.000000 zoomaker-0.4.0/PKG-INFO
```

### Comparing `zoomaker-0.3.1/README.md` & `zoomaker-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 Zoomaker is a command-line tool that helps install AI models, git repositories and run scripts.
 
 - **single source of truth**: all resources are neatly definied in the `zoo.yaml` file
 - **freeze versions**: know exactly which revision of a resources is installed at any time
 - **only download once**: optimize bandwidth and cache your models locally
 - **optimize disk usage**: downloaded models are symlinked to the installation folder (small files <5MB are duplicate)
 
-## 🛠 Installation
+## 😻 TL;DR
+
+1. Install Zoomaker `pip install zoomaker`
+2. Define your resources in the `zoo.yaml` file
+3. Run `zoomaker install` to install them
+
+
+## 📦 Installation
 
 ```bash
 pip install zoomaker
 ```
 
 ## 🦁 zoo.yaml Examples
```

### Comparing `zoomaker-0.3.1/pyproject.toml` & `zoomaker-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zoomaker"
-version = "0.3.1"
+version = "0.4.0"
 description = "Zoomaker - Friendly house keeping for your AI model zoo and related resources."
 authors = ["Benedikt Groß"]
 readme = "README.md"
 homepage = "https://github.com/hfg-gmuend/zoomaker"
 documentation = "https://github.com/hfg-gmuend/zoomaker"
 repository = "https://github.com/hfg-gmuend/zoomaker"
```

### Comparing `zoomaker-0.3.1/zoomaker.py` & `zoomaker-0.4.0/zoomaker.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,33 @@
         self.yaml_file = yaml_file
         with open(yaml_file, "r") as f:
             self.data = yaml.safe_load(f)
         self._check_yaml()
 
     def _check_yaml(self):
         if "name" not in self.data:
-            raise Exception("👊 'name' is missing in zoo.yaml")
+            raise Exception("❌ 'name' is missing in zoo.yaml")
         if "resources" not in self.data:
-            raise Exception("👊 'resources' is missing in zoo.yaml")
+            raise Exception("❌ 'resources' is missing in zoo.yaml")
         for group, resources in self.data["resources"].items():
             for resource in resources:
                 if "name" not in resource:
-                    raise Exception("👊 Resource must have 'name' attribute")
+                    raise Exception("❌ Resource must have 'name' attribute")
                 if "src" not in resource:
-                    raise Exception("👊 Resource must have 'src' attribute")
+                    raise Exception("❌ Resource must have 'src' attribute")
                 if "type" not in resource:
-                    raise Exception("👊 Resource must have 'type' attribute")
+                    raise Exception("❌ Resource must have 'type' attribute")
                 if "install_to" not in resource:
-                    raise Exception("👊 Resource must have 'install_to' attribute")
+                    raise Exception("❌ Resource must have 'install_to' attribute")
                 type = resource["type"]
                 if type not in ["huggingface", "git", "download"]:
-                    raise Exception(f"👊 Unknown resource type: {type}")
+                    raise Exception(f"❌ Unknown resource type: {type}")
 
     def install(self):
-        print(f"👋 -- {self.yaml_file} --")
+        print(f"👋 ===> {self.yaml_file} <===")
         print(f"name: {self.data.get('name', 'N/A')}")
         print(f"version: {self.data.get('version', 'N/A')}\n")
         print(f"👇 installing resources ...")
         counter = 0;
         for group, resources in self.data["resources"].items():
             print(f"\n{group}:")
 
@@ -122,27 +122,22 @@
         progress_bar.close()
         if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
             print("Error: Failed to download the complete file.")
             return None
         return filename
 
 def main():
-    parser = argparse.ArgumentParser(description="Install models, git repos and run scripts defined in the zoo.yaml file")
-    parser.add_argument("command", nargs="?", default="help", choices=["install", "run"], help="The command to execute.")
+    parser = argparse.ArgumentParser(description="Install models, git repos and run scripts defined in the zoo.yaml file.")
+    parser.add_argument("command", nargs="?", choices=["install", "run"], help="The command to execute.")
     parser.add_argument("script", nargs="?", help="The script name to execute.")
-    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.3.1")
+    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.4.0")
+    args = parser.parse_args()
 
-    # print help if no arguments are provided
-    try:
-        args = parser.parse_args()
-    except:
-        parser.print_help()
-        return
-
-    zoomaker = Zoomaker("zoo.yaml")
     if args.command == "install":
-        zoomaker.install()
+        Zoomaker("zoo.yaml").install()
     elif args.command == "run":
-        zoomaker.run(args.script)
+        Zoomaker("zoo.yaml").run(args.script)
+    else:
+        parser.print_help()
 
 if __name__ == "__main__":
     main()
```

### Comparing `zoomaker-0.3.1/PKG-INFO` & `zoomaker-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoomaker
-Version: 0.3.1
+Version: 0.4.0
 Summary: Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 Home-page: https://github.com/hfg-gmuend/zoomaker
 Author: Benedikt Groß
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,15 +21,22 @@
 Zoomaker is a command-line tool that helps install AI models, git repositories and run scripts.
 
 - **single source of truth**: all resources are neatly definied in the `zoo.yaml` file
 - **freeze versions**: know exactly which revision of a resources is installed at any time
 - **only download once**: optimize bandwidth and cache your models locally
 - **optimize disk usage**: downloaded models are symlinked to the installation folder (small files <5MB are duplicate)
 
-## 🛠 Installation
+## 😻 TL;DR
+
+1. Install Zoomaker `pip install zoomaker`
+2. Define your resources in the `zoo.yaml` file
+3. Run `zoomaker install` to install them
+
+
+## 📦 Installation
 
 ```bash
 pip install zoomaker
 ```
 
 ## 🦁 zoo.yaml Examples
```

