# Comparing `tmp/streamflow-0.2.0.dev4.tar.gz` & `tmp/streamflow-0.2.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamflow-0.2.0.dev4.tar", last modified: Fri Apr 14 13:07:17 2023, max compression
+gzip compressed data, was "streamflow-0.2.0.dev5.tar", last modified: Sat May  6 16:06:51 2023, max compression
```

## Comparing `streamflow-0.2.0.dev4.tar` & `streamflow-0.2.0.dev5.tar`

### file list

```diff
@@ -1,174 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/bandit-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.130355 streamflow-0.2.0.dev4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/report-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.130355 streamflow-0.2.0.dev4/streamflow/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.134355 streamflow-0.2.0.dev4/streamflow/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.126355 streamflow-0.2.0.dev4/streamflow/config/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.134355 streamflow-0.2.0.dev4/streamflow/config/schemas/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/config/schemas/v1.0/config_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/config/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.134355 streamflow-0.2.0.dev4/streamflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/asyncache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.134355 streamflow-0.2.0.dev4/streamflow/cwl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/cwl/antlr/
--rw-r--r--   0 runner    (1001) docker     (123)    51958 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    33090 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptListener.py
--rw-r--r--   0 runner    (1001) docker     (123)   228628 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/antlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/cwl/requirement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/docker.json
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/kubernetes.json
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/singularity.json
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22258 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)   113737 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)    39908 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/data/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/data/remotepath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/data/schemas/data_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36140 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/aiotarstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    53904 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    43913 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/occam.py
--rw-r--r--   0 runner    (1001) docker     (123)    22133 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/docker-compose.json
--rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/docker.json
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/helm3.json
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/kubernetes.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/local.json
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/occam.json
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/queue_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/singularity.json
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/ssh.json
--rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/deployment_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/filter/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/filter/schemas/shuffle.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/filter/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/future.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/schemas/deployment_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/ext/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/ext/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/loading_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/persistence/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/schemas/sqlite.json
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/schemas/sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)    19471 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53948 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/provenance/run_crate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/recovery/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/checkpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/failure_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/recovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/recovery/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/schemas/default_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/schemas/default_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/schemas/dummy_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/schemas/dummy_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/streamflow/scheduling/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/policy/data_locality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/streamflow/scheduling/policy/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/policy/schemas/data_locality.json
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/streamflow/scheduling/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/schemas/scheduler.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/streamflow/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    62216 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.130355 streamflow-0.2.0.dev4/streamflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:07:16.000000 streamflow-0.2.0.dev4/streamflow.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_cwl_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    24802 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_cwl_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_remotepath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.756713 streamflow-0.2.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-06 16:06:51.756713 streamflow-0.2.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/bandit-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.708713 streamflow-0.2.0.dev5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/report-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:06:51.756713 streamflow-0.2.0.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.712713 streamflow-0.2.0.dev5/streamflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.716713 streamflow-0.2.0.dev5/streamflow/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.700713 streamflow-0.2.0.dev5/streamflow/config/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.716713 streamflow-0.2.0.dev5/streamflow/config/schemas/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/config/schemas/v1.0/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/config/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.720713 streamflow-0.2.0.dev5/streamflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/asyncache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.724713 streamflow-0.2.0.dev5/streamflow/cwl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.728713 streamflow-0.2.0.dev5/streamflow/cwl/antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)    51958 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33090 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   228628 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/antlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.728713 streamflow-0.2.0.dev5/streamflow/cwl/requirement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.728713 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.728713 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22258 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113743 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40610 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.732713 streamflow-0.2.0.dev5/streamflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/data/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/data/remotepath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.732713 streamflow-0.2.0.dev5/streamflow/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/data/schemas/data_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.736713 streamflow-0.2.0.dev5/streamflow/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36140 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/aiotarstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.736713 streamflow-0.2.0.dev5/streamflow/deployment/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53904 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44082 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/occam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22133 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.740713 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/docker-compose.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/helm3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/local.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/occam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/queue_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/ssh.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/deployment_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.740713 streamflow-0.2.0.dev5/streamflow/deployment/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.740713 streamflow-0.2.0.dev5/streamflow/deployment/filter/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/filter/schemas/shuffle.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/filter/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/future.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.740713 streamflow-0.2.0.dev5/streamflow/deployment/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/schemas/deployment_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.744713 streamflow-0.2.0.dev5/streamflow/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/ext/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.744713 streamflow-0.2.0.dev5/streamflow/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/loading_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.744713 streamflow-0.2.0.dev5/streamflow/persistence/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/schemas/sqlite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/schemas/sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.744713 streamflow-0.2.0.dev5/streamflow/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64182 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/provenance/run_crate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.748713 streamflow-0.2.0.dev5/streamflow/recovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/checkpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/failure_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/recovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.748713 streamflow-0.2.0.dev5/streamflow/recovery/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/schemas/default_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/schemas/default_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/schemas/dummy_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/schemas/dummy_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.748713 streamflow-0.2.0.dev5/streamflow/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.748713 streamflow-0.2.0.dev5/streamflow/scheduling/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/policy/data_locality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.752713 streamflow-0.2.0.dev5/streamflow/scheduling/policy/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/policy/schemas/data_locality.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.752713 streamflow-0.2.0.dev5/streamflow/scheduling/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/schemas/scheduler.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.752713 streamflow-0.2.0.dev5/streamflow/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62216 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.712713 streamflow-0.2.0.dev5/streamflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.756713 streamflow-0.2.0.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_cwl_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24802 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_cwl_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_remotepath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_transfer.py
```

### Comparing `streamflow-0.2.0.dev4/LICENSE` & `streamflow-0.2.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/PKG-INFO` & `streamflow-0.2.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev4
+Version: 0.2.0.dev5
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
```

### Comparing `streamflow-0.2.0.dev4/README.md` & `streamflow-0.2.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/pyproject.toml` & `streamflow-0.2.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/config/config.py` & `streamflow-0.2.0.dev5/streamflow/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,17 +95,19 @@
         current_node = self.filesystem
         for part in path.parts:
             if part not in current_node["children"]:
                 return default
             current_node = current_node["children"][part]
         return current_node.get(name)
 
-    def propagate(self, path: PurePosixPath, name: str) -> Any | None:
+    def propagate(
+        self, path: PurePosixPath, name: str, default: Any | None = None
+    ) -> Any | None:
         current_node = self.filesystem
-        value = None
+        value = default
         for part in path.parts:
             if part not in current_node["children"]:
                 return value
             current_node = current_node["children"][part]
             if name in current_node:
                 value = current_node[name]
         return value
```

### Comparing `streamflow-0.2.0.dev4/streamflow/config/schemas/v1.0/config_schema.json` & `streamflow-0.2.0.dev5/streamflow/config/schemas/v1.0/config_schema.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/config/validator.py` & `streamflow-0.2.0.dev5/streamflow/config/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import os
 from typing import TYPE_CHECKING
 
+import jsonref
 import pkg_resources
-from jsonref import loads
 from jsonschema import Draft7Validator
 from ruamel.yaml import YAML
 
 from streamflow.core import utils
 from streamflow.core.exception import WorkflowDefinitionException
 from streamflow.cwl.requirement.docker import cwl_docker_translator_classes
 from streamflow.data import data_manager_classes
