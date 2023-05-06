# Comparing `tmp/kopf-1.36.0.tar.gz` & `tmp/kopf-1.36.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kopf-1.36.0.tar", last modified: Fri Nov  4 15:53:54 2022, max compression
+gzip compressed data, was "kopf-1.36.1.tar", last modified: Sat May  6 17:02:19 2023, max compression
```

## Comparing `kopf-1.36.0.tar` & `kopf-1.36.1.tar`

### file list

```diff
@@ -1,473 +1,475 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.329904 kopf-1.36.0/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-04 15:53:43.000000 kopf-1.36.0/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.293904 kopf-1.36.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.293904 kopf-1.36.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/ISSUE_TEMPLATE/bug-report.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/ISSUE_TEMPLATE/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/ISSUE_TEMPLATE/feature-request.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/ISSUE_TEMPLATE/question.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.293904 kopf-1.36.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5097 2022-11-04 15:53:43.000000 kopf-1.36.0/.github/workflows/thorough.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-11-04 15:53:43.000000 kopf-1.36.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-11-04 15:53:43.000000 kopf-1.36.0/.importlinter
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-04 15:53:43.000000 kopf-1.36.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-11-04 15:53:43.000000 kopf-1.36.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2022-11-04 15:53:43.000000 kopf-1.36.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-11-04 15:53:43.000000 kopf-1.36.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-11-04 15:53:43.000000 kopf-1.36.0/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     3973 2022-11-04 15:53:43.000000 kopf-1.36.0/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-11-04 15:53:43.000000 kopf-1.36.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-04 15:53:43.000000 kopf-1.36.0/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (121)     9006 2022-11-04 15:53:54.329904 kopf-1.36.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7612 2022-11-04 15:53:43.000000 kopf-1.36.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-04 15:53:43.000000 kopf-1.36.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-11-04 15:53:43.000000 kopf-1.36.0/_importlinter_conditional.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (121)    30976 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/admission.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5034 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/alternatives.rst
--rw-r--r--   0 runner    (1001) docker     (121)   815980 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/architecture-layers.png
--rw-r--r--   0 runner    (1001) docker     (121)     6656 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/architecture-layers.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5384 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/async.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7474 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    21375 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/continuity.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13470 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/daemons.rst
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/deployment-depl.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/deployment-rbac.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5143 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4470 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3677 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12679 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/filters.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10116 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/handlers.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12768 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/hierarchies.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/idempotence.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    19300 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/indexing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11998 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/kwargs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/loading.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5561 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/memos.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/minikube.rst
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/naming.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6472 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/peering.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/probing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/reconciliation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7396 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/results.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/scopes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/shutdown.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/startup.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6679 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/timers.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/tips-and-tricks.rst
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/vision.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/docs/walkthrough/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/walkthrough/cleanup.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2605 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/walkthrough/creation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/walkthrough/deletion.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4314 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/walkthrough/diffs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/walkthrough/prerequisites.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3015 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/walkthrough/problem.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/walkthrough/resources.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6290 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/walkthrough/starting.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-11-04 15:53:43.000000 kopf-1.36.0/docs/walkthrough/updates.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/01-minimal/
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/01-minimal/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/01-minimal/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/02-children/
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/02-children/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/02-children/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/03-exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/03-exceptions/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/03-exceptions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/04-events/
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/04-events/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/04-events/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/05-handlers/
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/05-handlers/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/05-handlers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/06-peering/
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/06-peering/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/06-peering/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/07-subhandlers/
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/07-subhandlers/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/07-subhandlers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/08-events/
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/08-events/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/08-events/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/09-testing/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/09-testing/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/09-testing/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/09-testing/test_example_09.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.301904 kopf-1.36.0/examples/10-builtins/
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/10-builtins/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/10-builtins/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/10-builtins/test_example_10.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/examples/11-filtering-handlers/
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/11-filtering-handlers/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/11-filtering-handlers/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/11-filtering-handlers/test_example_11.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/examples/12-embedded/
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/12-embedded/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/12-embedded/example.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/12-embedded/test_nothing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/examples/13-hooks/
--rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/13-hooks/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/13-hooks/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/examples/14-daemons/
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/14-daemons/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/examples/15-timers/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/15-timers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/examples/16-indexing/
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/16-indexing/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/examples/17-admission/
--rw-r--r--   0 runner    (1001) docker     (121)     3902 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/17-admission/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/examples/99-all-at-once/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/99-all-at-once/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/99-all-at-once/example.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/crd.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/obj.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-04 15:53:43.000000 kopf-1.36.0/examples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/kopf/
--rw-r--r--   0 runner    (1001) docker     (121)     5798 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/kopf/_cogs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/kopf/_cogs/aiokits/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/aiokits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/aiokits/aioadapters.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/aiokits/aiobindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     7544 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/aiokits/aioenums.py
--rw-r--r--   0 runner    (1001) docker     (121)    16283 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/aiokits/aiotasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/aiokits/aiotime.py
--rw-r--r--   0 runner    (1001) docker     (121)     5412 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/aiokits/aiotoggles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/aiokits/aiovalues.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/kopf/_cogs/clients/
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8911 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     8068 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/creating.py
--rw-r--r--   0 runner    (1001) docker     (121)     4603 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/fetching.py
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/patching.py
--rw-r--r--   0 runner    (1001) docker     (121)     4479 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/scanning.py
--rw-r--r--   0 runner    (1001) docker     (121)    10991 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/clients/watching.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.309904 kopf-1.36.0/kopf/_cogs/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16282 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/configs/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    13196 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/configs/conventions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9210 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/configs/diffbase.py
--rw-r--r--   0 runner    (1001) docker     (121)    15586 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/configs/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.309904 kopf-1.36.0/kopf/_cogs/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/helpers/hostnames.py
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/helpers/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/helpers/thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/helpers/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/helpers/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.309904 kopf-1.36.0/kopf/_cogs/structs/
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8109 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/bodies.py
--rw-r--r--   0 runner    (1001) docker     (121)    16065 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)    11883 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/dicts.py
--rw-r--r--   0 runner    (1001) docker     (121)     6222 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/diffs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2716 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/ephemera.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/finalizers.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/ids.py
--rw-r--r--   0 runner    (1001) docker     (121)     3894 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/patches.py
--rw-r--r--   0 runner    (1001) docker     (121)    22210 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/references.py
--rw-r--r--   0 runner    (1001) docker     (121)     3752 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_cogs/structs/reviews.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.309904 kopf-1.36.0/kopf/_core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.309904 kopf-1.36.0/kopf/_core/actions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6146 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/actions/application.py
--rw-r--r--   0 runner    (1001) docker     (121)    15011 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/actions/execution.py
--rw-r--r--   0 runner    (1001) docker     (121)     5979 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/actions/invocation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/actions/lifecycles.py
--rw-r--r--   0 runner    (1001) docker     (121)     8399 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/actions/loggers.py
--rw-r--r--   0 runner    (1001) docker     (121)    15223 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/actions/progression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3486 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/actions/throttlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.309904 kopf-1.36.0/kopf/_core/engines/
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5628 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/engines/activities.py
--rw-r--r--   0 runner    (1001) docker     (121)    19689 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/engines/admission.py
--rw-r--r--   0 runner    (1001) docker     (121)    25971 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/engines/daemons.py
--rw-r--r--   0 runner    (1001) docker     (121)    12315 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/engines/indexing.py
--rw-r--r--   0 runner    (1001) docker     (121)    12396 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/engines/peering.py
--rw-r--r--   0 runner    (1001) docker     (121)     8534 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/engines/posting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/engines/probing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.313904 kopf-1.36.0/kopf/_core/intents/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/intents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10586 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/intents/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)    11464 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/intents/causes.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/intents/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/intents/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10892 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/intents/piggybacking.py
--rw-r--r--   0 runner    (1001) docker     (121)    21818 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/intents/registries.py
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/intents/stoppers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.313904 kopf-1.36.0/kopf/_core/reactor/
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/reactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/reactor/inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)    15421 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/reactor/observation.py
--rw-r--r--   0 runner    (1001) docker     (121)    11714 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/reactor/orchestration.py
--rw-r--r--   0 runner    (1001) docker     (121)    20921 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/reactor/processing.py
--rw-r--r--   0 runner    (1001) docker     (121)    16941 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/reactor/queueing.py
--rw-r--r--   0 runner    (1001) docker     (121)    24302 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/reactor/running.py
--rw-r--r--   0 runner    (1001) docker     (121)     6920 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_core/reactor/subhandling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.313904 kopf-1.36.0/kopf/_kits/
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_kits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11261 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_kits/hierarchies.py
--rw-r--r--   0 runner    (1001) docker     (121)     6247 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_kits/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3896 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_kits/webhacks.py
--rw-r--r--   0 runner    (1001) docker     (121)    30171 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/_kits/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     7326 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    42263 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/on.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-04 15:53:43.000000 kopf-1.36.0/kopf/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.305904 kopf-1.36.0/kopf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9006 2022-11-04 15:53:54.000000 kopf-1.36.0/kopf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12368 2022-11-04 15:53:54.000000 kopf-1.36.0/kopf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 15:53:54.000000 kopf-1.36.0/kopf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-04 15:53:54.000000 kopf-1.36.0/kopf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-11-04 15:53:54.000000 kopf-1.36.0/kopf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-04 15:53:54.000000 kopf-1.36.0/kopf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 15:53:54.000000 kopf-1.36.0/kopf.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-04 15:53:43.000000 kopf-1.36.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-11-04 15:53:43.000000 kopf-1.36.0/peering.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-04 15:53:43.000000 kopf-1.36.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-11-04 15:53:43.000000 kopf-1.36.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 15:53:54.329904 kopf-1.36.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-11-04 15:53:43.000000 kopf-1.36.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.313904 kopf-1.36.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.313904 kopf-1.36.0/tests/admission/
--rw-r--r--   0 runner    (1001) docker     (121)     4592 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8408 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_admission_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_admission_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_certificates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_jsonpatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     9185 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_managed_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_serving_ephemeral_memos.py
--rw-r--r--   0 runner    (1001) docker     (121)     7830 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_serving_handler_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_serving_kwargs_passthrough.py
--rw-r--r--   0 runner    (1001) docker     (121)     6849 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_serving_responses.py
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_webhook_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_webhook_ngrok.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/admission/test_webhook_server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.313904 kopf-1.36.0/tests/apis/
--rw-r--r--   0 runner    (1001) docker     (121)     9968 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/apis/test_api_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/apis/test_default_namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     9346 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/apis/test_error_retries.py
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/apis/test_iterjsonlines.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.317904 kopf-1.36.0/tests/authentication/
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/authentication/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/authentication/test_connectioninfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     8916 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/authentication/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)    10189 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/authentication/test_login_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/authentication/test_login_serviceaccount.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/authentication/test_reauthentication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/authentication/test_tempfiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     7474 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/authentication/test_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.317904 kopf-1.36.0/tests/basic-structs/
--rw-r--r--   0 runner    (1001) docker     (121)     3317 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/basic-structs/test_causes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/basic-structs/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/basic-structs/test_memories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/basic-structs/test_memos.py
--rw-r--r--   0 runner    (1001) docker     (121)    11433 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/basic-structs/test_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.317904 kopf-1.36.0/tests/causation/
--rw-r--r--   0 runner    (1001) docker     (121)     8417 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/causation/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)    12825 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/causation/test_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.317904 kopf-1.36.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/cli/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/cli/test_help.py
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/cli/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     2590 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/cli/test_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/cli/test_preloading.py
--rw-r--r--   0 runner    (1001) docker     (121)    24367 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.317904 kopf-1.36.0/tests/dicts/
--rw-r--r--   0 runner    (1001) docker     (121)     3345 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/dicts/test_cherrypicking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5085 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/dicts/test_dictviews.py
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/dicts/test_ensuring.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/dicts/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/dicts/test_removing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5402 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/dicts/test_resolving.py
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/dicts/test_walking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.317904 kopf-1.36.0/tests/diffs/
--rw-r--r--   0 runner    (1001) docker     (121)     5355 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/diffs/test_calculation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/diffs/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)     2692 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/diffs/test_reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.317904 kopf-1.36.0/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     9649 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/e2e/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.317904 kopf-1.36.0/tests/handling/
--rw-r--r--   0 runner    (1001) docker     (121)     7457 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/handling/daemons/
--rw-r--r--   0 runner    (1001) docker     (121)     3893 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/test_daemon_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/test_daemon_filtration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/test_daemon_rematching.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/test_daemon_spawning.py
--rw-r--r--   0 runner    (1001) docker     (121)    10261 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/test_daemon_termination.py
--rw-r--r--   0 runner    (1001) docker     (121)     6267 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/test_timer_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/test_timer_filtration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/test_timer_intervals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/daemons/test_timer_triggering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/handling/indexing/
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/indexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/indexing/test_blocking_until_indexed.py
--rw-r--r--   0 runner    (1001) docker     (121)     8776 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/indexing/test_index_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (121)     4899 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/indexing/test_index_population.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/handling/subhandling/
--rw-r--r--   0 runner    (1001) docker     (121)     5369 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/subhandling/test_subhandling.py
--rw-r--r--   0 runner    (1001) docker     (121)     6167 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_activity_triggering.py
--rw-r--r--   0 runner    (1001) docker     (121)     7416 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_cause_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)     5422 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_cause_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     5098 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_delays.py
--rw-r--r--   0 runner    (1001) docker     (121)     6120 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_event_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)     4818 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_multistep.py
--rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_no_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_parametrization.py
--rw-r--r--   0 runner    (1001) docker     (121)     4017 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_retrying_limits.py
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/handling/test_timing_consistency.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/hierarchies/
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/hierarchies/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4710 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/hierarchies/test_contextual_owner.py
--rw-r--r--   0 runner    (1001) docker     (121)     9396 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/hierarchies/test_labelling.py
--rw-r--r--   0 runner    (1001) docker     (121)    11783 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/hierarchies/test_name_harmonizing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5895 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/hierarchies/test_namespace_adjusting.py
--rw-r--r--   0 runner    (1001) docker     (121)    10983 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/hierarchies/test_owner_referencing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/hierarchies/test_type_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/invocations/
--rw-r--r--   0 runner    (1001) docker     (121)     5298 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/invocations/test_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/k8s/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_creating.py
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     5785 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_list_objs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9822 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_patching.py
--rw-r--r--   0 runner    (1001) docker     (121)    13308 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_scanning.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_watching_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (121)     7215 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_watching_continuously.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_watching_infinitely.py
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/k8s/test_watching_with_freezes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/lifecycles/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/lifecycles/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/lifecycles/test_global_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     3691 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/lifecycles/test_handler_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/lifecycles/test_real_invocation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/logging/
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/logging/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/logging/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4659 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/logging/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/logging/test_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/observation/
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/observation/test_processing_of_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     8696 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/observation/test_processing_of_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     3229 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/observation/test_revision_of_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     8314 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/observation/test_revision_of_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.321904 kopf-1.36.0/tests/orchestration/
--rw-r--r--   0 runner    (1001) docker     (121)     8535 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/orchestration/test_task_adjustments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.325904 kopf-1.36.0/tests/peering/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/peering/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    11445 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/peering/test_freeze_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     4300 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/peering/test_id_generation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/peering/test_keepalive.py
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/peering/test_peer_patching.py
--rw-r--r--   0 runner    (1001) docker     (121)     2723 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/peering/test_peers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/peering/test_resource_guessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.325904 kopf-1.36.0/tests/persistence/
--rw-r--r--   0 runner    (1001) docker     (121)     7354 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/persistence/test_annotations_hashing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5597 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/persistence/test_essences.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/persistence/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (121)    33099 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/persistence/test_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     6181 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/persistence/test_storing_of_diffbase.py
--rw-r--r--   0 runner    (1001) docker     (121)    12624 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/persistence/test_storing_of_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.325904 kopf-1.36.0/tests/posting/
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/posting/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4163 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/posting/test_log2k8s.py
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/posting/test_poster.py
--rw-r--r--   0 runner    (1001) docker     (121)     3613 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/posting/test_threadsafety.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.325904 kopf-1.36.0/tests/primitives/
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/primitives/test_conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/primitives/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/primitives/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/primitives/test_toggles.py
--rw-r--r--   0 runner    (1001) docker     (121)     9213 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/primitives/test_togglesets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.325904 kopf-1.36.0/tests/reactor/
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/reactor/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5877 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/reactor/test_patching_inconsistencies.py
--rw-r--r--   0 runner    (1001) docker     (121)    10090 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/reactor/test_queueing.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/reactor/test_uids.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.325904 kopf-1.36.0/tests/references/
--rw-r--r--   0 runner    (1001) docker     (121)     3005 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/references/test_backbone.py
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/references/test_namespace_matching.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/references/test_namespace_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     7038 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/references/test_selector_matching.py
--rw-r--r--   0 runner    (1001) docker     (121)     8577 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/references/test_selector_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/references/test_selector_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.329904 kopf-1.36.0/tests/registries/
--rw-r--r--   0 runner    (1001) docker     (121)     6122 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (121)    23936 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_default_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     6008 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_handler_getting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_id_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)    29042 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_matching_for_changing.py
--rw-r--r--   0 runner    (1001) docker     (121)    17256 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_matching_for_indexing.py
--rw-r--r--   0 runner    (1001) docker     (121)    17724 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_matching_for_spawning.py
--rw-r--r--   0 runner    (1001) docker     (121)    17312 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_matching_for_watching.py
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_matching_of_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_matching_of_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_requires_finalizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2184 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_resumes_mixed_in.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/registries/test_subhandlers_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.329904 kopf-1.36.0/tests/settings/
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/settings/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/settings/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/test_absent_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/test_filtering_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/test_finalizers.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/test_it.py
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/test_liveness.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/test_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/test_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.329904 kopf-1.36.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/testing/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.329904 kopf-1.36.0/tests/timing/
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/timing/test_sleeping.py
--rw-r--r--   0 runner    (1001) docker     (121)    11112 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/timing/test_throttling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.293904 kopf-1.36.0/tests/utilities/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.329904 kopf-1.36.0/tests/utilities/aiotasks/
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/utilities/aiotasks/test_coro_cancellation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5145 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/utilities/aiotasks/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/utilities/aiotasks/test_task_creation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/utilities/aiotasks/test_task_guarding.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/utilities/aiotasks/test_task_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3725 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/utilities/aiotasks/test_task_stopping.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-04 15:53:43.000000 kopf-1.36.0/tests/utilities/aiotasks/test_task_waiting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 15:53:54.329904 kopf-1.36.0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (121)      717 2022-11-04 15:53:43.000000 kopf-1.36.0/tools/install-kind.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      504 2022-11-04 15:53:43.000000 kopf-1.36.0/tools/install-kubectl.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      945 2022-11-04 15:53:43.000000 kopf-1.36.0/tools/install-minikube.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.741712 kopf-1.36.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-06 17:02:08.000000 kopf-1.36.1/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.689712 kopf-1.36.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.689712 kopf-1.36.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE/bug-report.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE/feature-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE/question.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.689712 kopf-1.36.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     4336 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/workflows/thorough.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-05-06 17:02:08.000000 kopf-1.36.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-05-06 17:02:08.000000 kopf-1.36.1/.importlinter
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-06 17:02:08.000000 kopf-1.36.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-06 17:02:08.000000 kopf-1.36.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-05-06 17:02:08.000000 kopf-1.36.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-05-06 17:02:08.000000 kopf-1.36.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-05-06 17:02:08.000000 kopf-1.36.1/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-05-06 17:02:08.000000 kopf-1.36.1/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-06 17:02:08.000000 kopf-1.36.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-06 17:02:08.000000 kopf-1.36.1/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     9006 2023-05-06 17:02:19.741712 kopf-1.36.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7612 2023-05-06 17:02:08.000000 kopf-1.36.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-06 17:02:08.000000 kopf-1.36.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-05-06 17:02:08.000000 kopf-1.36.1/_importlinter_conditional.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (122)    30976 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/admission.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5034 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/alternatives.rst
+-rw-r--r--   0 runner    (1001) docker     (122)   815980 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/architecture-layers.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6656 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/architecture-layers.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     5384 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/async.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7474 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3295 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2728 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21375 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/continuity.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4318 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13470 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/daemons.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/deployment-depl.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/deployment-rbac.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5143 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12679 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10116 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12768 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/hierarchies.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/idempotence.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    19300 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/indexing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12007 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/kwargs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/loading.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/memos.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/minikube.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/naming.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6472 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/peering.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3244 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/probing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/reconciliation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7396 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/results.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/scopes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/shutdown.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/startup.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/timers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/tips-and-tricks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/vision.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/docs/walkthrough/
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/cleanup.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/creation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2458 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/deletion.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4314 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/diffs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/prerequisites.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3015 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/problem.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6290 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/starting.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/updates.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/01-minimal/
+-rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/01-minimal/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/01-minimal/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/02-children/
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/02-children/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      987 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/02-children/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/03-exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/03-exceptions/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/03-exceptions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/04-events/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/04-events/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/04-events/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/05-handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/05-handlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/05-handlers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/06-peering/
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/06-peering/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/06-peering/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/07-subhandlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/07-subhandlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/07-subhandlers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/08-events/
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/08-events/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/08-events/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/09-testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/09-testing/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/09-testing/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2217 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/09-testing/test_example_09.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/10-builtins/
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/10-builtins/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/10-builtins/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/10-builtins/test_example_10.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/11-filtering-handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/11-filtering-handlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/11-filtering-handlers/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/11-filtering-handlers/test_example_11.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/12-embedded/
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/12-embedded/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/12-embedded/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/12-embedded/test_nothing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/13-hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)     3494 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/13-hooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/13-hooks/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/14-daemons/
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/14-daemons/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/15-timers/
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/15-timers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/16-indexing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/16-indexing/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/17-admission/
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/17-admission/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/99-all-at-once/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/99-all-at-once/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/99-all-at-once/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/crd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/obj.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.705712 kopf-1.36.1/kopf/
+-rw-r--r--   0 runner    (1001) docker     (122)     5798 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.705712 kopf-1.36.1/kopf/_cogs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.705712 kopf-1.36.1/kopf/_cogs/aiokits/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aioadapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiobindings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7613 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aioenums.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16483 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiotasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiotime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5412 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiotoggles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiovalues.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_cogs/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8911 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8087 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/creating.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/fetching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4479 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/scanning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11684 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/watching.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_cogs/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16266 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13196 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9210 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/diffbase.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15586 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_cogs/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1672 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_cogs/structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8109 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/bodies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16065 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12021 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6222 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/ephemera.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/finalizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/patches.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22210 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/references.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/reviews.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.713712 kopf-1.36.1/kopf/_core/actions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6146 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/application.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14779 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/execution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5963 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/invocation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/lifecycles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8220 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15223 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/progression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3486 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/throttlers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.713712 kopf-1.36.1/kopf/_core/engines/
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5628 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/activities.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19689 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/admission.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26590 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/daemons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12333 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12443 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/peering.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8534 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/posting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/probing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.713712 kopf-1.36.1/kopf/_core/intents/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10586 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11464 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/causes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10892 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/piggybacking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21818 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/registries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/stoppers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.713712 kopf-1.36.1/kopf/_core/reactor/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15421 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/observation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11714 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20921 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/processing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17116 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/queueing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24225 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/running.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/subhandling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.717712 kopf-1.36.1/kopf/_kits/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11261 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/hierarchies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/loops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6247 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/webhacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30289 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42263 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/on.py
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.705712 kopf-1.36.1/kopf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9006 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12417 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-06 17:02:08.000000 kopf-1.36.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-05-06 17:02:08.000000 kopf-1.36.1/peering.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-06 17:02:08.000000 kopf-1.36.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-06 17:02:08.000000 kopf-1.36.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-06 17:02:19.741712 kopf-1.36.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-05-06 17:02:08.000000 kopf-1.36.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.717712 kopf-1.36.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.717712 kopf-1.36.1/tests/admission/
+-rw-r--r--   0 runner    (1001) docker     (122)     4592 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8414 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_admission_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3009 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_admission_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_jsonpatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9185 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_managed_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_serving_ephemeral_memos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7830 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_serving_handler_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_serving_kwargs_passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6849 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_serving_responses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_webhook_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_webhook_ngrok.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5264 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_webhook_server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)    10028 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/apis/test_api_requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/apis/test_default_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9346 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/apis/test_error_retries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/apis/test_iterjsonlines.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/authentication/
+-rw-r--r--   0 runner    (1001) docker     (122)     2429 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_connectioninfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8916 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10189 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_login_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3488 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_login_serviceaccount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_reauthentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_tempfiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7474 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/basic-structs/
+-rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_causes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2892 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_memories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1858 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_memos.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11433 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/causation/
+-rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/causation/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/causation/test_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     1527 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/test_preloading.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24579 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/dicts/
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_cherrypicking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5085 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_dictviews.py
+-rw-r--r--   0 runner    (1001) docker     (122)      953 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_ensuring.py
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_removing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5402 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_resolving.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_walking.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/diffs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/diffs/test_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/diffs/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/diffs/test_reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9649 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/e2e/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/handling/
+-rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/handling/daemons/
+-rw-r--r--   0 runner    (1001) docker     (122)     3893 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5763 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_filtration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_rematching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_spawning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10261 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_termination.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6267 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_timer_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_timer_filtration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_timer_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_timer_triggering.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/handling/indexing/
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/indexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3817 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/indexing/test_blocking_until_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8776 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/indexing/test_index_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4899 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/indexing/test_index_population.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/handling/subhandling/
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/subhandling/test_subhandling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_activity_triggering.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7416 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_cause_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5422 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_cause_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_delays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6120 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4818 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_multistep.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_no_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1879 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_parametrization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_retrying_limits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_timing_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/hierarchies/
+-rw-r--r--   0 runner    (1001) docker     (122)      916 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_contextual_owner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9396 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_labelling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11783 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_name_harmonizing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5895 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_namespace_adjusting.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10983 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_owner_referencing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_type_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)     5298 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/invocations/test_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/k8s/
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_creating.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3882 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5785 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_list_objs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9822 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13308 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_scanning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_watching_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_watching_continuously.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_watching_infinitely.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_watching_with_freezes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/lifecycles/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/lifecycles/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/lifecycles/test_global_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3691 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/lifecycles/test_handler_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/lifecycles/test_real_invocation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/logging/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/logging/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/logging/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/logging/test_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/observation/
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/observation/test_processing_of_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/observation/test_processing_of_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/observation/test_revision_of_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8324 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/observation/test_revision_of_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/orchestration/
+-rw-r--r--   0 runner    (1001) docker     (122)     8535 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/orchestration/test_task_adjustments.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/peering/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11445 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_freeze_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_id_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_keepalive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_peer_patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_peers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_resource_guessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/persistence/
+-rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_annotations_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5597 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_essences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33091 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_storing_of_diffbase.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12624 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_storing_of_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/posting/
+-rw-r--r--   0 runner    (1001) docker     (122)      485 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/posting/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4163 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/posting/test_log2k8s.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/posting/test_poster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3613 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/posting/test_threadsafety.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2783 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_toggles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9213 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_togglesets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/reactor/
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/reactor/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5877 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/reactor/test_patching_inconsistencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10090 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/reactor/test_queueing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/reactor/test_uids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/references/
+-rw-r--r--   0 runner    (1001) docker     (122)     3005 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_namespace_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_namespace_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7038 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_selector_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8577 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_selector_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_selector_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/registries/
+-rw-r--r--   0 runner    (1001) docker     (122)     6122 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23936 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_default_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6010 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_handler_getting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_id_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29077 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_for_changing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17265 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_for_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17733 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_for_spawning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17321 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_for_watching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_of_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_of_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_requires_finalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_resumes_mixed_in.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_subhandlers_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/settings/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/settings/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_absent_modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_filtering_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_finalizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_it.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_liveness.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/testing/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.741712 kopf-1.36.1/tests/timing/
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/timing/test_sleeping.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11112 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/timing/test_throttling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.685712 kopf-1.36.1/tests/utilities/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.741712 kopf-1.36.1/tests/utilities/aiotasks/
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_coro_cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_creation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_guarding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_waiting.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.741712 kopf-1.36.1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      717 2023-05-06 17:02:08.000000 kopf-1.36.1/tools/install-kind.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      504 2023-05-06 17:02:08.000000 kopf-1.36.1/tools/install-kubectl.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      945 2023-05-06 17:02:08.000000 kopf-1.36.1/tools/install-minikube.sh
```

### Comparing `kopf-1.36.0/.github/ISSUE_TEMPLATE/bug-report.yaml` & `kopf-1.36.1/.github/ISSUE_TEMPLATE/bug-report.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/.github/ISSUE_TEMPLATE/feature-request.yaml` & `kopf-1.36.1/.github/ISSUE_TEMPLATE/feature-request.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/.github/ISSUE_TEMPLATE/question.yaml` & `kopf-1.36.1/.github/ISSUE_TEMPLATE/question.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/.github/workflows/ci.yaml` & `kopf-1.36.1/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         if: ${{ matrix.install-extras }}
       - run: pytest --color=yes --timeout=2 --no-cov
 
   functional:
     strategy:
       fail-fast: false
       matrix:
-        k3s: [latest, v1.24, v1.23, v1.22]
+        k3s: [latest, v1.26, v1.25, v1.24, v1.23]
     name: K3s ${{matrix.k3s}}
     runs-on: ubuntu-22.04
     timeout-minutes: 10  # usually 4-5 mins
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
```

### Comparing `kopf-1.36.0/.github/workflows/publish.yaml` & `kopf-1.36.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/.github/workflows/thorough.yaml` & `kopf-1.36.1/.github/workflows/thorough.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         if: ${{ matrix.install-extras }}
       - run: pytest --color=yes --timeout=2 --no-cov
 
   functional:
     strategy:
       fail-fast: false
       matrix:
-        k3s: [latest, v1.24, v1.23, v1.22]
+        k3s: [latest, v1.26, v1.25, v1.24, v1.23]
     name: K3s ${{matrix.k3s}}
     runs-on: ubuntu-22.04
     timeout-minutes: 10  # usually 4-5 mins
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
@@ -123,15 +123,15 @@
       - run: pip install -r requirements.txt -r examples/requirements.txt
       - run: pytest --color=yes --timeout=30 --only-e2e
 
   full-scale:
     strategy:
       fail-fast: false
       matrix:
-        k8s: [latest, v1.24.6, v1.23.12, v1.22.15]
+        k8s: [latest, v1.26.4, v1.25.9, v1.24.13, v1.23.17]
     name: K8s ${{matrix.k8s}}
     runs-on: ubuntu-22.04
     timeout-minutes: 10  # usually 4-5 mins
     env:
       K8S: ${{ matrix.k8s }}
     steps:
       - uses: actions/checkout@v3
```

### Comparing `kopf-1.36.0/.importlinter` & `kopf-1.36.1/.importlinter`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/.pre-commit-config.yaml` & `kopf-1.36.1/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 exclude: |
   (?x)^(
     docs/.*\.xml|
     docs/.*\.png
   )
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.4.0
+    rev: v4.4.0
     hooks:
       - id: check-ast
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: fix-byte-order-marker
       - id: check-xml
       - id: check-toml
@@ -42,47 +42,47 @@
         args: [--django]
       - id: requirements-txt-fixer
 
       # Intentionally disabled:
       # - id: double-quote-string-fixer
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.8.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
       - id: python-check-mock-methods
       - id: python-no-eval
       - id: python-use-type-annotations
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
       - id: text-unicode-replacement-char
 
       # Intentionally disabled:
       # - id: python-no-log-warn  # overreacts to `kopf.warn()`.
 
   - repo: https://github.com/seddonym/import-linter
-    rev: v1.2.1
+    rev: v1.7.0
     hooks:
       - id: import-linter
         additional_dependencies:
           - astpath[xpath]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.8.0
+    rev: 5.12.0
     hooks:
       - id: isort
         name: isort-source-code
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.8.0
+    rev: 5.12.0
     hooks:
       - id: isort
         name: isort-examples
         args: [--settings=examples]
         files: '^examples/'
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.34.0
+    rev: v3.3.1
     hooks:
     -   id: pyupgrade
         args: [--py37-plus, --keep-mock]
```

