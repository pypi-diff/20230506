# Comparing `tmp/project-structure-0.8.27.tar.gz` & `tmp/project-structure-0.8.28b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-structure-0.8.27.tar", last modified: Fri May  5 14:56:43 2023, max compression
+gzip compressed data, was "project-structure-0.8.28b0.tar", last modified: Fri May  5 22:56:26 2023, max compression
```

## Comparing `project-structure-0.8.27.tar` & `project-structure-0.8.28b0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.315921 project-structure-0.8.27/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      819 2023-05-05 14:54:58.000000 project-structure-0.8.27/.cz.toml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      643 2023-05-05 14:54:58.000000 project-structure-0.8.27/.dir-locals.el.in
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1716 2023-05-05 14:54:58.000000 project-structure-0.8.27/.dockerignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1058 2023-05-05 14:54:58.000000 project-structure-0.8.27/.env.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.292919 project-structure-0.8.27/.github/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.302919 project-structure-0.8.27/.github/workflows/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4573 2023-05-05 14:54:58.000000 project-structure-0.8.27/.github/workflows/build-test.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1716 2023-05-05 14:54:58.000000 project-structure-0.8.27/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     6288 2023-05-05 14:54:58.000000 project-structure-0.8.27/.gitlab-ci.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      877 2023-05-05 14:54:58.000000 project-structure-0.8.27/.pre-commit-config.yaml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2471 2023-05-05 14:54:58.000000 project-structure-0.8.27/.prospector.yaml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.302919 project-structure-0.8.27/.reuse/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      790 2023-05-05 14:54:58.000000 project-structure-0.8.27/.reuse/dep5
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.302919 project-structure-0.8.27/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/.tox/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5403 2023-05-05 14:54:58.000000 project-structure-0.8.27/CONTRIBUTING.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2555 2023-05-05 14:54:58.000000 project-structure-0.8.27/Dockerfile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3374 2023-05-05 14:54:58.000000 project-structure-0.8.27/Dockerfile.devel
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.302919 project-structure-0.8.27/LICENSES/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1071 2023-05-05 14:54:58.000000 project-structure-0.8.27/LICENSES/MIT.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    59007 2023-05-05 14:54:58.000000 project-structure-0.8.27/Makefile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      136 2023-05-05 14:54:58.000000 project-structure-0.8.27/NEWS-VERSION.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    13104 2023-05-05 14:54:58.000000 project-structure-0.8.27/NEWS.rst
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17777 2023-05-05 14:56:43.315921 project-structure-0.8.27/PKG-INFO
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    16758 2023-05-05 14:54:58.000000 project-structure-0.8.27/README.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4388 2023-05-05 14:54:58.000000 project-structure-0.8.27/TODO.rst
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.303920 project-structure-0.8.27/bin/
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2860 2023-05-05 14:54:58.000000 project-structure-0.8.27/bin/cz-check-bump
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1052 2023-05-05 14:54:58.000000 project-structure-0.8.27/bin/entrypoint
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1202 2023-05-05 14:54:58.000000 project-structure-0.8.27/bin/get-base-version
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)      422 2023-05-05 14:54:58.000000 project-structure-0.8.27/bin/hadolint
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.305920 project-structure-0.8.27/build-host/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2150 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/Dockerfile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1584 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/Makefile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      849 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/README.rst
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.305920 project-structure-0.8.27/build-host/bin/
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2152 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/bin/entrypoint
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      730 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/requirements-py310.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      673 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/requirements-py311.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      947 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/requirements-py37.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/requirements-py38.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/requirements-py39.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      104 2023-05-05 14:54:58.000000 project-structure-0.8.27/build-host/requirements.txt.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.305920 project-structure-0.8.27/dist/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      222 2023-05-05 14:54:58.000000 project-structure-0.8.27/dist/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5290 2023-05-05 14:54:58.000000 project-structure-0.8.27/docker-compose.override.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      741 2023-05-05 14:54:58.000000 project-structure-0.8.27/docker-compose.yml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.305920 project-structure-0.8.27/gitlab-runner/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.306920 project-structure-0.8.27/gitlab-runner/config/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1423 2023-05-05 14:54:58.000000 project-structure-0.8.27/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      666 2023-05-05 14:54:58.000000 project-structure-0.8.27/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.306920 project-structure-0.8.27/home/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      246 2023-05-05 14:54:58.000000 project-structure-0.8.27/home/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      427 2023-05-05 14:54:58.000000 project-structure-0.8.27/home/.pypirc.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.306920 project-structure-0.8.27/newsfragments/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      187 2023-05-05 14:54:58.000000 project-structure-0.8.27/newsfragments/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1862 2023-05-05 14:54:58.000000 project-structure-0.8.27/pyproject.toml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.306920 project-structure-0.8.27/requirements/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      679 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/build.txt.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.307920 project-structure-0.8.27/requirements/py310/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2383 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py310/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5053 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py310/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      257 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py310/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.308920 project-structure-0.8.27/requirements/py311/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2383 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py311/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4827 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py311/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      264 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py311/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.308920 project-structure-0.8.27/requirements/py37/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2660 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py37/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5501 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py37/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      399 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py37/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.309920 project-structure-0.8.27/requirements/py38/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2503 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py38/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5093 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py38/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py38/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.309920 project-structure-0.8.27/requirements/py39/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2381 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py39/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5080 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py39/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-05 14:54:58.000000 project-structure-0.8.27/requirements/py39/user.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1652 2023-05-05 14:56:43.316921 project-structure-0.8.27/setup.cfg
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.295919 project-structure-0.8.27/src/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.311921 project-structure-0.8.27/src/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/src/project_structure.egg-info/.gitignore
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17777 2023-05-05 14:56:43.000000 project-structure-0.8.27/src/project_structure.egg-info/PKG-INFO
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)     2460 2023-05-05 14:56:43.000000 project-structure-0.8.27/src/project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)        1 2023-05-05 14:56:43.000000 project-structure-0.8.27/src/project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)       60 2023-05-05 14:56:43.000000 project-structure-0.8.27/src/project_structure.egg-info/entry_points.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)      143 2023-05-05 14:56:43.000000 project-structure-0.8.27/src/project_structure.egg-info/requires.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)       17 2023-05-05 14:56:43.000000 project-structure-0.8.27/src/project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.311921 project-structure-0.8.27/src/projectstructure/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4356 2023-05-05 14:54:58.000000 project-structure-0.8.27/src/projectstructure/__init__.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      303 2023-05-05 14:54:58.000000 project-structure-0.8.27/src/projectstructure/__main__.py
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.312921 project-structure-0.8.27/src/projectstructure/tests/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      165 2023-05-05 14:54:58.000000 project-structure-0.8.27/src/projectstructure/tests/__init__.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4457 2023-05-05 14:54:58.000000 project-structure-0.8.27/src/projectstructure/tests/test_cli.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      495 2023-05-05 14:54:58.000000 project-structure-0.8.27/src/projectstructure/utils.py
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)      162 2023-05-05 14:56:43.000000 project-structure-0.8.27/src/projectstructure/version.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      281 2023-05-05 14:54:58.000000 project-structure-0.8.27/towncrier.toml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3306 2023-05-05 14:54:58.000000 project-structure-0.8.27/tox.ini
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.312921 project-structure-0.8.27/var/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.312921 project-structure-0.8.27/var-docker/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      229 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.312921 project-structure-0.8.27/var-docker/py310/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py310/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.312921 project-structure-0.8.27/var-docker/py310/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py310/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.313921 project-structure-0.8.27/var-docker/py310/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py310/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.313921 project-structure-0.8.27/var-docker/py311/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py311/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.313921 project-structure-0.8.27/var-docker/py311/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py311/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.313921 project-structure-0.8.27/var-docker/py311/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py311/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.313921 project-structure-0.8.27/var-docker/py37/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py37/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.314921 project-structure-0.8.27/var-docker/py37/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py37/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.314921 project-structure-0.8.27/var-docker/py37/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py37/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.314921 project-structure-0.8.27/var-docker/py38/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py38/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.314921 project-structure-0.8.27/var-docker/py38/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py38/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.314921 project-structure-0.8.27/var-docker/py38/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py38/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.314921 project-structure-0.8.27/var-docker/py39/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py39/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.315921 project-structure-0.8.27/var-docker/py39/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py39/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 14:56:43.315921 project-structure-0.8.27/var-docker/py39/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 14:54:58.000000 project-structure-0.8.27/var-docker/py39/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      821 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.cz.toml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      643 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.dir-locals.el.in
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1716 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.dockerignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1058 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.env.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.123400 project-structure-0.8.28b0/.github/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/.github/workflows/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4573 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1716 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     6288 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.gitlab-ci.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      877 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2471 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.prospector.yaml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/.reuse/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      790 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.reuse/dep5
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.tox/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5403 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2555 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/Dockerfile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3374 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/Dockerfile.devel
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/LICENSES/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1071 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/LICENSES/MIT.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    59098 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/Makefile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      140 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/NEWS-VERSION.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    13245 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/NEWS.rst
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17779 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/PKG-INFO
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    16758 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/README.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4388 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/TODO.rst
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/bin/
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2860 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/bin/cz-check-bump
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1052 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/bin/entrypoint
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1202 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/bin/get-base-version
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)      422 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/bin/hadolint
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/build-host/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2150 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/Dockerfile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1584 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/Makefile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      849 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/README.rst
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/build-host/bin/
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2152 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      730 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      673 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      947 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      104 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements.txt.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/dist/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      222 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/dist/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5290 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/docker-compose.override.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      741 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/docker-compose.yml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/gitlab-runner/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/gitlab-runner/config/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1423 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      666 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/home/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      246 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/home/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      427 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/home/.pypirc.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/newsfragments/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      187 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/newsfragments/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1862 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/pyproject.toml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      679 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/build.txt.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py310/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2383 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py310/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5053 2023-05-05 22:53:41.000000 project-structure-0.8.28b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      257 2023-05-05 22:53:31.000000 project-structure-0.8.28b0/requirements/py310/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py311/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2383 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py311/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4827 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      264 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py311/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py37/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2660 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py37/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5501 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      399 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py37/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py38/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2503 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py38/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5093 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py38/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py39/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2381 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py39/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5080 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py39/user.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1652 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/setup.cfg
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.123400 project-structure-0.8.28b0/src/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/src/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/project_structure.egg-info/.gitignore
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17779 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)     2460 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)        1 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)       60 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)      143 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/requires.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)       17 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/src/projectstructure/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4356 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/__init__.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      303 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/__main__.py
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/src/projectstructure/tests/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      165 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/tests/__init__.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4457 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/tests/test_cli.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      495 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/utils.py
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)      164 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/projectstructure/version.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      281 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/towncrier.toml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3306 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/tox.ini
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      229 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py310/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py310/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py310/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py310/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py310/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py310/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py311/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py311/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py311/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py311/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py311/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py311/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py37/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py37/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py37/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py37/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py37/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py37/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py38/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py38/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py38/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py38/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py38/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py38/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py39/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py39/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py39/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py39/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py39/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py39/project_structure.egg-info/.gitignore
```

### Comparing `project-structure-0.8.27/.cz.toml` & `project-structure-0.8.28b0/.cz.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.27"
+version = "0.8.28b0"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `project-structure-0.8.27/.dir-locals.el.in` & `project-structure-0.8.28b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/.dockerignore` & `project-structure-0.8.28b0/.dockerignore`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/.env.in` & `project-structure-0.8.28b0/.env.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/.github/workflows/build-test.yml` & `project-structure-0.8.28b0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/.gitignore` & `project-structure-0.8.28b0/.gitignore`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/.gitlab-ci.yml` & `project-structure-0.8.28b0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/.pre-commit-config.yaml` & `project-structure-0.8.28b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/.prospector.yaml` & `project-structure-0.8.28b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/.reuse/dep5` & `project-structure-0.8.28b0/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/CONTRIBUTING.rst` & `project-structure-0.8.28b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/Dockerfile` & `project-structure-0.8.28b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/Dockerfile.devel` & `project-structure-0.8.28b0/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/LICENSES/MIT.txt` & `project-structure-0.8.28b0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/Makefile` & `project-structure-0.8.28b0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -862,32 +862,33 @@
 # requirements again.
 	touch \
 	    $(PYTHON_ENVS:%=./requirements/%/user.txt) \
 	    $(PYTHON_ENVS:%=./requirements/%/devel.txt) \
 	    $(PYTHON_ENVS:%=./build-host/requirements-%.txt)
 ifeq ($(VCS_BRANCH),main)
 # Merge the bumped version back into `develop`:
-	bump_rev="$$(git rev-parse HEAD)"
-	git switch -C "develop" --track "$(VCS_COMPARE_REMOTE)/develop" --
-	git merge --ff --gpg-sign \
-	    -m "Merge branch 'main' release back into develop" "$${bump_rev}"
+	$(MAKE) VCS_BRANCH="main" VCS_MERGE_BRANCH="develop" \
+	    VCS_REMOTE="$(VCS_COMPARE_REMOTE)" VCS_MERGE_BRANCH="develop" devel-merge
 ifeq ($(CI),true)
-	git push --no-verify --tags "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
+	git push --no-verify "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
 endif
-	git switch -C "$(VCS_BRANCH)" "$${bump_rev}" --
+	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)" --
 endif
 ifneq ($(GITHUB_ACTIONS),true)
 ifneq ($(PROJECT_GITHUB_PAT),)
 # Ensure the tag is available for creating the GitHub release below but push *before* to
 # GitLab to avoid a race with repository mirrorying:
-	git push --no-verify --tags "github" "HEAD:$(VCS_BRANCH)"
+	git push --no-verify "github" tag "v$${next_version}"
 endif
 endif
 ifeq ($(CI),true)
-	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)"
+# Push just this tag to avoid clashes with any previously failed release:
+	git push --no-verify "$(VCS_REMOTE)" tag "v$${next_version}"
+# Also push the branch:
+	git push --no-verify "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)"
 endif
 
 
 ## Development Targets:
 #
 # Recipes used by developers to make changes to the code.
 
@@ -969,15 +970,15 @@
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_MERGE_BRANCH)
 	merge_rev="$$(git rev-parse HEAD)"
 	git switch -C "$(VCS_MERGE_BRANCH)" --track "$(VCS_REMOTE)/$(VCS_MERGE_BRANCH)"
 	git merge --ff --gpg-sign -m \
 	    $$'Merge branch \'$(VCS_BRANCH)\' into $(VCS_MERGE_BRANCH)\n\n[ci merge]' \
 	    "$${merge_rev}"
 ifeq ($(CI),true)
-	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:$(VCS_MERGE_BRANCH)"
+	git push --no-verify "$(VCS_REMOTE)" "HEAD:$(VCS_MERGE_BRANCH)"
 endif
 
 
 ## Clean Targets:
 #
 # Recipes used to restore the checkout to initial conditions.
 
@@ -1270,15 +1271,15 @@
 	set +x
 	echo "ERROR: PROJECT_GITHUB_PAT missing from ./.env or CI secrets"
 	false
 endif
 endif
 	set -x
 # Fail fast if there's still no push access
-	git push --no-verify --tags "origin" | tee -a "$(@)"
+	git push --no-verify "origin" "HEAD:$(VCS_BRANCH)" | tee -a "$(@)"
 
 # Ensure release publishing authentication, mostly useful in automation such as CI.
 ~/.pypirc: ./home/.pypirc.in
 	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
 
 ./var/log/docker-login-DOCKER.log: ./.env
 	mkdir -pv "$(dir $(@))"
```