@@ -42,15 +42,15 @@
         )
     except pkg_resources.ResolutionError:
         raise Exception(f"Version {config_file['version']} is unsupported")
     filename = os.path.join(base_path, "config_schema.json")
     if not os.path.exists(filename):
         raise Exception(f'Version in "{filename}" is unsupported')
     with open(filename) as f:
-        return loads(f.read(), base_uri=f"file://{base_path}/", jsonschema=True)
+        return jsonref.loads(f.read(), base_uri=f"file://{base_path}/", jsonschema=True)
 
 
 class SfValidator:
     def __init__(self) -> None:
         super().__init__()
         self.yaml = YAML(typ="safe")
```

### Comparing `streamflow-0.2.0.dev4/streamflow/core/asyncache.py` & `streamflow-0.2.0.dev5/streamflow/core/asyncache.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/core/config.py` & `streamflow-0.2.0.dev5/streamflow/core/config.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/core/context.py` & `streamflow-0.2.0.dev5/streamflow/core/context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/core/data.py` & `streamflow-0.2.0.dev5/streamflow/core/data.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/core/deployment.py` & `streamflow-0.2.0.dev5/streamflow/core/deployment.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/core/exception.py` & `streamflow-0.2.0.dev5/streamflow/core/exception.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/core/persistence.py` & `streamflow-0.2.0.dev5/streamflow/core/persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/core/provenance.py` & `streamflow-0.2.0.dev5/streamflow/core/provenance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import MutableSequence, TYPE_CHECKING
+from typing import MutableMapping, MutableSequence, TYPE_CHECKING
 
 from streamflow.core.persistence import DatabaseLoadingContext
 
 if TYPE_CHECKING:
     from streamflow.core.context import StreamFlowContext
     from streamflow.core.workflow import Workflow
 
@@ -19,10 +19,15 @@
     ) -> None:
         self.context: StreamFlowContext = context
         self.db_context: DatabaseLoadingContext = db_context
         self.workflows: MutableSequence[Workflow] = workflows
 
     @abstractmethod
     async def create_archive(
-        self, outdir: str, filename: str | None, config: str | None
+        self,
+        outdir: str,
+        filename: str | None,
+        config: str | None,
+        additional_files: MutableSequence[MutableMapping[str, str]] | None,
+        additional_properties: MutableSequence[MutableMapping[str, str]] | None,
     ):
         ...
```

### Comparing `streamflow-0.2.0.dev4/streamflow/core/recovery.py` & `streamflow-0.2.0.dev5/streamflow/core/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/core/scheduling.py` & `streamflow-0.2.0.dev5/streamflow/core/scheduling.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/core/utils.py` & `streamflow-0.2.0.dev5/streamflow/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import (
     Any,
     MutableMapping,
     MutableSequence,
     TYPE_CHECKING,
 )
 
-from jsonref import loads
+import jsonref
 
 from streamflow.core.exception import WorkflowExecutionException
 
 if TYPE_CHECKING:
     from streamflow.core.context import SchemaEntity
     from streamflow.core.deployment import Connector, Location
     from streamflow.core.workflow import Token
@@ -233,15 +233,15 @@
     schema: MutableMapping[str, Any],
     classes: MutableMapping[str, type[SchemaEntity]],
     definition_name: str,
 ):
     for name, entity in classes.items():
         if entity_schema := entity.get_schema():
             with open(entity_schema) as f:
