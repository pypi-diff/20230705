# Comparing `tmp/compliance-trestle-2.2.0.tar.gz` & `tmp/compliance-trestle-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compliance-trestle-2.2.0.tar", last modified: Mon Jun 26 21:32:06 2023, max compression
+gzip compressed data, was "compliance-trestle-2.2.1.tar", last modified: Wed Jul  5 18:23:15 2023, max compression
```

## Comparing `compliance-trestle-2.2.0.tar` & `compliance-trestle-2.2.1.tar`

### file list

```diff
@@ -1,1637 +1,1637 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.585586 compliance-trestle-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.265584 compliance-trestle-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.265584 compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/new_collaborator.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/proposed_change.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.265584 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/develop.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/hotfix.md
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/release.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/dco.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.269584 compliance-trestle-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/workflows/conventional-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/workflows/python-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.pylintrc_tests
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/.yapf-config
--rw-r--r--   0 runner    (1001) docker     (123)    92397 2023-06-26 21:32:03.000000 compliance-trestle-2.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/DCO1.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-06-26 21:32:06.585586 compliance-trestle-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.269584 compliance-trestle-2.2.0/compliance_trestle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    97672 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 21:32:06.000000 compliance-trestle-2.2.0/compliance_trestle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.269584 compliance-trestle-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.common_types.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.const.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.err.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.file_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.list_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.load_validate.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.log.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.model_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.str_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.trash.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.common.type_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.all_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.base_model.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_api.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_interface.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_merger.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_reader.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog.catalog_writer.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.catalog_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.add.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.assemble.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.command.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.common.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.component.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.consts.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.docs.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.folders.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.headers.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.profile.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.ssp.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.author.versioning.template_versioning.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.command_docs.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.common.cmd_utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.common.return_codes.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.create.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.describe.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.href.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.import_.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.init.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.merge.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.partial_object_validate.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.remove.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.replicate.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.split.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.task.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.validate.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.commands.version.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.control_context.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.control_interface.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.control_reader.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.control_writer.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.docs_control_writer.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.draw_io.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.duplicates_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.generators.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.generic_oscal.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.links_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.base_markdown_node.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.control_markdown_node.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.docs_markdown_node.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.markdown_api.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.markdown_const.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.markdown_processor.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.markdown_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.markdown.md_writer.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.actions.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.elements.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.file_content_type.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.interfaces.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.models.plans.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.object_factory.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.parser.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.pipeline.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.profile_resolver.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.refs_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.remote.cache.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.repository.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.resolver.merge.md
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.resolver.modify.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.resolver.prune.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.rule_parameters_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.ssp_io.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.trestle_base_model.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.validator.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.core.validator_factory.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.assessment_plan.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.assessment_results.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.common.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.component.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.poam.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.profile.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.oscal.ssp.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.base_task.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.cis_xlsx_to_oscal_catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.csv_to_oscal_cd.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_cd.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.oscal_catalog_to_csv.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.oscal_profile_to_osco_profile.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.osco_result_to_oscal_ar.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.tanium_result_to_oscal_ar.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.transform.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.xccdf_result_to_oscal_ar.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.xlsx_helper.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.xlsx_to_oscal_cd.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.tasks.xlsx_to_oscal_profile.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.implementations.osco.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.implementations.tanium.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.implementations.xccdf.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.results.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.transformer_factory.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.transformer_helper.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/api_reference/trestle.transforms.transformer_singleton.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   161907 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/Canonical_trestle_auditree_workflows.png
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/README
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/canonical_trestle_auditree_workflows.drawio
--rw-r--r--   0 runner    (1001) docker     (123)   329379 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/drawio_data_menu.png
--rw-r--r--   0 runner    (1001) docker     (123)   264094 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/drawio_editing_data.png
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/sample_ssp.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    44185 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/assets/template_versioning.png
--rw-r--r--   0 runner    (1001) docker     (123)    58223 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/cli.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/DCO.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/mkdocs_contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/trestle_oscal_object_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/contributing/website.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/demonstrations-content.md
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/errors.md
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/maintainers.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/mkdocs_code_of_conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.289584 compliance-trestle-2.2.0/docs/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/plugins/compliance-trestle-fedramp.md
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/python_trestle_setup.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)   146161 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.png
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/reference/third-party-result-schema-SCC.md
--rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/trestle_author.md
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/trestle_author_jinja.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/ContinuousCompliance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/ContinuousCompliance.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/continuous-compliance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.png
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/profile_does.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    37208 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/profile_does.png
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.png
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    67327 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.png
--rw-r--r--   0 runner    (1001) docker     (123)    76787 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring.md
--rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_options.docx
--rw-r--r--   0 runner    (1001) docker     (123)    75117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/trestle_ssp_author_options.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.293584 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/component-definition.json
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/demo-csv-to-oscal-cd.config
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/ocp4-sample-input.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/transformation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/demo-ocp4-cis-profile-to-oscal-catalog.config
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/transformation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/demo-ocp4-cis-profile-to-oscal-cd.config
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/enabled_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/selected_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/transformation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.copyright-info.txt
--rw-r--r--   0 runner    (1001) docker     (123)   111352 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/transformation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/
--rw-r--r--   0 runner    (1001) docker     (123)    56735 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results-nist.png
--rw-r--r--   0 runner    (1001) docker     (123)   100092 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    43615 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.md
--rw-r--r--   0 runner    (1001) docker     (123)    27754 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/docs/tutorials/trestle_sample_workflow.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.297584 compliance-trestle-2.2.0/internal_spec_documents/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/internal_spec_documents/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/internal_spec_documents/caching_spec.md
--rw-r--r--   0 runner    (1001) docker     (123)    30894 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/internal_spec_documents/trestle-spec.md
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/internal_spec_documents/trestle-task-spec.md
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.301584 compliance-trestle-2.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.301584 compliance-trestle-2.2.0/scripts/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/json_serialize_ben.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/profile_json_seriallze_ben.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/profile_tanium_ben.sh
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/profiling_tools_setup_OSX.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/experiments/tanium_ben.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/flatten_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/gen_oscal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/have_files_changed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/order_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    35528 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/oscal_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/schema_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/simplify_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/simplify_retain_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/tanium_transform_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/update_uuids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/utf8me.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/scripts/website_automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-26 21:32:06.585586 compliance-trestle-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.301584 compliance-trestle-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.261583 compliance-trestle-2.2.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.301584 compliance-trestle-2.2.0/tests/data/author/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.237583 compliance-trestle-2.2.0/tests/data/author/0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.305584 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/not_mxfile.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_extra_fields_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_missing_fields_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_metadata_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_metadata_uncompressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_bad_internal_structure.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed_mangled.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_compressed.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_bad_md.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_compressed.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.305584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_bold_heading.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_heading_wrong_type.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_missing_heading.md
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_no_header.md
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_reordered.md
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/bad_instance_yaml_header_change.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/correct_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/correct_instance_extra_features.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/template.md
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_1_md_format/yaml_header_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.305584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/bad_heading_content_changed_header.md
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/bad_heading_content_extra_lines.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/template.md
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/wrong_heading_title.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.305584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_000.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_001.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_002.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_bold_heading.md
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_heading_wrong_type.md
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_missing_heading.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_reordered.md
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_yaml_header_change.md
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance_extra_features.md
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/bad_added_header.md
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/bad_modified_header_deep.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/correct_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/correct_instance_empty_subs.md
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_substitutions/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/__ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/correct_instance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/correct_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/0.0.1/test_5_md_ignored/template.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/bad_md_header.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.309584 compliance-trestle-2.2.0/tests/data/author/controls/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_no_labels.md
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_some_labels.md
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_bad_component.md
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_bad_system_comp.md
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_components.md
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_components_and_param_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_components_and_params.md
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/controls/control_with_double_comp.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.237583 compliance-trestle-2.2.0/tests/data/author/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/docs/candidate_invalid_readme/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_invalid_readme/correct_instance_extra_features.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_invalid_readme/not_valid.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_invalid_readme/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/docs/candidate_valid_readme/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_valid_readme/correct_instance_extra_features.md
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_valid_readme/correct_instance_extra_features_2.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/candidate_valid_readme/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_invalid/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_invalid/extra_file.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_invalid/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_invalid/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_valid_with_readme/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_valid_with_readme/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/docs/template_folder_valid_with_readme/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_folder_is_a_file
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_bad_content/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_bad_content/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_bad_content/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_missing/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_missing/architecture.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_mixed_name/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_mixed_name/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_mixed_name/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_no_header/subdir/architecture.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_renamed/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_renamed/architecture_really_bad.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_renamed/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.313584 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_limits_of_changes/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_limits_of_changes/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_limits_of_changes/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/.hidden_test
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/network.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/__ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/_ignore_not_instance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/diagram.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore_not_instance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/architecture.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.317584 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/.hidden_does_not_affect
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/network.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_with_readme/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_with_readme/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_with_readme/network.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/template_with_readme/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/utf16test_bad/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/utf16test_bad/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/governed_folders/utf16test_good/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/governed_folders/utf16test_good/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_drawio/template.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_drawio/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_md/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_md/template.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_md/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_wrong_names/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_wrong_names/templatesss.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_wrong_names/templatessss.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/b copy.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/b.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio/a_file.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio/whos_is_this.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio_bad_file/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio_bad_file/a_markdown_file.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio_bad_file/another_file.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.321584 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md/my_drawio.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md/my_md.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md_bad_file/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md_bad_file/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md_bad_file/b.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/global/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/good/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/global/good/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/good/catalogs/my_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/catalogs/my_catalog/catalogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/good/sample_indexable_1/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/sample_indexable_1/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/good/sample_indexable_2/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/sample_indexable_2/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/good/unindexed.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/bad_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/bad_sample/bad_sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/catalogs/my_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/catalogs/my_catalog/catalogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_1/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_1/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_2/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_2/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_exceptions/unindexed.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.241583 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/my_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/my_catalog/catalogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/bad/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/bad/bad_sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/good/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/good/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/nested/sample.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/sample_indexable_1/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/sample_indexable_1/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/global/pass_with_nested_exceptions/unindexed.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/good_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/good_templates/template.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/good_templates/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.325584 compliance-trestle-2.2.0/tests/data/author/headers/good_templates_wo_drawio/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/good_templates_wo_drawio/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/__ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/_ignore_not_instance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_b.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_instance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/_ignore_not_instance.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/correct_instance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore_not_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/correct_a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/correct_instance.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/b.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/d.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/b.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/d.drawio
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/irrelevant.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/b copy.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/b.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/d.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/a.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/b copy.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/b.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/d.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.329584 compliance-trestle-2.2.0/tests/data/author/ssp/
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/ssp/ssp_example.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/author/utf16test/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/utf16test/sample_okay.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/utf16test/sample_utf16.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/author/versions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/author/versions/1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.0.0/bad_template_wrong_folder.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.0.0/good_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/bad_instance_mismatched_versions.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/bad_template_mismatched_versions.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/good_instance.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/1.1.0/good_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/bad_template_with_version_outside_structure.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/author/versions/good_instance_with_version_outside_structure.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/csv/
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/csv/bp.sample.v2.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/csv/component-definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/csv/component-definitions/bp/
--rw-r--r--   0 runner    (1001) docker     (123)    42744 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/csv/component-definitions/bp/component-definition.json
--rw-r--r--   0 runner    (1001) docker     (123)    54973 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/csv/ocp4-user.v2.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.333584 compliance-trestle-2.2.0/tests/data/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/lookup_table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_invalid.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_no_part_prose.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_only_some_sections.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_with_group_title.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_with_subparts.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/ssp_template.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/ssp_template_no_input_profile_ssp.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/sub_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/sub_content_with_subs.md
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja/use_lookup_table.md.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.337584 compliance-trestle-2.2.0/tests/data/jinja_cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_cmd/empty_test.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_cmd/number_captions_data.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_cmd/number_captions_expected_output.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.337584 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDDatestamp_default.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDDatestamp_format.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDDatestamp_invalid.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDDatestamp_newline.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_nested.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_nested.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_top_level.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_top_level.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_top_level_adjusted.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/MDSection_include_top_level_adjusted.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_include.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_include.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_include_adjusted.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_include_adjusted.md
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c.md
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c_double.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c_double.md
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_n.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_n.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/nested_c.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/nested_n.jinja.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/jinja_markdown_include/test_markdown.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.345584 compliance-trestle-2.2.0/tests/data/json/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/bad_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)    21655 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_def.json
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_def_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_def_b.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_def_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof.json
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_aa.json
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_ab.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_ba.json
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_bad.json
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_bb.json
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/comp_prof_part_none.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/good_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/leveraged_ssp.json
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/leveraged_ssp_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_bad_oscal_version.json
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_extra_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_missing_roles.json
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_missing_uuid.json
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_no_responsible-parties.json
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles.json
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles_double.json
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles_double_rp.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/minimal_catalog_with_groups.json
--rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/nist_tutorial_catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/nist_tutorial_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_bad_control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_missing_position.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_with_alter_props.json
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_with_alter_subparts.json
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/profile_with_incorrect_alter.json
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/pull_nist_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_catalog_no_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile_less.json
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile_more.json
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile_no_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simple_test_profile_single.json
--rw-r--r--   0 runner    (1001) docker     (123)   221136 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simplified_nist_catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/simplified_nist_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_b.json
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_c.json
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_d.json
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_e.json
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_f.json
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/json/test_profile_g.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.345584 compliance-trestle-2.2.0/tests/data/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_complex_md.md
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_levels_no_text.md
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_levels_no_text_increased_level.md
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_no_headers.md
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/markdown/valid_no_lvl1_headers.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.345584 compliance-trestle-2.2.0/tests/data/ocp4-cis/
--rw-r--r--   0 runner    (1001) docker     (123)    23806 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/ocp4-cis/catalog.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.349584 compliance-trestle-2.2.0/tests/data/split_merge/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.349584 compliance-trestle-2.2.0/tests/data/split_merge/.trestle/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/.trestle/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.353584 compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/
--rw-r--r--   0 runner    (1001) docker     (123)  3169371 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/groups.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.357584 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.357584 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/
--rw-r--r--   0 runner    (1001) docker     (123)  4498050 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/next_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.361584 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.361584 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.369584 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/back-matter.json
--rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/groups.json
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/next_step.sh
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/previous_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.369584 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.369584 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.373584 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/back-matter.json
--rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/groups.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.373584 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/parties.json
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/responsible-parties.json
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/roles.json
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/next_step.sh
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/previous_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.373584 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.373584 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.377585 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/back-matter.json
--rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/groups.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/parties.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/00000__responsible-party.json
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/00001__responsible-party.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/00000__role.json
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/00001__role.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles.json
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/next_step.sh
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/previous_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.245583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.381585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/back-matter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.385584 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.389585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    48380 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    54960 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    70506 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    30598 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00023__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00024__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.389585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18701 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.393585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15966 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.393585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    24785 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.397585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    34660 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    28847 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.397585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    29166 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    21335 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.401585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    51627 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.401585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    38793 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.405585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.405585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.413585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    24929 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.413585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.421585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00023__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00024__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00025__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00026__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00027__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00028__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00029__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00030__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00031__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.425585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.425585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.429585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    30706 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.433585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    42212 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)   101326 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    25087 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    32683 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    37819 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.449585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    72606 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00023__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00024__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00025__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00026__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00027__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00028__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00029__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00030__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00031__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00032__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00033__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00034__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00035__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00036__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00037__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00038__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00039__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00040__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00041__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00042__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00043__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00044__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00045__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00046__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00047__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00048__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00049__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00050__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.453585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    67388 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    36771 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00012__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00013__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00014__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00015__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00016__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00017__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00018__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00019__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00020__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00021__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00022__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.249583 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.457585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00000__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00001__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00002__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00003__control.json
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00004__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00005__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00006__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00007__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00008__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00009__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00010__control.json
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00011__control.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.457585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/parties.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.457585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/00000__responsible-party.json
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/00001__responsible-party.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.457585 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/00000__role.json
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/00001__role.json
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/next_step.sh
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/previous_step.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.461585 compliance-trestle-2.2.0/tests/data/spread-sheet/
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/bad_parameter_name_and_description.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/duplicate_column_heading.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_goal_name_id.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_parameter_name.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_rule_name_id.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/good.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/good_with_blank_rows.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/missing_column_heading.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/missing_control_id.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/missing_resource_title.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/spread-sheet/missing_rule_name_id.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.257583 compliance-trestle-2.2.0/tests/data/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.461585 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_RedHat_OpenShift_Container_Platform_Benchmark_v1.2.0-2.snippet.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.snippet.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/test-cis-xlsx-to-oscal-catalog.ocp.config
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/test-cis-xlsx-to-oscal-catalog.rhel.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.461585 compliance-trestle-2.2.0/tests/data/tasks/csv-to-oscal-cd/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/csv-to-oscal-cd/test-csv-to-oscal-cd-bp.config
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/csv-to-oscal-cd/test-csv-to-oscal-cd.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.461585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/cis.profile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/cis.profile
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/test-ocp4-cis-profile-to-oscal-catalog.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.253584 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.253584 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_cni_conf/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_cni_conf/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_apiserver/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_controller_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_controller_manager/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_cni_conf/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_cni_conf/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_apiserver/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_controller_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_controller_manager/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_apiserver/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_controller_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_controller_manager/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_memory_available/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_memory_available/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.465585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_nodefs_available/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_nodefs_available/rule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules2.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules3.json
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/rule2var.json
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/
--rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/component-definition.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.253584 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.253584 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis-node.profile
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis.profile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test.profile
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test2.profile
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test3.profile
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd.config
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd2.config
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd3.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.469585 compliance-trestle-2.2.0/tests/data/tasks/oscal-catalog-to-csv/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-catalog-to-csv/test-oscal-catalog-to-csv-rev-5-by-control.config
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-catalog-to-csv/test-oscal-catalog-to-csv-rev-5-by-statement.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.473585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-no.json
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-yes.json
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-no.json
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-yes.json
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.2.0-parms-no.json
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-1.0.0-parms-yes.json
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-no.json
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-yes.json
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-scc.json
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-no.config
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-yes.config
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-no.config
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-yes.config
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.2.0-parms-no.config
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-1.0.0-parms-yes.config
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-bogus.config
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-input-file.config
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-output-dir.config
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-overwrite.config
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-parms-no.config
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-parms-yes.config
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-scc.config
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-set.config
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.257583 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/tailored-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.477585 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output-set/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output-set/osco-profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input/ignore.me
--rw-r--r--   0 runner    (1001) docker     (123)    52753 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    52859 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-bad-yaml/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-bad-yaml/bad.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.481585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-compressed/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-configmaps/
--rw-r--r--   0 runner    (1001) docker     (123)   608191 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-configmaps/configmaps.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/
--rw-r--r--   0 runner    (1001) docker     (123)   105678 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource.json
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_resources.json
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-ocp4/
--rw-r--r--   0 runner    (1001) docker     (123)    78761 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-ocp4/ocp4-check-result.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-rhel7/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-rhel7/rhel7-check-result.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/output/
--rw-r--r--   0 runner    (1001) docker     (123)   155263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.485585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)   155462 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.489585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-compressed/
--rw-r--r--   0 runner    (1001) docker     (123)   155263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.489585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-configmaps/
--rw-r--r--   0 runner    (1001) docker     (123)  1870504 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-configmaps/configmaps.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/
--rw-r--r--   0 runner    (1001) docker     (123)   366829 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_data.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_kind0.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_kind1.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_resources.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource_no_results.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-ocp4/
--rw-r--r--   0 runner    (1001) docker     (123)   273677 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-ocp4/ocp4-check-result.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-rhel7/
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-rhel7/rhel7-check-result.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-1.3.5.config
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-bad-yaml.config
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-compressed.config
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-configmaps.config
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-fetcher.config
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-xml-ocp4.config
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar-xml-rhel7.config
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/osco/test-osco-result-to-oscal-ar.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/tanium/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/demo-tanium-result-to-oscal-ar.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/tanium/input/
--rw-r--r--   0 runner    (1001) docker     (123)   314329 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/input/Tanium.comply-results-json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/tanium/input-bad/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/input-bad/Tanium.comply-results-bad
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.493585 compliance-trestle-2.2.0/tests/data/tasks/tanium/input-doc/
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/input-doc/Tanium.doc-json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.497585 compliance-trestle-2.2.0/tests/data/tasks/tanium/output/
--rw-r--r--   0 runner    (1001) docker     (123)  1997259 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/output/Tanium.oscal.2020.json
--rw-r--r--   0 runner    (1001) docker     (123)  1997259 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/tanium/output/Tanium.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.501586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.501586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output/
--rw-r--r--   0 runner    (1001) docker     (123)   157229 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.505586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)   157432 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.505586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-compressed/
--rw-r--r--   0 runner    (1001) docker     (123)   157229 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.505586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-configmaps/
--rw-r--r--   0 runner    (1001) docker     (123)  1891646 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-configmaps/configmaps.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/
--rw-r--r--   0 runner    (1001) docker     (123)   371515 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_data.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_kind0.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_kind1.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_resources.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_results.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-ocp4/
--rw-r--r--   0 runner    (1001) docker     (123)   276795 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-ocp4/ocp4-check-result.oscal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-rhel7/
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-rhel7/rhel7-check-result.oscal.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-1.3.5.config
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-bad-yaml.config
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-compressed.config
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-configmaps.config
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-fetcher.config
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-xml-ocp4.config
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-xml-rhel7.config
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/
--rw-r--r--   0 runner    (1001) docker     (123)    67226 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/component-definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-check/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-check/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-control/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-control/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-rule/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-rule/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.509586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-filtered/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-filtered/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.513586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-control-id/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-control-id/profile.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.513586 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-rule-name-id/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-rule-name-id/profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/test-xlsx-to-oscal-cd.config
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/tasks/xlsx/test-xlsx-to-oscal-profile.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.513586 compliance-trestle-2.2.0/tests/data/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/bad_component_dup_uuid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    99257 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/bad_component_no_tz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/bad_simple.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/good_component.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/good_component_diff_tz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/good_simple.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/data/yaml/header_with_metadata.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.513586 compliance-trestle-2.2.0/tests/functionality/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/functionality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/functionality/chevron_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/functionality/example_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/functionality/pathlib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.517586 compliance-trestle-2.2.0/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/split_test_1.sh
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/split_test_issue_630.sh
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/split_validate_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/manual_tests/test_binary.sh
--rw-r--r--   0 runner    (1001) docker     (123)    26384 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.517586 compliance-trestle-2.2.0/tests/trestle/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/cli_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.521586 compliance-trestle-2.2.0/tests/trestle/core/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/base_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.525586 compliance-trestle-2.2.0/tests/trestle/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/add_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/assemble_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.529586 compliance-trestle-2.2.0/tests/trestle/core/commands/author/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/component_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29859 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/docs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24635 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/folders_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/headers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/jinja_cmd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/profile_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32856 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/ssp_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.529586 compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/template_versioning_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/cmd_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/create_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/describe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/href_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/import__test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/init_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/merge_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/partial_object_validate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/remove_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/replicate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/split_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/task_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/validate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/commands/version_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/control_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/draw_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/err_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/jinja_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.529586 compliance-trestle-2.2.0/tests/trestle/core/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/markdown/markdown_node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17571 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/markdown/markdown_validator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.533586 compliance-trestle-2.2.0/tests/trestle/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/create_path_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/element_path_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/element_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/file_content_type_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/interfaces_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/plans_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/remove_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/remove_path_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/update_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/write_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/models/write_file_action_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21160 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/profile_resolver_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.533586 compliance-trestle-2.2.0/tests/trestle/core/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/remote/cache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/repository_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/ssp_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/core/validator_helper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.533586 compliance-trestle-2.2.0/tests/trestle/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/parsing/parsing_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.537586 compliance-trestle-2.2.0/tests/trestle/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/base_task_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/cis_xlsx_to_oscal_catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    46119 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/csv_to_oscal_cd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/ocp4_cis_profile_to_oscal_catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/ocp4_cis_profile_to_oscal_cd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/oscal_catalog_to_csv_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/oscal_profile_to_osco_profile_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/osco_result_to_oscal_ar_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/tanium_result_to_oscal_ar_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/transform_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/xccdf_result_to_oscal_ar_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/xlsx_to_oscal_cd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/tasks/xlsx_to_oscal_profile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.537586 compliance-trestle-2.2.0/tests/trestle/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/transforms/transformer_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/transforms/transformer_helper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.541586 compliance-trestle-2.2.0/tests/trestle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29420 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/fs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/list_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/load_distributed_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/md_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/tests/trestle/utils/trash_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.541586 compliance-trestle-2.2.0/trestle/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-26 21:32:03.000000 compliance-trestle-2.2.0/trestle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.545586 compliance-trestle-2.2.0/trestle/common/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/err.py
--rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/list_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/load_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    44383 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/trash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/common/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.553586 compliance-trestle-2.2.0/trestle/core/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/all_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.557586 compliance-trestle-2.2.0/trestle/core/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42306 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    22324 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog/catalog_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/catalog_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.561586 compliance-trestle-2.2.0/trestle/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/assemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.565586 compliance-trestle-2.2.0/trestle/core/commands/author/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)    33967 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    43643 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/ssp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.565586 compliance-trestle-2.2.0/trestle/core/commands/author/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/author/versioning/template_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/command_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.565586 compliance-trestle-2.2.0/trestle/core/commands/common/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/common/cmd_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/common/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/describe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/href.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/partial_object_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/replicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/control_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    49620 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/control_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/control_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    28904 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/control_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/docs_control_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/draw_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/duplicates_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20080 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/generic_oscal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/links_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.569586 compliance-trestle-2.2.0/trestle/core/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/base_markdown_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/control_markdown_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/docs_markdown_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/markdown_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/markdown_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/markdown_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/markdown_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/markdown/md_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.569586 compliance-trestle-2.2.0/trestle/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16242 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25162 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/file_content_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/profile_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/refs_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.569586 compliance-trestle-2.2.0/trestle/core/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20205 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/remote/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16329 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.573586 compliance-trestle-2.2.0/trestle/core/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/modify.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/resolver/prune.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/rule_parameters_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/ssp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/trestle_base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/core/validator_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.577586 compliance-trestle-2.2.0/trestle/oscal/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26369 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/assessment_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    35188 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/assessment_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    80055 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    26943 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/poam.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37519 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/oscal/ssp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.577586 compliance-trestle-2.2.0/trestle/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.577586 compliance-trestle-2.2.0/trestle/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/templates/FedRAMP_control_header_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/templates/template.drawio
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/resources/templates/template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.581586 compliance-trestle-2.2.0/trestle/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/cis_xlsx_to_oscal_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    63140 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/csv_to_oscal_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/ocp4_cis_profile_to_oscal_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    25634 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/ocp4_cis_profile_to_oscal_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/oscal_catalog_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/oscal_profile_to_osco_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/osco_result_to_oscal_ar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/tanium_result_to_oscal_ar.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/xccdf_result_to_oscal_ar.py
--rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/xlsx_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/xlsx_to_oscal_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/tasks/xlsx_to_oscal_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.581586 compliance-trestle-2.2.0/trestle/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:32:06.585586 compliance-trestle-2.2.0/trestle/transforms/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28870 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/implementations/osco.py
--rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/implementations/tanium.py
--rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/implementations/xccdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/transformer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/transformer_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-26 21:28:53.000000 compliance-trestle-2.2.0/trestle/transforms/transformer_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.818815 compliance-trestle-2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.554795 compliance-trestle-2.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.554795 compliance-trestle-2.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/ISSUE_TEMPLATE/new_collaborator.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/ISSUE_TEMPLATE/proposed_change.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.554795 compliance-trestle-2.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/PULL_REQUEST_TEMPLATE/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/PULL_REQUEST_TEMPLATE/hotfix.md
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/PULL_REQUEST_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/PULL_REQUEST_TEMPLATE/release.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/dco.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.554795 compliance-trestle-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/workflows/conventional-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/workflows/python-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.pylintrc_tests
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/.yapf-config
+-rw-r--r--   0 runner    (1001) docker     (123)    93328 2023-07-05 18:23:13.000000 compliance-trestle-2.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/DCO1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-07-05 18:23:15.818815 compliance-trestle-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.558795 compliance-trestle-2.2.1/compliance_trestle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-07-05 18:23:15.000000 compliance-trestle-2.2.1/compliance_trestle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    97672 2023-07-05 18:23:15.000000 compliance-trestle-2.2.1/compliance_trestle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:23:15.000000 compliance-trestle-2.2.1/compliance_trestle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 18:23:15.000000 compliance-trestle-2.2.1/compliance_trestle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-05 18:23:15.000000 compliance-trestle-2.2.1/compliance_trestle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 18:23:15.000000 compliance-trestle-2.2.1/compliance_trestle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.558795 compliance-trestle-2.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.578797 compliance-trestle-2.2.1/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.common_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.const.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.err.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.file_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.list_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.load_validate.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.log.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.model_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.str_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.trash.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.common.type_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.all_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.base_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.catalog.catalog_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.catalog.catalog_interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.catalog.catalog_merger.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.catalog.catalog_reader.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.catalog.catalog_writer.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.catalog_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.add.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.assemble.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.command.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.common.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.component.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.consts.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.docs.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.folders.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.headers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.ssp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.author.versioning.template_versioning.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.command_docs.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.common.cmd_utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.common.return_codes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.create.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.describe.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.href.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.import_.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.init.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.merge.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.partial_object_validate.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.remove.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.replicate.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.split.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.task.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.validate.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.commands.version.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.control_context.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.control_interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.control_reader.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.control_writer.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.docs_control_writer.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.draw_io.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.duplicates_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.generators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.generic_oscal.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.links_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.markdown.base_markdown_node.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.markdown.control_markdown_node.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.markdown.docs_markdown_node.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.markdown.markdown_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.markdown.markdown_const.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.markdown.markdown_processor.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.markdown.markdown_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.markdown.md_writer.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.models.actions.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.models.elements.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.models.file_content_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.models.interfaces.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.models.plans.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.object_factory.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.parser.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.profile_resolver.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.refs_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.remote.cache.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.repository.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.resolver.merge.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.resolver.modify.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.resolver.prune.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.rule_parameters_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.ssp_io.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.trestle_base_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.core.validator_factory.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.oscal.assessment_plan.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.oscal.assessment_results.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.oscal.catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.oscal.common.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.oscal.component.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.oscal.poam.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.oscal.profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.oscal.ssp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.base_task.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.cis_xlsx_to_oscal_catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.csv_to_oscal_cd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.ocp4_cis_profile_to_oscal_cd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.oscal_catalog_to_csv.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.oscal_profile_to_osco_profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.osco_result_to_oscal_ar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.tanium_result_to_oscal_ar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.transform.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.xccdf_result_to_oscal_ar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.xlsx_helper.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.xlsx_to_oscal_cd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.tasks.xlsx_to_oscal_profile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.transforms.implementations.osco.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.transforms.implementations.tanium.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.transforms.implementations.xccdf.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.transforms.results.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.transforms.transformer_factory.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.transforms.transformer_helper.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/api_reference/trestle.transforms.transformer_singleton.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.582797 compliance-trestle-2.2.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   161907 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/assets/Canonical_trestle_auditree_workflows.png
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/assets/README
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/assets/canonical_trestle_auditree_workflows.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)   329379 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/assets/drawio_data_menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)   264094 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/assets/drawio_editing_data.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/assets/sample_ssp.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    44185 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/assets/template_versioning.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58223 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/cli.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.582797 compliance-trestle-2.2.1/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/contributing/DCO.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/contributing/mkdocs_contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/contributing/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/contributing/trestle_oscal_object_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/contributing/website.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.582797 compliance-trestle-2.2.1/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/demonstrations-content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/errors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/maintainers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/mkdocs_code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.582797 compliance-trestle-2.2.1/docs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/plugins/compliance-trestle-fedramp.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/python_trestle_setup.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.582797 compliance-trestle-2.2.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)   146161 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/reference/third-party-result-schema-SCC.md
+-rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/trestle_author.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/trestle_author_jinja.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.586798 compliance-trestle-2.2.1/docs/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.586798 compliance-trestle-2.2.1/docs/tutorials/continuous-compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/continuous-compliance/ContinuousCompliance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/continuous-compliance/ContinuousCompliance.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/continuous-compliance/continuous-compliance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.586798 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/profile_does.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    37208 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/profile_does.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    67327 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76787 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_options.docx
+-rw-r--r--   0 runner    (1001) docker     (123)    75117 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/trestle_ssp_author_options.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.590798 compliance-trestle-2.2.1/docs/tutorials/task.csv-to-oscal-cd/
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.csv-to-oscal-cd/component-definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.csv-to-oscal-cd/demo-csv-to-oscal-cd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.csv-to-oscal-cd/ocp4-sample-input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.csv-to-oscal-cd/transformation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.590798 compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/demo-ocp4-cis-profile-to-oscal-catalog.config
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/transformation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.590798 compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/demo-ocp4-cis-profile-to-oscal-cd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/enabled_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/selected_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/transformation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.590798 compliance-trestle-2.2.1/docs/tutorials/task.tanium-result-to-oscal-ar/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.copyright-info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   111352 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.tanium-result-to-oscal-ar/transformation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.590798 compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/
+-rw-r--r--   0 runner    (1001) docker     (123)    56735 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/assessment-results-nist.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100092 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/assessment-results.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    43615 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/assessment-results.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/transformer-construction.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/transformer-construction.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/transformer-construction.md
+-rw-r--r--   0 runner    (1001) docker     (123)    27754 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/docs/tutorials/trestle_sample_workflow.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.594798 compliance-trestle-2.2.1/internal_spec_documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/internal_spec_documents/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/internal_spec_documents/caching_spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)    30894 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/internal_spec_documents/trestle-spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/internal_spec_documents/trestle-task-spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.594798 compliance-trestle-2.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.594798 compliance-trestle-2.2.1/scripts/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/experiments/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/experiments/json_serialize_ben.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/experiments/profile_json_seriallze_ben.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/experiments/profile_tanium_ben.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/experiments/profiling_tools_setup_OSX.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/experiments/tanium_ben.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/flatten_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/gen_oscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/have_files_changed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/order_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35528 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/oscal_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/schema_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/simplify_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/simplify_retain_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/tanium_transform_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/update_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/utf8me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/scripts/website_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-05 18:23:15.818815 compliance-trestle-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.598798 compliance-trestle-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.546795 compliance-trestle-2.2.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.598798 compliance-trestle-2.2.1/tests/data/author/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.514792 compliance-trestle-2.2.1/tests/data/author/0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.598798 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/not_mxfile.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_extra_fields_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_missing_fields_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_metadata_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_metadata_uncompressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_bad_internal_structure.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed_mangled.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_compressed.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_bad_md.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_compressed.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.598798 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_bold_heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_heading_wrong_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_missing_heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_no_header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_reordered.md
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/bad_instance_yaml_header_change.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/correct_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/correct_instance_extra_features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/template.md
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_1_md_format/yaml_header_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.602799 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_2_md_with_md_header/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_2_md_with_md_header/bad_heading_content_changed_header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_2_md_with_md_header/bad_heading_content_extra_lines.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_2_md_with_md_header/instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_2_md_with_md_header/template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_2_md_with_md_header/wrong_heading_title.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.602799 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_3_md_hand_edited/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_000.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_001.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_002.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_3_md_hand_edited/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.602799 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_bold_heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_heading_wrong_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_missing_heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_reordered.md
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/bad_instance_yaml_header_change.md
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance_extra_features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.602799 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_substitutions/bad_added_header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_substitutions/bad_modified_header_deep.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_substitutions/correct_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_substitutions/correct_instance_empty_subs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_substitutions/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.606799 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/__ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/correct_instance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.606799 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/subdirectory/correct_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/0.0.1/test_5_md_ignored/template.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/bad_md_header.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.606799 compliance-trestle-2.2.1/tests/data/author/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/controls/control_no_labels.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/controls/control_some_labels.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/controls/control_with_bad_component.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/controls/control_with_bad_system_comp.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/controls/control_with_components.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/controls/control_with_components_and_param_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/controls/control_with_components_and_params.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/controls/control_with_double_comp.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.518792 compliance-trestle-2.2.1/tests/data/author/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.606799 compliance-trestle-2.2.1/tests/data/author/docs/candidate_invalid_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/candidate_invalid_readme/correct_instance_extra_features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/candidate_invalid_readme/not_valid.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/candidate_invalid_readme/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.606799 compliance-trestle-2.2.1/tests/data/author/docs/candidate_valid_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/candidate_valid_readme/correct_instance_extra_features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/candidate_valid_readme/correct_instance_extra_features_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/candidate_valid_readme/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.606799 compliance-trestle-2.2.1/tests/data/author/docs/template_folder_invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/template_folder_invalid/extra_file.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/template_folder_invalid/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/template_folder_invalid/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.606799 compliance-trestle-2.2.1/tests/data/author/docs/template_folder_valid_with_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/template_folder_valid_with_readme/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/docs/template_folder_valid_with_readme/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.606799 compliance-trestle-2.2.1/tests/data/author/governed_folders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_folder_is_a_file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_bad_content/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_bad_content/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_bad_content/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_missing/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_missing/architecture.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_mixed_name/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_mixed_name/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_mixed_name/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_no_header/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_no_header/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_no_header/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_no_header/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_no_header/subdir/architecture.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_renamed/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_renamed/architecture_really_bad.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_renamed/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/folder_with_bad_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/folder_with_bad_drawio/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/folder_with_bad_drawio/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/folder_with_bad_drawio/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_limits_of_changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_limits_of_changes/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_limits_of_changes/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_readme/.hidden_test
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_readme/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_readme/network.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_readme/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.610799 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_version/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_version/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_version/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.614800 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/__ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/_ignore_not_instance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/diagram.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.614800 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore_not_instance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/architecture.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.614800 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.614800 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.614800 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_drawio/.hidden_does_not_affect
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_drawio/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_drawio/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_drawio/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.614800 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_version/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_version/diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_version/network.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.614800 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_with_readme/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_with_readme/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_with_readme/network.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/template_with_readme/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/governed_folders/utf16test_bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/utf16test_bad/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/governed_folders/utf16test_good/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/governed_folders/utf16test_good/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.522793 compliance-trestle-2.2.1/tests/data/author/headers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_drawio/template.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_drawio/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_md/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_md/template.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_md/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_wrong_names/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_wrong_names/templatesss.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_wrong_names/templatessss.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/empty_headers/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/empty_headers/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/empty_headers/b copy.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/empty_headers/b.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_drawio/a_file.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_drawio/whos_is_this.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_drawio_bad_file/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_drawio_bad_file/a_markdown_file.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_drawio_bad_file/another_file.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_md/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_md/my_drawio.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_md/my_md.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_md_bad_file/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_md_bad_file/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_md_bad_file/b.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.522793 compliance-trestle-2.2.1/tests/data/author/headers/global/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/global/good/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/good/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.522793 compliance-trestle-2.2.1/tests/data/author/headers/global/good/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/global/good/catalogs/my_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/good/catalogs/my_catalog/catalogs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/global/good/sample_indexable_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/good/sample_indexable_1/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/global/good/sample_indexable_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/good/sample_indexable_2/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/good/unindexed.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/bad_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/bad_sample/bad_sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.522793 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.618800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/catalogs/my_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/catalogs/my_catalog/catalogs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_1/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/sample_indexable_2/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_exceptions/unindexed.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.522793 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/my_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/catalogs/my_catalog/catalogs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/bad/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/bad/bad_sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/good/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/good/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/nested/sample.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/sample_indexable_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/sample_indexable_1/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/global/pass_with_nested_exceptions/unindexed.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/good_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/good_templates/template.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/good_templates/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/good_templates_wo_drawio/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/good_templates_wo_drawio/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/__ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/_ignore_not_instance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/correct_a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/correct_b.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/correct_instance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.622800 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/_ignore_not_instance.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/correct_instance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.626800 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/even_deeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/even_deeper/_ignore_not_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/even_deeper/correct_a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/even_deeper/correct_instance.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.626800 compliance-trestle-2.2.1/tests/data/author/headers/meets_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/meets_templates/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/meets_templates/b.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/meets_templates/d.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.626800 compliance-trestle-2.2.1/tests/data/author/headers/passes_with_extraneous_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/passes_with_extraneous_files/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/passes_with_extraneous_files/b.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/passes_with_extraneous_files/d.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/passes_with_extraneous_files/irrelevant.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.626800 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/b copy.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/b.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/d.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.626800 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/some_depth/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/some_depth/a.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/some_depth/b copy.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/some_depth/b.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/some_depth/d.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.626800 compliance-trestle-2.2.1/tests/data/author/ssp/
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/ssp/ssp_example.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.626800 compliance-trestle-2.2.1/tests/data/author/utf16test/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/utf16test/sample_okay.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/utf16test/sample_utf16.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.626800 compliance-trestle-2.2.1/tests/data/author/versions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.626800 compliance-trestle-2.2.1/tests/data/author/versions/1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/versions/1.0.0/bad_template_wrong_folder.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/versions/1.0.0/good_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.630801 compliance-trestle-2.2.1/tests/data/author/versions/1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/versions/1.1.0/bad_instance_mismatched_versions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/versions/1.1.0/bad_template_mismatched_versions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/versions/1.1.0/good_instance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/versions/1.1.0/good_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/versions/bad_template_with_version_outside_structure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/author/versions/good_instance_with_version_outside_structure.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.630801 compliance-trestle-2.2.1/tests/data/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/csv/bp.sample.v2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.526793 compliance-trestle-2.2.1/tests/data/csv/component-definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.630801 compliance-trestle-2.2.1/tests/data/csv/component-definitions/bp/
+-rw-r--r--   0 runner    (1001) docker     (123)    42744 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/csv/component-definitions/bp/component-definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54973 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/csv/ocp4-user.v2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.630801 compliance-trestle-2.2.1/tests/data/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/lookup_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/profile_to_docs.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/profile_to_docs_invalid.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/profile_to_docs_no_part_prose.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/profile_to_docs_only_some_sections.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/profile_to_docs_with_group_title.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/profile_to_docs_with_subparts.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/ssp_template.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/ssp_template_no_input_profile_ssp.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/sub_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/sub_content_with_subs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja/use_lookup_table.md.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.630801 compliance-trestle-2.2.1/tests/data/jinja_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_cmd/empty_test.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_cmd/number_captions_data.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_cmd/number_captions_expected_output.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.634801 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDDatestamp_default.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDDatestamp_format.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDDatestamp_invalid.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDDatestamp_newline.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDSection_include_nested.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDSection_include_nested.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDSection_include_top_level.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDSection_include_top_level.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDSection_include_top_level_adjusted.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/MDSection_include_top_level_adjusted.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_include.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_include.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_include_adjusted.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_include_adjusted.md
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_nested_c_c.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_nested_c_c.md
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_nested_c_c_double.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_nested_c_c_double.md
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_nested_c_n.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_nested_c_n.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/nested_c.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/nested_n.jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/jinja_markdown_include/test_markdown.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.642802 compliance-trestle-2.2.1/tests/data/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/bad_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21655 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_def.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_def_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_def_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_def_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_prof.json
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_prof_aa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_prof_ab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_prof_ba.json
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_prof_bad.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_prof_bb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/comp_prof_part_none.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/good_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/leveraged_ssp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/leveraged_ssp_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog_bad_oscal_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog_extra_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog_missing_roles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog_missing_uuid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog_no_responsible-parties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog_roles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog_roles_double.json
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog_roles_double_rp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/minimal_catalog_with_groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/nist_tutorial_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/nist_tutorial_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/profile_bad_control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/profile_missing_position.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/profile_with_alter_props.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/profile_with_alter_subparts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/profile_with_incorrect_alter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/pull_nist_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/simple_catalog_no_parts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/simple_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/simple_test_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/simple_test_profile_less.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/simple_test_profile_more.json
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/simple_test_profile_no_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/simple_test_profile_single.json
+-rw-r--r--   0 runner    (1001) docker     (123)   221136 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/simplified_nist_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/simplified_nist_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/test_profile_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/test_profile_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/test_profile_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/test_profile_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/test_profile_e.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/test_profile_f.json
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/json/test_profile_g.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.642802 compliance-trestle-2.2.1/tests/data/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/markdown/valid_complex_md.md
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/markdown/valid_levels_no_text.md
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/markdown/valid_levels_no_text_increased_level.md
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/markdown/valid_no_headers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/markdown/valid_no_lvl1_headers.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.646802 compliance-trestle-2.2.1/tests/data/ocp4-cis/
+-rw-r--r--   0 runner    (1001) docker     (123)    23806 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/ocp4-cis/catalog.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.646802 compliance-trestle-2.2.1/tests/data/split_merge/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.646802 compliance-trestle-2.2.1/tests/data/split_merge/.trestle/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/.trestle/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.650802 compliance-trestle-2.2.1/tests/data/split_merge/load_distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)  3169371 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/load_distributed/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/load_distributed/groups.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.654802 compliance-trestle-2.2.1/tests/data/split_merge/step0-merged_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.526793 compliance-trestle-2.2.1/tests/data/split_merge/step0-merged_catalog/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.654802 compliance-trestle-2.2.1/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)  4498050 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step0-merged_catalog/next_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.658803 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.526793 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.658803 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.666803 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/back-matter.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/next_step.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/previous_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.666803 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.526793 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.666803 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.670804 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/back-matter.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/groups.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.670804 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/parties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/responsible-parties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/roles.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/next_step.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/previous_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.674804 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.526793 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.674804 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.678804 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/back-matter.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4079387 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/groups.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.678804 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/parties.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.678804 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/00000__responsible-party.json
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties/00001__responsible-party.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/responsible-parties.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.678804 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/00000__role.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles/00001__role.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/roles.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/next_step.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/previous_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.678804 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.678804 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.678804 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)   110356 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/back-matter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.682805 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.686805 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48380 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54960 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    70506 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30598 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18970 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00023__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00024__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.690805 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18701 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.690805 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15966 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.694805 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24785 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.694805 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34660 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28847 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.698806 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29166 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21335 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.698806 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51627 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.702806 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38793 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.702806 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.702806 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.706806 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24929 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.710807 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.714807 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00023__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00024__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00025__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00026__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00027__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00028__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00029__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00030__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00031__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.718807 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.530793 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.718807 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.534794 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.718807 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30706 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.534794 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.722808 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42212 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)   101326 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25087 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32683 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37819 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.534794 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.734809 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72606 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00023__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00024__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00025__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00026__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00027__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00028__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00029__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00030__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00031__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00032__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00033__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00034__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00035__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00036__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00037__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00038__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00039__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00040__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00041__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00042__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00043__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00044__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00045__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00046__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00047__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00048__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00049__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00050__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.534794 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.738809 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    67388 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36771 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00012__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00013__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00014__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00015__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00016__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00017__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00018__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00019__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00020__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00021__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00022__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.534794 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.738809 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00000__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00001__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00002__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00003__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00004__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00005__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00006__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00007__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00008__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00009__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00010__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00011__control.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.738809 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/parties.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.738809 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/00000__responsible-party.json
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/responsible-parties/00001__responsible-party.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.738809 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/00000__role.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/roles/00001__role.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/next_step.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/previous_step.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/spread-sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/bad_parameter_name_and_description.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/duplicate_column_heading.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/embedded_blank_in_goal_name_id.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/embedded_blank_in_parameter_name.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/embedded_blank_in_rule_name_id.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/good.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/good_with_blank_rows.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/missing_column_heading.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/missing_control_id.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/missing_resource_title.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/spread-sheet/missing_rule_name_id.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.542794 compliance-trestle-2.2.1/tests/data/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_RedHat_OpenShift_Container_Platform_Benchmark_v1.2.0-2.snippet.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.snippet.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/test-cis-xlsx-to-oscal-catalog.ocp.config
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/test-cis-xlsx-to-oscal-catalog.rhel.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/csv-to-oscal-cd/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/csv-to-oscal-cd/test-csv-to-oscal-cd-bp.config
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/csv-to-oscal-cd/test-csv-to-oscal-cd.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/cis.profile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/cis.profile
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/test-ocp4-cis-profile-to-oscal-catalog.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.534794 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.534794 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_cni_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_cni_conf/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_apiserver/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_controller_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_groupowner_kube_controller_manager/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_cni_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_cni_conf/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_apiserver/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_controller_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_owner_kube_controller_manager/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_apiserver/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_controller_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/file_permissions_kube_controller_manager/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.742809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_memory_available/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_memory_available/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.746809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_nodefs_available/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/applications/openshift/kubelet_eviction_thresholds_set_soft_nodefs_available/rule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.746809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/rule2var.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.746809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/
+-rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/component-definition.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.538794 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.538794 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.746809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis-node.profile
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis.profile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.746809 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test.profile
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test2.profile
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test3.profile
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd3.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.746809 compliance-trestle-2.2.1/tests/data/tasks/oscal-catalog-to-csv/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-catalog-to-csv/test-oscal-catalog-to-csv-rev-5-by-control.config
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-catalog-to-csv/test-oscal-catalog-to-csv-rev-5-by-statement.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-no.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-yes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-no.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-yes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.2.0-parms-no.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-1.0.0-parms-yes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-no.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-yes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-scc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-no.config
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.39-parms-yes.config
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-no.config
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.1.40-parms-yes.config
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-0.2.0-parms-no.config
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-1.0.0-parms-yes.config
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-bogus.config
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-input-file.config
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-output-dir.config
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-no-overwrite.config
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-parms-no.config
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-parms-yes.config
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-scc.config
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile-set.config
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/oscal-profile-to-osco-profile.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.542794 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/tailored-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.750810 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output-set/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output-set/osco-profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.754810 compliance-trestle-2.2.1/tests/data/tasks/osco/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.754810 compliance-trestle-2.2.1/tests/data/tasks/osco/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input/ignore.me
+-rw-r--r--   0 runner    (1001) docker     (123)    52753 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.754810 compliance-trestle-2.2.1/tests/data/tasks/osco/input-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    52859 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.754810 compliance-trestle-2.2.1/tests/data/tasks/osco/input-bad-yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-bad-yaml/bad.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.754810 compliance-trestle-2.2.1/tests/data/tasks/osco/input-compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.754810 compliance-trestle-2.2.1/tests/data/tasks/osco/input-configmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)   608191 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-configmaps/configmaps.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.758810 compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/
+-rw-r--r--   0 runner    (1001) docker     (123)   105678 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_resources.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.758810 compliance-trestle-2.2.1/tests/data/tasks/osco/input-xml-ocp4/
+-rw-r--r--   0 runner    (1001) docker     (123)    78761 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-xml-ocp4/ocp4-check-result.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.758810 compliance-trestle-2.2.1/tests/data/tasks/osco/input-xml-rhel7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/input-xml-rhel7/rhel7-check-result.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.758810 compliance-trestle-2.2.1/tests/data/tasks/osco/output/
+-rw-r--r--   0 runner    (1001) docker     (123)   155263 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.758810 compliance-trestle-2.2.1/tests/data/tasks/osco/output-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)   155462 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.758810 compliance-trestle-2.2.1/tests/data/tasks/osco/output-compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)   155263 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.758810 compliance-trestle-2.2.1/tests/data/tasks/osco/output-configmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)  1870504 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-configmaps/configmaps.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.762811 compliance-trestle-2.2.1/tests/data/tasks/osco/output-fetcher/
+-rw-r--r--   0 runner    (1001) docker     (123)   366829 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-fetcher/cluster_resource.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_data.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_kind0.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_kind1.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_resources.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-fetcher/cluster_resource_no_results.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.762811 compliance-trestle-2.2.1/tests/data/tasks/osco/output-xml-ocp4/
+-rw-r--r--   0 runner    (1001) docker     (123)   273677 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-xml-ocp4/ocp4-check-result.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.762811 compliance-trestle-2.2.1/tests/data/tasks/osco/output-xml-rhel7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/output-xml-rhel7/rhel7-check-result.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-1.3.5.config
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-bad-yaml.config
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-compressed.config
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-configmaps.config
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-fetcher.config
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-xml-ocp4.config
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar-xml-rhel7.config
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/osco/test-osco-result-to-oscal-ar.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.762811 compliance-trestle-2.2.1/tests/data/tasks/tanium/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/tanium/demo-tanium-result-to-oscal-ar.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.762811 compliance-trestle-2.2.1/tests/data/tasks/tanium/input/
+-rw-r--r--   0 runner    (1001) docker     (123)   314329 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/tanium/input/Tanium.comply-results-json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.762811 compliance-trestle-2.2.1/tests/data/tasks/tanium/input-bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/tanium/input-bad/Tanium.comply-results-bad
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.762811 compliance-trestle-2.2.1/tests/data/tasks/tanium/input-doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/tanium/input-doc/Tanium.doc-json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.766811 compliance-trestle-2.2.1/tests/data/tasks/tanium/output/
+-rw-r--r--   0 runner    (1001) docker     (123)  1997259 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/tanium/output/Tanium.oscal.2020.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1997259 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/tanium/output/Tanium.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.770811 compliance-trestle-2.2.1/tests/data/tasks/xccdf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.770811 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output/
+-rw-r--r--   0 runner    (1001) docker     (123)   157229 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.770811 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)   157432 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.770811 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)   157229 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.770811 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-configmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)  1891646 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-configmaps/configmaps.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.774811 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-fetcher/
+-rw-r--r--   0 runner    (1001) docker     (123)   371515 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_data.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_kind0.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_kind1.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_resources.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource_no_results.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.774811 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-xml-ocp4/
+-rw-r--r--   0 runner    (1001) docker     (123)   276795 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-xml-ocp4/ocp4-check-result.oscal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.774811 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-xml-rhel7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-xml-rhel7/rhel7-check-result.oscal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-1.3.5.config
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-bad-yaml.config
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-compressed.config
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-configmaps.config
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-fetcher.config
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-xml-ocp4.config
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar-xml-rhel7.config
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xccdf/test-xccdf-result-to-oscal-ar.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.774811 compliance-trestle-2.2.1/tests/data/tasks/xlsx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.774811 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output/
+-rw-r--r--   0 runner    (1001) docker     (123)    67226 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output/component-definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.774811 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-by-check/
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-by-check/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.778812 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-by-control/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-by-control/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.778812 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-by-rule/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-by-rule/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.778812 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-filtered/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-filtered/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.778812 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-missing-control-id/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-missing-control-id/profile.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.778812 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-missing-rule-name-id/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-missing-rule-name-id/profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/test-xlsx-to-oscal-cd.config
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/tasks/xlsx/test-xlsx-to-oscal-profile.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.778812 compliance-trestle-2.2.1/tests/data/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/yaml/bad_component_dup_uuid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    99257 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/yaml/bad_component_no_tz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/yaml/bad_simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/yaml/good_component.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    99263 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/yaml/good_component_diff_tz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/yaml/good_simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/data/yaml/header_with_metadata.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.778812 compliance-trestle-2.2.1/tests/functionality/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/functionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/functionality/chevron_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/functionality/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/functionality/pathlib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.778812 compliance-trestle-2.2.1/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/manual_tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/manual_tests/split_test_1.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/manual_tests/split_test_issue_630.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/manual_tests/split_validate_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/manual_tests/test_binary.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    26384 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.778812 compliance-trestle-2.2.1/tests/trestle/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.782812 compliance-trestle-2.2.1/tests/trestle/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/base_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.786812 compliance-trestle-2.2.1/tests/trestle/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/add_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/assemble_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.786812 compliance-trestle-2.2.1/tests/trestle/core/commands/author/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29859 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/docs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24635 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/folders_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/headers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/jinja_cmd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53442 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32856 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/ssp_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.786812 compliance-trestle-2.2.1/tests/trestle/core/commands/author/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/author/versioning/template_versioning_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/cmd_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/create_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/describe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/href_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/import__test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/merge_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/partial_object_validate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/remove_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/replicate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/split_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/task_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/validate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/commands/version_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/control_io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/draw_io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/err_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/jinja_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.786812 compliance-trestle-2.2.1/tests/trestle/core/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/markdown/markdown_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17571 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/markdown/markdown_validator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.790813 compliance-trestle-2.2.1/tests/trestle/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/create_path_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/element_path_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/element_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/file_content_type_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/interfaces_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/plans_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/remove_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/remove_path_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/update_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/write_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/models/write_file_action_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21160 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/profile_resolver_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.790813 compliance-trestle-2.2.1/tests/trestle/core/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/remote/cache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/repository_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/ssp_io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/core/validator_helper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.790813 compliance-trestle-2.2.1/tests/trestle/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/parsing/parsing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.794813 compliance-trestle-2.2.1/tests/trestle/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/base_task_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/cis_xlsx_to_oscal_catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46119 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/csv_to_oscal_cd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/ocp4_cis_profile_to_oscal_catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/ocp4_cis_profile_to_oscal_cd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/oscal_catalog_to_csv_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/oscal_profile_to_osco_profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/osco_result_to_oscal_ar_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/tanium_result_to_oscal_ar_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/transform_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/xccdf_result_to_oscal_ar_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/xlsx_to_oscal_cd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/tasks/xlsx_to_oscal_profile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.794813 compliance-trestle-2.2.1/tests/trestle/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/transforms/transformer_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/transforms/transformer_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.794813 compliance-trestle-2.2.1/tests/trestle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29420 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/utils/fs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/utils/list_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/utils/load_distributed_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/utils/md_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/tests/trestle/utils/trash_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.794813 compliance-trestle-2.2.1/trestle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-05 18:23:13.000000 compliance-trestle-2.2.1/trestle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.798813 compliance-trestle-2.2.1/trestle/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/err.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/load_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44383 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/trash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/common/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.802813 compliance-trestle-2.2.1/trestle/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/all_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.802813 compliance-trestle-2.2.1/trestle/core/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/catalog/catalog_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42306 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/catalog/catalog_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/catalog/catalog_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18787 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/catalog/catalog_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/catalog/catalog_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/catalog_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.806814 compliance-trestle-2.2.1/trestle/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/assemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.806814 compliance-trestle-2.2.1/trestle/core/commands/author/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35543 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43643 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/ssp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.806814 compliance-trestle-2.2.1/trestle/core/commands/author/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/author/versioning/template_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/command_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.806814 compliance-trestle-2.2.1/trestle/core/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/common/cmd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/common/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/href.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/partial_object_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/replicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/control_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49620 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/control_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23766 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/control_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/control_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/docs_control_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/draw_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/duplicates_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20080 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/generic_oscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/links_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.810814 compliance-trestle-2.2.1/trestle/core/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/markdown/base_markdown_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/markdown/control_markdown_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/markdown/docs_markdown_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/markdown/markdown_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/markdown/markdown_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/markdown/markdown_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/markdown/markdown_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/markdown/md_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.810814 compliance-trestle-2.2.1/trestle/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16242 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25162 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/models/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/models/file_content_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/models/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/models/plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/profile_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/refs_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.810814 compliance-trestle-2.2.1/trestle/core/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20205 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/remote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16329 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.810814 compliance-trestle-2.2.1/trestle/core/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/resolver/_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/resolver/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/resolver/modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/resolver/prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/rule_parameters_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/ssp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/trestle_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/core/validator_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.814814 compliance-trestle-2.2.1/trestle/oscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26369 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/assessment_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35188 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/assessment_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80055 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26943 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/poam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37519 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/oscal/ssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.814814 compliance-trestle-2.2.1/trestle/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/resources/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.814814 compliance-trestle-2.2.1/trestle/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/resources/templates/FedRAMP_control_header_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/resources/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/resources/templates/template.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/resources/templates/template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.818815 compliance-trestle-2.2.1/trestle/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/cis_xlsx_to_oscal_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63194 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/csv_to_oscal_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/ocp4_cis_profile_to_oscal_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25634 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/ocp4_cis_profile_to_oscal_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/oscal_catalog_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/oscal_profile_to_osco_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/osco_result_to_oscal_ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/tanium_result_to_oscal_ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/xccdf_result_to_oscal_ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/xlsx_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/xlsx_to_oscal_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/tasks/xlsx_to_oscal_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.818815 compliance-trestle-2.2.1/trestle/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:23:15.818815 compliance-trestle-2.2.1/trestle/transforms/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/transforms/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28870 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/transforms/implementations/osco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/transforms/implementations/tanium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/transforms/implementations/xccdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/transforms/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/transforms/transformer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/transforms/transformer_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-05 18:19:48.000000 compliance-trestle-2.2.1/trestle/transforms/transformer_singleton.py
```

### Comparing `compliance-trestle-2.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `compliance-trestle-2.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/develop.md` & `compliance-trestle-2.2.1/.github/PULL_REQUEST_TEMPLATE/develop.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE/release.md` & `compliance-trestle-2.2.1/.github/PULL_REQUEST_TEMPLATE/release.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `compliance-trestle-2.2.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/.github/workflows/codeql-analysis.yml` & `compliance-trestle-2.2.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/.github/workflows/conventional-pr.yml` & `compliance-trestle-2.2.1/.github/workflows/conventional-pr.yml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/.github/workflows/python-push.yml` & `compliance-trestle-2.2.1/.github/workflows/python-push.yml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/.github/workflows/python-test.yml` & `compliance-trestle-2.2.1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/.gitignore` & `compliance-trestle-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/.pre-commit-config.yaml` & `compliance-trestle-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/CHANGELOG.md` & `compliance-trestle-2.2.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # Compliance-trestle changelog
 
 
 <!--next-version-placeholder-->
 
