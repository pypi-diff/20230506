# Comparing `tmp/iambic_core-0.6.1.tar.gz` & `tmp/iambic_core-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.6.1.tar", max compression
+gzip compressed data, was "iambic_core-0.6.3.tar", max compression
```

## Comparing `iambic_core-0.6.1.tar` & `iambic_core-0.6.3.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0    11356 2023-05-03 18:51:35.034421 iambic_core-0.6.1/LICENSE.md
--rw-r--r--   0        0        0    10551 2023-05-03 18:51:35.034421 iambic_core-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/config/__init__.py
--rw-r--r--   0        0        0    20099 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/config/templates.py
--rw-r--r--   0        0        0     1955 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/config/utils.py
--rw-r--r--   0        0        0    74794 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/core/context.py
--rw-r--r--   0        0        0      609 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/core/logger.py
--rw-r--r--   0        0        0    24862 2023-05-03 18:51:35.058421 iambic_core-0.6.1/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/core/noq_json.py
--rw-r--r--   0        0        0     5244 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/core/parser.py
--rw-r--r--   0        0        0    46094 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/core/template_generation.py
--rw-r--r--   0        0        0    26626 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/lambda/app.py
--rw-r--r--   0        0        0    13694 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/main.py
--rw-r--r--   0        0        0      664 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/output/__init__.py
--rw-r--r--   0        0        0     2799 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1753 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     2149 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     2268 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
--rw-r--r--   0        0        0     2483 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     1902 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    14509 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0      660 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    33385 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10334 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    17683 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13616 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15824 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    17544 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10649 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16135 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21304 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    24395 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14064 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    20623 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22579 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     4534 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    31619 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20296 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35514 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    28137 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0     1086 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0     2973 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/template_generation.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-05-03 18:51:35.062420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    10183 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    13766 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8515 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8648 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      908 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     3366 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      284 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14549 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5247 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1154 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7852 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9282 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11393 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    20065 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2685 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1085 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9492 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13610 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      864 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      977 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      137 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12636 2023-05-03 18:51:35.066420 iambic_core-0.6.1/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     1922 2023-05-03 18:51:35.070420 iambic_core-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 iambic_core-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-06 19:36:22.982867 iambic_core-0.6.3/LICENSE.md
+-rw-r--r--   0        0        0    10551 2023-05-06 19:36:22.982867 iambic_core-0.6.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/__init__.py
+-rw-r--r--   0        0        0    20099 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0      460 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/templates.py
+-rw-r--r--   0        0        0     1955 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/utils.py
+-rw-r--r--   0        0        0    74846 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15217 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4592 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1685 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/logger.py
+-rw-r--r--   0        0        0    24862 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5516 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/parser.py
+-rw-r--r--   0        0        0    46094 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    26626 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/lambda/app.py
+-rw-r--r--   0        0        0    13694 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2799 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1753 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     2149 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     2268 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     2483 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     1902 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    14509 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    33385 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    17683 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13616 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15824 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    17544 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10649 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21304 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24395 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    20623 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22579 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     4534 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31619 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35514 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    28137 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0     1086 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     2973 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10183 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    13766 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3746 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2267 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     1795 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8515 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8648 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3709 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0      908 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    31334 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    11851 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     1553 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5345 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14549 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5247 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1154 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7852 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3020 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3167 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9282 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3105 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11393 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3535 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2478 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2685 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1085 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9492 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3424 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13610 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0      864 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4110 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      977 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      137 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     1922 2023-05-06 19:36:23.018868 iambic_core-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 iambic_core-0.6.3/PKG-INFO
```

### Comparing `iambic_core-0.6.1/LICENSE.md` & `iambic_core-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/README.md` & `iambic_core-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/config/dynamic_config.py` & `iambic_core-0.6.3/iambic/config/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/config/utils.py` & `iambic_core-0.6.3/iambic/config/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/config/wizard.py` & `iambic_core-0.6.3/iambic/config/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         self._cf_role_arn = None
         self._assume_as_arn = None
         self.caller_identity = {}
         self.profile_name = ""
         self._default_region = None
 
         asyncio.run(self.set_config_details())