-                entity_schema = loads(
+                entity_schema = jsonref.loads(
                     f.read(),
                     base_uri=f"file://{os.path.dirname(entity_schema)}/",
                     jsonschema=True,
                 )
             definition = schema["definitions"]
             for el in definition_name.split(posixpath.sep):
                 definition = definition[el]
```

### Comparing `streamflow-0.2.0.dev4/streamflow/core/workflow.py` & `streamflow-0.2.0.dev5/streamflow/core/workflow.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptLexer.py` & `streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptLexer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptListener.py` & `streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptListener.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptParser.py` & `streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptParser.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/combinator.py` & `streamflow-0.2.0.dev5/streamflow/cwl/combinator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/command.py` & `streamflow-0.2.0.dev5/streamflow/cwl/command.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/expression.py` & `streamflow-0.2.0.dev5/streamflow/cwl/expression.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/hardware.py` & `streamflow-0.2.0.dev5/streamflow/cwl/hardware.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/main.py` & `streamflow-0.2.0.dev5/streamflow/cwl/main.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/processor.py` & `streamflow-0.2.0.dev5/streamflow/cwl/processor.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/docker.py` & `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/docker.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/kubernetes.py` & `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/kubernetes.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/docker.json` & `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/docker.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2` & `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/kubernetes.json` & `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/kubernetes.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/singularity.json` & `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/singularity.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/singularity.py` & `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/singularity.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/translator.py` & `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/translator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/runner.py` & `streamflow-0.2.0.dev5/streamflow/cwl/runner.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/step.py` & `streamflow-0.2.0.dev5/streamflow/cwl/step.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/token.py` & `streamflow-0.2.0.dev5/streamflow/cwl/token.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/transformer.py` & `streamflow-0.2.0.dev5/streamflow/cwl/transformer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/translator.py` & `streamflow-0.2.0.dev5/streamflow/cwl/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1511,15 +1511,15 @@
             targets = []
             for target in binding_config.targets:
                 # If original target is local, use a container
                 if target.deployment.type == "local":
                     targets.append(
                         _process_docker_requirement(
                             config_dir=os.path.dirname(self.context.config["path"]),
-                            config=self.workflow_config.get(
+                            config=self.workflow_config.propagate(
                                 path=PurePosixPath(name_prefix),
                                 name="docker",
                                 default=CWLDockerTranslatorConfig(
                                     name="default", type="default", config={}
                                 ),
                             ),
                             context=context,
```

### Comparing `streamflow-0.2.0.dev4/streamflow/cwl/utils.py` & `streamflow-0.2.0.dev5/streamflow/cwl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,29 +52,41 @@
     effective_path: str,
 ) -> None:
     # Cannot glob outside the job output folder
     if not (
         effective_path.startswith(output_directory)
         or effective_path.startswith(input_directory)
         or effective_path.startswith(tmp_directory)
-        or workflow.context.data_manager.get_data_locations(path=path)
     ):
         path_processor = get_path_processor(connector)
-        input_dirs = await remotepath.listdir(
-            connector, location, input_directory, FileType.DIRECTORY
-        )
-        for input_dir in input_dirs:
-            input_path = path_processor.join(
-                input_dir, path_processor.relpath(path, output_directory)
-            )
-            if await remotepath.exists(connector, location, input_path):
-                return
-        raise WorkflowDefinitionException(
-            "Globs outside the job's output folder are not allowed"
-        )
+        relpath = path_processor.relpath(path, output_directory)
+        base_path = (
+            path_processor.normpath(effective_path[: -len(relpath)])
+            if effective_path.endswith(relpath)
+            else path_processor.dirname(effective_path)
+        )
+        if not await search_in_parent_locations(
+            context=workflow.context,
+            connector=connector,
+            path=effective_path,
+            relpath=path_processor.relpath(path, output_directory),
+            base_path=base_path,
+        ):
+            input_dirs = await remotepath.listdir(
+                connector, location, input_directory, FileType.DIRECTORY
+            )
+            for input_dir in input_dirs:
+                input_path = path_processor.join(
+                    input_dir, path_processor.relpath(path, output_directory)
+                )
+                if await remotepath.exists(connector, location, input_path):
+                    return
+            raise WorkflowDefinitionException(
+                "Globs outside the job's output folder are not allowed"
+            )
 
 
 async def _process_secondary_file(
     context: StreamFlowContext,
     connector: Connector,
     locations: MutableSequence[Location],
     secondary_file: Any,
@@ -924,15 +936,20 @@
                         if previous_location is not None:
                             context.data_manager.register_relation(
                                 previous_location, current_location
                             )
                         previous_location = current_location
                 if not actual_locations:
                     raise WorkflowExecutionException(f"Error registering path {path}")
-            return list(actual_locations.values())
+                return list(actual_locations.values())
+            else:
+                return sorted(
+                    data_locations,
+                    key=lambda loc: 0 if loc.data_type == DataType.PRIMARY else 1,
+                )
         path_tokens = [path_processor.sep]
         path_tokens.extend(
             current_path.lstrip(path_processor.sep).split(path_processor.sep)[:-1]
         )
         current_path = path_processor.normpath(path_processor.join(*path_tokens))
     return []
```

### Comparing `streamflow-0.2.0.dev4/streamflow/data/data_manager.py` & `streamflow-0.2.0.dev5/streamflow/data/data_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/data/remotepath.py` & `streamflow-0.2.0.dev5/streamflow/data/remotepath.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/aiotarstream.py` & `streamflow-0.2.0.dev5/streamflow/deployment/aiotarstream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/__init__.py` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/base.py` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/base.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/container.py` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/container.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/kubernetes.py` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,18 @@
                 while content := await reader.read(source_connector.transferBufferSize):
                     await asyncio.gather(
                         *(
                             asyncio.create_task(writer.write(content))
                             for writer in writers
                         )
                     )
+                # Close writers
+                await asyncio.gather(
+                    *(asyncio.create_task(writer.close()) for writer in writers)
+                )
 
     async def _get_container(self, location: Location) -> tuple[str, V1Container]:
         pod_name, container_name = location.name.split(":")
         pod = await self.client.read_namespaced_pod(
             name=pod_name, namespace=self.namespace or "default"
         )
         for container in pod.spec.containers:
```

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/local.py` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/local.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/occam.py` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/occam.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/queue_manager.py` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/queue_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/docker-compose.json` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/docker-compose.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/docker.json` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/docker.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/helm3.json` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/helm3.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/kubernetes.json` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/kubernetes.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/occam.json` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/occam.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/queue_manager.json` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/queue_manager.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/singularity.json` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/singularity.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/ssh.json` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/ssh.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/connector/ssh.py` & `streamflow-0.2.0.dev5/streamflow/deployment/connector/ssh.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/deployment_manager.py` & `streamflow-0.2.0.dev5/streamflow/deployment/deployment_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,17 +192,17 @@
                 del self.dependency_graph[deployment_name]
                 await connector.undeploy(config.external)
                 if logger.isEnabledFor(logging.INFO):
                     if not config.external:
                         logger.info(f"COMPLETED Undeployment of {deployment_name}")
                 self.events_map[deployment_name].set()
             # Remove the current environment from all the other dependency graphs
-            for name, deps in {
-                k: v for k, v in self.dependency_graph.items() if k != deployment_name
-            }.items():
+            for name, deps in (
+                (k, v) for k, v in self.dependency_graph.items() if k != deployment_name
+            ):
                 deps.discard(deployment_name)
                 # If there are no more dependencies, undeploy the environment
                 if len(deps) == 0:
                     await self.undeploy(name)
 
     async def undeploy_all(self):
         undeployments = []
```

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/filter/shuffle.py` & `streamflow-0.2.0.dev5/streamflow/deployment/filter/shuffle.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/future.py` & `streamflow-0.2.0.dev5/streamflow/deployment/future.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/stream.py` & `streamflow-0.2.0.dev5/streamflow/deployment/stream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/template.py` & `streamflow-0.2.0.dev5/streamflow/deployment/template.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/utils.py` & `streamflow-0.2.0.dev5/streamflow/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/deployment/wrapper.py` & `streamflow-0.2.0.dev5/streamflow/deployment/wrapper.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/ext/plugin.py` & `streamflow-0.2.0.dev5/streamflow/ext/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
-from typing import MutableMapping
+from typing import Any, MutableMapping, MutableSequence
 
 from streamflow.core.data import DataManager
 from streamflow.core.deployment import BindingFilter, Connector, DeploymentManager
 from streamflow.core.persistence import Database
 from streamflow.core.recovery import CheckpointManager, FailureManager
 from streamflow.core.scheduling import Policy, Scheduler
 from streamflow.cwl.requirement.docker import cwl_docker_translator_classes
@@ -18,51 +18,74 @@
 from streamflow.log_handler import logger
 from streamflow.persistence import database_classes
 from streamflow.recovery import checkpoint_manager_classes, failure_manager_classes
 from streamflow.scheduling import scheduler_classes
 from streamflow.scheduling.policy import policy_classes
 
 
+extension_points = {
+    "binding_filter": binding_filter_classes,
+    "checkpoint_manager": checkpoint_manager_classes,
+    "cwl_docker_translator": cwl_docker_translator_classes,
+    "connector": connector_classes,
+    "data_manager": data_manager_classes,
+    "database": database_classes,
+    "deployment_manager": deployment_manager_classes,
+    "failure_manager": failure_manager_classes,
+    "policy": policy_classes,
+    "scheduler": scheduler_classes,
+}
+
+
 class StreamFlowPlugin(ABC):
-    def _register(self, name: str, cls: type, classes: MutableMapping[str, type]):
-        if name in classes:
+    def __init__(self):
+        self.classes_: MutableMapping[str, MutableSequence[Any]] = {}
+
+    def _register(self, name: str, cls: type, extension_point: str):
+        self.classes_.setdefault(extension_point, []).append(
+            {
+                "name": name,
+                "class": cls,
+            }
+        )
+        if name in extension_points[extension_point]:
             if logger.isEnabledFor(logging.WARN):
                 logger.warn(
                     "{} is already installed and will be overridden by {}".format(
                         name, self.__class__.__module__ + "." + self.__class__.__name__
                     )
                 )
-        classes[name] = cls
+        extension_points[extension_point][name] = cls
 
     @abstractmethod
     def register(self) -> None:
         ...
 
     def register_binding_filter(self, name: str, cls: type[BindingFilter]):
-        self._register(name, cls, binding_filter_classes)
+        self._register(name, cls, "binding_filter")
 
     def register_checkpoint_manager(self, name: str, cls: type[CheckpointManager]):
-        self._register(name, cls, checkpoint_manager_classes)
+        self._register(name, cls, "checkpoint_manager")
 
     def register_cwl_docker_translator(self, name: str, cls: type[CWLDockerTranslator]):
-        self._register(name, cls, cwl_docker_translator_classes)
+        self._register(name, cls, "cwl_docker_translator")
 
     def register_connector(self, name: str, cls: type[Connector]):
-        self._register(name, cls, connector_classes)
+        self._register(name, cls, "connector")
 
     def register_data_manager(self, name: str, cls: type[DataManager]):
-        self._register(name, cls, data_manager_classes)
+        self._register(name, cls, "data_manager")
 
     def register_database(self, name: str, cls: type[Database]):
-        self._register(name, cls, database_classes)
+        self._register(name, cls, "database")
 
     def register_deployment_manager(self, name: str, cls: type[DeploymentManager]):
-        self._register(name, cls, deployment_manager_classes)
+        self._register(name, cls, "deployment_manager")
 
     def register_failure_manager(self, name: str, cls: type[FailureManager]):
-        self._register(name, cls, failure_manager_classes)
+        self._register(name, cls, "failure_manager")
 
     def register_policy(self, name: str, cls: type[Policy]):
-        self._register(name, cls, policy_classes)
+        self._register(name, cls, "policy")
 
     def register_scheduler(self, name: str, cls: type[Scheduler]):
-        self._register(name, cls, scheduler_classes)
+        self._register(name, cls, "scheduler")
```

### Comparing `streamflow-0.2.0.dev4/streamflow/log_handler.py` & `streamflow-0.2.0.dev5/streamflow/log_handler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/main.py` & `streamflow-0.2.0.dev5/streamflow/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,19 @@
 from streamflow.core.context import StreamFlowContext
 from streamflow.core.exception import WorkflowProvenanceException
 from streamflow.core.provenance import ProvenanceManager
 from streamflow.core.workflow import Workflow
 from streamflow.cwl.main import main as cwl_main
 from streamflow.data import data_manager_classes
 from streamflow.deployment import deployment_manager_classes
-from streamflow.ext.utils import load_extensions
+from streamflow.ext.utils import list_extensions, load_extensions, show_extension
 from streamflow.log_handler import CustomFormatter, HighlitingFilter, logger
 from streamflow.parser import parser
 from streamflow.persistence import database_classes
 from streamflow.persistence.loading_context import DefaultDatabaseLoadingContext
-from streamflow.persistence.sqlite import DEFAULT_SQLITE_CONNECTION
 from streamflow.provenance import prov_classes
 from streamflow.recovery import checkpoint_manager_classes, failure_manager_classes
 from streamflow.scheduling import scheduler_classes
 
 
 async def _async_list(args: argparse.Namespace):
     context = _get_context_from_config(args.file)
@@ -75,14 +74,21 @@
                     print(format_string.format(w["name"], w["type"], w["num"]))
         else:
             print("No workflow objects found.")
     finally:
         await context.close()
 
 
+async def _async_plugin(args: argparse.Namespace):
+    if args.plugin_context == "list":
+        list_extensions()
+    elif args.plugin_context == "show":
+        show_extension(args.plugin, args.name, args.type, args.show_schema)
+
+
 async def _async_prov(args: argparse.Namespace):
     context = _get_context_from_config(args.file)
     try:
         db_context = DefaultDatabaseLoadingContext()
         workflows = await context.database.get_workflows_by_name(
             args.workflow, last_only=not args.all
         )
@@ -119,14 +125,16 @@
             provenance_manager: ProvenanceManager = prov_classes[args.type][wf_type](
                 context, db_context, workflows
             )
             await provenance_manager.create_archive(
                 outdir=args.outdir,
                 filename=args.name,
                 config=args.file if os.path.exists(args.file) else None,
+                additional_files=args.add_file,
+                additional_properties=args.add_property,
             )
     finally:
         await context.close()
 
 
 async def _async_report(args: argparse.Namespace):
     context = _get_context_from_config(args.streamflow_file, args.outdir)
@@ -191,18 +199,15 @@
         {"context": context},
         enabled_by_default=False,
     )
     context.database = _get_instance_from_config(
         config,
         database_classes,
         "database",
-        {
-            "context": context,
-            "connection": DEFAULT_SQLITE_CONNECTION,
-        },
+        {"context": context},
     )
     context.data_manager = _get_instance_from_config(
         config, data_manager_classes, "dataManager", {"context": context}
     )
     context.deployment_manager = _get_instance_from_config(
         config, deployment_manager_classes, "deploymentManager", {"context": context}
     )
@@ -227,14 +232,16 @@
         args = parser.parse_args(args)
         if args.context == "version":
             from streamflow.version import VERSION
 
             print(f"StreamFlow version {VERSION}")
         elif args.context == "list":
             asyncio.run(_async_list(args))
+        elif args.context == "plugin":
+            asyncio.run(_async_plugin(args))
         elif args.context == "prov":
             asyncio.run(_async_prov(args))
         elif args.context == "report":
             asyncio.run(_async_report(args))
         elif args.context == "run":
             if args.quiet:
                 logger.setLevel(logging.WARN)
```

### Comparing `streamflow-0.2.0.dev4/streamflow/persistence/loading_context.py` & `streamflow-0.2.0.dev5/streamflow/persistence/loading_context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/persistence/schemas/sqlite.json` & `streamflow-0.2.0.dev5/streamflow/persistence/schemas/sqlite.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/persistence/schemas/sqlite.sql` & `streamflow-0.2.0.dev5/streamflow/persistence/schemas/sqlite.sql`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/persistence/sqlite.py` & `streamflow-0.2.0.dev5/streamflow/persistence/sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,31 @@
 from __future__ import annotations
 
 import asyncio
 import os
-import sys
-from abc import ABC
 from typing import Any, MutableMapping, MutableSequence
 
 import aiosqlite
 import pkg_resources
-from cachetools import Cache, LRUCache
 
 from streamflow.core import utils
 from streamflow.core.asyncache import cachedmethod
 from streamflow.core.context import StreamFlowContext
 from streamflow.core.deployment import Target
-from streamflow.core.persistence import Database, DependencyType
+from streamflow.core.persistence import DependencyType
 from streamflow.core.utils import get_date_from_ns
 from streamflow.core.workflow import Port, Status, Step, Token
+from streamflow.persistence.base import CachedDatabase
 from streamflow.version import VERSION
 
 DEFAULT_SQLITE_CONNECTION = os.path.join(
     os.path.expanduser("~"), ".streamflow", VERSION, "sqlite.db"
 )
 
 
-class CachedDatabase(Database, ABC):
-    def __init__(self, context: StreamFlowContext):
-        super().__init__(context)
-        self.deployment_cache: Cache = LRUCache(maxsize=sys.maxsize)
-        self.port_cache: Cache = LRUCache(maxsize=sys.maxsize)
-        self.step_cache: Cache = LRUCache(maxsize=sys.maxsize)
-        self.target_cache: Cache = LRUCache(maxsize=sys.maxsize)
-        self.token_cache: Cache = LRUCache(maxsize=sys.maxsize)
-        self.workflow_cache: Cache = LRUCache(maxsize=sys.maxsize)
-
-
 class SqliteConnection:
     def __init__(self, connection: str, timeout: int, init_db: bool):
         self.connection: str = connection
         self.timeout: int = timeout
         self.init_db: bool = init_db
         self._connection: aiosqlite.Connection | None = None
         self.__row_factory = None
@@ -65,15 +52,20 @@
 
     async def close(self):
         if self._connection:
             await self._connection.close()
 
 
 class SqliteDatabase(CachedDatabase):
-    def __init__(self, context: StreamFlowContext, connection: str, timeout: int = 20):
+    def __init__(
+        self,
+        context: StreamFlowContext,
+        connection: str = DEFAULT_SQLITE_CONNECTION,
+        timeout: int = 20,
+    ):
         super().__init__(context)
         # Open connection to database
         if connection != ":memory:":
             os.makedirs(os.path.dirname(connection), exist_ok=True)
         self.connection: SqliteConnection = SqliteConnection(
             connection=connection,
             timeout=timeout,
```

### Comparing `streamflow-0.2.0.dev4/streamflow/provenance/run_crate.py` & `streamflow-0.2.0.dev5/streamflow/provenance/run_crate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import asyncio
 import datetime
 import hashlib
 import json
+import logging
 import os.path
 import posixpath
+import re
 import urllib.parse
 import uuid
 from abc import ABC, abstractmethod
+from json import JSONDecodeError
 from typing import Any, MutableMapping, MutableSequence, cast
 from zipfile import ZipFile
 
 import cwltool.command_line_tool
 import cwltool.context
 import cwltool.process
 import cwltool.workflow
@@ -30,34 +33,39 @@
 from streamflow.core.workflow import Port, Status, Token, Workflow
 from streamflow.log_handler import logger
 from streamflow.version import VERSION
 from streamflow.workflow.token import FileToken, ListToken, ObjectToken
 from streamflow.workflow.utils import get_token_value
 
 
+ESCAPED_COMMA = re.compile(r"\\,")
+ESCAPED_DOT = re.compile(r"\\.")
+ESCAPED_EQUAL = re.compile(r"\\=")
+
+
 def _checksum(data: str) -> str:
     sha1_checksum = hashlib.new("sha1", usedforsecurity=False)
     sha1_checksum.update(data.encode("utf-8"))
     return sha1_checksum.hexdigest()
 
 
 def _file_checksum(path: str, hash_function) -> str:
     with open(path, "rb") as f:
         while data := f.read(2**16):
             hash_function.update(data)
     return hash_function.hexdigest()
 
 
-def _has_type(obj: MutableMapping[str, Any], type: str) -> bool:
+def _has_type(obj: MutableMapping[str, Any], _type: str) -> bool:
     if "@type" not in obj:
         return False
     elif isinstance(obj["@type"], str):
-        return obj["@type"] == type
+        return obj["@type"] == _type
     elif isinstance(obj["@type"], MutableSequence):
-        return type in obj["@type"]
+        return _type in obj["@type"]
     else:
         raise WorkflowProvenanceException(
             f"Invalid type {obj['@type']} for object {obj['@id']}"
         )
 
 
 def _get_action_status(status: Status) -> str:
@@ -154,14 +162,22 @@
         "name": name,
         "input": [],
         "output": [],
         "conformsTo": "https://bioschemas.org/profiles/ComputationalWorkflow/1.0-RELEASE/",
     }
 
 
+def _is_existing_directory(path: str, graph: MutableMapping[str, Any]) -> bool:
+    if path == posixpath.sep:
+        return True
+    else:
+        path = posixpath.relpath(posixpath.normpath(path), posixpath.sep)
+        return graph.get(path, {}).get("@type") == "Directory"
+
+
 def _process_cwl_type(
     cwl_type: str | MutableSequence[Any] | MutableMapping[str, Any],
     jsonld_param: MutableMapping[str, Any],
     cwl_param: MutableMapping[str, Any],
 ) -> None:
     if isinstance(cwl_type, str):
         if cwl_type == "boolean":
@@ -207,14 +223,20 @@
         workflows: MutableSequence[Workflow],
     ):
         super().__init__(context, db_context, workflows)
         self.graph: MutableMapping[str, Any] = {
             "./": {
                 "@id": "./",
                 "@type": "Dataset",
+                "conformsTo": [
+                    {"@id": "https://w3id.org/ro/wfrun/process/0.1"},
+                    {"@id": "https://w3id.org/ro/wfrun/workflow/0.1"},
+                    {"@id": "https://w3id.org/ro/wfrun/provenance/0.1"},
+                    {"@id": "https://w3id.org/workflowhub/workflow-ro-crate/1.0"},
+                ],
                 "datePublished": (
                     datetime.datetime.utcnow()
                     .replace(tzinfo=datetime.timezone.utc)
                     .replace(microsecond=0)
                     .isoformat()
                 ),
                 "hasPart": [],
@@ -224,14 +246,38 @@
                 "@type": "CreativeWork",
                 "about": {"@id": "./"},
                 "conformsTo": [
                     {"@id": "https://w3id.org/ro/crate/1.1"},
                     {"@id": "https://w3id.org/workflowhub/workflow-ro-crate/1.0"},
                 ],
             },
+            "https://w3id.org/ro/wfrun/process/0.1": {
+                "@id": "https://w3id.org/ro/wfrun/process/0.1",
+                "@type": "CreativeWork",
+                "name": "Process Run Crate",
+                "version": "0.1",
+            },
+            "https://w3id.org/ro/wfrun/workflow/0.1": {
+                "@id": "https://w3id.org/ro/wfrun/workflow/0.1",
+                "@type": "CreativeWork",
+                "name": "Workflow Run Crate",
+                "version": "0.1",
+            },
+            "https://w3id.org/ro/wfrun/provenance/0.1": {
+                "@id": "https://w3id.org/ro/wfrun/provenance/0.1",
+                "@type": "CreativeWork",
+                "name": "Provenance Run Crate",
+                "version": "0.1",
+            },
+            "https://w3id.org/workflowhub/workflow-ro-crate/1.0": {
+                "@id": "https://w3id.org/workflowhub/workflow-ro-crate/1.0",
+                "@type": "CreativeWork",
+                "name": "Workflow RO-Crate",
+                "version": "1.0",
+            },
         }
         self.create_action_map: MutableMapping[
             int,
             MutableMapping[
                 str, MutableMapping[str, MutableMapping[str, MutableMapping[str, Any]]]
             ],
         ] = {}
@@ -419,14 +465,72 @@
                 property_value["exampleOfWork"] = [
                     {"@id": eow} for eow in example_of_work
                 ]
             else:
                 property_value["exampleOfWork"] = {"@id": next(iter(example_of_work))}
         return property_values
 
+    async def _list_dir(
+        self, path: str, jsonld_map: [MutableMapping[str, Any]]
+    ) -> MutableSequence[MutableMapping[str, Any]]:
+        has_part = []
+        if os.path.exists(path):
+            dir_content = os.listdir(path)
+            for element in dir_content:
+                element_path = os.path.join(path, element)
+                if os.path.isdir(element_path):
+                    jsonld_object = {"@type": "Dataset"}
+                    if inner_has_part := await self._list_dir(element_path, jsonld_map):
+                        jsonld_object["hasPart"] = inner_has_part
+                        jsonld_object["@id"] = _checksum(
+                            "".join(sorted([part["@id"] for part in inner_has_part]))
+                        )
+                        jsonld_object["alternateName"] = os.path.basename(element_path)
+                    else:
+                        jsonld_object["@id"] = os.path.basename(element_path)
+                else:
+                    checksum = _file_checksum(
+                        element_path, hashlib.new("sha1", usedforsecurity=False)
+                    )
+                    jsonld_object = {
+                        "@id": checksum,
+                        "@type": "File",
+                        "alternateName": os.path.basename(element_path),
+                        "sha1": checksum,
+                    }
+                jsonld_map[jsonld_object["@id"]] = element_path
+                has_part.append(jsonld_object)
+        return has_part
+
+    def _rename_parts(
+        self,
+        parts: MutableSequence[MutableMapping[str, Any]],
+        jsonld_map: MutableMapping[str, str],
+        prefix: str,
+        alternatePrefix: str,
+    ) -> MutableSequence[MutableMapping[str, Any]]:
+        for part in parts:
+            path = jsonld_map.pop(part["@id"])
+            part["@id"] = os.path.join(prefix, part["@id"])
+            if "alternateName" in part:
+                part["alternateName"] = os.path.join(
+                    alternatePrefix, part["alternateName"]
+                )
+            self.files_map[path] = part["@id"]
+            if part["@id"] not in self.graph:
+                self.graph[part["@id"]] = part
+            if part["@type"] == "Dataset" and "hasPart" in part:
+                part["hasPart"] = self._rename_parts(
+                    part["hasPart"],
+                    jsonld_map,
+                    part["@id"],
+                    part.get("alternateName", part["@id"]),
+                )
+        return [{"@id": part["@id"]} for part in parts]
+
     def _update_actions(
         self,
         wf_id: int,
         property_values: MutableMapping[str, MutableMapping[str, Any]],
         step_name: str,
         is_input: bool,
     ) -> None:
@@ -455,20 +559,151 @@
                         ]:
                             jsonld_result = create_action.setdefault("result", [])
                             if property_value["@id"] not in [
                                 res["@id"] for res in jsonld_result
                             ]:
                                 jsonld_result.append({"@id": property_value["@id"]})
 