### Comparing `kopf-1.36.0/CODE_OF_CONDUCT.md` & `kopf-1.36.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/CONTRIBUTING.md` & `kopf-1.36.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/CONTRIBUTORS.md` & `kopf-1.36.1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/DEVELOPMENT.md` & `kopf-1.36.1/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/LICENSE` & `kopf-1.36.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/PKG-INFO` & `kopf-1.36.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kopf
-Version: 1.36.0
+Version: 1.36.1
 Summary: Kubernetes Operator Pythonic Framework (Kopf)
 Home-page: https://github.com/nolar/kopf
 Author: Sergey Vasilyev
 Author-email: nolar@nolar.info
 Maintainer: Sergey Vasilyev
 Maintainer-email: nolar@nolar.info
 License: MIT
```

### Comparing `kopf-1.36.0/README.md` & `kopf-1.36.1/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/_importlinter_conditional.py` & `kopf-1.36.1/_importlinter_conditional.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 https://import-linter.readthedocs.io/en/stable/custom_contract_types.html
 """
 import os.path
 
 import astpath
 from importlinter import Contract, ContractCheck, fields, output
+from importlinter.domain.ports.graph import ImportGraph
 
 
 class ConditionalImportContract(Contract):
     """
     Contract that defines a single forbidden import between
     two modules.
     """
     source_modules = fields.ListField(subfield=fields.ModuleField())
     conditional_modules = fields.ListField(subfield=fields.ModuleField())
 
-    def check(self, graph):
+    def check(self, graph: ImportGraph, verbose: bool) -> ContractCheck:
         failed_details = []
 
         # Combine all source x all target (secured) modules.
         conditional_modules = [m for m in self.conditional_modules if m.name in graph.modules]
         for source_module in self.source_modules:
             for conditional_module in conditional_modules:
```

### Comparing `kopf-1.36.0/docs/admission.rst` & `kopf-1.36.1/docs/admission.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/alternatives.rst` & `kopf-1.36.1/docs/alternatives.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/architecture-layers.png` & `kopf-1.36.1/docs/architecture-layers.png`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/architecture-layers.xml` & `kopf-1.36.1/docs/architecture-layers.xml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/architecture.rst` & `kopf-1.36.1/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/async.rst` & `kopf-1.36.1/docs/async.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/authentication.rst` & `kopf-1.36.1/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/cli.rst` & `kopf-1.36.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/concepts.rst` & `kopf-1.36.1/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/conf.py` & `kopf-1.36.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/configuration.rst` & `kopf-1.36.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/continuity.rst` & `kopf-1.36.1/docs/continuity.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/contributing.rst` & `kopf-1.36.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/daemons.rst` & `kopf-1.36.1/docs/daemons.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/deployment-rbac.yaml` & `kopf-1.36.1/docs/deployment-rbac.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/deployment.rst` & `kopf-1.36.1/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/embedding.rst` & `kopf-1.36.1/docs/embedding.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/errors.rst` & `kopf-1.36.1/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/events.rst` & `kopf-1.36.1/docs/events.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/filters.rst` & `kopf-1.36.1/docs/filters.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/handlers.rst` & `kopf-1.36.1/docs/handlers.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/hierarchies.rst` & `kopf-1.36.1/docs/hierarchies.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/idempotence.rst` & `kopf-1.36.1/docs/idempotence.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/index.rst` & `kopf-1.36.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/indexing.rst` & `kopf-1.36.1/docs/indexing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/install.rst` & `kopf-1.36.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/kwargs.rst` & `kopf-1.36.1/docs/kwargs.rst`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,16 @@
 
 .. code-block:: python
 
     import kopf
 
     @kopf.on.update('KopfExample', param=10, field='spec.field')
     @kopf.on.update('KopfExample', param=1, field='spec')
-    def fn(param, **_): ...
+    def fn(param, **_):
+        pass
 
 
 .. kwarg:: settings
 
 Operator configuration
 ======================
```

### Comparing `kopf-1.36.0/docs/loading.rst` & `kopf-1.36.1/docs/loading.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/memos.rst` & `kopf-1.36.1/docs/memos.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/minikube.rst` & `kopf-1.36.1/docs/minikube.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/peering.rst` & `kopf-1.36.1/docs/peering.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/probing.rst` & `kopf-1.36.1/docs/probing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/reconciliation.rst` & `kopf-1.36.1/docs/reconciliation.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/resources.rst` & `kopf-1.36.1/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/results.rst` & `kopf-1.36.1/docs/results.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/scopes.rst` & `kopf-1.36.1/docs/scopes.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/shutdown.rst` & `kopf-1.36.1/docs/shutdown.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/startup.rst` & `kopf-1.36.1/docs/startup.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/testing.rst` & `kopf-1.36.1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/timers.rst` & `kopf-1.36.1/docs/timers.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/tips-and-tricks.rst` & `kopf-1.36.1/docs/tips-and-tricks.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/troubleshooting.rst` & `kopf-1.36.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/vision.rst` & `kopf-1.36.1/docs/vision.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/walkthrough/creation.rst` & `kopf-1.36.1/docs/walkthrough/creation.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/walkthrough/deletion.rst` & `kopf-1.36.1/docs/walkthrough/deletion.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/walkthrough/diffs.rst` & `kopf-1.36.1/docs/walkthrough/diffs.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/walkthrough/prerequisites.rst` & `kopf-1.36.1/docs/walkthrough/prerequisites.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/walkthrough/problem.rst` & `kopf-1.36.1/docs/walkthrough/problem.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/walkthrough/resources.rst` & `kopf-1.36.1/docs/walkthrough/resources.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/walkthrough/starting.rst` & `kopf-1.36.1/docs/walkthrough/starting.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/docs/walkthrough/updates.rst` & `kopf-1.36.1/docs/walkthrough/updates.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/01-minimal/README.md` & `kopf-1.36.1/examples/01-minimal/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/02-children/README.md` & `kopf-1.36.1/examples/02-children/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/02-children/example.py` & `kopf-1.36.1/examples/02-children/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/03-exceptions/README.md` & `kopf-1.36.1/examples/03-exceptions/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/03-exceptions/example.py` & `kopf-1.36.1/examples/03-exceptions/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/04-events/README.md` & `kopf-1.36.1/examples/04-events/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/04-events/example.py` & `kopf-1.36.1/examples/04-events/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/05-handlers/README.md` & `kopf-1.36.1/examples/05-handlers/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/05-handlers/example.py` & `kopf-1.36.1/examples/05-handlers/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/06-peering/README.md` & `kopf-1.36.1/examples/06-peering/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/07-subhandlers/README.md` & `kopf-1.36.1/examples/07-subhandlers/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/08-events/README.md` & `kopf-1.36.1/examples/08-events/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/09-testing/test_example_09.py` & `kopf-1.36.1/examples/09-testing/test_example_09.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/10-builtins/README.md` & `kopf-1.36.1/examples/10-builtins/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/10-builtins/example.py` & `kopf-1.36.1/examples/10-builtins/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/10-builtins/test_example_10.py` & `kopf-1.36.1/examples/10-builtins/test_example_10.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/11-filtering-handlers/README.md` & `kopf-1.36.1/examples/11-filtering-handlers/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/11-filtering-handlers/example.py` & `kopf-1.36.1/examples/11-filtering-handlers/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/11-filtering-handlers/test_example_11.py` & `kopf-1.36.1/examples/11-filtering-handlers/test_example_11.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/12-embedded/README.md` & `kopf-1.36.1/examples/12-embedded/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/12-embedded/example.py` & `kopf-1.36.1/examples/12-embedded/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/13-hooks/README.md` & `kopf-1.36.1/examples/13-hooks/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/13-hooks/example.py` & `kopf-1.36.1/examples/13-hooks/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/14-daemons/example.py` & `kopf-1.36.1/examples/14-daemons/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/16-indexing/example.py` & `kopf-1.36.1/examples/16-indexing/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/17-admission/example.py` & `kopf-1.36.1/examples/17-admission/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/99-all-at-once/example.py` & `kopf-1.36.1/examples/99-all-at-once/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/examples/crd.yaml` & `kopf-1.36.1/examples/crd.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/__init__.py` & `kopf-1.36.1/kopf/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/aiokits/aioadapters.py` & `kopf-1.36.1/kopf/_cogs/aiokits/aioadapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     Wait for a flag to be raised.
 
     Non-asyncio primitives are generally not our worry,
     but we support them for convenience.
     """
     if flag is None:
-        pass
+        return None
     elif isinstance(flag, asyncio.Future):
         return await flag
     elif isinstance(flag, asyncio.Event):
         return await flag.wait()
     elif isinstance(flag, concurrent.futures.Future):
         loop = asyncio.get_running_loop()
         return await loop.run_in_executor(None, flag.result)
@@ -39,15 +39,15 @@
     """
     Raise a flag.
 
     Non-asyncio primitives are generally not our worry,
     but we support them for convenience.
     """
     if flag is None:
-        pass
+        return None
     elif isinstance(flag, asyncio.Future):
         flag.set_result(None)
     elif isinstance(flag, asyncio.Event):
         flag.set()
     elif isinstance(flag, concurrent.futures.Future):
         flag.set_result(None)
     elif isinstance(flag, threading.Event):
```

### Comparing `kopf-1.36.0/kopf/_cogs/aiokits/aiobindings.py` & `kopf-1.36.1/kopf/_cogs/aiokits/aiobindings.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/aiokits/aioenums.py` & `kopf-1.36.1/kopf/_cogs/aiokits/aioenums.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,9 +168,9 @@
     def __await__(self) -> Generator[None, None, AsyncFlagWaiter[FlagReasonT]]:
         name = f"time-limited waiting for the daemon stopper {self._setter!r}"
         coro = asyncio.wait_for(self._setter.async_event.wait(), timeout=self._timeout)
         task = aiotasks.create_task(coro, name=name)
         try:
             yield from task
         except asyncio.TimeoutError:
-            pass
+            pass  # the requested time limit is reached, exit regardless of the state
         return self._waiter  # the original checker! not the time-limited one!
```

### Comparing `kopf-1.36.0/kopf/_cogs/aiokits/aiotasks.py` & `kopf-1.36.1/kopf/_cogs/aiokits/aiotasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     except AttributeError:
         # The official way is to create an extra task object, thus to waste some memory.
         corotask = create_task(coro=coro, name=name)
         corotask.cancel()
         try:
             await corotask
         except asyncio.CancelledError:
-            pass
+            pass  # cancellations are expected at this point
 
 
 async def guard(
         coro: Coroutine[Any, Any, Any],
         name: str,
         *,
         flag: Optional[asyncio.Event] = None,
@@ -233,15 +233,15 @@
     """
     Re-raise errors from tasks, if any. Do nothing if all tasks have succeeded.
     """
     for task in tasks:
         try:
             task.result()  # can raise the regular (non-cancellation) exceptions.
         except asyncio.CancelledError:
-            pass
+            pass  # re-raise anything except regular cancellations/exits
 
 
 async def all_tasks(
         *,
         ignored: Collection[Task] = frozenset(),
 ) -> Collection[Task]:
     """
@@ -382,14 +382,15 @@
         while True:
             task = await self._cleaning_queue.get()
 
             # Await the task from an outer context to prevent RuntimeWarnings/ResourceWarnings.
             try:
                 await task
             except BaseException:
+                # The errors are handled in the done-callback. Suppress what has leaked for safety.
                 pass
 
             # Ping other tasks to refill the pool of running tasks (or to close the scheduler).
             async with self._condition:
                 self._running_tasks.discard(task)
                 self._condition.notify_all()  # -> task_spawner() & close()
```

### Comparing `kopf-1.36.0/kopf/_cogs/aiokits/aiotime.py` & `kopf-1.36.1/kopf/_cogs/aiokits/aiotime.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/aiokits/aiotoggles.py` & `kopf-1.36.1/kopf/_cogs/aiokits/aiotoggles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/aiokits/aiovalues.py` & `kopf-1.36.1/kopf/_cogs/aiokits/aiovalues.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/clients/__init__.py` & `kopf-1.36.1/kopf/_cogs/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/clients/api.py` & `kopf-1.36.1/kopf/_cogs/clients/api.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/clients/auth.py` & `kopf-1.36.1/kopf/_cogs/clients/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,9 +209,9 @@
         return self._paths[item]
 
     def purge(self) -> None:
         for _, path in self._paths.items():
             try:
                 os.remove(path)
             except OSError:
-                pass
+                pass  # already removed
         self._paths.clear()
```

### Comparing `kopf-1.36.0/kopf/_cogs/clients/creating.py` & `kopf-1.36.1/kopf/_cogs/clients/creating.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/clients/errors.py` & `kopf-1.36.1/kopf/_cogs/clients/errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/clients/events.py` & `kopf-1.36.1/kopf/_cogs/clients/events.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/clients/fetching.py` & `kopf-1.36.1/kopf/_cogs/clients/fetching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/clients/patching.py` & `kopf-1.36.1/kopf/_cogs/clients/patching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/clients/scanning.py` & `kopf-1.36.1/kopf/_cogs/clients/scanning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/clients/watching.py` & `kopf-1.36.1/kopf/_cogs/clients/watching.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,23 @@
 import enum
 import logging
 from typing import AsyncIterator, Dict, Optional, Union, cast
 
 import aiohttp
 
 from kopf._cogs.aiokits import aiotasks, aiotoggles
-from kopf._cogs.clients import api, fetching
+from kopf._cogs.clients import api, errors, fetching
 from kopf._cogs.configs import configuration
 from kopf._cogs.structs import bodies, references
 
 logger = logging.getLogger(__name__)
 
+HTTP_TOO_MANY_REQUESTS_CODE = 429
+DEFAULT_RETRY_DELAY_SECONDS = 1
+
 
 class WatchingError(Exception):
     """
     Raised when an unexpected error happens in the watch-stream API.
     """
 
 
@@ -75,16 +78,28 @@
             ) as operator_pause_waiter:
                 stream = continuous_watch(
                     settings=settings,
                     resource=resource,
                     namespace=namespace,
                     operator_pause_waiter=operator_pause_waiter,
                 )
-                async for raw_event in stream:
-                    yield raw_event
+                try:
+                    async for raw_event in stream:
+                        yield raw_event
+                except errors.APIClientError as ex:
+                    if ex.code != HTTP_TOO_MANY_REQUESTS_CODE:
+                        raise
+
+                    retry_after = ex.details.get("retryAfterSeconds") if ex.details else None
+                    retry_wait = retry_after or DEFAULT_RETRY_DELAY_SECONDS
+                    logger.warning(
+                        f"Receiving `too many requests` error from server, will retry after "
+                        f"{retry_wait} seconds. Error details: {ex}"
+                    )
+                    await asyncio.sleep(retry_wait)
             await asyncio.sleep(settings.watching.reconnect_backoff)
     finally:
         logger.debug(f"Stopping the watch-stream for {resource} {where}.")
 
 
 @contextlib.asynccontextmanager
 async def streaming_block(
```

### Comparing `kopf-1.36.0/kopf/_cogs/configs/configuration.py` & `kopf-1.36.1/kopf/_cogs/configs/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
     @max_workers.setter
     def max_workers(self, value: int) -> None:
         if value < 1:
             raise ValueError("Can't set thread pool limit lower than 1.")
         self._max_workers = value
 
         if hasattr(self.executor, '_max_workers'):
-            self.executor._max_workers = value  # type: ignore
+            self.executor._max_workers = value
         else:
             raise TypeError("Current executor does not support `max_workers`.")
 
 
 @dataclasses.dataclass
 class NetworkingSettings:
```

### Comparing `kopf-1.36.0/kopf/_cogs/configs/conventions.py` & `kopf-1.36.1/kopf/_cogs/configs/conventions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/configs/diffbase.py` & `kopf-1.36.1/kopf/_cogs/configs/diffbase.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/configs/progress.py` & `kopf-1.36.1/kopf/_cogs/configs/progress.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/helpers/__init__.py` & `kopf-1.36.1/kopf/_cogs/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/helpers/hostnames.py` & `kopf-1.36.1/kopf/_cogs/helpers/hostnames.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/helpers/loaders.py` & `kopf-1.36.1/kopf/_cogs/helpers/loaders.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/helpers/thirdparty.py` & `kopf-1.36.1/kopf/_cogs/helpers/thirdparty.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/helpers/typedefs.py` & `kopf-1.36.1/kopf/_cogs/helpers/typedefs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/helpers/versions.py` & `kopf-1.36.1/kopf/_cogs/helpers/versions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/structs/bodies.py` & `kopf-1.36.1/kopf/_cogs/structs/bodies.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/structs/credentials.py` & `kopf-1.36.1/kopf/_cogs/structs/credentials.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/structs/dicts.py` & `kopf-1.36.1/kopf/_cogs/structs/dicts.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,22 +173,22 @@
     if not path:
         raise ValueError("Removing a root of a dict is impossible. Provide a specific field.")
 
     elif len(path) == 1:
         try:
             del d[path[0]]
         except KeyError:
-            pass
+            pass  # already absent
 
     else:
         try:
             # Recursion is the easiest way to implement it, assuming the bodies/patches are shallow.
             remove(d[path[0]], path[1:])
         except KeyError:
-            pass
+            pass  # already absent
         else:
             # Clean the parent dict if it has become empty due to deletion of the only sub-key.
             # Upper parents will be handled by upper recursion functions.
             if d[path[0]] == {}:  # but not None, and not False, etc.
                 del d[path[0]]
 
 
@@ -241,22 +241,22 @@
         yield from walk(objs.obj, nested=nested)
     elif isinstance(objs, thirdparty.KubernetesModel):
         yield objs  # type: ignore
         for subfield in (nested if nested is not None else []):
             try:
                 yield resolve_obj(objs, parse_field(subfield))
             except (AttributeError, KeyError):
-                pass
+                pass  # do not dive deep into non-existent fields or non-dicts
     elif isinstance(objs, collections.abc.Mapping):
         yield objs  # type: ignore
         for subfield in (nested if nested is not None else []):
             try:
                 yield resolve(objs, parse_field(subfield))
             except KeyError:
-                pass
+                pass  # avoid diving into non-dicts, ignore them
     elif isinstance(objs, collections.abc.Iterable):
         for obj in objs:
             yield from walk(obj, nested=nested)
     else:
         yield objs  # NB: not a mapping or a known type => no nested sub-fields.
```

### Comparing `kopf-1.36.0/kopf/_cogs/structs/diffs.py` & `kopf-1.36.1/kopf/_cogs/structs/diffs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/structs/ephemera.py` & `kopf-1.36.1/kopf/_cogs/structs/ephemera.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/structs/finalizers.py` & `kopf-1.36.1/kopf/_cogs/structs/finalizers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/structs/patches.py` & `kopf-1.36.1/kopf/_cogs/structs/patches.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/structs/references.py` & `kopf-1.36.1/kopf/_cogs/structs/references.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_cogs/structs/reviews.py` & `kopf-1.36.1/kopf/_cogs/structs/reviews.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/actions/application.py` & `kopf-1.36.1/kopf/_core/actions/application.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/actions/execution.py` & `kopf-1.36.1/kopf/_core/actions/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,18 +140,15 @@
         # Similar to `dataclasses.asdict()`, but not recursive for other dataclasses.
         return {field.name: getattr(self, field.name) for field in dataclasses.fields(self)}
 
 
 CauseT = TypeVar('CauseT', bound=Cause)
 
 
-# FIXME: Must be frozen, but mypy fails in _call_handler() with a cryptic error:
-# FIXME:    Argument 1 to "invoke" has incompatible type "Optional[HandlerResult]";
-# FIXME:    expected "Union[LifeCycleFn, ActivityHandlerFn, ResourceHandlerFn]"
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Handler:
     """ A handler is a function bound with its behavioral constraints. """
     id: ids.HandlerId
     fn: invocation.Invokable
     param: Optional[Any]
     errors: Optional[ErrorsMode]
     timeout: Optional[float]
```

### Comparing `kopf-1.36.0/kopf/_core/actions/invocation.py` & `kopf-1.36.1/kopf/_core/actions/invocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,10 +150,10 @@
         fn: Optional[Invokable],
 ) -> bool:
     if fn is None:
         return False
     elif isinstance(fn, functools.partial):
         return is_async_fn(fn.func)
     elif hasattr(fn, '__wrapped__'):  # @functools.wraps()
-        return is_async_fn(fn.__wrapped__)  # type: ignore
+        return is_async_fn(fn.__wrapped__)
     else:
         return asyncio.iscoroutinefunction(fn)
```

### Comparing `kopf-1.36.0/kopf/_core/actions/lifecycles.py` & `kopf-1.36.1/kopf/_core/actions/lifecycles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/actions/loggers.py` & `kopf-1.36.1/kopf/_core/actions/loggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 Everything logged to the object logger (except for debug information) is also
 posted as a k8s-event -- in the background by `kopf._core.engines.posting`.
 
 This eliminates the need to log & post the same messages, which complicates
 the operators' code, and can lead to information loss or mismatch
 (e.g. when logging call is added, but posting is forgotten).
 """
-import asyncio
 import copy
 import enum
 import logging
-from typing import Any, MutableMapping, Optional, Tuple
+from typing import Any, Dict, MutableMapping, Optional, Tuple
 
 import pythonjsonlogger.jsonlogger
 
 from kopf._cogs.configs import configuration
 from kopf._cogs.helpers import typedefs
 from kopf._cogs.structs import bodies
 
@@ -37,35 +36,35 @@
     pass
 
 
 class ObjectTextFormatter(ObjectFormatter, logging.Formatter):
     pass
 
 
-class ObjectJsonFormatter(ObjectFormatter, pythonjsonlogger.jsonlogger.JsonFormatter):  # type: ignore
+class ObjectJsonFormatter(ObjectFormatter, pythonjsonlogger.jsonlogger.JsonFormatter):
     def __init__(
             self,
             *args: Any,
             refkey: Optional[str] = None,
             **kwargs: Any,
     ) -> None:
         # Avoid type checking, as the args are not in the parent consructor.
         reserved_attrs = kwargs.pop('reserved_attrs', pythonjsonlogger.jsonlogger.RESERVED_ATTRS)
         reserved_attrs = set(reserved_attrs)
         reserved_attrs |= {'k8s_skip', 'k8s_ref', 'settings'}
         kwargs.update(reserved_attrs=reserved_attrs)
         kwargs.setdefault('timestamp', True)
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)  # type: ignore  # for untyped JsonFormatter.__init__()
         self._refkey: str = refkey or DEFAULT_JSON_REFKEY
 
     def add_fields(
             self,
-            log_record: MutableMapping[str, object],
+            log_record: Dict[str, object],
             record: logging.LogRecord,
-            message_dict: MutableMapping[str, object],
+            message_dict: Dict[str, object],
     ) -> None:
         super().add_fields(log_record, record, message_dict)
 
         if self._refkey and hasattr(record, 'k8s_ref'):
             ref = getattr(record, 'k8s_ref')
             log_record[self._refkey] = ref
 
@@ -189,18 +188,14 @@
     # For no-propagation loggers, add a dummy null handler to prevent printing the messages.
     for name in ['asyncio']:
         logger = logging.getLogger(name)
         logger.propagate = bool(debug)
         if not debug:
             logger.handlers[:] = [logging.NullHandler()]
 
-    # Since Python 3.10, get_event_loop() is deprecated, issues a warning. Here is a way around:
-    loop = asyncio.get_event_loop_policy().get_event_loop()
-    loop.set_debug(bool(debug))
-
 
 def make_formatter(
         log_format: LogFormat = LogFormat.FULL,
         log_prefix: Optional[bool] = False,
         log_refkey: Optional[str] = None,
 ) -> ObjectFormatter:
     log_prefix = log_prefix if log_prefix is not None else bool(log_format is not LogFormat.JSON)
```

### Comparing `kopf-1.36.0/kopf/_core/actions/progression.py` & `kopf-1.36.1/kopf/_core/actions/progression.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/actions/throttlers.py` & `kopf-1.36.1/kopf/_core/actions/throttlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/engines/activities.py` & `kopf-1.36.1/kopf/_core/engines/activities.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/engines/admission.py` & `kopf-1.36.1/kopf/_core/engines/admission.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/engines/daemons.py` & `kopf-1.36.1/kopf/_core/engines/daemons.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,14 +416,28 @@
     finally:
 
         # Prevent future re-spawns for those exited on their own, for no reason.
         # Only the filter-mismatching or peering-pausing daemons can be re-spawned.
         if stopper.reason is None:
             memory.forever_stopped.add(handler.id)
 
+        # If this daemon is never going to be called again, we can release the
+        # live_fresh_body to save some memory.
+        if handler.id in memory.forever_stopped:
+            # If any other running daemon is referencing this Kubernetes
+            # resource, we can't free it
+            can_free = True
+            this_daemon = daemons[handler.id]
+            for running_daemon in memory.running_daemons.values():
+                if running_daemon is not this_daemon:
+                    can_free = False
+                    break
+            if can_free:
+                memory.live_fresh_body = None
+
         # Save the memory by not remembering the exited daemons (they may be never re-spawned).
         del daemons[handler.id]
 
         # Whatever happened, make sure the sync threads of asyncio threaded executor are notified:
         # in a hope that they will exit maybe some time later to free the OS/asyncio resources.
         # A possible case: operator is exiting and cancelling all "hung" non-root tasks, etc.
         stopper.set(reason=stoppers.DaemonStoppingReason.DONE)
```

### Comparing `kopf-1.36.0/kopf/_core/engines/indexing.py` & `kopf-1.36.1/kopf/_core/engines/indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         return any(val == obj for val in self.__items.values())
 
     # Indexers' internal protocol. Must not be used by handlers & operators.
     def _discard(self, acckey: Key) -> None:
         try:
             del self.__items[acckey]
         except KeyError:
-            pass
+            pass  # already absent
 
     # Indexers' internal protocol. Must not be used by handlers & operators.
     def _replace(self, acckey: Key, obj: _V) -> None:
         # Minimise the dict updates and rehashes for no need: only update if really changed.
         if acckey not in self.__items or self.__items[acckey] != obj:
             self.__items[acckey] = obj
```

### Comparing `kopf-1.36.0/kopf/_core/engines/peering.py` & `kopf-1.36.1/kopf/_core/engines/peering.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                 identity=identity,
                 settings=settings,
                 resource=resource,
                 namespace=namespace,
                 lifetime=0,
             ))
         except asyncio.CancelledError:
-            pass
+            pass  # cancellations are treated as normal exiting
         except Exception:
             logger.exception(f"Couldn't remove self from the peering. Ignoring.")
 
 
 async def touch(
         *,
         identity: Identity,
```

### Comparing `kopf-1.36.0/kopf/_core/engines/posting.py` & `kopf-1.36.1/kopf/_core/engines/posting.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/engines/probing.py` & `kopf-1.36.1/kopf/_core/engines/probing.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     probing_timestamp: Optional[datetime.datetime] = None
     probing_max_age = datetime.timedelta(seconds=10.0)
     probing_lock = asyncio.Lock()
 
     async def get_health(
             request: aiohttp.web.Request,
     ) -> aiohttp.web.Response:
-        nonlocal probing_timestamp
+        nonlocal probing_container, probing_timestamp, probing_max_age, probing_lock
 
         # Recollect the data on-demand, and only if is is older that a reasonable caching period.
         # Protect against multiple parallel requests performing the same heavy activity.
         now = datetime.datetime.utcnow()
         if probing_timestamp is None or now - probing_timestamp >= probing_max_age:
             async with probing_lock:
                 now = datetime.datetime.utcnow()
```

### Comparing `kopf-1.36.0/kopf/_core/intents/callbacks.py` & `kopf-1.36.1/kopf/_core/intents/callbacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/intents/causes.py` & `kopf-1.36.1/kopf/_core/intents/causes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/intents/filters.py` & `kopf-1.36.1/kopf/_core/intents/filters.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/intents/handlers.py` & `kopf-1.36.1/kopf/_core/intents/handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from typing import Optional, cast
 
 from kopf._cogs.structs import dicts, diffs, references
 from kopf._core.actions import execution
 from kopf._core.intents import callbacks, causes, filters
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class ActivityHandler(execution.Handler):
     fn: callbacks.ActivityFn  # typing clarification
     activity: Optional[causes.Activity]
     _fallback: bool = False  # non-public!
 
     def __str__(self) -> str:
         return f"Activity {self.id!r}"
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class ResourceHandler(execution.Handler):
     selector: Optional[references.Selector]  # None is used only in sub-handlers
     labels: Optional[filters.MetaFilter]
     annotations: Optional[filters.MetaFilter]
     when: Optional[callbacks.WhenFilterFn]
     field: Optional[dicts.FieldPath]
     value: Optional[filters.ValueFilter]
@@ -32,71 +32,71 @@
             diff = diffs.reduce(cause.diff, self.field)
             new_cause = dataclasses.replace(cause, old=old, new=new, diff=diff)
             return cast(execution.CauseT, new_cause)  # TODO: mypy bug?
         else:
             return cause
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class WebhookHandler(ResourceHandler):
     fn: callbacks.WebhookFn  # typing clarification
     reason: causes.WebhookType
     operation: Optional[str]
     subresource: Optional[str]
     persistent: Optional[bool]
     side_effects: Optional[bool]
     ignore_failures: Optional[bool]
 
     def __str__(self) -> str:
         return f"Webhook {self.id!r}"
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class IndexingHandler(ResourceHandler):
     fn: callbacks.IndexingFn  # typing clarification
 
     def __str__(self) -> str:
         return f"Indexer {self.id!r}"
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class WatchingHandler(ResourceHandler):
     fn: callbacks.WatchingFn  # typing clarification
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class ChangingHandler(ResourceHandler):
     fn: callbacks.ChangingFn  # typing clarification
     reason: Optional[causes.Reason]
     initial: Optional[bool]
     deleted: Optional[bool]  # used for mixed-in (initial==True) @on.resume handlers only.
     requires_finalizer: Optional[bool]
     field_needs_change: Optional[bool]  # to identify on-field/on-update with support for old=/new=.
     old: Optional[filters.ValueFilter]
     new: Optional[filters.ValueFilter]
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class SpawningHandler(ResourceHandler):
     requires_finalizer: Optional[bool]
     initial_delay: Optional[float]
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class DaemonHandler(SpawningHandler):
     fn: callbacks.DaemonFn  # typing clarification
     cancellation_backoff: Optional[float]  # how long to wait before actual cancellation.
     cancellation_timeout: Optional[float]  # how long to wait before giving up on cancellation.
     cancellation_polling: Optional[float]  # how often to check for cancellation status.
 
     def __str__(self) -> str:
         return f"Daemon {self.id!r}"
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class TimerHandler(SpawningHandler):
     fn: callbacks.TimerFn  # typing clarification
     sharp: Optional[bool]
     idle: Optional[float]
     interval: Optional[float]
 
     def __str__(self) -> str:
```

### Comparing `kopf-1.36.0/kopf/_core/intents/piggybacking.py` & `kopf-1.36.1/kopf/_core/intents/piggybacking.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/intents/registries.py` & `kopf-1.36.1/kopf/_core/intents/registries.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/intents/stoppers.py` & `kopf-1.36.1/kopf/_core/intents/stoppers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/reactor/inventory.py` & `kopf-1.36.1/kopf/_core/reactor/inventory.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/reactor/observation.py` & `kopf-1.36.1/kopf/_core/reactor/observation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/reactor/orchestration.py` & `kopf-1.36.1/kopf/_core/reactor/orchestration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/reactor/processing.py` & `kopf-1.36.1/kopf/_core/reactor/processing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_core/reactor/queueing.py` & `kopf-1.36.1/kopf/_core/reactor/queueing.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     we can make a decision on whether it was a real cancellation, or our own.
     """
 
     # In case of a failed worker, stop the watcher, and escalate to the operator to stop it.
     watcher_task = asyncio.current_task()
     worker_error: Optional[BaseException] = None
     def exception_handler(exc: BaseException) -> None:
-        nonlocal worker_error
+        nonlocal worker_error, watcher_task
         if worker_error is None:
             worker_error = exc
             if watcher_task is not None:  # never happens, but is needed for type-checking.
                 watcher_task.cancel()
 
     # All per-object workers are handled as fire-and-forget jobs via the scheduler,
     # and communicated via the per-object event queues.
@@ -302,15 +302,15 @@
                         prev_event = raw_event
                         next_event = await asyncio.wait_for(
                             backlog.get(),
                             timeout=settings.batching.batch_window)
                         shouldstop = shouldstop or isinstance(next_event, EOS)
                         raw_event = prev_event if isinstance(next_event, EOS) else next_event
                 except asyncio.TimeoutError:
-                    pass
+                    pass  # the batch accumulation is over, we can proceed to the processing
 
             # Exit gracefully and immediately on the end-of-stream marker sent by the watcher.
             if isinstance(raw_event, EOS):
                 break
 
             # Try the processor. In case of errors, show the error, but continue the processing.
             pressure.clear()
@@ -329,15 +329,15 @@
 
     finally:
         # Whether an exception or a break or a success, notify the caller, and garbage-collect our queue.
         # The queue must not be left in the queue-cache without a corresponding job handling this queue.
         try:
             del streams[key]
         except KeyError:
-            pass
+            pass  # already absent
 
         # Notify the depletion routine about the changes in the workers'/streams' overall state.
         # * This should happen STRICTLY AFTER the removal from the streams[], and
         # * This should happen A MOMENT BEFORE the job ends (within the scheduler's close_timeout).
         async with signaller:
             signaller.notify_all()
 
@@ -359,12 +359,12 @@
     # NB: the scheduler is checked for a case of mocked workers; otherwise, the streams are enough.
     async with signaller:
         try:
             await asyncio.wait_for(
                 signaller.wait_for(lambda: not streams or scheduler.empty()),
                 timeout=settings.batching.exit_timeout)
         except asyncio.TimeoutError:
-            pass
+            pass  # if not depleted as configured, proceed with what's left and let it fail
 
     # The last check if the termination is going to be graceful or not.
     if streams:
         logger.warning(f"Unprocessed streams left for {list(streams.keys())!r}.")
```

### Comparing `kopf-1.36.0/kopf/_core/reactor/running.py` & `kopf-1.36.1/kopf/_core/reactor/running.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,37 +49,40 @@
     of the current _context_ (by asyncio's default, the current thread).
     See: https://docs.python.org/3/library/asyncio-policy.html for details.
 
     Alternatively, use `asyncio.run(kopf.operator(...))` with the same options.
     It will take care of a new event loop's creation and finalization for this
     call. See: :func:`asyncio.run`.
     """
-    loop = loop if loop is not None else asyncio.get_event_loop_policy().get_event_loop()
+    coro = operator(
+        lifecycle=lifecycle,
+        indexers=indexers,
+        registry=registry,
+        settings=settings,
+        memories=memories,
+        insights=insights,
+        identity=identity,
+        standalone=standalone,
+        clusterwide=clusterwide,
+        namespaces=namespaces,
+        namespace=namespace,
+        priority=priority,
+        peering_name=peering_name,
+        liveness_endpoint=liveness_endpoint,
+        stop_flag=stop_flag,
+        ready_flag=ready_flag,
+        vault=vault,
+        memo=memo,
+        _command=_command,
+    )
     try:
-        loop.run_until_complete(operator(
-            lifecycle=lifecycle,
-            indexers=indexers,
-            registry=registry,
-            settings=settings,
-            memories=memories,
-            insights=insights,
-            identity=identity,
-            standalone=standalone,
-            clusterwide=clusterwide,
-            namespaces=namespaces,
-            namespace=namespace,
-            priority=priority,
-            peering_name=peering_name,
-            liveness_endpoint=liveness_endpoint,
-            stop_flag=stop_flag,
-            ready_flag=ready_flag,
-            vault=vault,
-            memo=memo,
-            _command=_command,
-        ))
+        if loop is not None:
+            loop.run_until_complete(coro)
+        else:
+            asyncio.run(coro)
     except asyncio.CancelledError:
         pass
 
 
 async def operator(
         *,
         lifecycle: Optional[execution.LifeCycleFn] = None,
```

### Comparing `kopf-1.36.0/kopf/_core/reactor/subhandling.py` & `kopf-1.36.1/kopf/_core/reactor/subhandling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_kits/__init__.py` & `kopf-1.36.1/kopf/_kits/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_kits/hierarchies.py` & `kopf-1.36.1/kopf/_kits/hierarchies.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_kits/runner.py` & `kopf-1.36.1/kopf/_kits/runner.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_kits/webhacks.py` & `kopf-1.36.1/kopf/_kits/webhacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf/_kits/webhooks.py` & `kopf-1.36.1/kopf/_kits/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,19 +380,19 @@
         # Detect which ones of the hostnames are probably IPv4/IPv6 addresses.
         # A side-effect: bring them all to their canonical forms.
         parsed_ips: Dict[str, Union[ipaddress.IPv4Address, ipaddress.IPv6Address]] = {}
         for hostname in hostnames:
             try:
                 parsed_ips[hostname] = ipaddress.IPv4Address(hostname)
             except ipaddress.AddressValueError:
-                pass
+                pass  # non-parsable IPs are considered to be regular hostnames
             try:
                 parsed_ips[hostname] = ipaddress.IPv6Address(hostname)
             except ipaddress.AddressValueError:
-                pass
+                pass  # non-parsable IPs are considered to be regular hostnames
 
         # Later, only the normalised IPs are used as SANs, not the raw IPs.
         # Remove bindable but non-accessible addresses (like 0.0.0.0) form the SANs.
         true_hostnames = [hostname for hostname in hostnames if hostname not in parsed_ips]
         accessible_ips = [str(ip) for ip in parsed_ips.values() if not ip.is_unspecified]
 
         # Build a certificate as the framework believe is good enough for itself.
```

### Comparing `kopf-1.36.0/kopf/cli.py` & `kopf-1.36.1/kopf/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from kopf._cogs.configs import configuration
 from kopf._cogs.helpers import loaders
 from kopf._cogs.structs import credentials, references
 from kopf._core.actions import loggers
 from kopf._core.engines import peering
 from kopf._core.intents import registries
 from kopf._core.reactor import running
+from kopf._kits import loops
 
 
 @dataclasses.dataclass()
 class CLIControls:
     """ `KopfRunner` controls, which are impossible to pass via CLI. """
     ready_flag: Optional[aioadapters.Flag] = None
     stop_flag: Optional[aioadapters.Flag] = None
@@ -63,21 +64,15 @@
 
 @click.group(name='kopf', context_settings=dict(
     auto_envvar_prefix='KOPF',
 ))
 @click.version_option(prog_name='kopf')
 @click.make_pass_decorator(CLIControls, ensure=True)
 def main(__controls: CLIControls) -> None:
-    if __controls.loop is None:  # the pure CLI use, not a KopfRunner or other code
-        try:
-            import uvloop
-        except ImportError:
-            pass
-        else:
-            asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+    pass
 
 
 @main.command()
 @logging_options
 @click.option('-A', '--all-namespaces', 'clusterwide', is_flag=True)
 @click.option('-n', '--namespace', 'namespaces', multiple=True)
 @click.option('--standalone', is_flag=True, default=None)
@@ -106,89 +101,96 @@
         raise click.UsageError("Either --namespace or --all-namespaces can be used, not both.")
     if __controls.registry is not None:
         registries.set_default_registry(__controls.registry)
     loaders.preload(
         paths=paths,
         modules=modules,
     )
-    return running.run(
-        standalone=standalone,
-        namespaces=namespaces,
-        clusterwide=clusterwide,
-        priority=priority,
-        peering_name=peering_name,
-        liveness_endpoint=liveness_endpoint,
-        registry=__controls.registry,
-        settings=__controls.settings,
-        stop_flag=__controls.stop_flag,
-        ready_flag=__controls.ready_flag,
-        vault=__controls.vault,
-        loop=__controls.loop,
-    )
+    with loops.proper_loop(__controls.loop):
+        return running.run(
+            standalone=standalone,
+            namespaces=namespaces,
+            clusterwide=clusterwide,
+            priority=priority,
+            peering_name=peering_name,
+            liveness_endpoint=liveness_endpoint,
+            registry=__controls.registry,
+            settings=__controls.settings,
+            stop_flag=__controls.stop_flag,
+            ready_flag=__controls.ready_flag,
+            vault=__controls.vault,
+            loop=__controls.loop,
+        )
 
 
 @main.command()
 @logging_options
 @click.option('-n', '--namespace', 'namespaces', multiple=True)
 @click.option('-A', '--all-namespaces', 'clusterwide', is_flag=True)
 @click.option('-i', '--id', type=str, default=None)
 @click.option('--dev', 'priority', flag_value=666)
 @click.option('-P', '--peering', 'peering_name', required=True, envvar='KOPF_FREEZE_PEERING')
 @click.option('-p', '--priority', type=int, default=100, required=True)
 @click.option('-t', '--lifetime', type=int, required=True)
 @click.option('-m', '--message', type=str)
+@click.make_pass_decorator(CLIControls, ensure=True)
 def freeze(
+        __controls: CLIControls,
         id: Optional[str],
         message: Optional[str],
         lifetime: int,
         namespaces: Collection[references.NamespacePattern],
         clusterwide: bool,
         peering_name: str,
         priority: int,
 ) -> None:
     """ Pause the resource handling in the operator(s). """
     identity = peering.Identity(id) if id else peering.detect_own_id(manual=True)
     insights = references.Insights()
     settings = configuration.OperatorSettings()
     settings.peering.name = peering_name
     settings.peering.priority = priority
-    return running.run(
-        clusterwide=clusterwide,
-        namespaces=namespaces,
-        insights=insights,
-        identity=identity,
-        settings=settings,
-        _command=peering.touch_command(
+    with loops.proper_loop(__controls.loop):
+        return running.run(
+            clusterwide=clusterwide,
+            namespaces=namespaces,
             insights=insights,
             identity=identity,
             settings=settings,
-            lifetime=lifetime))
+            _command=peering.touch_command(
+                insights=insights,
+                identity=identity,
+                settings=settings,
+                lifetime=lifetime))
 
 
 @main.command()
 @logging_options
 @click.option('-n', '--namespace', 'namespaces', multiple=True)
 @click.option('-A', '--all-namespaces', 'clusterwide', is_flag=True)
 @click.option('-i', '--id', type=str, default=None)
 @click.option('-P', '--peering', 'peering_name', required=True, envvar='KOPF_RESUME_PEERING')
+@click.make_pass_decorator(CLIControls, ensure=True)
 def resume(
+        __controls: CLIControls,
         id: Optional[str],
         namespaces: Collection[references.NamespacePattern],
         clusterwide: bool,
         peering_name: str,
 ) -> None:
     """ Resume the resource handling in the operator(s). """
     identity = peering.Identity(id) if id else peering.detect_own_id(manual=True)
     insights = references.Insights()
     settings = configuration.OperatorSettings()
     settings.peering.name = peering_name
-    return running.run(
-        clusterwide=clusterwide,
-        namespaces=namespaces,
-        insights=insights,
-        identity=identity,
-        settings=settings,
-        _command=peering.touch_command(
+    with loops.proper_loop(__controls.loop):
+        return running.run(
+            clusterwide=clusterwide,
+            namespaces=namespaces,
             insights=insights,
             identity=identity,
             settings=settings,
-            lifetime=0))
+            _command=peering.touch_command(
+                insights=insights,
+                identity=identity,
+                settings=settings,
+                lifetime=0))
```

### Comparing `kopf-1.36.0/kopf/on.py` & `kopf-1.36.1/kopf/on.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/kopf.egg-info/PKG-INFO` & `kopf-1.36.1/kopf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kopf
-Version: 1.36.0
+Version: 1.36.1
 Summary: Kubernetes Operator Pythonic Framework (Kopf)
 Home-page: https://github.com/nolar/kopf
 Author: Sergey Vasilyev
 Author-email: nolar@nolar.info
 Maintainer: Sergey Vasilyev
 Maintainer-email: nolar@nolar.info
 License: MIT
```

### Comparing `kopf-1.36.0/kopf.egg-info/SOURCES.txt` & `kopf-1.36.1/kopf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/ISSUE_TEMPLATE/bug-report.yaml
 .github/ISSUE_TEMPLATE/config.yaml
 .github/ISSUE_TEMPLATE/feature-request.yaml
 .github/ISSUE_TEMPLATE/question.yaml
 .github/workflows/ci.yaml
+.github/workflows/codeql.yml
 .github/workflows/publish.yaml
 .github/workflows/thorough.yaml
 docs/.gitattributes
 docs/admission.rst
 docs/alternatives.rst
 docs/architecture-layers.png
 docs/architecture-layers.xml
@@ -210,14 +211,15 @@
 kopf/_core/reactor/orchestration.py
 kopf/_core/reactor/processing.py
 kopf/_core/reactor/queueing.py
 kopf/_core/reactor/running.py
 kopf/_core/reactor/subhandling.py
 kopf/_kits/__init__.py
 kopf/_kits/hierarchies.py
+kopf/_kits/loops.py
 kopf/_kits/runner.py
 kopf/_kits/webhacks.py
 kopf/_kits/webhooks.py
 tests/conftest.py
 tests/test_absent_modules.py
 tests/test_async.py
 tests/test_filtering_helpers.py
```

### Comparing `kopf-1.36.0/peering.yaml` & `kopf-1.36.1/peering.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/requirements.txt` & `kopf-1.36.1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import-linter
 isort
 lxml
 # Generally, `unittest.mock` is enough, but it lacks `AsyncMock` for Py 3.7.
 # TODO: Once 3.7 is removed (Jun 2023), roll back to unittest.mock.
 mock
 # Mypy requires typed-ast, which is broken on PyPy 3.7 (could work in PyPy 3.8).
-mypy==0.982; implementation_name == "cpython"
+mypy==1.2.0; implementation_name == "cpython"
 pre-commit
 pyngrok
 pytest>=6.0.0
 pytest-aiohttp
 pytest-asyncio
 pytest-cov
 pytest-mock
```

### Comparing `kopf-1.36.0/setup.py` & `kopf-1.36.1/setup.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/conftest.py` & `kopf-1.36.1/tests/admission/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_admission_manager.py` & `kopf-1.36.1/tests/admission/test_admission_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,18 +112,18 @@
 
 @pytest.mark.parametrize('reason', set(WebhookType))
 @pytest.mark.parametrize('selector', {VALIDATING_WEBHOOK, MUTATING_WEBHOOK})
 async def test_patching_on_changes(
         mocker, settings, registry, insights, selector, resource, reason, k8s_mocked):
 
     @kopf.on.validate(*resource, registry=registry)
-    def fn_v(**_): ...
+    def fn_v(**_): pass
 
     @kopf.on.mutate(*resource, registry=registry)
-    def fn_m(**_): ...
+    def fn_m(**_): pass
 
     container = Container()
     mocker.patch.object(container, 'as_changed', return_value=aiter([
         {'url': 'https://hostname1/'},
         {'url': 'https://hostname2/'},
     ]))
 
@@ -160,18 +160,18 @@
 
 @pytest.mark.parametrize('reason', set(WebhookType))
 @pytest.mark.parametrize('selector', {VALIDATING_WEBHOOK, MUTATING_WEBHOOK})
 async def test_patching_purges_non_permanent_webhooks(
         mocker, settings, registry, insights, selector, resource, reason, k8s_mocked):
 
     @kopf.on.validate(*resource, registry=registry, persistent=False)
-    def fn_v(**_): ...
+    def fn_v(**_): pass
 
     @kopf.on.mutate(*resource, registry=registry, persistent=False)
-    def fn_m(**_): ...
+    def fn_m(**_): pass
 
     container = Container()
     mocker.patch.object(container, 'as_changed', return_value=aiter([
         {'url': 'https://hostname/'},
     ]))
 
     settings.admission.managed = 'xyz'
@@ -191,18 +191,18 @@
 
 @pytest.mark.parametrize('reason', set(WebhookType))
 @pytest.mark.parametrize('selector', {VALIDATING_WEBHOOK, MUTATING_WEBHOOK})
 async def test_patching_leaves_permanent_webhooks(
         mocker, settings, registry, insights, selector, resource, reason, k8s_mocked):
 
     @kopf.on.validate(*resource, registry=registry, persistent=True)
-    def fn_v(**_): ...
+    def fn_v(**_): pass
 
     @kopf.on.mutate(*resource, registry=registry, persistent=True)
-    def fn_m(**_): ...
+    def fn_m(**_): pass
 
     container = Container()
     mocker.patch.object(container, 'as_changed', return_value=aiter([
         {'url': 'https://hostname/'},
     ]))
 
     settings.admission.managed = 'xyz'
```

### Comparing `kopf-1.36.0/tests/admission/test_admission_server.py` & `kopf-1.36.1/tests/admission/test_admission_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     pass
 
 
 async def test_requires_webserver_if_webhooks_are_defined(
         settings, registry, insights, resource):
 
     @kopf.on.validate(*resource, registry=registry)
-    def fn_v(**_): ...
+    def fn_v(**_): pass
 
     @kopf.on.mutate(*resource, registry=registry)
-    def fn_m(**_): ...
+    def fn_m(**_): pass
 
     container = Container()
     with pytest.raises(Exception) as err:
         settings.admission.server = None
         await admission_webhook_server(
             registry=registry,
             settings=settings,
```

### Comparing `kopf-1.36.0/tests/admission/test_certificates.py` & `kopf-1.36.1/tests/admission/test_certificates.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_jsonpatch.py` & `kopf-1.36.1/tests/admission/test_jsonpatch.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_managed_webhooks.py` & `kopf-1.36.1/tests/admission/test_managed_webhooks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_serving_ephemeral_memos.py` & `kopf-1.36.1/tests/admission/test_serving_ephemeral_memos.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_serving_handler_selection.py` & `kopf-1.36.1/tests/admission/test_serving_handler_selection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_serving_kwargs_passthrough.py` & `kopf-1.36.1/tests/admission/test_serving_kwargs_passthrough.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_serving_responses.py` & `kopf-1.36.1/tests/admission/test_serving_responses.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_webhook_detection.py` & `kopf-1.36.1/tests/admission/test_webhook_detection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_webhook_ngrok.py` & `kopf-1.36.1/tests/admission/test_webhook_ngrok.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/admission/test_webhook_server.py` & `kopf-1.36.1/tests/admission/test_webhook_server.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/apis/test_api_requests.py` & `kopf-1.36.1/tests/apis/test_api_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,15 @@
         try:
             await asyncio.sleep(0.05)
             await response.write(b'{"fake": "result1"}\n')
             await asyncio.sleep(0.15)
             await response.write(b'{"fake": "result2"}\n')
             await response.write_eof()
         except ConnectionError:
-            pass
+            pass  # the client side sometimes disconnects earlier, ignore it
         return response
 
     aresponses.add(hostname, '/url', method, stream_slowly)
 
     stopper = asyncio.Future()
     asyncio.get_running_loop().call_later(delay, stopper.set_result, None)
```

### Comparing `kopf-1.36.0/tests/apis/test_error_retries.py` & `kopf-1.36.1/tests/apis/test_error_retries.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/apis/test_iterjsonlines.py` & `kopf-1.36.1/tests/apis/test_iterjsonlines.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/authentication/test_authentication.py` & `kopf-1.36.1/tests/authentication/test_authentication.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/authentication/test_connectioninfo.py` & `kopf-1.36.1/tests/authentication/test_connectioninfo.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/authentication/test_credentials.py` & `kopf-1.36.1/tests/authentication/test_credentials.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/authentication/test_login_kubeconfig.py` & `kopf-1.36.1/tests/authentication/test_login_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/authentication/test_login_serviceaccount.py` & `kopf-1.36.1/tests/authentication/test_login_serviceaccount.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/authentication/test_reauthentication.py` & `kopf-1.36.1/tests/authentication/test_reauthentication.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/authentication/test_tempfiles.py` & `kopf-1.36.1/tests/authentication/test_tempfiles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/authentication/test_vault.py` & `kopf-1.36.1/tests/authentication/test_vault.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/basic-structs/test_causes.py` & `kopf-1.36.1/tests/basic-structs/test_causes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/basic-structs/test_handlers.py` & `kopf-1.36.1/tests/basic-structs/test_handlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/basic-structs/test_memories.py` & `kopf-1.36.1/tests/basic-structs/test_memories.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/basic-structs/test_memos.py` & `kopf-1.36.1/tests/basic-structs/test_memos.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/basic-structs/test_resource.py` & `kopf-1.36.1/tests/basic-structs/test_resource.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/causation/test_detection.py` & `kopf-1.36.1/tests/causation/test_detection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/causation/test_kwargs.py` & `kopf-1.36.1/tests/causation/test_kwargs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/cli/conftest.py` & `kopf-1.36.1/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/cli/test_help.py` & `kopf-1.36.1/tests/cli/test_help.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/cli/test_logging.py` & `kopf-1.36.1/tests/cli/test_logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import logging
 
 import pytest
 
 
 @pytest.mark.parametrize('expect_debug, expect_info, options, envvars', [
     (False, True, [], {}),
@@ -55,23 +54,21 @@
     assert result.exit_code == 0
 
     # TODO: This also goes to the pytest's output. Try to suppress it there (how?).
     logging.getLogger('asyncio').error('boom!')
 
     alien_records = [m for m in caplog.records if not m.name.startswith('kopf')]
     assert len(alien_records) == 0
-    assert not asyncio.get_event_loop_policy().get_event_loop().get_debug()
 
 
 @pytest.mark.parametrize('options', [
     (['-d']),
     (['--debug']),
 ], ids=['d', 'debug'])
 def test_lowlevel_dumps_in_debug_mode(invoke, caplog, options, preload, real_run):
     result = invoke(['run'] + options)
     assert result.exit_code == 0
 
     logging.getLogger('asyncio').debug('hello!')
 
     alien_records = [m for m in caplog.records if not m.name.startswith('kopf')]
     assert len(alien_records) >= 1
-    assert asyncio.get_event_loop_policy().get_event_loop().get_debug()
```

### Comparing `kopf-1.36.0/tests/cli/test_options.py` & `kopf-1.36.1/tests/cli/test_options.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/cli/test_preloading.py` & `kopf-1.36.1/tests/cli/test_preloading.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/conftest.py` & `kopf-1.36.1/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     config.addinivalue_line('filterwarnings', 'error')
 
     # Warnings from the testing tools out of our control should not fail the tests.
     config.addinivalue_line('filterwarnings', 'ignore:The loop argument:DeprecationWarning:aiohttp')
     config.addinivalue_line('filterwarnings', 'ignore:The loop argument:DeprecationWarning:asyncio')
     config.addinivalue_line('filterwarnings', 'ignore:is deprecated, use current_thread:DeprecationWarning:threading')
 
+    # TODO: Remove when fixed in https://github.com/pytest-dev/pytest-asyncio/issues/460:
+    config.addinivalue_line('filterwarnings', 'ignore:There is no current event loop:DeprecationWarning:pytest_asyncio')
+
 
 def pytest_addoption(parser):
     parser.addoption("--only-e2e", action="store_true", help="Execute end-to-end tests only.")
     parser.addoption("--with-e2e", action="store_true", help="Include end-to-end tests.")
 
 
 # This logic is not applied if pytest is started explicitly on ./examples/.
```

### Comparing `kopf-1.36.0/tests/dicts/test_cherrypicking.py` & `kopf-1.36.1/tests/dicts/test_cherrypicking.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/dicts/test_dictviews.py` & `kopf-1.36.1/tests/dicts/test_dictviews.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/dicts/test_ensuring.py` & `kopf-1.36.1/tests/dicts/test_ensuring.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/dicts/test_parsing.py` & `kopf-1.36.1/tests/dicts/test_parsing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/dicts/test_removing.py` & `kopf-1.36.1/tests/dicts/test_removing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/dicts/test_resolving.py` & `kopf-1.36.1/tests/dicts/test_resolving.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/dicts/test_walking.py` & `kopf-1.36.1/tests/dicts/test_walking.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/diffs/test_calculation.py` & `kopf-1.36.1/tests/diffs/test_calculation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/diffs/test_protocols.py` & `kopf-1.36.1/tests/diffs/test_protocols.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/diffs/test_reduction.py` & `kopf-1.36.1/tests/diffs/test_reduction.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/e2e/conftest.py` & `kopf-1.36.1/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/e2e/test_examples.py` & `kopf-1.36.1/tests/e2e/test_examples.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/conftest.py` & `kopf-1.36.1/tests/handling/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/conftest.py` & `kopf-1.36.1/tests/handling/daemons/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/test_daemon_errors.py` & `kopf-1.36.1/tests/handling/daemons/test_daemon_errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/test_daemon_filtration.py` & `kopf-1.36.1/tests/handling/daemons/test_daemon_filtration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/test_daemon_rematching.py` & `kopf-1.36.1/tests/handling/daemons/test_daemon_rematching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/test_daemon_spawning.py` & `kopf-1.36.1/tests/handling/daemons/test_daemon_spawning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/test_daemon_termination.py` & `kopf-1.36.1/tests/handling/daemons/test_daemon_termination.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/test_timer_errors.py` & `kopf-1.36.1/tests/handling/daemons/test_timer_errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/test_timer_filtration.py` & `kopf-1.36.1/tests/handling/daemons/test_timer_filtration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/test_timer_intervals.py` & `kopf-1.36.1/tests/handling/daemons/test_timer_intervals.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/daemons/test_timer_triggering.py` & `kopf-1.36.1/tests/handling/daemons/test_timer_triggering.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/indexing/conftest.py` & `kopf-1.36.1/tests/handling/indexing/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/indexing/test_blocking_until_indexed.py` & `kopf-1.36.1/tests/handling/indexing/test_blocking_until_indexed.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/indexing/test_index_exclusion.py` & `kopf-1.36.1/tests/handling/indexing/test_index_exclusion.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/indexing/test_index_population.py` & `kopf-1.36.1/tests/handling/indexing/test_index_population.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/subhandling/test_subhandling.py` & `kopf-1.36.1/tests/handling/subhandling/test_subhandling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_activity_triggering.py` & `kopf-1.36.1/tests/handling/test_activity_triggering.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_cause_handling.py` & `kopf-1.36.1/tests/handling/test_cause_handling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_cause_logging.py` & `kopf-1.36.1/tests/handling/test_cause_logging.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_delays.py` & `kopf-1.36.1/tests/handling/test_delays.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_error_handling.py` & `kopf-1.36.1/tests/handling/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_event_handling.py` & `kopf-1.36.1/tests/handling/test_event_handling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_multistep.py` & `kopf-1.36.1/tests/handling/test_multistep.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_no_handlers.py` & `kopf-1.36.1/tests/handling/test_no_handlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_parametrization.py` & `kopf-1.36.1/tests/handling/test_parametrization.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_retrying_limits.py` & `kopf-1.36.1/tests/handling/test_retrying_limits.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/handling/test_timing_consistency.py` & `kopf-1.36.1/tests/handling/test_timing_consistency.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/hierarchies/conftest.py` & `kopf-1.36.1/tests/hierarchies/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/hierarchies/test_contextual_owner.py` & `kopf-1.36.1/tests/hierarchies/test_contextual_owner.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/hierarchies/test_labelling.py` & `kopf-1.36.1/tests/hierarchies/test_labelling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/hierarchies/test_name_harmonizing.py` & `kopf-1.36.1/tests/hierarchies/test_name_harmonizing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/hierarchies/test_namespace_adjusting.py` & `kopf-1.36.1/tests/hierarchies/test_namespace_adjusting.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/hierarchies/test_owner_referencing.py` & `kopf-1.36.1/tests/hierarchies/test_owner_referencing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/hierarchies/test_type_validation.py` & `kopf-1.36.1/tests/hierarchies/test_type_validation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/invocations/test_callbacks.py` & `kopf-1.36.1/tests/invocations/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/k8s/test_creating.py` & `kopf-1.36.1/tests/k8s/test_creating.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/k8s/test_errors.py` & `kopf-1.36.1/tests/k8s/test_errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/k8s/test_events.py` & `kopf-1.36.1/tests/k8s/test_events.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/k8s/test_list_objs.py` & `kopf-1.36.1/tests/k8s/test_list_objs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/k8s/test_patching.py` & `kopf-1.36.1/tests/k8s/test_patching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/k8s/test_scanning.py` & `kopf-1.36.1/tests/k8s/test_scanning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/k8s/test_watching_bookmarks.py` & `kopf-1.36.1/tests/k8s/test_watching_bookmarks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/k8s/test_watching_continuously.py` & `kopf-1.36.1/tests/k8s/test_watching_continuously.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/k8s/test_watching_infinitely.py` & `kopf-1.36.1/tests/k8s/test_watching_infinitely.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from kopf._cogs.clients.errors import APIError
+from kopf._cogs.clients.errors import APIClientError, APIError
 from kopf._cogs.clients.watching import Bookmark, infinite_watch
 
 STREAM_WITH_UNKNOWN_EVENT = [
     {'type': 'ADDED', 'object': {'spec': 'a'}},
     {'type': 'UNKNOWN', 'object': {}},
     {'type': 'ADDED', 'object': {'spec': 'b'}},
 ]
@@ -59,7 +59,32 @@
 
     assert len(events) == 5
     assert events[0] == Bookmark.LISTED
     assert events[1]['object']['spec'] == 'a'
     assert events[2] == Bookmark.LISTED
     assert events[3]['object']['spec'] == 'a'
     assert events[4]['object']['spec'] == 'b'
+
+
+async def test_too_many_requests_exception(
+        settings, resource, stream, namespace, enforced_session, mocker):
+
+    exc = APIClientError({
+        "apiVersion": "v1",
+        "code": 429,
+        "status": "Failure",
+        "details": {
+            "retryAfterSeconds": 1,
+        }
+    }, status=429)
+    enforced_session.request = mocker.Mock(side_effect=exc)
+    stream.feed([], namespace=namespace)
+    stream.close(namespace=namespace)
+
+    events = []
+    async for event in infinite_watch(settings=settings,
+                                      resource=resource,
+                                      namespace=namespace,
+                                      _iterations=1):
+        events.append(event)
+
+    assert len(events) == 0
```

### Comparing `kopf-1.36.0/tests/k8s/test_watching_with_freezes.py` & `kopf-1.36.1/tests/k8s/test_watching_with_freezes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/lifecycles/test_global_defaults.py` & `kopf-1.36.1/tests/lifecycles/test_global_defaults.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/lifecycles/test_handler_selection.py` & `kopf-1.36.1/tests/lifecycles/test_handler_selection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/lifecycles/test_real_invocation.py` & `kopf-1.36.1/tests/lifecycles/test_real_invocation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/logging/conftest.py` & `kopf-1.36.1/tests/logging/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/logging/test_configuration.py` & `kopf-1.36.1/tests/logging/test_configuration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/logging/test_formatters.py` & `kopf-1.36.1/tests/logging/test_formatters.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/logging/test_loggers.py` & `kopf-1.36.1/tests/logging/test_loggers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/observation/test_processing_of_namespaces.py` & `kopf-1.36.1/tests/observation/test_processing_of_namespaces.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/observation/test_processing_of_resources.py` & `kopf-1.36.1/tests/observation/test_processing_of_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,26 +100,26 @@
     (kopf.on.validate, 'webhook_resources'),
     (kopf.on.mutate, 'webhook_resources'),
 ])
 def insights_resources(request, registry, insights):
     decorator, insights_field = request.param
 
     @decorator('group1', 'version1', 'plural1')
-    def fn(**_): ...
+    def fn(**_): pass
 
     return getattr(insights, insights_field)
 
 
 @pytest.mark.parametrize('decorator', [kopf.on.validate, kopf.on.mutate])
 @pytest.mark.parametrize('etype', ['ADDED', 'MODIFIED'])
 async def test_nonwatchable_resources_are_ignored(
         settings, registry, apis_mock, group1_mock, timer, etype, decorator, insights):
 
     @decorator('group1', 'version1', 'plural1')
-    def fn(**_): ...
+    def fn(**_): pass
 
     e1 = RawEvent(type=etype, object=RawBody(spec={'group': 'group1'}))
 
     async def delayed_injection(delay: float):
         await asyncio.sleep(delay)
         await process_discovered_resource_event(
             insights=insights, raw_event=e1, registry=registry, settings=settings)
```

### Comparing `kopf-1.36.0/tests/observation/test_revision_of_namespaces.py` & `kopf-1.36.1/tests/observation/test_revision_of_namespaces.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/observation/test_revision_of_resources.py` & `kopf-1.36.1/tests/observation/test_revision_of_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     (kopf.on.mutate, 'webhook_resources'),
 ])
 def insights_resources(request, registry, insights):
     decorator, insights_field = request.param
 
     @decorator('group1', 'version1', 'plural1')
     @decorator('group2', 'version2', 'plural2')
-    def fn(**_): ...
+    def fn(**_): pass
 
     return getattr(insights, insights_field)
 
 
 def test_initial_population(registry, insights, insights_resources):
     r1 = Resource(group='group1', version='version1', plural='plural1', verbs=VERBS)
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1])
@@ -70,15 +70,15 @@
     kopf.on.resume, kopf.on.create, kopf.on.update, kopf.on.delete,
 ])
 def test_ambiguity_in_specific_selectors(registry, decorator, caplog, assert_logs, insights):
     r1 = Resource(group='g1', version='v1', plural='plural', verbs=VERBS)
     r2 = Resource(group='g2', version='v2', plural='plural', verbs=VERBS)
 
     @decorator(plural='plural')