-
+        check_and_update_resource_limit(self.config)
         log.debug("Starting configuration wizard", config_path=self.config_path)
 
     @property
     def has_cf_permissions(self):
         if self._has_cf_permissions is None:
             try:
                 click.echo(
```

### Comparing `iambic_core-0.6.1/iambic/core/aio_utils/__init__.py` & `iambic_core-0.6.3/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/core/exceptions.py` & `iambic_core-0.6.3/iambic/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/core/git.py` & `iambic_core-0.6.3/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/core/iambic_enum.py` & `iambic_core-0.6.3/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/core/iambic_plugin.py` & `iambic_core-0.6.3/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/core/logger.py` & `iambic_core-0.6.3/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/core/models.py` & `iambic_core-0.6.3/iambic/core/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/core/noq_json.py` & `iambic_core-0.6.3/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/core/parser.py` & `iambic_core-0.6.3/iambic/core/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,25 +89,36 @@
             "Invalid template structure", file_path=template_path, error=repr(err)
         )
         if raise_validation_err:
             raise ValueError(f"{template_path} template has validation error.") from err
 
 
 def load_templates(
-    template_paths: list[str], raise_validation_err: bool = True
+    template_paths: list[str],
+    raise_validation_err: bool = True,
+    use_multiprocessing=True,
 ) -> list[BaseTemplate]:
     templates = []
-    load_template_fn = partial(load_template, raise_validation_err=raise_validation_err)
-    with Pool(max(1, cpu_count() // 2)) as p:
-        template_dicts = p.map(load_template_fn, template_paths)
-        if getattr(sys, "gettrace", None):
-            # When in debug mode, subprocesses can exit
-            # before debugger can attach
-            # https://github.com/microsoft/debugpy/issues/712
-            time.sleep(0.5)
+    template_dicts = None
+
+    if use_multiprocessing:
+        load_template_fn = partial(
+            load_template, raise_validation_err=raise_validation_err
+        )
+        with Pool(max(1, cpu_count() // 2)) as p:
+            template_dicts = p.map(load_template_fn, template_paths)
+            if getattr(sys, "gettrace", None):
+                # When in debug mode, subprocesses can exit
+                # before debugger can attach
+                # https://github.com/microsoft/debugpy/issues/712
+                time.sleep(0.5)
+    else:
+        template_dicts = [
+            load_template(path, raise_validation_err) for path in template_paths
+        ]
 
     for template_dict in template_dicts:
         if not template_dict:
             continue
 
         try:
             template_cls = TEMPLATES.template_map[template_dict["template_type"]]
```

### Comparing `iambic_core-0.6.1/iambic/core/template_generation.py` & `iambic_core-0.6.3/iambic/core/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/core/utils.py` & `iambic_core-0.6.3/iambic/core/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.6.3/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.6.3/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.6.3/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/github/templates/iambic-import.yml` & `iambic_core-0.6.3/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/github/utils.py` & `iambic_core-0.6.3/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/lambda/app.py` & `iambic_core-0.6.3/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/main.py` & `iambic_core-0.6.3/iambic/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/output/__init__.py` & `iambic_core-0.6.3/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/output/filters.py` & `iambic_core-0.6.3/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/output/models.py` & `iambic_core-0.6.3/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.6.3/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.6.3/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.6.3/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/output/text.py` & `iambic_core-0.6.3/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/README.md` & `iambic_core-0.6.3/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/request_handler/expire_resources.py` & `iambic_core-0.6.3/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/request_handler/git_apply.py` & `iambic_core-0.6.3/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/request_handler/git_plan.py` & `iambic_core-0.6.3/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.1/pyproject.toml` & `iambic_core-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.6.1"
+version = "0.6.3"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
```

### Comparing `iambic_core-0.6.1/PKG-INFO` & `iambic_core-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.6.1
+Version: 0.6.3
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