+    async def add_file(self, file: MutableMapping[str, str]) -> None:
+        if "src" not in file:
+            raise WorkflowProvenanceException(
+                "Property `src` is mandatory when specifying the `--add-file` option."
+            )
+        src = file["src"]
+        dst = file.get("dst", posixpath.sep)
+        dst_parent = posixpath.dirname(posixpath.normpath(dst))
+        if logger.isEnabledFor(logging.WARN):
+            if src in self.files_map:
+                logger.warn(f"File {src} is already present in the archive.")
+        else:
+            if os.path.isfile(os.path.realpath(src)):
+                checksum = _file_checksum(
+                    src, hashlib.new("sha1", usedforsecurity=False)
+                )
+                jsonld_file = {
+                    "@type": "File",
+                    "sha1": checksum,
+                }
+
+                if _is_existing_directory(dst, self.graph):
+                    dst = posixpath.relpath(
+                        posixpath.join(dst, checksum), posixpath.sep
+                    )
+                    jsonld_file["alternateName"] = os.path.basename(src)
+                    if dst_parent != posixpath.dirname:
+                        self.graph[dst_parent].setdefault("hasPart", []).append(
+                            {"@id": dst}
+                        )
+                elif _is_existing_directory(dst_parent, self.graph):
+                    dst = posixpath.relpath(dst, posixpath.sep)
+                    if dst_parent != posixpath.sep:
+                        self.graph[dst_parent].setdefault("hasPart", []).append(
+                            {"@id": dst}
+                        )
+                else:
+                    raise WorkflowProvenanceException(
+                        f"Property `dst` points to the non-existing location `{dst}`."
+                    )
+                jsonld_file["@id"] = dst
+                self.graph[dst] = jsonld_file
+            else:
+                jsonld_dataset = {"@type": "Dataset"}
+                jsonld_map = {}
+                has_part = await self._list_dir(src, jsonld_map)
+                if _is_existing_directory(dst, self.graph):
+                    if has_part:
+                        dst = posixpath.relpath(
+                            posixpath.join(
+                                dst,
+                                _checksum(
+                                    "".join(sorted([part["@id"] for part in has_part]))
+                                ),
+                            ),
+                            posixpath.sep,
+                        )
+                        jsonld_dataset["alternateName"] = os.path.basename(src)
+                    else:
+                        dst = posixpath.relpath(os.path.basename(src), posixpath.sep)
+                    if dst_parent != posixpath.sep:
+                        self.graph[dst_parent].setdefault("hasPart", []).append(
+                            {"@id": dst}
+                        )
+                elif _is_existing_directory(dst_parent, self.graph):
+                    dst = posixpath.relpath(dst, posixpath.sep)
+                    if dst_parent != posixpath.sep:
+                        self.graph[dst_parent].setdefault("hasPart", []).append(
+                            {"@id": dst}
+                        )
+                else:
+                    raise WorkflowProvenanceException(
+                        f"Property `dst` points to the non-existing location `{dst}`."
+                    )
+                jsonld_dataset["@id"] = dst
+                if has_part:
+                    jsonld_dataset["hasPart"] = self._rename_parts(
+                        has_part,
+                        jsonld_map,
+                        dst,
+                        os.path.basename(src),
+                    )
+                    for entry in cast(
+                        MutableSequence[MutableMapping[str, Any]],
+                        jsonld_dataset["hasPart"],
+                    ):
+                        self.graph["./"]["hasPart"].append({"@id": entry["@id"]})
+                self.graph[dst] = jsonld_dataset
+            self.graph["./"]["hasPart"].append({"@id": self.graph[dst]["@id"]})
+            self.files_map[src] = dst
+            for k, v in (
+                (k, v)
+                for k, v in file.items()
+                if k not in ["src", "dst", "@id", "@type"]
+            ):
+                v = ESCAPED_EQUAL.sub("=", v)
+                v = ESCAPED_COMMA.sub(",", v)
+                try:
+                    self.graph[dst][k] = json.loads(v)
+                except JSONDecodeError:
+                    self.graph[dst][k] = v
+
     @abstractmethod
     async def add_initial_inputs(self, wf_id: int, workflow: Workflow) -> None:
         ...
 