-    def fn(**_): ...
+    def fn(**_): pass
 
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1, r2])
     assert not insights.watched_resources
     assert not insights.webhook_resources
     assert_logs([r"Ambiguous resources will not be served"])
 
 
@@ -87,15 +87,15 @@
     kopf.on.resume, kopf.on.create, kopf.on.update, kopf.on.delete,
 ])
 def test_corev1_overrides_ambuigity(registry, decorator, caplog, assert_logs, insights):
     r1 = Resource(group='', version='v1', plural='pods', verbs=VERBS)
     r2 = Resource(group='metrics.k8s.io', version='v1', plural='pods', verbs=VERBS)
 
     @decorator(plural='pods')
-    def fn(**_): ...
+    def fn(**_): pass
 
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1, r2])
     assert insights.watched_resources == {r1}
     assert_logs([], prohibited=[r"Ambiguous resources will not be served"])
 
 
 @pytest.mark.parametrize('decorator', [
@@ -103,15 +103,15 @@
     kopf.on.resume, kopf.on.create, kopf.on.update, kopf.on.delete,
 ])
 def test_no_ambiguity_in_generic_selector(registry, decorator, caplog, assert_logs, insights):
     r1 = Resource(group='g1', version='v1', plural='plural', verbs=VERBS)
     r2 = Resource(group='g2', version='v2', plural='plural', verbs=VERBS)
 
     @decorator(EVERYTHING)