+## v2.2.1 (2023-07-05)
+
+### Fix
+
+* Parameter value default is never required ([#1419](https://github.com/IBM/compliance-trestle/issues/1419)) ([`01434f1`](https://github.com/IBM/compliance-trestle/commit/01434f13b16054b035767985a9a02ed9fa91154f))
+* Pydantic 2.0.0 break unit tests ([#1418](https://github.com/IBM/compliance-trestle/issues/1418)) ([`2138831`](https://github.com/IBM/compliance-trestle/commit/2138831f9bb36c5f91ab17cccc4412128c468a82))
+* Adding parameter aggregation from other parameter values for given control ([#1412](https://github.com/IBM/compliance-trestle/issues/1412)) ([`7b8cad0`](https://github.com/IBM/compliance-trestle/commit/7b8cad03e05024a406742720e5abed2e3febdf6f))
+* Assessment objectives formatting in markdown is not correct ([#1414](https://github.com/IBM/compliance-trestle/issues/1414)) ([`dbfc1d6`](https://github.com/IBM/compliance-trestle/commit/dbfc1d6c59339a7f542f86cb74da4f05fe8a9a60))
+
 ## v2.2.0 (2023-06-26)
 
 ### Feature
 
 * Add profile-inherit command ([#1392](https://github.com/IBM/compliance-trestle/issues/1392)) ([`3bd53ff`](https://github.com/IBM/compliance-trestle/commit/3bd53ff370cece77fc78082dbc04304af12c6647))
 * Oscal-catalog-to-csv ([#1396](https://github.com/IBM/compliance-trestle/issues/1396)) ([`5f59a7f`](https://github.com/IBM/compliance-trestle/commit/5f59a7fc7cf8b88a9f77ba4554dd493acff67114))
 * Adds control origination to ssp-filter ([#1375](https://github.com/IBM/compliance-trestle/issues/1375)) ([`509afa7`](https://github.com/IBM/compliance-trestle/commit/509afa7df124f8a6c3516ad06db256777baaef98))
```

### Comparing `compliance-trestle-2.2.0/CODE_OF_CONDUCT.md` & `compliance-trestle-2.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/CONTRIBUTING.md` & `compliance-trestle-2.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/DCO1.1.txt` & `compliance-trestle-2.2.1/DCO1.1.txt`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/LICENSE` & `compliance-trestle-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/MAINTAINERS.md` & `compliance-trestle-2.2.1/MAINTAINERS.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/Makefile` & `compliance-trestle-2.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/PKG-INFO` & `compliance-trestle-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compliance-trestle
-Version: 2.2.0
+Version: 2.2.1
 Summary: Tools to manage & autogenerate python objects representing the OSCAL layers/models
 Home-page: https://ibm.github.io/compliance-trestle
 Author: IBM
 Author-email: avikas@in.ibm.com
 License: Apache Software License v2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `compliance-trestle-2.2.0/README.md` & `compliance-trestle-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/compliance_trestle.egg-info/PKG-INFO` & `compliance-trestle-2.2.1/compliance_trestle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compliance-trestle
-Version: 2.2.0
+Version: 2.2.1
 Summary: Tools to manage & autogenerate python objects representing the OSCAL layers/models
 Home-page: https://ibm.github.io/compliance-trestle
 Author: IBM
 Author-email: avikas@in.ibm.com
 License: Apache Software License v2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `compliance-trestle-2.2.0/compliance_trestle.egg-info/SOURCES.txt` & `compliance-trestle-2.2.1/compliance_trestle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/compliance_trestle.egg-info/requires.txt` & `compliance-trestle-2.2.1/compliance_trestle.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 attrs
 ilcli
 cryptography
 paramiko
 ruamel.yaml
 furl
-pydantic[email]>=1.8.2
+pydantic[email]<2.0.0,>=1.8.2
 python-dotenv>=0.10.4
 datamodel-code-generator[http]>=0.11.14
 python-frontmatter
 defusedxml
 openpyxl~=3.0
 Jinja2>=3.0.1
 cmarkgfm==0.6.*
```

### Comparing `compliance-trestle-2.2.0/docs/assets/Canonical_trestle_auditree_workflows.png` & `compliance-trestle-2.2.1/docs/assets/Canonical_trestle_auditree_workflows.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/assets/canonical_trestle_auditree_workflows.drawio` & `compliance-trestle-2.2.1/docs/assets/canonical_trestle_auditree_workflows.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/assets/drawio_data_menu.png` & `compliance-trestle-2.2.1/docs/assets/drawio_data_menu.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/assets/drawio_editing_data.png` & `compliance-trestle-2.2.1/docs/assets/drawio_editing_data.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/assets/sample_ssp.md.jinja` & `compliance-trestle-2.2.1/docs/assets/sample_ssp.md.jinja`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/assets/template_versioning.png` & `compliance-trestle-2.2.1/docs/assets/template_versioning.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/cli.md` & `compliance-trestle-2.2.1/docs/cli.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/contributing/DCO.md` & `compliance-trestle-2.2.1/docs/contributing/DCO.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/contributing/plugins.md` & `compliance-trestle-2.2.1/docs/contributing/plugins.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/contributing/trestle_oscal_object_model.md` & `compliance-trestle-2.2.1/docs/contributing/trestle_oscal_object_model.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/contributing/website.md` & `compliance-trestle-2.2.1/docs/contributing/website.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/css/mkdocstrings.css` & `compliance-trestle-2.2.1/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/demonstrations-content.md` & `compliance-trestle-2.2.1/docs/demonstrations-content.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/index.md` & `compliance-trestle-2.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/license.md` & `compliance-trestle-2.2.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/plugins/compliance-trestle-fedramp.md` & `compliance-trestle-2.2.1/docs/plugins/compliance-trestle-fedramp.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/python_trestle_setup.md` & `compliance-trestle-2.2.1/docs/python_trestle_setup.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.png` & `compliance-trestle-2.2.1/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.xlsx` & `compliance-trestle-2.2.1/docs/reference/Unification-SCC-class-for-OSCO-and-Tanium-to-OSCAL.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/reference/third-party-result-schema-SCC.md` & `compliance-trestle-2.2.1/docs/reference/third-party-result-schema-SCC.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/trestle_author.md` & `compliance-trestle-2.2.1/docs/trestle_author.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/trestle_author_jinja.md` & `compliance-trestle-2.2.1/docs/trestle_author_jinja.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/ContinuousCompliance.drawio` & `compliance-trestle-2.2.1/docs/tutorials/continuous-compliance/ContinuousCompliance.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/ContinuousCompliance.jpg` & `compliance-trestle-2.2.1/docs/tutorials/continuous-compliance/ContinuousCompliance.jpg`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/continuous-compliance/continuous-compliance.md` & `compliance-trestle-2.2.1/docs/tutorials/continuous-compliance/continuous-compliance.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.drawio` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.png` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/complex_resolved_profile_catalog.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/profile_does.drawio` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/profile_does.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/profile_does.png` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/profile_does.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.drawio` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.png` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_catalog.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.drawio` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.png` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/resolved_profile_diagram.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.drawio` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.png` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/simple_catalog.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring.md` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_options.docx` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/ssp_profile_options.docx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/ssp_profile_catalog_authoring/trestle_ssp_author_options.png` & `compliance-trestle-2.2.1/docs/tutorials/ssp_profile_catalog_authoring/trestle_ssp_author_options.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/component-definition.json` & `compliance-trestle-2.2.1/docs/tutorials/task.csv-to-oscal-cd/component-definition.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/ocp4-sample-input.csv` & `compliance-trestle-2.2.1/docs/tutorials/task.csv-to-oscal-cd/ocp4-sample-input.csv`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.csv-to-oscal-cd/transformation.md` & `compliance-trestle-2.2.1/docs/tutorials/task.csv-to-oscal-cd/transformation.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/transformation.md` & `compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-catalog/transformation.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/demo-ocp4-cis-profile-to-oscal-cd.config` & `compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/demo-ocp4-cis-profile-to-oscal-cd.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/enabled_rules.json` & `compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/enabled_rules.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/transformation.md` & `compliance-trestle-2.2.1/docs/tutorials/task.ocp4-cis-profile-to-oscal-cd/transformation.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.jpg` & `compliance-trestle-2.2.1/docs/tutorials/task.tanium-result-to-oscal-ar/800px-Australia_scarsdale_nimons_bridge.jpg`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.tanium-result-to-oscal-ar/transformation.md` & `compliance-trestle-2.2.1/docs/tutorials/task.tanium-result-to-oscal-ar/transformation.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results-nist.png` & `compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/assessment-results-nist.png`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results.drawio` & `compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/assessment-results.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/assessment-results.jpg` & `compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/assessment-results.jpg`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.drawio` & `compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/transformer-construction.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.jpg` & `compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/transformer-construction.jpg`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/task.transformer-construction/transformer-construction.md` & `compliance-trestle-2.2.1/docs/tutorials/task.transformer-construction/transformer-construction.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/docs/tutorials/trestle_sample_workflow.md` & `compliance-trestle-2.2.1/docs/tutorials/trestle_sample_workflow.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/internal_spec_documents/caching_spec.md` & `compliance-trestle-2.2.1/internal_spec_documents/caching_spec.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/internal_spec_documents/trestle-spec.md` & `compliance-trestle-2.2.1/internal_spec_documents/trestle-spec.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/internal_spec_documents/trestle-task-spec.md` & `compliance-trestle-2.2.1/internal_spec_documents/trestle-task-spec.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/mkdocs.yml` & `compliance-trestle-2.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/cleanup.py` & `compliance-trestle-2.2.1/scripts/cleanup.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/experiments/README.md` & `compliance-trestle-2.2.1/scripts/experiments/README.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/experiments/json_serialize_ben.py` & `compliance-trestle-2.2.1/scripts/experiments/json_serialize_ben.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/experiments/tanium_ben.py` & `compliance-trestle-2.2.1/scripts/experiments/tanium_ben.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/flatten_schema.py` & `compliance-trestle-2.2.1/scripts/flatten_schema.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/gen_oscal.py` & `compliance-trestle-2.2.1/scripts/gen_oscal.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/have_files_changed.py` & `compliance-trestle-2.2.1/scripts/have_files_changed.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/order_classes.py` & `compliance-trestle-2.2.1/scripts/order_classes.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/oscal_normalize.py` & `compliance-trestle-2.2.1/scripts/oscal_normalize.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/schema_integrity.py` & `compliance-trestle-2.2.1/scripts/schema_integrity.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/simplify_catalog.py` & `compliance-trestle-2.2.1/scripts/simplify_catalog.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/simplify_retain_ac.py` & `compliance-trestle-2.2.1/scripts/simplify_retain_ac.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/tanium_transform_script.py` & `compliance-trestle-2.2.1/scripts/tanium_transform_script.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/update_uuids.py` & `compliance-trestle-2.2.1/scripts/update_uuids.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/utf8me.py` & `compliance-trestle-2.2.1/scripts/utf8me.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/scripts/website_automation.py` & `compliance-trestle-2.2.1/scripts/website_automation.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/setup.cfg` & `compliance-trestle-2.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 install_requires = 
 	attrs
 	ilcli
 	cryptography
 	paramiko
 	ruamel.yaml
 	furl
-	pydantic[email]>=1.8.2
+	pydantic[email]>=1.8.2,<2.0.0
 	python-dotenv>=0.10.4
 	datamodel-code-generator[http] >= 0.11.14
 	python-frontmatter
 	pywin32 >= 1.0;platform_system=='Windows'
 	defusedxml
 	openpyxl~=3.0
 	Jinja2 >= 3.0.1
```

### Comparing `compliance-trestle-2.2.0/setup.py` & `compliance-trestle-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/__init__.py` & `compliance-trestle-2.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/conftest.py` & `compliance-trestle-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_extra_fields_compressed.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_extra_fields_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_missing_fields_compressed.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_bad_metadata_missing_fields_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_metadata_compressed.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_metadata_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_metadata_uncompressed.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_metadata_uncompressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_bad_internal_structure.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_bad_internal_structure.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_compressed.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed_mangled.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/single_tab_no_metadata_uncompressed_mangled.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_compressed.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_bad_md.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_bad_md.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_compressed.drawio` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/drawio/two_tabs_metadata_second_tab_compressed.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_2_md_with_md_header/template.md` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/test_2_md_with_md_header/template.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_000.md` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_000.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_001.md` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_001.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_002.md` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/test_3_md_hand_edited/decisions_002.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_3_md_hand_edited/template.md` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/test_3_md_hand_edited/template.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance_extra_features.md` & `compliance-trestle-2.2.1/tests/data/author/0.0.1/test_4_md_format_extras/correct_instance_extra_features.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/controls/control_with_bad_component.md` & `compliance-trestle-2.2.1/tests/data/author/controls/control_with_bad_component.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/controls/control_with_bad_system_comp.md` & `compliance-trestle-2.2.1/tests/data/author/controls/control_with_bad_system_comp.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/controls/control_with_components.md` & `compliance-trestle-2.2.1/tests/data/author/controls/control_with_components.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/controls/control_with_components_and_param_template.md` & `compliance-trestle-2.2.1/tests/data/author/controls/control_with_components_and_param_template.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/controls/control_with_components_and_params.md` & `compliance-trestle-2.2.1/tests/data/author/controls/control_with_components_and_params.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/controls/control_with_double_comp.md` & `compliance-trestle-2.2.1/tests/data/author/controls/control_with_double_comp.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_bad_content/network.md` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_bad_content/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_mixed_name/architecture.md` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_mixed_name/architecture.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/bad_instance_renamed/network.md` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/bad_instance_renamed/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/folder_with_bad_drawio/diagram.drawio` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/folder_with_bad_drawio/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance/network.md` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_limits_of_changes/network.md` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_limits_of_changes/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_readme/network.md` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_readme/network.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/good_instance_with_version/diagram.drawio` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/good_instance_with_version/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/diagram.drawio` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/diagram.drawio` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/ignored_files/ignore_subfolder/ignore_even_deeper/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_drawio/diagram.drawio` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_drawio/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/governed_folders/template_folder_with_version/diagram.drawio` & `compliance-trestle-2.2.1/tests/data/author/governed_folders/template_folder_with_version/diagram.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_drawio/template.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_drawio/template.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_md/template.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_md/template.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/bad_templates_wrong_names/templatesss.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/bad_templates_wrong_names/templatesss.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/empty_headers/a.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/empty_headers/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio/whos_is_this.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_drawio/whos_is_this.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_drawio_bad_file/a_markdown_file.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_drawio_bad_file/a_markdown_file.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md/my_drawio.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_md/my_drawio.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/fails_validation_md_bad_file/a.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/fails_validation_md_bad_file/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/good_templates/template.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/good_templates/template.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_a.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/correct_a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/correct_b.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/correct_b.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/ignored_files/deep/even_deeper/correct_a.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/ignored_files/deep/even_deeper/correct_a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/a.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/meets_templates/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/meets_templates/d.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/meets_templates/d.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/a.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/passes_with_extraneous_files/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/passes_with_extraneous_files/d.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/passes_with_extraneous_files/d.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/a.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/d.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/d.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/a.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/some_depth/a.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/headers/recursive_pass/some_depth/d.drawio` & `compliance-trestle-2.2.1/tests/data/author/headers/recursive_pass/some_depth/d.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/author/ssp/ssp_example.json` & `compliance-trestle-2.2.1/tests/data/author/ssp/ssp_example.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/csv/bp.sample.v2.csv` & `compliance-trestle-2.2.1/tests/data/csv/bp.sample.v2.csv`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/csv/component-definitions/bp/component-definition.json` & `compliance-trestle-2.2.1/tests/data/csv/component-definitions/bp/component-definition.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/csv/ocp4-user.v2.csv` & `compliance-trestle-2.2.1/tests/data/csv/ocp4-user.v2.csv`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/jinja/profile_to_docs_no_part_prose.md.jinja` & `compliance-trestle-2.2.1/tests/data/jinja/profile_to_docs_no_part_prose.md.jinja`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/jinja/ssp_template.md.jinja` & `compliance-trestle-2.2.1/tests/data/jinja/ssp_template.md.jinja`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/jinja_markdown_include/env_nested_c_c_double.md` & `compliance-trestle-2.2.1/tests/data/jinja_markdown_include/env_nested_c_c_double.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_def.json` & `compliance-trestle-2.2.1/tests/data/json/comp_def.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_def_a.json` & `compliance-trestle-2.2.1/tests/data/json/comp_def_a.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_def_b.json` & `compliance-trestle-2.2.1/tests/data/json/comp_def_b.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_def_readme.md` & `compliance-trestle-2.2.1/tests/data/json/comp_def_readme.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_prof.json` & `compliance-trestle-2.2.1/tests/data/json/comp_prof.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_prof_aa.json` & `compliance-trestle-2.2.1/tests/data/json/comp_prof_aa.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_prof_ab.json` & `compliance-trestle-2.2.1/tests/data/json/comp_prof_ab.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_prof_ba.json` & `compliance-trestle-2.2.1/tests/data/json/comp_prof_ba.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_prof_bad.json` & `compliance-trestle-2.2.1/tests/data/json/comp_prof_bad.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_prof_bb.json` & `compliance-trestle-2.2.1/tests/data/json/comp_prof_bb.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/comp_prof_part_none.json` & `compliance-trestle-2.2.1/tests/data/json/comp_prof_part_none.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/leveraged_ssp.json` & `compliance-trestle-2.2.1/tests/data/json/leveraged_ssp.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/minimal_catalog.json` & `compliance-trestle-2.2.1/tests/data/json/minimal_catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_bad_oscal_version.json` & `compliance-trestle-2.2.1/tests/data/json/minimal_catalog_bad_oscal_version.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_extra_fields.json` & `compliance-trestle-2.2.1/tests/data/json/minimal_catalog_extra_fields.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles.json` & `compliance-trestle-2.2.1/tests/data/json/minimal_catalog_roles.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles_double.json` & `compliance-trestle-2.2.1/tests/data/json/minimal_catalog_roles_double.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_roles_double_rp.json` & `compliance-trestle-2.2.1/tests/data/json/minimal_catalog_roles_double_rp.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/minimal_catalog_with_groups.json` & `compliance-trestle-2.2.1/tests/data/json/minimal_catalog_with_groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/nist_tutorial_catalog.json` & `compliance-trestle-2.2.1/tests/data/json/nist_tutorial_catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/nist_tutorial_profile.json` & `compliance-trestle-2.2.1/tests/data/json/nist_tutorial_profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/profile_bad_control.json` & `compliance-trestle-2.2.1/tests/data/json/profile_bad_control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/profile_missing_position.json` & `compliance-trestle-2.2.1/tests/data/json/profile_missing_position.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/profile_with_alter_props.json` & `compliance-trestle-2.2.1/tests/data/json/profile_with_alter_props.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/profile_with_alter_subparts.json` & `compliance-trestle-2.2.1/tests/data/json/profile_with_alter_subparts.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/profile_with_incorrect_alter.json` & `compliance-trestle-2.2.1/tests/data/json/profile_with_incorrect_alter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/pull_nist_profile.json` & `compliance-trestle-2.2.1/tests/data/json/pull_nist_profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/simple_catalog_no_parts.json` & `compliance-trestle-2.2.1/tests/data/json/simple_catalog_no_parts.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/simple_mapping.json` & `compliance-trestle-2.2.1/tests/data/json/simple_mapping.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/simple_test_profile.json` & `compliance-trestle-2.2.1/tests/data/json/simple_test_profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/simple_test_profile_less.json` & `compliance-trestle-2.2.1/tests/data/json/simple_test_profile_less.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/simple_test_profile_more.json` & `compliance-trestle-2.2.1/tests/data/json/simple_test_profile_more.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/simple_test_profile_no_params.json` & `compliance-trestle-2.2.1/tests/data/json/simple_test_profile_no_params.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/simple_test_profile_single.json` & `compliance-trestle-2.2.1/tests/data/json/simple_test_profile_single.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/simplified_nist_catalog.json` & `compliance-trestle-2.2.1/tests/data/json/simplified_nist_catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/simplified_nist_profile.json` & `compliance-trestle-2.2.1/tests/data/json/simplified_nist_profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/test_profile_a.json` & `compliance-trestle-2.2.1/tests/data/json/test_profile_a.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/test_profile_b.json` & `compliance-trestle-2.2.1/tests/data/json/test_profile_b.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/test_profile_c.json` & `compliance-trestle-2.2.1/tests/data/json/test_profile_c.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/test_profile_d.json` & `compliance-trestle-2.2.1/tests/data/json/test_profile_d.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/test_profile_e.json` & `compliance-trestle-2.2.1/tests/data/json/test_profile_e.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/test_profile_f.json` & `compliance-trestle-2.2.1/tests/data/json/test_profile_f.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/json/test_profile_g.json` & `compliance-trestle-2.2.1/tests/data/json/test_profile_g.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/markdown/valid_complex_md.md` & `compliance-trestle-2.2.1/tests/data/markdown/valid_complex_md.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/markdown/valid_no_headers.md` & `compliance-trestle-2.2.1/tests/data/markdown/valid_no_headers.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/markdown/valid_no_lvl1_headers.md` & `compliance-trestle-2.2.1/tests/data/markdown/valid_no_lvl1_headers.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/ocp4-cis/catalog.json` & `compliance-trestle-2.2.1/tests/data/ocp4-cis/catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/.trestle/config.ini` & `compliance-trestle-2.2.1/tests/data/split_merge/.trestle/config.ini`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/README.md` & `compliance-trestle-2.2.1/tests/data/split_merge/README.md`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/catalog.json` & `compliance-trestle-2.2.1/tests/data/split_merge/load_distributed/catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/load_distributed/groups.json` & `compliance-trestle-2.2.1/tests/data/split_merge/load_distributed/groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/catalog.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step0-merged_catalog/catalogs/mycatalog/catalog.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step0-merged_catalog/next_step.sh` & `compliance-trestle-2.2.1/tests/data/split_merge/step0-merged_catalog/next_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/back-matter.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/back-matter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/groups.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/metadata.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/catalogs/mycatalog/catalog/metadata.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/next_step.sh` & `compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/next_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step1-split_root_elements/previous_step.sh` & `compliance-trestle-2.2.1/tests/data/split_merge/step1-split_root_elements/previous_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/back-matter.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/back-matter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/groups.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/parties.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata/parties.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/catalogs/mycatalog/catalog/metadata.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/next_step.sh` & `compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/next_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step2-split_metadata_elements/previous_step.sh` & `compliance-trestle-2.2.1/tests/data/split_merge/step2-split_metadata_elements/previous_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/back-matter.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/back-matter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/groups.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/groups.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/parties.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata/parties.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/catalogs/mycatalog/catalog/metadata.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/next_step.sh` & `compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/next_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/previous_step.sh` & `compliance-trestle-2.2.1/tests/data/split_merge/step3-split_metadata_array_additionalproperties_elements/previous_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/back-matter.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/back-matter.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00012__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00013__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00014__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00015__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00016__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00017__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00018__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00019__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00020__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00021__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00022__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00023__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00023__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00024__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00000__group/controls/00024__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00001__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00012__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00013__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00014__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00015__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00002__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00003__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00012__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00013__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00004__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00012__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00005__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00006__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00007__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00008__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00009__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00012__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00013__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00014__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00015__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00016__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00017__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00018__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00019__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00020__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00021__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00022__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00010__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00011__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00012__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00013__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00014__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00015__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00016__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00017__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00018__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00019__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00020__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00021__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00022__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00023__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00023__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00024__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00024__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00025__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00025__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00026__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00026__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00027__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00027__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00028__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00028__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00029__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00029__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00030__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00030__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00031__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group/controls/00031__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00012__group.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00013__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00014__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00015__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00012__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00013__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00014__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00015__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00016__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00017__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00018__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00019__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00020__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00021__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00022__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00016__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00012__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00013__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00014__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00015__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00016__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00017__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00018__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00019__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00020__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00021__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00022__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00023__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00023__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00024__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00024__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00025__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00025__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00026__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00026__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00027__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00027__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00028__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00028__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00029__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00029__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00030__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00030__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00031__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00031__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00032__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00032__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00033__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00033__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00034__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00034__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00035__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00035__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00036__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00036__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00037__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00037__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00038__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00038__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00039__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00039__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00040__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00040__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00041__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00041__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00042__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00042__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00043__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00043__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00044__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00044__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00045__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00045__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00046__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00046__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00047__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00047__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00048__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00048__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00049__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00049__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00050__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00017__group/controls/00050__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00012__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00012__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00013__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00013__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00014__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00014__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00015__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00015__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00016__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00016__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00017__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00017__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00018__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00018__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00019__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00019__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00020__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00020__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00021__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00021__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00022__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00018__group/controls/00022__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00000__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00000__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00001__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00001__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00002__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00002__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00003__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00003__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00004__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00004__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00005__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00005__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00006__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00006__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00007__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00007__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00008__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00008__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00009__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00009__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00010__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00010__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00011__control.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/groups/00019__group/controls/00011__control.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/parties.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata/parties.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata.json` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/catalogs/mycatalog/catalog/metadata.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/split_merge/step4_split_groups_array/previous_step.sh` & `compliance-trestle-2.2.1/tests/data/split_merge/step4_split_groups_array/previous_step.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/bad_parameter_name_and_description.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/bad_parameter_name_and_description.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/duplicate_column_heading.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/duplicate_column_heading.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_goal_name_id.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/embedded_blank_in_goal_name_id.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_parameter_name.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/embedded_blank_in_parameter_name.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/embedded_blank_in_rule_name_id.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/embedded_blank_in_rule_name_id.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/good.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/good.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/good_with_blank_rows.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/good_with_blank_rows.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/missing_column_heading.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/missing_column_heading.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/missing_control_id.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/missing_control_id.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/missing_resource_title.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/missing_resource_title.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/spread-sheet/missing_rule_name_id.xlsx` & `compliance-trestle-2.2.1/tests/data/spread-sheet/missing_rule_name_id.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_RedHat_OpenShift_Container_Platform_Benchmark_v1.2.0-2.snippet.xlsx` & `compliance-trestle-2.2.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_RedHat_OpenShift_Container_Platform_Benchmark_v1.2.0-2.snippet.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.snippet.xlsx` & `compliance-trestle-2.2.1/tests/data/tasks/cis-xlsx-to-oscal-catalog/CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.snippet.xlsx`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/cis.profile` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input/cis.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/cis.profile` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-catalog/input-bogus/cis.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules.json` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules2.json` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/enabled_rules2.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/rule2var.json` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/rule2var.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules.json` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules2.json` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/extras/selected_rules2.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/component-definition.json` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/output/component-definition.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis-node.profile` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis-node.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis.profile` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/products/ocp4/profiles/cis.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test2.profile` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/profiles/cis-test2.profile`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd.config` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd2.config` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd2.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd3.config` & `compliance-trestle-2.2.1/tests/data/tasks/ocp4-cis-profile-to-oscal-cd/test-ocp4-cis-profile-to-oscal-cd3.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-no.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-no.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-yes.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.39-parms-yes.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-no.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-no.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-yes.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.1.40-parms-yes.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.2.0-parms-no.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-0.2.0-parms-no.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-1.0.0-parms-yes.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-1.0.0-parms-yes.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-no.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-no.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-yes.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-osco-parms-yes.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-scc.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile-scc.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/input/profile.json` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/input/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/osco-profile.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-no/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/osco-profile.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.39-parms-yes/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/osco-profile.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-no/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/osco-profile.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.1.40-parms-yes/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/osco-profile.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-0.2.0-parms-no/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/osco-profile.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-1.0.0-parms-yes/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/osco-profile.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-no/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/osco-profile.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-osco-parms-yes/osco-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/tailored-profile.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/oscal-profile-to-osco-profile/output/profile-scc/tailored-profile.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-configmaps/configmaps.yaml` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-configmaps/configmaps.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_data.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_data.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind0.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind0.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind1.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_kind1.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_resources.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_resources.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-fetcher/cluster_resource_no_results.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-fetcher/cluster_resource_no_results.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-ocp4/ocp4-check-result.xml` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-xml-ocp4/ocp4-check-result.xml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/input-xml-rhel7/rhel7-check-result.xml` & `compliance-trestle-2.2.1/tests/data/tasks/osco/input-xml-rhel7/rhel7-check-result.xml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/output-configmaps/configmaps.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/output-configmaps/configmaps.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/output-fetcher/cluster_resource.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/output-fetcher/cluster_resource.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-ocp4/ocp4-check-result.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/output-xml-ocp4/ocp4-check-result.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/osco/output-xml-rhel7/rhel7-check-result.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/osco/output-xml-rhel7/rhel7-check-result.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/tanium/input/Tanium.comply-results-json` & `compliance-trestle-2.2.1/tests/data/tasks/tanium/input/Tanium.comply-results-json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/tanium/input-doc/Tanium.doc-json` & `compliance-trestle-2.2.1/tests/data/tasks/tanium/input-doc/Tanium.doc-json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/tanium/output/Tanium.oscal.2020.json` & `compliance-trestle-2.2.1/tests/data/tasks/tanium/output/Tanium.oscal.2020.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/tanium/output/Tanium.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/tanium/output/Tanium.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/xccdf/output/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-1.3.5/ssg-ocp4-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-compressed/ssg-rhel7-ds-cis-111.222.333.444-pod.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-configmaps/configmaps.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-configmaps/configmaps.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-fetcher/cluster_resource.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-fetcher/cluster_resource.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-ocp4/ocp4-check-result.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-xml-ocp4/ocp4-check-result.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xccdf/output-xml-rhel7/rhel7-check-result.oscal.json` & `compliance-trestle-2.2.1/tests/data/tasks/xccdf/output-xml-rhel7/rhel7-check-result.oscal.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/component-definition.json` & `compliance-trestle-2.2.1/tests/data/tasks/xlsx/output/component-definition.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output/profile.json` & `compliance-trestle-2.2.1/tests/data/tasks/xlsx/output/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-check/profile.json` & `compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-by-check/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-control/profile.json` & `compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-by-control/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-by-rule/profile.json` & `compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-by-rule/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-filtered/profile.json` & `compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-filtered/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-control-id/profile.json` & `compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-missing-control-id/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xlsx/output-missing-rule-name-id/profile.json` & `compliance-trestle-2.2.1/tests/data/tasks/xlsx/output-missing-rule-name-id/profile.json`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/tasks/xlsx/test-xlsx-to-oscal-cd.config` & `compliance-trestle-2.2.1/tests/data/tasks/xlsx/test-xlsx-to-oscal-cd.config`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/yaml/bad_component_dup_uuid.yaml` & `compliance-trestle-2.2.1/tests/data/yaml/bad_component_dup_uuid.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/yaml/bad_component_no_tz.yaml` & `compliance-trestle-2.2.1/tests/data/yaml/bad_component_no_tz.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/yaml/good_component.yaml` & `compliance-trestle-2.2.1/tests/data/yaml/good_component.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/yaml/good_component_diff_tz.yaml` & `compliance-trestle-2.2.1/tests/data/yaml/good_component_diff_tz.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/data/yaml/header_with_metadata.yaml` & `compliance-trestle-2.2.1/tests/data/yaml/header_with_metadata.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/functionality/__init__.py` & `compliance-trestle-2.2.1/tests/functionality/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/functionality/chevron_test.py` & `compliance-trestle-2.2.1/tests/functionality/chevron_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/functionality/example_test.py` & `compliance-trestle-2.2.1/tests/functionality/example_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/functionality/pathlib_test.py` & `compliance-trestle-2.2.1/tests/functionality/pathlib_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/manual_tests/split_test_1.sh` & `compliance-trestle-2.2.1/tests/manual_tests/split_test_1.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/manual_tests/split_test_issue_630.sh` & `compliance-trestle-2.2.1/tests/manual_tests/split_test_issue_630.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/manual_tests/split_validate_test.sh` & `compliance-trestle-2.2.1/tests/manual_tests/split_validate_test.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/manual_tests/test_binary.sh` & `compliance-trestle-2.2.1/tests/manual_tests/test_binary.sh`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/test_utils.py` & `compliance-trestle-2.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/cli_test.py` & `compliance-trestle-2.2.1/tests/trestle/cli_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/core/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/base_model_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/base_model_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/add_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/add_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/assemble_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/assemble_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/catalog_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/catalog_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/command_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/command_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/component_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/component_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/docs_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/docs_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/folders_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/folders_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/headers_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/headers_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/jinja_cmd_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/jinja_cmd_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/profile_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/profile_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import pytest
 
 from ruamel.yaml import YAML
 
 from tests import test_utils
 
 import trestle.common.const as const
+import trestle.core.generators as gens
 import trestle.oscal.catalog as cat
 import trestle.oscal.common as com
 import trestle.oscal.profile as prof
 from trestle.cli import Trestle
 from trestle.common import file_utils
 from trestle.common.err import TrestleError
 from trestle.common.list_utils import comma_colon_sep_to_dict, comma_sep_to_list
@@ -270,15 +271,15 @@
                                                  prof.Profile, FileContentType.JSON)
     assert ModelUtils.model_age(profile) < test_utils.NEW_MODEL_AGE_SECONDS
     # get the set_params from the assembled profile
     set_params = profile.modify.set_parameters
     if set_parameters_flag:
         assert set_params[2].values[0] == 'new value'
         assert set_params[1].props[0].ns == const.TRESTLE_GENERIC_NS
-        assert len(set_params) == 15
+        assert len(set_params) == 18
     else:
         # the original profile did not have ns set for this display name
         # confirm the namespace is not defined unless set_parameters_flag is True
         # i.e. the setting of ns for display-name is not automatic unless set-parameters is true
         assert set_params[2].values[0] == 'officer'
         assert set_params[1].props[0].ns is None
         assert len(set_params) == 15
@@ -376,15 +377,15 @@
         profile, _ = ModelUtils.load_model_for_class(
             tmp_trestle_dir, assembled_prof_name,
             prof.Profile,
             FileContentType.JSON
         )
         set_params = profile.modify.set_parameters
 
-        assert len(set_params) == 15
+        assert len(set_params) == 18
         assert set_params[0].values[0] == 'all personnel'
         # the label is present in the header so it ends up in the set_parameter
         assert set_params[0].label == 'label from edit'
         assert set_params[1].param_id == 'ac-1_prm_2'
         assert set_params[1].values[0] == 'Organization-level'
         assert set_params[1].values[1] == 'System-level'
         assert set_params[2].values[0] == 'new value'
@@ -1111,7 +1112,126 @@
     prof_inherit = ProfileInherit()
     assert prof_inherit._run(args) == 1
 
     # Force a failure with a cyclic dependency
     args.output = args.profile
     prof_inherit = ProfileInherit()
     assert prof_inherit._run(args) == 2
+
+
+def test_profile_generate_assemble_parameter_aggregation(
+    tmp_trestle_dir: pathlib.Path, monkeypatch: MonkeyPatch
+) -> None:
+    """Test the profile markdown generator."""
+    _, assembled_prof_dir, _, markdown_path = setup_profile_generate(tmp_trestle_dir, 'simple_test_profile.json')
+    yaml_header_path = test_utils.YAML_TEST_DATA_PATH / 'good_simple.yaml'
+    ac_path = markdown_path / 'ac'
+
+    nist_cat, _ = ModelUtils.load_model_for_class(tmp_trestle_dir, 'nist_cat', cat.Catalog, FileContentType.JSON)
+
+    appended_prop = {'name': 'aggregates', 'value': 'at-02_odp.01'}
+    ac_1 = nist_cat.groups[0].controls[0]
+    ac_1.params[2].props = []
+    ac_1.params[2].props.append(appended_prop)
+    appended_extra_param = {
+        'id': 'at-02_odp.01',
+        'props': [{
+            'name': 'label', 'value': 'AT-02_ODP[01]', 'class': 'sp800-53a'
+        }],
+        'label': 'frequency',
+        'guidelines': [{
+            'prose': 'blah'
+        }]
+    }
+    ac_1.params.append(appended_extra_param)
+
+    ModelUtils.save_top_level_model(nist_cat, tmp_trestle_dir, 'nist_cat', FileContentType.JSON)
+
+    # convert resolved profile catalog to markdown then assemble it after adding an item to a control
+    # generate, edit, assemble
+    test_args = f'trestle author profile-generate -n {prof_name} -o {md_name} -rs NeededExtra'.split(  # noqa E501
+    )
+    test_args.extend(['-y', str(yaml_header_path)])
+    test_args.extend(['-s', all_sections_str])
+    monkeypatch.setattr(sys, 'argv', test_args)
+
+    assert Trestle().run() == 0
+
+    fc = test_utils.FileChecker(ac_path)
+
+    assert Trestle().run() == 0
+
+    assert fc.files_unchanged()
+
+    # assemble based on set_parameters_flag
+    test_args = f'trestle author profile-assemble -n {prof_name} -m {md_name} -o {assembled_prof_name}'.split()
+    test_args.append('-sp')
+    assembled_prof_dir.mkdir()
+    monkeypatch.setattr(sys, 'argv', test_args)
+    assert Trestle().run() == 0
+
+
+def test_profile_generate_assesment_objectives(tmp_trestle_dir: pathlib.Path, monkeypatch: MonkeyPatch) -> None:
+    """Test the profile markdown generator."""
+    _, _, _, _ = setup_profile_generate(tmp_trestle_dir, 'simple_test_profile.json')
+    yaml_header_path = test_utils.YAML_TEST_DATA_PATH / 'good_simple.yaml'
+
+    profile, _ = ModelUtils.load_model_for_class(tmp_trestle_dir, 'my_prof', prof.Profile, FileContentType.JSON)
+
+    # create with-id to load at-2 control with its corresponding assesment objectives
+    with_id_at_2 = gens.generate_sample_model(prof.WithId)
+    with_id_at_2.__root__ = 'at-2'
+
+    profile.imports[0].include_controls[0].with_ids.append(with_id_at_2)
+
+    ModelUtils.save_top_level_model(profile, tmp_trestle_dir, 'my_prof', FileContentType.JSON)
+
+    nist_cat, _ = ModelUtils.load_model_for_class(tmp_trestle_dir, 'nist_cat', cat.Catalog, FileContentType.JSON)
+    # create assesment objectives json for adding it to the control in the catalog
+    assesment_objectives = {
+        'id': 'at-2_obj',
+        'name': 'assessment-objective',
+        'props': [{
+            'name': 'label', 'value': 'AT-02', 'class': 'sp800-53a'
+        }],
+        'parts': [
+            {
+                'id': 'at-2_obj.a',
+                'name': 'assessment-objective',
+                'props': [{
+                    'name': 'label', 'value': 'AT-02a.', 'class': 'sp800-53a'
+                }],
+                'parts': [
+                    {
+                        'id': 'at-2_obj.a.1-2',
+                        'name': 'assessment-objective',
+                        'props': [{
+                            'name': 'label', 'value': 'AT-02a.01[02]', 'class': 'sp800-53a'
+                        }],
+                        'prose': 'some example prose'
+                    },
+                    {
+                        'id': 'at-2_obj.a.1-3',
+                        'name': 'assessment-objective',
+                        'props': [{
+                            'name': 'label', 'value': 'AT-02a.01[03]', 'class': 'sp800-53a'
+                        }],
+                        'prose': 'some example prose'
+                    }
+                ]
+            }
+        ]
+    }
+
+    at_2 = nist_cat.groups[1].controls[1]
+    at_2.parts.append(assesment_objectives)
+    ModelUtils.save_top_level_model(nist_cat, tmp_trestle_dir, 'nist_cat', FileContentType.JSON)
+
+    # convert resolved profile catalog to markdown then assemble it after adding an item to a control
+    # generate, edit, assemble
+    test_args = f'trestle author profile-generate -n {prof_name} -o {md_name} -rs NeededExtra'.split(  # noqa E501
+    )
+    test_args.extend(['-y', str(yaml_header_path)])
+    test_args.extend(['-s', all_sections_str])
+    monkeypatch.setattr(sys, 'argv', test_args)
+
+    assert Trestle().run() == 0
```

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/ssp_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/ssp_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/author/versioning/template_versioning_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/author/versioning/template_versioning_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/cmd_utils_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/cmd_utils_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/create_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/create_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/describe_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/describe_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/href_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/href_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/import__test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/import__test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/init_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/init_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/merge_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/merge_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/partial_object_validate_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/partial_object_validate_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/remove_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/remove_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/replicate_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/replicate_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/split_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/split_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/task_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/task_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/validate_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/validate_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/commands/version_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/commands/version_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/control_io_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/control_io_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/draw_io_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/draw_io_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/err_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/err_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/generator_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/generator_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/jinja_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/jinja_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/markdown/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/core/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/markdown/markdown_node_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/markdown/markdown_node_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/markdown/markdown_validator_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/markdown/markdown_validator_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/create_path_action_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/create_path_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/element_path_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/element_path_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/element_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/element_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/file_content_type_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/file_content_type_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/interfaces_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/interfaces_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/plans_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/plans_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/remove_action_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/remove_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/remove_path_action_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/remove_path_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/update_action_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/update_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/write_action_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/write_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/models/write_file_action_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/models/write_file_action_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/parser_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/parser_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/profile_resolver_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/profile_resolver_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/remote/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/core/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/remote/cache_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/remote/cache_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/repository_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/repository_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/ssp_io_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/ssp_io_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/utils_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/utils_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/core/validator_helper_test.py` & `compliance-trestle-2.2.1/tests/trestle/core/validator_helper_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/main_test.py` & `compliance-trestle-2.2.1/tests/trestle/main_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/parsing/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/parsing/parsing_test.py` & `compliance-trestle-2.2.1/tests/trestle/parsing/parsing_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/base_task_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/base_task_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/cis_xlsx_to_oscal_catalog_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/cis_xlsx_to_oscal_catalog_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/csv_to_oscal_cd_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/csv_to_oscal_cd_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -657,15 +657,15 @@
     assert row[13] == 'allowed_admins_per_account'
     assert row[15] == '10'
     row[15] = ''
     with mock.patch('trestle.tasks.csv_to_oscal_cd.csv.reader') as mock_csv_reader:
         mock_csv_reader.return_value = rows
         tgt = csv_to_oscal_cd.CsvToOscalComponentDefinition(section)
         retval = tgt.execute()
-        assert retval == TaskOutcome.FAILURE
+        assert retval == TaskOutcome.SUCCESS
 
 
 def test_execute_change_param_default_value(tmp_path: pathlib.Path) -> None:
     """Test execute change param default_value."""
     config, section = _get_config_section_init(tmp_path, 'test-csv-to-oscal-cd-bp.config')
     section['component-definition'] = 'tests/data/csv/component-definitions/bp/component-definition.json'
     # change default param default value
```

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/ocp4_cis_profile_to_oscal_catalog_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/ocp4_cis_profile_to_oscal_catalog_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/ocp4_cis_profile_to_oscal_cd_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/ocp4_cis_profile_to_oscal_cd_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/oscal_catalog_to_csv_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/oscal_catalog_to_csv_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/oscal_profile_to_osco_profile_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/oscal_profile_to_osco_profile_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/osco_result_to_oscal_ar_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/osco_result_to_oscal_ar_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/tanium_result_to_oscal_ar_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/tanium_result_to_oscal_ar_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/transform_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/transform_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/xccdf_result_to_oscal_ar_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/xccdf_result_to_oscal_ar_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/xlsx_to_oscal_cd_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/xlsx_to_oscal_cd_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/tasks/xlsx_to_oscal_profile_test.py` & `compliance-trestle-2.2.1/tests/trestle/tasks/xlsx_to_oscal_profile_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/transforms/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/transforms/transformer_factory_test.py` & `compliance-trestle-2.2.1/tests/trestle/transforms/transformer_factory_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/transforms/transformer_helper_test.py` & `compliance-trestle-2.2.1/tests/trestle/transforms/transformer_helper_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/utils/__init__.py` & `compliance-trestle-2.2.1/tests/trestle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/utils/fs_test.py` & `compliance-trestle-2.2.1/tests/trestle/utils/fs_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/utils/list_utils_test.py` & `compliance-trestle-2.2.1/tests/trestle/utils/list_utils_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/utils/load_distributed_test.py` & `compliance-trestle-2.2.1/tests/trestle/utils/load_distributed_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/utils/md_writer_test.py` & `compliance-trestle-2.2.1/tests/trestle/utils/md_writer_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/tests/trestle/utils/trash_test.py` & `compliance-trestle-2.2.1/tests/trestle/utils/trash_test.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/__init__.py` & `compliance-trestle-2.2.1/trestle/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 Trestle is a tool to which enables the creation and validation of
 documentation artifacts for compliance requirements. It leverages NIST's
 OSCAL (https://pages.nist.gov/OSCAL/documentation/) as a standard data
 format for interchange between tools & people and provides an
 opinionated approach to OSCAL adoption.
 """
 
-__version__ = '2.2.0'
+__version__ = '2.2.1'
```

### Comparing `compliance-trestle-2.2.0/trestle/__main__.py` & `compliance-trestle-2.2.1/trestle/__main__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/cli.py` & `compliance-trestle-2.2.1/trestle/cli.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/__init__.py` & `compliance-trestle-2.2.1/trestle/common/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/common_types.py` & `compliance-trestle-2.2.1/trestle/common/common_types.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/const.py` & `compliance-trestle-2.2.1/trestle/common/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,15 @@
 # extracts foo and bar from ...[foo](bar)...
 MARKDOWN_URL_REGEX = r'\[([^\]]+)\]\(([^)]+)\)'
 
 # Governed header template version
 TEMPLATE_VERSION_REGEX = r'[0-9]+.[0-9]+.[0-9]+'
 
 OBJECTIVE_PART = 'objective'
+ASSESMENT_OBJECTIVE_PART = 'assessment-objective'
 TABLE_OF_PARAMS_PART = 'table_of_parameters'
 
 # extracts standalone uuid's from anywhere in string
 UUID_REGEX = r'(?:^|[0-9A-Za-f])([0-9A-Fa-f]{8}-[0-9A-Fa-f]{4}-4[0-9A-Fa-f]{3}-[89ABab][0-9A-Fa-f]{3}-[0-9A-Fa-f]{12})(?:$|[^0-9A-Za-z])'  # noqa FS003 E501
 
 SSP_MAIN_COMP_NAME = 'This System'
```

### Comparing `compliance-trestle-2.2.0/trestle/common/err.py` & `compliance-trestle-2.2.1/trestle/common/err.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/file_utils.py` & `compliance-trestle-2.2.1/trestle/common/file_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/list_utils.py` & `compliance-trestle-2.2.1/trestle/common/list_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/load_validate.py` & `compliance-trestle-2.2.1/trestle/common/load_validate.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/log.py` & `compliance-trestle-2.2.1/trestle/common/log.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/model_utils.py` & `compliance-trestle-2.2.1/trestle/common/model_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/str_utils.py` & `compliance-trestle-2.2.1/trestle/common/str_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/trash.py` & `compliance-trestle-2.2.1/trestle/common/trash.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/common/type_utils.py` & `compliance-trestle-2.2.1/trestle/common/type_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/__init__.py` & `compliance-trestle-2.2.1/trestle/core/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/all_validator.py` & `compliance-trestle-2.2.1/trestle/core/all_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/base_model.py` & `compliance-trestle-2.2.1/trestle/core/base_model.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/catalog/__init__.py` & `compliance-trestle-2.2.1/trestle/core/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/catalog/catalog_api.py` & `compliance-trestle-2.2.1/trestle/core/catalog/catalog_api.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/catalog/catalog_interface.py` & `compliance-trestle-2.2.1/trestle/core/catalog/catalog_interface.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/catalog/catalog_merger.py` & `compliance-trestle-2.2.1/trestle/core/catalog/catalog_merger.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/catalog/catalog_reader.py` & `compliance-trestle-2.2.1/trestle/core/catalog/catalog_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,16 @@
                     write_mode
                 )
                 alters_map[sort_id] = control_alters
                 for param_id, param_dict in control_param_dict.items():
                     # if profile_values are present, overwrite values with them
                     if const.PROFILE_VALUES in param_dict:
                         param_dict[const.VALUES] = param_dict.pop(const.PROFILE_VALUES)
-                        final_param_dict[param_id] = param_dict
-                        param_sort_map[param_id] = sort_id
+                    final_param_dict[param_id] = param_dict
+                    param_sort_map[param_id] = sort_id
         new_alters: List[prof.Alter] = []
         # fill the alters according to the control sorting order
         for key in sorted(alters_map.keys()):
             new_alters.extend(alters_map[key])
         return new_alters, final_param_dict, param_sort_map
 
     def read_catalog_from_markdown(self, md_path: pathlib.Path, set_parameters_flag: bool) -> cat.Catalog:
```

### Comparing `compliance-trestle-2.2.0/trestle/core/catalog/catalog_writer.py` & `compliance-trestle-2.2.1/trestle/core/catalog/catalog_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import copy
 import logging
 from typing import Any, Dict, List
 
 import trestle.common.const as const
 import trestle.oscal.catalog as cat
-from trestle.common.list_utils import as_list, deep_get, none_if_empty
+from trestle.common.list_utils import as_list, deep_get, delete_list_from_list, none_if_empty
 from trestle.common.model_utils import ModelUtils
 from trestle.core.catalog.catalog_interface import CatalogInterface
 from trestle.core.catalog.catalog_merger import CatalogMerger
 from trestle.core.control_context import ContextPurpose, ControlContext
 from trestle.core.control_interface import ComponentImpInfo, ControlInterface
 from trestle.core.control_writer import ControlWriter
 from trestle.oscal import common
@@ -59,14 +59,25 @@
             new_context = ControlContext.clone(context)
             new_context.merged_header = {}
 
             new_context = self._add_inherited_props_to_header(new_context, control.id)
 
             # get all params and vals for this control from the resolved profile catalog with block adds in effect
             control_param_dict = ControlInterface.get_control_param_dict(control, False)
+            to_delete = []
+            # removes aggregate parameters to be non-editable in markdowns
+            props_by_param_ids = {}
+            for param_id, values_dict in control_param_dict.items():
+                props_by_param_ids[param_id] = [
+                    prop for prop in as_list(values_dict.props) if prop.name == 'aggregates'
+                ]
+            to_delete = list({k: v for k, v in props_by_param_ids.items() if v != []}.keys())
+            unique_params_to_del = list(set(to_delete))
+            if unique_params_to_del:
+                delete_list_from_list(control_param_dict, unique_params_to_del)
 
             set_param_dict = self._construct_set_parameters_dict(profile_set_param_dict, control_param_dict, context)
 
             if set_param_dict:
                 self._add_set_params_from_cli_yaml_header_to_header(new_context, set_param_dict, control_param_dict)
 
             elif const.SET_PARAMS_TAG in new_context.merged_header:
```

### Comparing `compliance-trestle-2.2.0/trestle/core/catalog_validator.py` & `compliance-trestle-2.2.1/trestle/core/catalog_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/__init__.py` & `compliance-trestle-2.2.1/trestle/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/add.py` & `compliance-trestle-2.2.1/trestle/core/commands/add.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/assemble.py` & `compliance-trestle-2.2.1/trestle/core/commands/assemble.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/__init__.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/catalog.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/catalog.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/command.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/command.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/common.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/common.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/component.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/component.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/consts.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/consts.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/docs.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/docs.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/folders.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/folders.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/headers.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/headers.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/jinja.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/jinja.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/profile.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,15 @@
             if sections_dict and const.STATEMENT in sections_dict:
                 logger.warning('statement is not allowed as a section name.')
                 return CmdReturnCodes.COMMAND_ERROR.value
             _, _, profile = ModelUtils.load_distributed(profile_path, trestle_root)
             catalog, inherited_props = ProfileResolver().get_resolved_profile_catalog_and_inherited_props(
                 trestle_root, profile_path, True, True, None, ParameterRep.LEAVE_MOUSTACHE
             )
+
             deep_set(yaml_header, [const.TRESTLE_GLOBAL_TAG, const.PROFILE, const.TITLE], profile.metadata.title)
 
             context = ControlContext.generate(ContextPurpose.PROFILE, True, trestle_root, markdown_path)
             context.cli_yaml_header = yaml_header
             context.sections_dict = sections_dict
             context.profile = profile
             context.overwrite_header_values = overwrite_header_values
@@ -281,14 +282,41 @@
                 new_set_params, key=lambda param: (param_map[param.param_id], param.param_id)
             )
         if profile.modify:
             profile.modify.set_parameters = none_if_empty(profile.modify.set_parameters)
         return changed
 
     @staticmethod
+    def _add_aggregated_parameter(
+        param: Any, param_dict: Dict[str, Any], control_id: str, controls: Any, param_map: Dict[str, str]
+    ) -> None:
+        """
+        Add aggregated parameter value to original parameter.
+
+        Notes:
+            None
+        """
+        # verifies aggregated param is not on grabbed param dict
+        if param.id not in list(param_dict.keys()):
+            param.values = []
+            agg_props = [prop for prop in param.props if prop.name == 'aggregates']
+            for prop in as_list(agg_props):
+                if param_dict[prop.value].get('values'):
+                    agg_param_values = param_dict[prop.value].get('values')
+                    for value in as_list(agg_param_values):
+                        param.values.append(value)
+                else:
+                    agg_param_values = [p for p in controls[control_id] if p.id == prop.value][0]
+                    param.values.append(agg_param_values.props[0].value)
+                dict_param = ModelUtils.parameter_to_dict(param, False)
+                param_dict[param.id] = dict_param
+                param_map[param.id] = control_id
+        return None
+
+    @staticmethod
     def assemble_profile(
         trestle_root: pathlib.Path,
         parent_prof_name: str,
         md_name: str,
         assem_prof_name: str,
         set_parameters_flag: bool,
         regenerate: bool,
@@ -349,14 +377,21 @@
 
         # load the editable sections of the markdown and create Adds for them
         # then overwrite the Adds in the existing profile with the new ones
         # keep track if any changes were made
         catalog_api = CatalogAPI(catalog=catalog, context=context)
         found_alters, param_dict, param_map = catalog_api.read_additional_content_from_md(label_as_key=True)
 
+        controls = {}
+        for group in as_list(catalog.groups):
+            for control in as_list(group.controls):
+                controls[control.id] = control.params
+        for control_id, params in controls.items():
+            for param in as_list(params):
+                ProfileAssemble._add_aggregated_parameter(param, param_dict, control_id, controls, param_map)
         # technically if allowed sections is [] it means no sections are allowed
         if allowed_sections is not None:
             for bad_part in [
                     part for alter in found_alters for add in as_list(alter.adds)
                     for part in as_filtered_list(add.parts, lambda a: a.name not in allowed_sections)  # type: ignore
             ]:
                 raise TrestleError(f'Profile has alter with name {bad_part.name} not in allowed sections.')
```

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/ssp.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/ssp.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/versioning/__init__.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/author/versioning/template_versioning.py` & `compliance-trestle-2.2.1/trestle/core/commands/author/versioning/template_versioning.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/command_docs.py` & `compliance-trestle-2.2.1/trestle/core/commands/command_docs.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/common/__init__.py` & `compliance-trestle-2.2.1/trestle/core/commands/common/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/common/cmd_utils.py` & `compliance-trestle-2.2.1/trestle/core/commands/common/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/common/return_codes.py` & `compliance-trestle-2.2.1/trestle/core/commands/common/return_codes.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/create.py` & `compliance-trestle-2.2.1/trestle/core/commands/create.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/describe.py` & `compliance-trestle-2.2.1/trestle/core/commands/describe.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/href.py` & `compliance-trestle-2.2.1/trestle/core/commands/href.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/import_.py` & `compliance-trestle-2.2.1/trestle/core/commands/import_.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/init.py` & `compliance-trestle-2.2.1/trestle/core/commands/init.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/merge.py` & `compliance-trestle-2.2.1/trestle/core/commands/merge.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/partial_object_validate.py` & `compliance-trestle-2.2.1/trestle/core/commands/partial_object_validate.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/remove.py` & `compliance-trestle-2.2.1/trestle/core/commands/remove.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/replicate.py` & `compliance-trestle-2.2.1/trestle/core/commands/replicate.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/split.py` & `compliance-trestle-2.2.1/trestle/core/commands/split.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/task.py` & `compliance-trestle-2.2.1/trestle/core/commands/task.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/validate.py` & `compliance-trestle-2.2.1/trestle/core/commands/validate.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/commands/version.py` & `compliance-trestle-2.2.1/trestle/core/commands/version.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/control_context.py` & `compliance-trestle-2.2.1/trestle/core/control_context.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/control_interface.py` & `compliance-trestle-2.2.1/trestle/core/control_interface.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/control_reader.py` & `compliance-trestle-2.2.1/trestle/core/control_reader.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/control_writer.py` & `compliance-trestle-2.2.1/trestle/core/control_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,26 +76,28 @@
         self._md_file.set_indent_level(-1)
         self._add_part_and_its_items(control, const.STATEMENT, const.ITEM)
         self._md_file.set_indent_level(-1)
 
     def _add_control_objective(self, control: cat.Control) -> None:
         if control.parts:
             for part in control.parts:
-                if part.name == 'objective':
+                if part.name == const.OBJECTIVE_PART or part.name == const.ASSESMENT_OBJECTIVE_PART:
                     self._md_file.new_paragraph()
                     heading_title = 'Control Objective'
+                    if part.name == const.ASSESMENT_OBJECTIVE_PART:
+                        heading_title = 'Control Assessment Objective'
                     self._md_file.new_header(level=2, title=heading_title)
                     self._md_file.set_indent_level(-1)
-                    self._add_part_and_its_items(control, 'objective', 'objective')
+                    self._add_part_and_its_items(control, part.name, part.name)
                     self._md_file.set_indent_level(-1)
                     return
 
     def _add_sections(self, control: cat.Control, allowed_sections: Optional[List[str]]) -> None:
         """Add the extra control sections after the main ones."""
-        skip_section_list = [const.STATEMENT, const.ITEM, const.OBJECTIVE_PART]
+        skip_section_list = [const.STATEMENT, const.ITEM, const.OBJECTIVE_PART, const.ASSESMENT_OBJECTIVE_PART]
         while True:
             _, name, title, prose = ControlInterface.get_section(control, skip_section_list)
             if not name:
                 return
             if allowed_sections and name not in allowed_sections:
                 skip_section_list.append(name)
                 continue
```

### Comparing `compliance-trestle-2.2.0/trestle/core/docs_control_writer.py` & `compliance-trestle-2.2.1/trestle/core/docs_control_writer.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/draw_io.py` & `compliance-trestle-2.2.1/trestle/core/draw_io.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/duplicates_validator.py` & `compliance-trestle-2.2.1/trestle/core/duplicates_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/generators.py` & `compliance-trestle-2.2.1/trestle/core/generators.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/generic_oscal.py` & `compliance-trestle-2.2.1/trestle/core/generic_oscal.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/jinja.py` & `compliance-trestle-2.2.1/trestle/core/jinja.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/links_validator.py` & `compliance-trestle-2.2.1/trestle/core/links_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/markdown/__init__.py` & `compliance-trestle-2.2.1/trestle/core/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/markdown/base_markdown_node.py` & `compliance-trestle-2.2.1/trestle/core/markdown/base_markdown_node.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/markdown/control_markdown_node.py` & `compliance-trestle-2.2.1/trestle/core/markdown/control_markdown_node.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/markdown/docs_markdown_node.py` & `compliance-trestle-2.2.1/trestle/core/markdown/docs_markdown_node.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/markdown/markdown_api.py` & `compliance-trestle-2.2.1/trestle/core/markdown/markdown_api.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/markdown/markdown_const.py` & `compliance-trestle-2.2.1/trestle/core/markdown/markdown_const.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/markdown/markdown_processor.py` & `compliance-trestle-2.2.1/trestle/core/markdown/markdown_processor.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/markdown/markdown_validator.py` & `compliance-trestle-2.2.1/trestle/core/markdown/markdown_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/markdown/md_writer.py` & `compliance-trestle-2.2.1/trestle/core/markdown/md_writer.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/models/__init__.py` & `compliance-trestle-2.2.1/trestle/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/models/actions.py` & `compliance-trestle-2.2.1/trestle/core/models/actions.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/models/elements.py` & `compliance-trestle-2.2.1/trestle/core/models/elements.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/models/file_content_type.py` & `compliance-trestle-2.2.1/trestle/core/models/file_content_type.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/models/interfaces.py` & `compliance-trestle-2.2.1/trestle/core/models/interfaces.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/models/plans.py` & `compliance-trestle-2.2.1/trestle/core/models/plans.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/object_factory.py` & `compliance-trestle-2.2.1/trestle/core/object_factory.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/parser.py` & `compliance-trestle-2.2.1/trestle/core/parser.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/pipeline.py` & `compliance-trestle-2.2.1/trestle/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/profile_resolver.py` & `compliance-trestle-2.2.1/trestle/core/profile_resolver.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/refs_validator.py` & `compliance-trestle-2.2.1/trestle/core/refs_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/remote/__init__.py` & `compliance-trestle-2.2.1/trestle/core/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/remote/cache.py` & `compliance-trestle-2.2.1/trestle/core/remote/cache.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/repository.py` & `compliance-trestle-2.2.1/trestle/core/repository.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/resolver/__init__.py` & `compliance-trestle-2.2.1/trestle/core/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/resolver/_import.py` & `compliance-trestle-2.2.1/trestle/core/resolver/_import.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/resolver/merge.py` & `compliance-trestle-2.2.1/trestle/core/resolver/merge.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/resolver/modify.py` & `compliance-trestle-2.2.1/trestle/core/resolver/modify.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/resolver/prune.py` & `compliance-trestle-2.2.1/trestle/core/resolver/prune.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/rule_parameters_validator.py` & `compliance-trestle-2.2.1/trestle/core/rule_parameters_validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/ssp_io.py` & `compliance-trestle-2.2.1/trestle/core/ssp_io.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/trestle_base_model.py` & `compliance-trestle-2.2.1/trestle/core/trestle_base_model.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/validator.py` & `compliance-trestle-2.2.1/trestle/core/validator.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/core/validator_factory.py` & `compliance-trestle-2.2.1/trestle/core/validator_factory.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/oscal/__init__.py` & `compliance-trestle-2.2.1/trestle/oscal/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/oscal/assessment_plan.py` & `compliance-trestle-2.2.1/trestle/oscal/assessment_plan.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/oscal/assessment_results.py` & `compliance-trestle-2.2.1/trestle/oscal/assessment_results.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/oscal/catalog.py` & `compliance-trestle-2.2.1/trestle/oscal/catalog.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/oscal/common.py` & `compliance-trestle-2.2.1/trestle/oscal/common.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/oscal/component.py` & `compliance-trestle-2.2.1/trestle/oscal/component.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/oscal/poam.py` & `compliance-trestle-2.2.1/trestle/oscal/poam.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/oscal/profile.py` & `compliance-trestle-2.2.1/trestle/oscal/profile.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/oscal/ssp.py` & `compliance-trestle-2.2.1/trestle/oscal/ssp.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/resources/__init__.py` & `compliance-trestle-2.2.1/trestle/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/resources/templates/FedRAMP_control_header_template.yaml` & `compliance-trestle-2.2.1/trestle/resources/templates/FedRAMP_control_header_template.yaml`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/resources/templates/__init__.py` & `compliance-trestle-2.2.1/trestle/resources/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/resources/templates/template.drawio` & `compliance-trestle-2.2.1/trestle/resources/templates/template.drawio`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/__init__.py` & `compliance-trestle-2.2.1/trestle/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/base_task.py` & `compliance-trestle-2.2.1/trestle/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/cis_xlsx_to_oscal_catalog.py` & `compliance-trestle-2.2.1/trestle/tasks/cis_xlsx_to_oscal_catalog.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/csv_to_oscal_cd.py` & `compliance-trestle-2.2.1/trestle/tasks/csv_to_oscal_cd.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,26 +542,27 @@
         component.control_implementations.append(control_implementation)
         return control_implementation
 
     def _create_set_parameter(self, rule_key: tuple) -> SetParameter:
         """Create create set parameters."""
         set_parameter = None
         name = self._csv_mgr.get_value(rule_key, PARAMETER_ID)
-        if name:
+        value = self._csv_mgr.get_value(rule_key, PARAMETER_VALUE_DEFAULT)
+        if name and value:
             value = self._csv_mgr.get_value(rule_key, PARAMETER_VALUE_DEFAULT)
-            if value == '':
-                row_number = self._csv_mgr.get_row_number(rule_key)
-                column_name = PARAMETER_VALUE_DEFAULT
-                text = f'row "{row_number}" missing value for "{column_name}"'
-                raise RuntimeError(text)
             values = value.split(',')
             set_parameter = SetParameter(
                 param_id=name,
                 values=values,
             )
+        elif name:
+            row_number = self._csv_mgr.get_row_number(rule_key)
+            column_name = PARAMETER_VALUE_DEFAULT
+            text = f'row "{row_number}" missing value for "{column_name}"'
+            logger.debug(text)
         return set_parameter
 
     def _get_implemented_requirement(
         self, control_implementation: ControlImplementation, control_id: str
     ) -> ImplementedRequirement:
         """Find or create implemented requirement."""
         if self._validate_controls != 'off':
```

### Comparing `compliance-trestle-2.2.0/trestle/tasks/ocp4_cis_profile_to_oscal_catalog.py` & `compliance-trestle-2.2.1/trestle/tasks/ocp4_cis_profile_to_oscal_catalog.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/ocp4_cis_profile_to_oscal_cd.py` & `compliance-trestle-2.2.1/trestle/tasks/ocp4_cis_profile_to_oscal_cd.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/oscal_catalog_to_csv.py` & `compliance-trestle-2.2.1/trestle/tasks/oscal_catalog_to_csv.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/oscal_profile_to_osco_profile.py` & `compliance-trestle-2.2.1/trestle/tasks/oscal_profile_to_osco_profile.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/osco_result_to_oscal_ar.py` & `compliance-trestle-2.2.1/trestle/tasks/osco_result_to_oscal_ar.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/tanium_result_to_oscal_ar.py` & `compliance-trestle-2.2.1/trestle/tasks/tanium_result_to_oscal_ar.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/transform.py` & `compliance-trestle-2.2.1/trestle/tasks/transform.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/xccdf_result_to_oscal_ar.py` & `compliance-trestle-2.2.1/trestle/tasks/xccdf_result_to_oscal_ar.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/xlsx_helper.py` & `compliance-trestle-2.2.1/trestle/tasks/xlsx_helper.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/xlsx_to_oscal_cd.py` & `compliance-trestle-2.2.1/trestle/tasks/xlsx_to_oscal_cd.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/tasks/xlsx_to_oscal_profile.py` & `compliance-trestle-2.2.1/trestle/tasks/xlsx_to_oscal_profile.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/transforms/__init__.py` & `compliance-trestle-2.2.1/trestle/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/transforms/implementations/__init__.py` & `compliance-trestle-2.2.1/trestle/transforms/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/transforms/implementations/osco.py` & `compliance-trestle-2.2.1/trestle/transforms/implementations/osco.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/transforms/implementations/tanium.py` & `compliance-trestle-2.2.1/trestle/transforms/implementations/tanium.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/transforms/implementations/xccdf.py` & `compliance-trestle-2.2.1/trestle/transforms/implementations/xccdf.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/transforms/results.py` & `compliance-trestle-2.2.1/trestle/transforms/results.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/transforms/transformer_factory.py` & `compliance-trestle-2.2.1/trestle/transforms/transformer_factory.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/transforms/transformer_helper.py` & `compliance-trestle-2.2.1/trestle/transforms/transformer_helper.py`

 * *Files identical despite different names*

### Comparing `compliance-trestle-2.2.0/trestle/transforms/transformer_singleton.py` & `compliance-trestle-2.2.1/trestle/transforms/transformer_singleton.py`

 * *Files identical despite different names*