### Comparing `project-structure-0.8.27/NEWS.rst` & `project-structure-0.8.28b0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+project-structure 0.8.28b0 (2023-05-05)
+=======================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
 project-structure 0.8.27 (2023-05-05)
 =====================================
 
 Bugfixes
 --------
 
 - Simulate a patch release. (simulate)
```

### Comparing `project-structure-0.8.27/PKG-INFO` & `project-structure-0.8.28b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-structure
-Version: 0.8.27
+Version: 0.8.28b0
 Summary: Project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `project-structure-0.8.27/README.rst` & `project-structure-0.8.28b0/README.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/TODO.rst` & `project-structure-0.8.28b0/TODO.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/bin/cz-check-bump` & `project-structure-0.8.28b0/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/bin/entrypoint` & `project-structure-0.8.28b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/bin/get-base-version` & `project-structure-0.8.28b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/build-host/Dockerfile` & `project-structure-0.8.28b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/build-host/Makefile` & `project-structure-0.8.28b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/build-host/README.rst` & `project-structure-0.8.28b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/build-host/bin/entrypoint` & `project-structure-0.8.28b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/build-host/requirements-py310.txt` & `project-structure-0.8.28b0/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/build-host/requirements-py311.txt` & `project-structure-0.8.28b0/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/build-host/requirements-py37.txt` & `project-structure-0.8.28b0/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/build-host/requirements-py38.txt` & `project-structure-0.8.28b0/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/build-host/requirements-py39.txt` & `project-structure-0.8.28b0/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/docker-compose.override.yml` & `project-structure-0.8.28b0/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/docker-compose.yml` & `project-structure-0.8.28b0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/gitlab-runner/config/config.toml.in` & `project-structure-0.8.28b0/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/gitlab-runner/docker-compose.yml` & `project-structure-0.8.28b0/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/pyproject.toml` & `project-structure-0.8.28b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/build.txt.in` & `project-structure-0.8.28b0/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py310/build.txt` & `project-structure-0.8.28b0/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py310/devel.txt` & `project-structure-0.8.28b0/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py311/build.txt` & `project-structure-0.8.28b0/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py311/devel.txt` & `project-structure-0.8.28b0/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py37/build.txt` & `project-structure-0.8.28b0/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py37/devel.txt` & `project-structure-0.8.28b0/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py38/build.txt` & `project-structure-0.8.28b0/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py38/devel.txt` & `project-structure-0.8.28b0/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py39/build.txt` & `project-structure-0.8.28b0/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/requirements/py39/devel.txt` & `project-structure-0.8.28b0/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/setup.cfg` & `project-structure-0.8.28b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/src/project_structure.egg-info/PKG-INFO` & `project-structure-0.8.28b0/src/project_structure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-structure
-Version: 0.8.27
+Version: 0.8.28b0
 Summary: Project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `project-structure-0.8.27/src/project_structure.egg-info/SOURCES.txt` & `project-structure-0.8.28b0/src/project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/src/projectstructure/__init__.py` & `project-structure-0.8.28b0/src/projectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/src/projectstructure/tests/test_cli.py` & `project-structure-0.8.28b0/src/projectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.27/tox.ini` & `project-structure-0.8.28b0/tox.ini`

 * *Files identical despite different names*