-    def fn(**_): ...
+    def fn(**_): pass
 
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1, r2])
     assert insights.watched_resources == {r1, r2}
     assert_logs([], prohibited=[r"Ambiguous resources will not be served"])
 
 
 @pytest.mark.parametrize('decorator', [
@@ -119,45 +119,45 @@
     kopf.on.resume, kopf.on.create, kopf.on.update, kopf.on.delete,
 ])
 def test_selectors_with_no_resources(registry, decorator, caplog, assert_logs, insights):
     r1 = Resource(group='group1', version='version1', plural='plural1', verbs=VERBS)
     r2 = Resource(group='group2', version='version2', plural='plural2', verbs=VERBS)
 
     @decorator(plural='plural3')
-    def fn(**_): ...
+    def fn(**_): pass
 
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1, r2])
     assert not insights.watched_resources
     assert_logs([r"Unresolved resources cannot be served"])
 
 
 @pytest.mark.parametrize('decorator', [
     kopf.daemon, kopf.timer,
     kopf.on.resume, kopf.on.create, kopf.on.update, kopf.on.delete,
 ])
 def test_nonwatchable_excluded(registry, decorator, caplog, assert_logs, insights):
     r1 = Resource(group='group1', version='version1', plural='plural1', verbs=[])
 
     @decorator('group1', 'version1', 'plural1')
-    def fn(**_): ...
+    def fn(**_): pass
 
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1])
     assert not insights.watched_resources
     assert_logs([r"Non-watchable resources will not be served: {plural1.version1.group1}"])
 
 
 @pytest.mark.parametrize('decorator', [
     kopf.daemon, kopf.timer,
     kopf.on.resume, kopf.on.create, kopf.on.update, kopf.on.delete,
 ])
 def test_nonpatchable_excluded(registry, decorator, caplog, assert_logs, insights):
     r1 = Resource(group='group1', version='version1', plural='plural1', verbs=['watch', 'list'])
 
     @decorator('group1', 'version1', 'plural1')  # because it patches!
-    def fn(**_): ...
+    def fn(**_): pass
 
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1])
     assert not insights.watched_resources
     assert_logs([r"Non-patchable resources will not be served: {plural1.version1.group1}"])
 
 
 @pytest.mark.parametrize('decorator', [
@@ -165,15 +165,15 @@
     kopf.on.resume, kopf.on.create, kopf.on.update, kopf.on.delete,
 ])
 def test_watchedonly_resources_are_excluded_from_other_sets(registry, decorator, insights):
 
     r1 = Resource(group='group1', version='version1', plural='plural1', verbs=VERBS)
 
     @decorator('group1', 'version1', 'plural1')
-    def fn(**_): ...
+    def fn(**_): pass
 
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1])
     assert insights.watched_resources
     assert not insights.indexed_resources
     assert not insights.webhook_resources
 
 
@@ -181,15 +181,15 @@
     kopf.on.mutate, kopf.on.validate,
 ])
 def test_webhookonly_resources_are_excluded_from_other_sets(registry, decorator, insights):
 
     r1 = Resource(group='group1', version='version1', plural='plural1', verbs=VERBS)
 
     @decorator('group1', 'version1', 'plural1')
-    def fn(**_): ...
+    def fn(**_): pass
 
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1])
     assert not insights.watched_resources
     assert not insights.indexed_resources
     assert insights.webhook_resources
 
 
@@ -197,13 +197,13 @@
     kopf.index,
 ])
 def test_indexed_resources_are_duplicated_in_watched_resources(registry, decorator, insights):
 
     r1 = Resource(group='group1', version='version1', plural='plural1', verbs=VERBS)
 
     @decorator('group1', 'version1', 'plural1')
-    def fn(**_): ...
+    def fn(**_): pass
 
     revise_resources(registry=registry, insights=insights, group=None, resources=[r1])
     assert insights.watched_resources
     assert insights.indexed_resources
     assert not insights.webhook_resources
```

### Comparing `kopf-1.36.0/tests/orchestration/test_task_adjustments.py` & `kopf-1.36.1/tests/orchestration/test_task_adjustments.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/peering/test_freeze_mode.py` & `kopf-1.36.1/tests/peering/test_freeze_mode.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/peering/test_id_generation.py` & `kopf-1.36.1/tests/peering/test_id_generation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/peering/test_keepalive.py` & `kopf-1.36.1/tests/peering/test_keepalive.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/peering/test_peer_patching.py` & `kopf-1.36.1/tests/peering/test_peer_patching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/peering/test_peers.py` & `kopf-1.36.1/tests/peering/test_peers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/peering/test_resource_guessing.py` & `kopf-1.36.1/tests/peering/test_resource_guessing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/persistence/test_annotations_hashing.py` & `kopf-1.36.1/tests/persistence/test_annotations_hashing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/persistence/test_essences.py` & `kopf-1.36.1/tests/persistence/test_essences.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/persistence/test_outcomes.py` & `kopf-1.36.1/tests/persistence/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/persistence/test_states.py` & `kopf-1.36.1/tests/persistence/test_states.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from kopf._cogs.structs.bodies import Body
 from kopf._cogs.structs.patches import Patch
 from kopf._core.actions.execution import Outcome
 from kopf._core.actions.progression import State, StateCounters, deliver_results
 from kopf._core.intents.causes import HANDLER_REASONS, Reason
 
 # Timestamps: time zero (0), before (B), after (A), and time zero+1s (1).
-TSB = datetime.datetime(2020, 12, 31, 23, 59, 59, 000000)
+TSB = datetime.datetime(2020, 12, 31, 23, 59, 59)
 TS0 = datetime.datetime(2020, 12, 31, 23, 59, 59, 123456)
 TS1 = datetime.datetime(2021,  1,  1, 00, 00, 00, 123456)
 TSA = datetime.datetime(2020, 12, 31, 23, 59, 59, 999999)
 TSB_ISO = '2020-12-31T23:59:59.000000'
 TS0_ISO = '2020-12-31T23:59:59.123456'
 TS1_ISO = '2021-01-01T00:00:00.123456'
 TSA_ISO = '2020-12-31T23:59:59.999999'
```

### Comparing `kopf-1.36.0/tests/persistence/test_storing_of_diffbase.py` & `kopf-1.36.1/tests/persistence/test_storing_of_diffbase.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/persistence/test_storing_of_progress.py` & `kopf-1.36.1/tests/persistence/test_storing_of_progress.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/posting/test_log2k8s.py` & `kopf-1.36.1/tests/posting/test_log2k8s.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/posting/test_poster.py` & `kopf-1.36.1/tests/posting/test_poster.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/posting/test_threadsafety.py` & `kopf-1.36.1/tests/posting/test_threadsafety.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/primitives/test_conditions.py` & `kopf-1.36.1/tests/primitives/test_conditions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/primitives/test_containers.py` & `kopf-1.36.1/tests/primitives/test_containers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/primitives/test_flags.py` & `kopf-1.36.1/tests/primitives/test_flags.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 async def test_waiting_of_none_does_nothing():
     await wait_flag(None)
 
 
 async def test_waiting_for_unraised_times_out(flag, timer):
     with pytest.raises(asyncio.TimeoutError), timer:
         await asyncio.wait_for(wait_flag(flag), timeout=0.1)
-    assert timer.seconds >= 0.1
+    assert timer.seconds >= 0.099  # uvloop finishes it earlier than 0.1
 
 
 async def test_waiting_for_preraised_is_instant(flag, timer):
     await raise_flag(flag)  # tested separately above
     with timer:
         await wait_flag(flag)
     assert timer.seconds < 0.5  # near-instant, plus code overhead
```

### Comparing `kopf-1.36.0/tests/primitives/test_toggles.py` & `kopf-1.36.1/tests/primitives/test_toggles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/primitives/test_togglesets.py` & `kopf-1.36.1/tests/primitives/test_togglesets.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/reactor/conftest.py` & `kopf-1.36.1/tests/reactor/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,8 +64,8 @@
         yield task
     finally:
         # Terminate the watcher to cleanup the loop.
         task.cancel()
         try:
             event_loop.run_until_complete(task)
         except asyncio.CancelledError:
-            pass
+            pass  # cancellations are expected at this point
```

### Comparing `kopf-1.36.0/tests/reactor/test_patching_inconsistencies.py` & `kopf-1.36.1/tests/reactor/test_patching_inconsistencies.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/reactor/test_queueing.py` & `kopf-1.36.1/tests/reactor/test_queueing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/reactor/test_uids.py` & `kopf-1.36.1/tests/reactor/test_uids.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/references/test_backbone.py` & `kopf-1.36.1/tests/references/test_backbone.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/references/test_namespace_matching.py` & `kopf-1.36.1/tests/references/test_namespace_matching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/references/test_namespace_selection.py` & `kopf-1.36.1/tests/references/test_namespace_selection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/references/test_selector_matching.py` & `kopf-1.36.1/tests/references/test_selector_matching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/references/test_selector_parsing.py` & `kopf-1.36.1/tests/references/test_selector_parsing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/references/test_selector_properties.py` & `kopf-1.36.1/tests/references/test_selector_properties.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/registries/conftest.py` & `kopf-1.36.1/tests/registries/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/registries/test_creation.py` & `kopf-1.36.1/tests/registries/test_creation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/registries/test_decorators.py` & `kopf-1.36.1/tests/registries/test_decorators.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/registries/test_handler_getting.py` & `kopf-1.36.1/tests/registries/test_handler_getting.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     @kopf.on.event('resource', registry=registry)
     @kopf.on.create('resource', registry=registry)
     @kopf.on.update('resource', registry=registry)
     @kopf.on.delete('resource', registry=registry)
     @kopf.on.resume('resource', registry=registry)
     @kopf.on.timer('resource', registry=registry)
     @kopf.on.daemon('resource', registry=registry)
-    def fn(**_): ...
+    def fn(**_): pass
 
     assert len(registry._indexing.get_all_handlers()) == 1
     assert len(registry._watching.get_all_handlers()) == 2
     assert len(registry._spawning.get_all_handlers()) == 2
     assert len(registry._changing.get_all_handlers()) == 4
 
 
@@ -156,14 +156,14 @@
     @kopf.on.event('resource2', registry=registry)
     @kopf.on.create('resource1', registry=registry)
     @kopf.on.update('resource2', registry=registry)
     @kopf.on.delete('resource3', registry=registry)
     @kopf.on.resume('resource4', registry=registry)
     @kopf.on.timer('resource5', registry=registry)
     @kopf.on.daemon('resource6', registry=registry)
-    def fn(**_): ...
+    def fn(**_): pass
 
     assert registry._indexing.get_all_selectors() == {Selector('resource0')}
     assert registry._watching.get_all_selectors() == {Selector('resource1'), Selector('resource2')}
     assert registry._spawning.get_all_selectors() == {Selector('resource5'), Selector('resource6')}
     assert registry._changing.get_all_selectors() == {Selector('resource1'), Selector('resource2'),
                                                       Selector('resource3'), Selector('resource4')}