+    async def add_property(self, key: str, value: str):
+        current_obj = self.graph
+        keys = re.split(r"(?<!\\)\.", key)
+        for k in keys[:-1]:
+            k = ESCAPED_EQUAL.sub("=", k)
+            k = ESCAPED_COMMA.sub(",", k)
+            k = ESCAPED_DOT.sub(".", k)
+            if k not in current_obj:
+                raise WorkflowProvenanceException(
+                    f"Token `{k}` of key `{key}` does not exist in archive manifest."
+                )
+            current_obj = current_obj[k]
+        if logger.isEnabledFor(logging.WARN):
+            if keys[-1] in current_obj:
+                logger.warn(
+                    f"Key {key} already exists in archive manifest and will be overridden."
+                )
+        value = ESCAPED_EQUAL.sub("=", value)
+        value = ESCAPED_COMMA.sub(",", value)
+        try:
+            current_obj[keys[-1]] = json.loads(value)
+        except JSONDecodeError:
+            current_obj[keys[-1]] = value
+
     async def create_archive(
-        self, outdir: str, filename: str | None, config: str | None
+        self,
+        outdir: str,
+        filename: str | None,
+        config: str | None,
+        additional_files: MutableSequence[MutableMapping[str, str]] | None,
+        additional_properties: MutableSequence[MutableMapping[str, str]] | None,
     ):
         # Add main entity
         main_entity = await self.get_main_entity()
         self.step_map[posixpath.sep] = main_entity
         self.graph[main_entity["@id"]] = main_entity
         self.graph["./"]["hasPart"].append({"@id": main_entity["@id"]})
         self.graph["./"]["mainEntity"] = {"@id": main_entity["@id"]}
