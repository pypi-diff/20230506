# Comparing `tmp/pyproject_tag_check-0.3.1.tar.gz` & `tmp/pyproject_tag_check-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_tag_check-0.3.1.tar", max compression
+gzip compressed data, was "pyproject_tag_check-1.0.0.tar", max compression
```

## Comparing `pyproject_tag_check-0.3.1.tar` & `pyproject_tag_check-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-01-18 22:47:07.733701 pyproject_tag_check-0.3.1/LICENSE
--rw-r--r--   0        0        0      983 2023-01-18 22:47:07.733701 pyproject_tag_check-0.3.1/README.md
--rw-r--r--   0        0        0      613 2023-01-18 22:47:07.733701 pyproject_tag_check-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      983 2023-01-18 22:47:07.733701 pyproject_tag_check-0.3.1/pyproject_tag_check/__init__.py
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 pyproject_tag_check-0.3.1/setup.py
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 pyproject_tag_check-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 09:22:02.917245 pyproject_tag_check-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1043 2023-05-06 09:22:02.917245 pyproject_tag_check-1.0.0/README.md
+-rw-r--r--   0        0        0      611 2023-05-06 09:22:02.917245 pyproject_tag_check-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1178 2023-05-06 09:22:02.917245 pyproject_tag_check-1.0.0/pyproject_tag_check/__init__.py
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 pyproject_tag_check-1.0.0/PKG-INFO
```

### Comparing `pyproject_tag_check-0.3.1/LICENSE` & `pyproject_tag_check-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_tag_check-0.3.1/pyproject.toml` & `pyproject_tag_check-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
-name = "pyproject-tag-check"
-version = "0.3.1"
-description = "Verify version in pyproject.toml is not already used"
 authors = ["rafsaf <rafal.safin12@gmail.com>"]
+description = "Verify version in pyproject.toml is not already used"
 license = "MIT"
+name = "pyproject-tag-check"
+packages = [{include = "pyproject_tag_check"}]
 readme = "README.md"
-packages = [{ include = "pyproject_tag_check" }]
+version = "1.0.0"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
 requests = "^2.28.2"
 toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
@@ -17,9 +17,9 @@
 isort = "^5.10.1"
 pre-commit = "^2.20.0"
 
 [tool.poetry.scripts]
 pyproject-tag-check = "pyproject_tag_check.__init__:main"
 
 [build-system]
-requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core"]
```

### Comparing `pyproject_tag_check-0.3.1/pyproject_tag_check/__init__.py` & `pyproject_tag_check-1.0.0/pyproject_tag_check/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,22 +17,26 @@
     parser.add_argument(
         "--pyproject_file",
         help="Path to pyproject.toml file",
         default="pyproject.toml",
         type=str,
     )
     args = parser.parse_args()
+    print(f"checking repo: {args.repo_url}")
 
     with open(args.pyproject_file, "r") as f:
         pyproject_toml = toml.load(f)
         version = pyproject_toml["tool"]["poetry"]["version"]
+    print(f"version from file {args.pyproject_file}: {version}")
 
     url = f"{args.repo_url}/releases/tag/{version}"
+    print(f"sending request: {url}")
     r = requests.get(url=url, stream=True)
     # 404 means such a tag is not used, 200 otherwise
-    if not r.status_code == 404:
-        sys.exit(f"Tag {version} from {args.pyproject_file} already exists at {url}")
-    print("OK")
+    print(f"github response code: {r.status_code}")
+    if r.status_code == 200:
+        sys.exit(f"tag {version} from {args.pyproject_file} already exists at {url}")
+    print("ok")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyproject_tag_check-0.3.1/PKG-INFO` & `pyproject_tag_check-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-tag-check
-Version: 0.3.1
+Version: 1.0.0
 Summary: Verify version in pyproject.toml is not already used
 License: MIT
 Author: rafsaf
 Author-email: rafal.safin12@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,25 +15,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 ## pyproject-tag-check
 
-I always forget to bump poetry version in pyproject.toml files. That's why I build this simple package. It is pre-commit hook which check that version in pyproject.toml is not used as a tag for given repo URL.
+I always forget to bump poetry version in pyproject.toml files. That's why I build this simple package. It is pre-commit hook which check that version in pyproject.toml is not used as a tag for given repo URL (must be public repository).
 
 ## Usage:
 
 
-Put it in `.pre-commit.config.yaml` repos and argument must be URL to repo on GH (for example this repo itself https://github.com/rafsaf/pyproject-tag-check).
+Put it in `.pre-commit.config.yaml` repos and argument must be URL to public repo on GH (for example this repo itself https://github.com/rafsaf/pyproject-tag-check).
 
 ```yml
 repos:
   - repo: https://github.com/rafsaf/pyproject-tag-check
-    rev: "0.3.1"
+    rev: "1.0.0"
     hooks:
       - id: pyproject-tag-check
         always_run: true
         args:
           - https://github.com/rafsaf/pyproject-tag-check
 
 ```
@@ -44,8 +44,8 @@
 `pyproject.toml` usually looks like 
 
 ```toml
 [tool.poetry]
 name = "some-name..."
 version = "0.1.0"
 ```
-If tag 0.1.0 already exists like it does for https://github.com/rafsaf/pyproject-tag-check, the check will not pass.
+If repository is public and tag 0.1.0 already exists like it does for https://github.com/rafsaf/pyproject-tag-check, the check will not pass.
```