```

### Comparing `kopf-1.36.0/tests/registries/test_id_detection.py` & `kopf-1.36.1/tests/registries/test_id_detection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/registries/test_matching_for_changing.py` & `kopf-1.36.1/tests/registries/test_matching_for_changing.py`

 * *Files 5% similar despite different names*

```diff
@@ -426,223 +426,223 @@
 
 
 @matching_reason_and_decorator_with_field
 def test_relevant_handlers_without_field_found(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, field=None)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert handlers
 
 
 @matching_reason_and_decorator_with_field
 def test_relevant_handlers_with_field_found(
         cause_with_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, field='known-field')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert handlers
 
 
 @matching_reason_and_decorator_with_field
 def test_relevant_handlers_with_field_ignored(
         cause_no_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, field='known-field')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_no_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @matching_reason_and_decorator
 def test_relevant_handlers_with_labels_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, labels={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert handlers
 
 
 @matching_reason_and_decorator
 def test_relevant_handlers_with_labels_not_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, labels={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @matching_reason_and_decorator
 def test_relevant_handlers_with_annotations_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, annotations={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert handlers
 
 
 @matching_reason_and_decorator
 def test_relevant_handlers_with_annotations_not_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, annotations={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @matching_reason_and_decorator
 def test_relevant_handlers_with_filter_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, when=_always)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert handlers
 
 
 @matching_reason_and_decorator
 def test_relevant_handlers_with_filter_not_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, when=_never)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @mismatching_reason_and_decorator
 def test_irrelevant_handlers_without_field_ignored(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @matching_reason_and_decorator_with_field
 def test_irrelevant_handlers_with_field_ignored(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, field='extra-field')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @mismatching_reason_and_decorator
 def test_irrelevant_handlers_with_labels_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, labels={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @mismatching_reason_and_decorator
 def test_irrelevant_handlers_with_labels_not_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, labels={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @mismatching_reason_and_decorator
 def test_irrelevant_handlers_with_annotations_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, annotations={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @mismatching_reason_and_decorator
 def test_irrelevant_handlers_with_annotations_not_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, annotations={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @mismatching_reason_and_decorator
 def test_irrelevant_handlers_with_when_callback_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, when=_always)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
 @mismatching_reason_and_decorator
 def test_irrelevant_handlers_with_when_callback_not_satisfied(
         cause_any_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, when=_never)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
     assert not handlers
 
 
@@ -650,45 +650,45 @@
 # Special case for nested fields with shorter/longer diffs.
 #
 
 @matching_reason_and_decorator_with_field
 def test_field_same_as_diff(cause_with_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, field='level1.level2')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_diff
     cause.reason = reason
     cause.old = {'level1': {'level2': 'old'}}
     cause.new = {'level1': {'level2': 'new'}}
     cause.body = Body({'level1': {'level2': 'new'}})
     handlers = registry._changing.get_handlers(cause)
     assert handlers
 
 
 @matching_reason_and_decorator_with_field
 def test_field_shorter_than_diff(cause_with_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, field='level1')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_diff
     cause.reason = reason
     cause.old = {'level1': {'level2': 'old'}}
     cause.new = {'level1': {'level2': 'new'}}
     cause.body = Body({'level1': {'level2': 'new'}})
     handlers = registry._changing.get_handlers(cause)
     assert handlers
 
 
 @matching_reason_and_decorator_with_field
 def test_field_longer_than_diff_for_wrong_field(cause_with_diff, registry, resource, reason, decorator):
 
     @decorator(*resource, field='level1.level2.level3')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_diff
     cause.reason = reason
     cause.old = {'level1': {'level2': 'old'}}
     cause.new = {'level1': {'level2': 'new'}}
     cause.body = Body({'level1': {'level2': 'new'}})
     handlers = registry._changing.get_handlers(cause)
@@ -704,15 +704,15 @@
     pytest.param({}, {'level3': 'new'}, id='empty2struct'),
     pytest.param({'level3': 'old'}, {}, id='struct2empty'),
 ])
 @matching_reason_and_decorator_with_field
 def test_field_longer_than_diff_for_right_field(cause_with_diff, registry, resource, old, new, reason, decorator):
 
     @decorator(*resource, field='level1.level2.level3')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_diff
     cause.reason = reason
     cause.old = {'level1': {'level2': old}} if old is not None else {'level1': {'level2': {}}}
     cause.new = {'level1': {'level2': new}} if new is not None else {'level1': {'level2': {}}}
     cause.body = Body(cause.new)
     handlers = registry._changing.get_handlers(cause)
@@ -723,27 +723,27 @@
 # The handlers must be returned in order of registration,
 # even if they are mixed with-/without- * -event/-field handlers.
 #
 
 def test_order_persisted_a(cause_with_diff, registry, resource):
 
     @kopf.on.create(*resource)
-    def some_fn_1(**_): ...  # used
+    def some_fn_1(**_): pass  # used
 
     @kopf.on.update(*resource)
-    def some_fn_2(**_): ...  # filtered out
+    def some_fn_2(**_): pass  # filtered out
 
     @kopf.on.create(*resource)
-    def some_fn_3(**_): ...  # used
+    def some_fn_3(**_): pass  # used
 
     @kopf.on.field(*resource, field='filtered-out-field')
-    def some_fn_4(**_): ...  # filtered out
+    def some_fn_4(**_): pass  # filtered out
 
     @kopf.on.field(*resource, field='known-field')
-    def some_fn_5(**_): ...  # used
+    def some_fn_5(**_): pass  # used
 
     cause = cause_with_diff
     cause.reason = Reason.CREATE
     handlers = registry._changing.get_handlers(cause)
 
     # Order must be preserved -- same as registered.
     assert len(handlers) == 3
@@ -751,27 +751,27 @@
     assert handlers[1].fn is some_fn_3
     assert handlers[2].fn is some_fn_5
 
 
 def test_order_persisted_b(cause_with_diff, registry, resource):
 
     @kopf.on.field(*resource, field='known-field')
-    def some_fn_1(**_): ...  # used
+    def some_fn_1(**_): pass  # used
 
     @kopf.on.field(*resource, field='filtered-out-field')
-    def some_fn_2(**_): ...  # filtered out
+    def some_fn_2(**_): pass  # filtered out
 
     @kopf.on.create(*resource)
-    def some_fn_3(**_): ...  # used
+    def some_fn_3(**_): pass  # used
 
     @kopf.on.update(*resource)
-    def some_fn_4(**_): ...  # filtered out
+    def some_fn_4(**_): pass  # filtered out
 
     @kopf.on.create(*resource)
-    def some_fn_5(**_): ...  # used
+    def some_fn_5(**_): pass  # used
 
     cause = cause_with_diff
     cause.reason = Reason.CREATE
     handlers = registry._changing.get_handlers(cause)
 
     # Order must be preserved -- same as registered.
     assert len(handlers) == 3
@@ -787,15 +787,15 @@
 @matching_reason_and_decorator
 def test_deduplication_by_fn_and_id(
         cause_with_diff, registry, resource, reason, decorator):
 
     # Note: the decorators are applied bottom-up -- hence, the order of ids:
     @decorator(*resource, id='a')
     @decorator(*resource, id='a')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
 
     assert len(handlers) == 1
     assert handlers[0].id == 'a'  # the first found one is returned
@@ -803,18 +803,18 @@
 
 @matching_reason_and_decorator
 def test_deduplication_distinguishes_different_fns(
         cause_with_diff, registry, resource, reason, decorator):
 
     # Note: the decorators are applied bottom-up -- hence, the order of ids:
     @decorator(*resource, id='a')
-    def some_fn1(**_): ...
+    def some_fn1(**_): pass
 
     @decorator(*resource, id='a')
-    def some_fn2(**_): ...
+    def some_fn2(**_): pass
 
     cause = cause_with_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
 
     assert len(handlers) == 2
 
@@ -822,14 +822,14 @@
 @matching_reason_and_decorator
 def test_deduplication_distinguishes_different_ids(
         cause_with_diff, registry, resource, reason, decorator):
 
     # Note: the decorators are applied bottom-up -- hence, the order of ids:
     @decorator(*resource, id='b')
     @decorator(*resource, id='a')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_diff
     cause.reason = reason
     handlers = registry._changing.get_handlers(cause)
 
     assert len(handlers) == 2
```

### Comparing `kopf-1.36.0/tests/registries/test_matching_for_indexing.py` & `kopf-1.36.1/tests/registries/test_matching_for_indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,100 +381,100 @@
     assert not handlers
 
 
 def test_decorator_without_field_found(
         cause_any_field, registry, resource):
 
     @kopf.index(*resource, field=None)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._indexing.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_field_found(
         cause_with_field, registry, resource):
 
     @kopf.index(*resource, field='known-field')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_field
     handlers = registry._indexing.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_field_ignored(
         cause_no_field, registry, resource):
 
     @kopf.index(*resource, field='known-field')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_no_field
     handlers = registry._indexing.get_handlers(cause)
     assert not handlers
 
 
 def test_decorator_with_labels_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.index(*resource, labels={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._indexing.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_labels_not_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.index(*resource, labels={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._indexing.get_handlers(cause)
     assert not handlers
 
 
 def test_decorator_with_annotations_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.index(*resource, annotations={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._indexing.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_annotations_not_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.index(*resource, annotations={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._indexing.get_handlers(cause)
     assert not handlers
 
 
 def test_decorator_with_filter_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.index(*resource, when=_always)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._indexing.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_filter_not_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.index(*resource, when=_never)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._indexing.get_handlers(cause)
     assert not handlers
```

### Comparing `kopf-1.36.0/tests/registries/test_matching_for_spawning.py` & `kopf-1.36.1/tests/registries/test_matching_for_spawning.py`

 * *Files 5% similar despite different names*

```diff
@@ -389,108 +389,108 @@
 
 
 @spawning_decorators
 def test_decorator_without_field_found(
         cause_any_field, registry, resource, decorator):
 
     @decorator(*resource, field=None)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._spawning.get_handlers(cause)
     assert handlers
 
 
 @spawning_decorators
 def test_decorator_with_field_found(
         cause_with_field, registry, resource, decorator):
 
     @decorator(*resource, field='known-field')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_field
     handlers = registry._spawning.get_handlers(cause)
     assert handlers
 
 
 @spawning_decorators
 def test_decorator_with_field_ignored(
         cause_no_field, registry, resource, decorator):
 
     @decorator(*resource, field='known-field')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_no_field
     handlers = registry._spawning.get_handlers(cause)
     assert not handlers
 
 
 @spawning_decorators
 def test_decorator_with_labels_satisfied(
         cause_any_field, registry, resource, decorator):
 
     @decorator(*resource, labels={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._spawning.get_handlers(cause)
     assert handlers
 
 
 @spawning_decorators
 def test_decorator_with_labels_not_satisfied(
         cause_any_field, registry, resource, decorator):
 
     @decorator(*resource, labels={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._spawning.get_handlers(cause)
     assert not handlers
 
 
 @spawning_decorators
 def test_decorator_with_annotations_satisfied(
         cause_any_field, registry, resource, decorator):
 
     @decorator(*resource, annotations={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._spawning.get_handlers(cause)
     assert handlers
 
 
 @spawning_decorators
 def test_decorator_with_annotations_not_satisfied(
         cause_any_field, registry, resource, decorator):
 
     @decorator(*resource, annotations={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._spawning.get_handlers(cause)
     assert not handlers
 
 
 @spawning_decorators
 def test_decorator_with_filter_satisfied(
         cause_any_field, registry, resource, decorator):
 
     @decorator(*resource, when=_always)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._spawning.get_handlers(cause)
     assert handlers
 
 
 @spawning_decorators
 def test_decorator_with_filter_not_satisfied(
         cause_any_field, registry, resource, decorator):
 
     @decorator(*resource, when=_never)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._spawning.get_handlers(cause)
     assert not handlers
```

### Comparing `kopf-1.36.0/tests/registries/test_matching_for_watching.py` & `kopf-1.36.1/tests/registries/test_matching_for_watching.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,100 +381,100 @@
     assert not handlers
 
 
 def test_decorator_without_field_found(
         cause_any_field, registry, resource):
 
     @kopf.on.event(*resource, field=None)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._watching.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_field_found(
         cause_with_field, registry, resource):
 
     @kopf.on.event(*resource, field='known-field')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_with_field
     handlers = registry._watching.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_field_ignored(
         cause_no_field, registry, resource):
 
     @kopf.on.event(*resource, field='known-field')
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_no_field
     handlers = registry._watching.get_handlers(cause)
     assert not handlers
 
 
 def test_decorator_with_labels_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.on.event(*resource, labels={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._watching.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_labels_not_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.on.event(*resource, labels={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._watching.get_handlers(cause)
     assert not handlers
 
 
 def test_decorator_with_annotations_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.on.event(*resource, annotations={'known': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._watching.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_annotations_not_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.on.event(*resource, annotations={'extra': PRESENT})
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._watching.get_handlers(cause)
     assert not handlers
 
 
 def test_decorator_with_filter_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.on.event(*resource, when=_always)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._watching.get_handlers(cause)
     assert handlers
 
 
 def test_decorator_with_filter_not_satisfied(
         cause_any_field, registry, resource):
 
     @kopf.on.event(*resource, when=_never)
-    def some_fn(**_): ...
+    def some_fn(**_): pass
 
     cause = cause_any_field
     handlers = registry._watching.get_handlers(cause)
     assert not handlers
```

### Comparing `kopf-1.36.0/tests/registries/test_matching_of_callbacks.py` & `kopf-1.36.1/tests/registries/test_matching_of_callbacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/registries/test_matching_of_resources.py` & `kopf-1.36.1/tests/registries/test_matching_of_resources.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/registries/test_requires_finalizer.py` & `kopf-1.36.1/tests/registries/test_requires_finalizer.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/registries/test_resumes_mixed_in.py` & `kopf-1.36.1/tests/registries/test_resumes_mixed_in.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/registries/test_subhandlers_ids.py` & `kopf-1.36.1/tests/registries/test_subhandlers_ids.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/settings/test_defaults.py` & `kopf-1.36.1/tests/settings/test_defaults.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/settings/test_executor.py` & `kopf-1.36.1/tests/settings/test_executor.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/test_async.py` & `kopf-1.36.1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/test_filtering_helpers.py` & `kopf-1.36.1/tests/test_filtering_helpers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/test_finalizers.py` & `kopf-1.36.1/tests/test_finalizers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/test_liveness.py` & `kopf-1.36.1/tests/test_liveness.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         await ready_flag.wait()
         yield f'http://localhost:{port}/xyz'
     finally:
         server.cancel()
         try:
             await server
         except asyncio.CancelledError:
-            pass
+            pass  # cancellations are expected at this point
 
 
 async def test_liveness_for_just_status(liveness_url):
     async with aiohttp.ClientSession() as session:
         async with session.get(liveness_url) as response:
             data = await response.json()
             assert isinstance(data, dict)
```

### Comparing `kopf-1.36.0/tests/test_thirdparty.py` & `kopf-1.36.1/tests/test_thirdparty.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/test_versions.py` & `kopf-1.36.1/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/testing/test_runner.py` & `kopf-1.36.1/tests/testing/test_runner.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/timing/test_sleeping.py` & `kopf-1.36.1/tests/timing/test_sleeping.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/timing/test_throttling.py` & `kopf-1.36.1/tests/timing/test_throttling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/utilities/aiotasks/test_coro_cancellation.py` & `kopf-1.36.1/tests/utilities/aiotasks/test_coro_cancellation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/utilities/aiotasks/test_scheduler.py` & `kopf-1.36.1/tests/utilities/aiotasks/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/utilities/aiotasks/test_task_creation.py` & `kopf-1.36.1/tests/utilities/aiotasks/test_task_creation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/utilities/aiotasks/test_task_guarding.py` & `kopf-1.36.1/tests/utilities/aiotasks/test_task_guarding.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tests/utilities/aiotasks/test_task_stopping.py` & `kopf-1.36.1/tests/utilities/aiotasks/test_task_stopping.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tools/install-kind.sh` & `kopf-1.36.1/tools/install-kind.sh`

 * *Files identical despite different names*

### Comparing `kopf-1.36.0/tools/install-minikube.sh` & `kopf-1.36.1/tools/install-minikube.sh`

 * *Files identical despite different names*