@@ -612,14 +847,22 @@
                             ):
                                 self._update_actions(
                                     wf_id=wf_id,
                                     property_values=property_values,
                                     step_name=step_name,
                                     is_input=False,
                                 )
+        # Add additional files
+        for file in additional_files or []:
+            await self.add_file(file)
+        # Add additional properties
+        for prop in additional_properties or []:
+            await asyncio.gather(
+                *(asyncio.create_task(self.add_property(k, v)) for k, v in prop.items())
+            )
         # Create metadata
         metadata = {
             "@context": [
                 "https://w3id.org/ro/crate/1.1/context",
                 {
                     "ParameterConnection": "https://w3id.org/ro/terms/workflow-run#ParameterConnection",
                     "connection": "https://w3id.org/ro/terms/workflow-run#connection",
@@ -685,26 +928,68 @@
         workflows: MutableSequence[Workflow],
     ):
         super().__init__(context, db_context, workflows)
         paths = set()
         for workflow in self.workflows:
             path = workflow.config["file"]
             if not os.path.isabs(path):
-                path = os.path.join(context.config_dir, path)
+                path = os.path.join(os.path.dirname(context.config["path"]), path)
             paths.add(path)
         if len(paths) != 1:
             raise WorkflowProvenanceException(
                 "Cannot build a single workflow provenance for multiple workflow definitions."
             )
         (
             self.cwl_definition,
             self.loading_context,
         ) = streamflow.cwl.utils.load_cwl_workflow(list(paths)[0])
         self.scatter_map: MutableMapping[str, MutableSequence[str]] = {}
 
+    def _add_metadata(
+        self,
+        cwl_object: cwltool.process.Process,
+        jsonld_object: MutableMapping[str, Any],
+    ) -> None:
+        for key, value in cwl_object.metadata.items():
+            if key.startswith("http://schema.org/"):
+                jsonld_object[key[18:]] = self._add_metadata_entry(value)
+            elif key.startswith("https://schema.org/"):
+                jsonld_object[key[19:]] = self._add_metadata_entry(value)
+
+    def _add_metadata_entry(self, metadata: Any) -> Any:
+        if isinstance(metadata, MutableMapping):
+            jsonld_metadata = {}
+            for key in metadata:
+                value = self._add_metadata_entry(metadata[key])
+                if key.startswith("http://schema.org/"):
+                    key = key[18:]
+                elif key.startswith("https://schema.org/"):
+                    key = key[19:]
+                if key == "class":
+                    jsonld_metadata["@type"] = value
+                elif key == "identifier":
+                    jsonld_metadata["@id"] = value
+                else:
+                    jsonld_metadata[key] = value
+            if "@id" not in jsonld_metadata:
+                jsonld_metadata["@id"] = "#" + str(uuid.uuid4())
+            self.graph[jsonld_metadata["@id"]] = jsonld_metadata
+            return {"@id": jsonld_metadata["@id"]}
+        elif isinstance(metadata, MutableSequence):
+            return [self._add_metadata_entry(v) for v in metadata]
+        elif isinstance(metadata, str):
+            if metadata.startswith("http://schema.org/"):
+                return metadata[18:]
+            elif metadata.startswith("https://schema.org/"):
+                return metadata[19:]
+            else:
+                return metadata
+        else:
+            return metadata
+
     def _add_params(
         self,
         cwl_prefix: str,
         prefix: str,
         jsonld_element: MutableMapping[str, Any],
         cwl_element: cwltool.process.Process,
     ) -> None:
@@ -832,14 +1117,16 @@
             "output": [],
             "sha1": _file_checksum(path, hashlib.new("sha1", usedforsecurity=False)),
             "@type": ["SoftwareApplication", "File"],
         }
         # Add description
         if "doc" in cwl_tool.tool:
             jsonld_tool["description"] = cwl_tool.tool["doc"]
+        # Add metadata
+        self._add_metadata(cwl_tool, jsonld_tool)
         # Add inputs and outputs
         self._add_params(cwl_prefix, prefix, jsonld_tool, cwl_tool)
         return jsonld_tool
 
     def _get_workflow(
         self, cwl_prefix: str, prefix: str, cwl_workflow: cwltool.workflow.Workflow
     ) -> MutableMapping[str, Any]:
@@ -853,14 +1140,16 @@
         if (path := cwl_workflow.tool["id"].split("#")[0][7:]) not in self.files_map:
             self.graph["./"]["hasPart"].append({"@id": entity_id})
             self.files_map[path] = os.path.basename(path)
         jsonld_workflow["@type"].append("File")
         # Add description
         if "doc" in cwl_workflow.tool:
             jsonld_workflow["description"] = cwl_workflow.tool["doc"]
+        # Add metadata
+        self._add_metadata(cwl_workflow, jsonld_workflow)
         # Add inputs and outputs
         self._add_params(cwl_prefix, prefix, jsonld_workflow, cwl_workflow)
         # Add steps
         if len(cwl_workflow.steps) > 0:
             jsonld_workflow["step"] = []
             jsonld_steps = [
                 self._get_step(cwl_prefix, prefix, s) for s in cwl_workflow.steps
@@ -961,46 +1250,14 @@
                 dataset["@id"] = token_value["basename"]
             return dataset
         else:
             raise WorkflowDefinitionException(
                 f"Invalid class {token_value['class']} for file token."
             )
 
-    async def _list_dir(
-        self, path: str, jsonld_map: [MutableMapping[str, Any]]
-    ) -> MutableSequence[MutableMapping[str, Any]]:
-        has_part = []
-        if os.path.exists(path):
-            dir_content = os.listdir(path)
-            for element in dir_content:
-                element_path = os.path.join(path, element)
-                if os.path.isdir(element_path):
-                    jsonld_object = {"@type": "Dataset"}
-                    if inner_has_part := await self._list_dir(element_path, jsonld_map):
-                        jsonld_object["hasPart"] = inner_has_part
-                        jsonld_object["@id"] = _checksum(
-                            "".join(sorted([part["@id"] for part in inner_has_part]))
-                        )
-                        jsonld_object["alternateName"] = os.path.basename(element_path)
-                    else:
-                        jsonld_object["@id"] = os.path.basename(element_path)
-                else:
-                    checksum = _file_checksum(
-                        element_path, hashlib.new("sha1", usedforsecurity=False)
-                    )
-                    jsonld_object = {
-                        "@id": checksum,
-                        "@type": "File",
-                        "alternateName": os.path.basename(element_path),
-                        "sha1": checksum,
-                    }
-                jsonld_map[jsonld_object["@id"]] = element_path
-                has_part.append(jsonld_object)
-        return has_part
-
     def _register_steps(
         self,
         cwl_prefix: str,
         prefix: str,
         jsonld_entity: MutableMapping[str, Any],
         jsonld_steps: MutableSequence[MutableMapping[str, Any]],
         cwl_steps: MutableSequence[cwltool.workflow.WorkflowStep],
@@ -1057,34 +1314,14 @@
                             self.graph[connection["@id"]] = connection
                             jsonld_step.setdefault("connection", []).append(
                                 {"@id": connection["@id"]}
                             )
                             break
         jsonld_entity["hasPart"] = [{"@id": p} for p in has_part]
 
-    def _rename_parts(
-        self,
-        parts: MutableSequence[MutableMapping[str, Any]],
-        jsonld_map: MutableMapping[str, str],
-        prefix: str,
-        alternatePrefix: str,
-    ) -> MutableSequence[MutableMapping[str, Any]]:
-        for part in parts:
-            path = jsonld_map.pop(part["@id"])
-            part["@id"] = os.path.join(prefix, part["@id"])
-            part["alternateName"] = os.path.join(alternatePrefix, part["alternateName"])
-            self.files_map[path] = part["@id"]
-            if part["@id"] not in self.graph:
-                self.graph[part["@id"]] = part
-            if part["@type"] == "Dataset" and "hasPart" in part:
-                part["hasPart"] = self._rename_parts(
-                    part["hasPart"], jsonld_map, part["@id"], part["alternateName"]
-                )
-        return [{"@id": part["@id"]} for part in parts]
-
     async def add_initial_inputs(self, wf_id: int, workflow: Workflow) -> None:
         if "settings" in workflow.config:
             cwl_prefix = (
                 streamflow.cwl.utils.get_name(
                     posixpath.sep, posixpath.sep, self.cwl_definition.tool["id"]
                 )
                 if "#" in self.cwl_definition.tool["id"]
@@ -1126,14 +1363,16 @@
         main_entity["sha1"] = _file_checksum(
             path, hashlib.new("sha1", usedforsecurity=False)
         )
         # Add programming language
         programming_language = _get_cwl_programming_language(self.loading_context)
         self.graph[programming_language["@id"]] = programming_language
         main_entity["programmingLanguage"] = {"@id": programming_language["@id"]}
+        # Add metadata
+        self._add_metadata(self.cwl_definition, main_entity)
         # Add inputs and outputs
         self._add_params(cwl_prefix, posixpath.sep, main_entity, self.cwl_definition)
         # Add steps if present
         if (
             isinstance(self.cwl_definition, cwltool.workflow.Workflow)
             and len(self.cwl_definition.steps) > 0
         ):
```

### Comparing `streamflow-0.2.0.dev4/streamflow/recovery/checkpoint_manager.py` & `streamflow-0.2.0.dev5/streamflow/recovery/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/recovery/failure_manager.py` & `streamflow-0.2.0.dev5/streamflow/recovery/failure_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/recovery/recovery.py` & `streamflow-0.2.0.dev5/streamflow/recovery/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/report.py` & `streamflow-0.2.0.dev5/streamflow/report.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/scheduling/policy/data_locality.py` & `streamflow-0.2.0.dev5/streamflow/scheduling/policy/data_locality.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/scheduling/scheduler.py` & `streamflow-0.2.0.dev5/streamflow/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/workflow/combinator.py` & `streamflow-0.2.0.dev5/streamflow/workflow/combinator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/workflow/executor.py` & `streamflow-0.2.0.dev5/streamflow/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/workflow/port.py` & `streamflow-0.2.0.dev5/streamflow/workflow/port.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/workflow/step.py` & `streamflow-0.2.0.dev5/streamflow/workflow/step.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/workflow/token.py` & `streamflow-0.2.0.dev5/streamflow/workflow/token.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/workflow/transformer.py` & `streamflow-0.2.0.dev5/streamflow/workflow/transformer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow/workflow/utils.py` & `streamflow-0.2.0.dev5/streamflow/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/streamflow.egg-info/PKG-INFO` & `streamflow-0.2.0.dev5/streamflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev4
+Version: 0.2.0.dev5
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
```

### Comparing `streamflow-0.2.0.dev4/streamflow.egg-info/SOURCES.txt` & `streamflow-0.2.0.dev5/streamflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 streamflow/deployment/filter/shuffle.py
 streamflow/deployment/filter/schemas/shuffle.json
 streamflow/deployment/schemas/deployment_manager.json
 streamflow/ext/__init__.py
 streamflow/ext/plugin.py
 streamflow/ext/utils.py
 streamflow/persistence/__init__.py
+streamflow/persistence/base.py
 streamflow/persistence/loading_context.py
 streamflow/persistence/sqlite.py
 streamflow/persistence/schemas/sqlite.json
 streamflow/persistence/schemas/sqlite.sql
 streamflow/provenance/__init__.py
 streamflow/provenance/run_crate.py
 streamflow/recovery/__init__.py
```

### Comparing `streamflow-0.2.0.dev4/streamflow.egg-info/requires.txt` & `streamflow-0.2.0.dev5/streamflow.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 aiohttp==3.8.4
-aiosqlite==0.18.0
+aiosqlite==0.19.0
 antlr4-python3-runtime==4.12.0
 asyncssh==2.13.1
 bcrypt==4.0.1
 cachetools==5.3.0
-cwltool==3.1.20230325110543
-cwl-utils==0.23
-importlib_metadata==6.3.0
+cwltool==3.1.20230425144158
+cwl-utils==0.25
+importlib_metadata==6.6.0
 Jinja2==3.1.2
 jsonref==1.1.0
 jsonschema==4.17.3
-kubernetes_asyncio==24.2.2
-psutil==5.9.4
+kubernetes_asyncio==24.2.3
+psutil==5.9.5
 rdflib==6.3.2
 yattag==1.15.1
 
 [bandit]
 bandit==1.7.5
 
 [docs]
-sphinx==6.1.3
+sphinx==7.0.0
 sphinx-jsonschema==1.19.1
 sphinx-rtd-theme==1.2.0
 
 [lint]
 black==23.3.0
 codespell==2.2.4
 flake8-bugbear==23.3.23
-pyupgrade==3.3.1
+pyupgrade==3.3.2
 
 [report]
-pandas==2.0.0
+pandas==2.0.1
 plotly==5.14.1
 kaleido==0.2.1.post1
 
 [test]
 cwltest==2.3.20230108193615
-pytest==7.3.0
+pytest==7.3.1
 pytest-asyncio==0.21.0
 pytest-cov==4.0.0
 pytest-xdist==3.2.1
```

### Comparing `streamflow-0.2.0.dev4/tests/test_cwl_loop.py` & `streamflow-0.2.0.dev5/tests/test_cwl_loop.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/tests/test_cwl_persistence.py` & `streamflow-0.2.0.dev5/tests/test_cwl_persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/tests/test_persistence.py` & `streamflow-0.2.0.dev5/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/tests/test_remotepath.py` & `streamflow-0.2.0.dev5/tests/test_remotepath.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/tests/test_scheduler.py` & `streamflow-0.2.0.dev5/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev4/tests/test_transfer.py` & `streamflow-0.2.0.dev5/tests/test_transfer.py`

 * *Files identical despite different names*

