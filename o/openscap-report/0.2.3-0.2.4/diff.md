# Comparing `tmp/openscap-report-0.2.3.tar.gz` & `tmp/openscap-report-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openscap-report-0.2.3.tar", last modified: Fri Apr 14 09:26:41 2023, max compression
+gzip compressed data, was "openscap-report-0.2.4.tar", last modified: Wed Jul  5 10:30:18 2023, max compression
```

## Comparing `openscap-report-0.2.3.tar` & `openscap-report-0.2.4.tar`

### file list

```diff
@@ -1,243 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.646995 openscap-report-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-14 09:26:29.000000 openscap-report-0.2.3/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-14 09:26:29.000000 openscap-report-0.2.3/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-14 09:26:29.000000 openscap-report-0.2.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-04-14 09:26:29.000000 openscap-report-0.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-04-14 09:26:29.000000 openscap-report-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 09:26:29.000000 openscap-report-0.2.3/LICENSE.spdx
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 09:26:29.000000 openscap-report-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-14 09:26:41.646995 openscap-report-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-14 09:26:29.000000 openscap-report-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.538993 openscap-report-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/README
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/docs/exts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.538993 openscap-report-0.2.3/docs/exts/sphinxarg/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/exts/sphinxarg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21796 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/exts/sphinxarg/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/exts/sphinxarg/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/exts/sphinxarg/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.538993 openscap-report-0.2.3/docs/manual/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.550994 openscap-report-0.2.3/docs/manual/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    46854 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/about_profile.png
--rw-r--r--   0 runner    (1001) docker     (123)    44006 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/compliance_and_scoring.png
--rw-r--r--   0 runner    (1001) docker     (123)   114896 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/cpe_aplicability_language.png
--rw-r--r--   0 runner    (1001) docker     (123)    79764 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/evaluation_characteristics.png
--rw-r--r--   0 runner    (1001) docker     (123)  8589473 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/example_report.html
--rw-r--r--   0 runner    (1001) docker     (123)  1072728 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/oval.gif
--rw-r--r--   0 runner    (1001) docker     (123)    41993 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/remediation.png
--rw-r--r--   0 runner    (1001) docker     (123)   168763 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/rule_detail.png
--rw-r--r--   0 runner    (1001) docker     (123)    50802 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/assets/rule_overview_section.png
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/manual/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.554994 openscap-report-0.2.3/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.report_generators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.data_structures.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.parsers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/oscap-report.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 09:26:29.000000 openscap-report-0.2.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.554994 openscap-report-0.2.3/openscap_report/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/debug_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.554994 openscap-report-0.2.3/openscap_report/report_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.558994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.558994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   102224 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    79100 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.558994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/base_report.html
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/cpe_graph.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.562994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/
--rw-r--r--   0 runner    (1001) docker     (123)  1413415 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/patternfly.css
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/evaluation_characteristics.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.562994 openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/debug_script.js
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/interactive_script.js
--rw-r--r--   0 runner    (1001) docker     (123)    27002 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/oval_definition_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/oval_graph.html
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/profile_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/remedations.html
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/rule_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/rule_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/rules_overview.html
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/score_bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/search_input.html
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/severity_of_failed_rules.html
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/summary_banner.html
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/html_templates/template_report.html
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/old_style_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/report_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.562994 openscap-report-0.2.3/openscap_report/report_generators/xsl/
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-branding.xsl
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-references.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    55343 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report-impl.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report.xsl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.566994 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json
--rw-r--r--   0 runner    (1001) docker     (123)    88498 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css
--rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/openscap.css
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/openscap.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources-build.sh
--rw-r--r--   0 runner    (1001) docker     (123)   223540 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    21382 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-share.xsl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.566994 openscap-report-0.2.3/openscap_report/scap_results_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.570994 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/json_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_result_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/profile_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/remediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/result_of_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.574994 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/cpe_al_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/full_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/group_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_definition_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_object_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_state_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_test_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/profile_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/remediation_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/report_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/scan_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/scap_results_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.574994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    45405 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    22573 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    72864 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    29292 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/catalog.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xlink.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xml.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    13324 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    13927 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.534994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.578994 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd
--rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd
--rw-r--r--   0 runner    (1001) docker     (123)   230463 2023-04-14 09:26:29.000000 openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.554994 openscap-report-0.2.3/openscap_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 09:26:41.000000 openscap-report-0.2.3/openscap_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:26:29.000000 openscap-report-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:26:41.646995 openscap-report-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-14 09:26:29.000000 openscap-report-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.582994 openscap-report-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration.fmf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.582994 openscap-report-0.2.3/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration_tests/test_basic_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/integration_tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/json_schema_of_report.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/smoke.fmf
--rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/smoke.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.646995 openscap-report-0.2.3/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123) 12129838 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf-container.xml
--rw-r--r--   0 runner    (1001) docker     (123) 23777754 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf-dangling-reference-to.xml
--rw-r--r--   0 runner    (1001) docker     (123) 19008654 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf-report.xml
--rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf-with-removed-info.xml
--rw-r--r--   0 runner    (1001) docker     (123)    48058 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_cpe_check_os_platform.xml
--rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_multi_check.xml
--rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_no_system_data.xml
--rw-r--r--   0 runner    (1001) docker     (123)    36477 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_rule_and_cpe_check.xml
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_simple_rule_fail.xml
--rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/arf_simple_rule_pass.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/empty.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/empty.xml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/plant_catalog.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.646995 openscap-report-0.2.3/tests/test_data/remediations_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt
--rw-r--r--   0 runner    (1001) docker     (123)  7631650 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf-report.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf-with-removed-info.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_multi_check.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_no_system_data.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_rule_and_cpe_check.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_simple_rule_fail.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_data/xccdf_simple_rule_pass.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:41.646995 openscap-report-0.2.3/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_cpe_al_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_debug_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_full_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_json_transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_oval_result_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_oval_tree_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_scap_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tests/unit_tests/test_shared_static_methods_of_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-14 09:26:29.000000 openscap-report-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.274274 openscap-report-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 10:30:06.000000 openscap-report-0.2.4/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-05 10:30:06.000000 openscap-report-0.2.4/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-05 10:30:06.000000 openscap-report-0.2.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-07-05 10:30:06.000000 openscap-report-0.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-07-05 10:30:06.000000 openscap-report-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-05 10:30:06.000000 openscap-report-0.2.4/LICENSE.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-05 10:30:06.000000 openscap-report-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-05 10:30:18.274274 openscap-report-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-05 10:30:06.000000 openscap-report-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.150266 openscap-report-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/README
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.146266 openscap-report-0.2.4/docs/exts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.150266 openscap-report-0.2.4/docs/exts/sphinxarg/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/exts/sphinxarg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21796 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/exts/sphinxarg/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/exts/sphinxarg/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/exts/sphinxarg/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.154266 openscap-report-0.2.4/docs/manual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.166267 openscap-report-0.2.4/docs/manual/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    46854 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/assets/about_profile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44006 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/assets/compliance_and_scoring.png
+-rw-r--r--   0 runner    (1001) docker     (123)   114896 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/assets/cpe_aplicability_language.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79764 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/assets/evaluation_characteristics.png
+-rw-r--r--   0 runner    (1001) docker     (123)  8589473 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/assets/example_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1072728 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/assets/oval.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    41993 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/assets/remediation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   168763 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/assets/rule_detail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50802 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/assets/rule_overview_section.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/test-suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/manual/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.166267 openscap-report-0.2.4/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/modules/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/modules/openscap_report.report_generators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/modules/openscap_report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/modules/openscap_report.scap_results_parser.data_structures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/modules/openscap_report.scap_results_parser.parsers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/modules/openscap_report.scap_results_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/oscap-report.1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-05 10:30:06.000000 openscap-report-0.2.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.166267 openscap-report-0.2.4/openscap_report/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/debug_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.170268 openscap-report-0.2.4/openscap_report/report_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.174268 openscap-report-0.2.4/openscap_report/report_generators/html_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.146266 openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.146266 openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.174268 openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/fonts/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   102224 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    79100 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.174268 openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/pficon/
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/base_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/cpe_graph.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.174268 openscap-report-0.2.4/openscap_report/report_generators/html_templates/css/
+-rw-r--r--   0 runner    (1001) docker     (123)  1413415 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/css/patternfly.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/evaluation_characteristics.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.178268 openscap-report-0.2.4/openscap_report/report_generators/html_templates/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/js/debug_script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/js/interactive_script.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30123 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/oval_definition_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/oval_graph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/profile_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/remedations.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/rule_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/rule_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/rules_overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/score_bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/search_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/severity_of_failed_rules.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/summary_banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/html_templates/template_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/old_style_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/report_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.178268 openscap-report-0.2.4/openscap_report/report_generators/xsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-branding.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-references.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    55343 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-report-impl.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-report.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.182268 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    88498 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/openscap.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/openscap.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources-build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)   223540 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    21382 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-share.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.182268 openscap-report-0.2.4/openscap_report/scap_results_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.186269 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/cpe_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/json_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_result_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/profile_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/remediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/result_of_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.190269 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/cpe_al_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/full_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/group_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_definition_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_object_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_state_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_test_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/profile_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/remediation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/report_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/scan_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/scap_results_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.150266 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.146266 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.190269 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    45405 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    22573 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    72864 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    29292 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.190269 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/common/catalog.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/common/xlink.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/common/xml.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.150266 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.190269 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.190269 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.190269 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.190269 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13324 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    13927 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.150266 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.194269 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)   230463 2023-07-05 10:30:06.000000 openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.170268 openscap-report-0.2.4/openscap_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-05 10:30:18.000000 openscap-report-0.2.4/openscap_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-07-05 10:30:18.000000 openscap-report-0.2.4/openscap_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:30:18.000000 openscap-report-0.2.4/openscap_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 10:30:18.000000 openscap-report-0.2.4/openscap_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:30:17.000000 openscap-report-0.2.4/openscap_report.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 10:30:18.000000 openscap-report-0.2.4/openscap_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 10:30:18.000000 openscap-report-0.2.4/openscap_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:30:06.000000 openscap-report-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:30:18.274274 openscap-report-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-05 10:30:06.000000 openscap-report-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.194269 openscap-report-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/integration.fmf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.194269 openscap-report-0.2.4/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/integration_tests/test_basic_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/integration_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/integration_tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/json_schema_of_report.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/smoke.fmf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/smoke.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.270274 openscap-report-0.2.4/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123) 12129838 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf-container.xml
+-rw-r--r--   0 runner    (1001) docker     (123) 23777754 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf-dangling-reference-to.xml
+-rw-r--r--   0 runner    (1001) docker     (123) 19008654 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf-report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf-with-removed-info.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    48058 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf_cpe_check_os_platform.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf_multi_check.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf_no_system_data.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    36477 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf_rule_and_cpe_check.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf_simple_rule_fail.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/arf_simple_rule_pass.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/empty.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/plant_catalog.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.270274 openscap-report-0.2.4/tests/test_data/remediations_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  7631650 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/xccdf-report.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/xccdf-with-removed-info.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/xccdf_multi_check.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/xccdf_no_system_data.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/xccdf_rule_and_cpe_check.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/xccdf_simple_rule_fail.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_data/xccdf_simple_rule_pass.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:18.274274 openscap-report-0.2.4/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_cpe_al_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_debug_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_full_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_json_transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_oval_result_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_oval_tree_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_scap_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tests/unit_tests/test_shared_static_methods_of_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-05 10:30:06.000000 openscap-report-0.2.4/tox.ini
```

### Comparing `openscap-report-0.2.3/.eslintrc.yml` & `openscap-report-0.2.4/.eslintrc.yml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   default-case: error
   default-case-last: error
   default-param-last: error
   dot-location: error
   dot-notation: 'off'
   eol-last:
     - error
-    - never
+    - always
   eqeqeq: 'off'
   func-call-spacing: error
   func-name-matching: error
   func-names: 'off'
   func-style:
     - error
     - declaration
```

### Comparing `openscap-report-0.2.3/.pylintrc` & `openscap-report-0.2.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/LICENSE` & `openscap-report-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/PKG-INFO` & `openscap-report-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openscap-report
-Version: 0.2.3
+Version: 0.2.4
 Summary: Tool for generating report from results of oscap scan.
 Home-page: https://github.com/OpenSCAP/oscap-report
 Author: Jan Rodak
 Author-email: jrodak@redhat.com
 License: LGPL-2.1 License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openscap-report-0.2.3/README.md` & `openscap-report-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/conf.py` & `openscap-report-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/exts/sphinxarg/ext.py` & `openscap-report-0.2.4/docs/exts/sphinxarg/ext.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/exts/sphinxarg/markdown.py` & `openscap-report-0.2.4/docs/exts/sphinxarg/markdown.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/exts/sphinxarg/parser.py` & `openscap-report-0.2.4/docs/exts/sphinxarg/parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/assets/about_profile.png` & `openscap-report-0.2.4/docs/manual/assets/about_profile.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/assets/compliance_and_scoring.png` & `openscap-report-0.2.4/docs/manual/assets/compliance_and_scoring.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/assets/cpe_aplicability_language.png` & `openscap-report-0.2.4/docs/manual/assets/cpe_aplicability_language.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/assets/evaluation_characteristics.png` & `openscap-report-0.2.4/docs/manual/assets/evaluation_characteristics.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/assets/example_report.html` & `openscap-report-0.2.4/docs/manual/assets/example_report.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/assets/oval.gif` & `openscap-report-0.2.4/docs/manual/assets/oval.gif`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/assets/remediation.png` & `openscap-report-0.2.4/docs/manual/assets/remediation.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/assets/rule_detail.png` & `openscap-report-0.2.4/docs/manual/assets/rule_detail.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/assets/rule_overview_section.png` & `openscap-report-0.2.4/docs/manual/assets/rule_overview_section.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/manual/report.rst` & `openscap-report-0.2.4/docs/manual/report.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/modules/openscap_report.report_generators.rst` & `openscap-report-0.2.4/docs/modules/openscap_report.report_generators.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/modules/openscap_report.rst` & `openscap-report-0.2.4/docs/modules/openscap_report.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.data_structures.rst` & `openscap-report-0.2.4/docs/modules/openscap_report.scap_results_parser.data_structures.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,37 @@
 openscap\_report.scap\_results\_parser.data\_structures package
 ===============================================================
 
 Submodules
 ----------
 
+openscap\_report.scap\_results\_parser.data\_structures.cpe\_logical\_test module
+---------------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.data_structures.cpe_logical_test
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+openscap\_report.scap\_results\_parser.data\_structures.cpe\_platform module
+----------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.data_structures.cpe_platform
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+openscap\_report.scap\_results\_parser.data\_structures.cpe\_result\_eval module
+--------------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.data_structures.cpe_result_eval
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 openscap\_report.scap\_results\_parser.data\_structures.group module
 --------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.data_structures.group
    :members:
    :undoc-members:
    :show-inheritance:
@@ -16,14 +40,22 @@
 -------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.data_structures.identifier
    :members:
    :undoc-members:
    :show-inheritance:
 
+openscap\_report.scap\_results\_parser.data\_structures.json\_transformation module
+-----------------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.data_structures.json_transformation
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 openscap\_report.scap\_results\_parser.data\_structures.oval\_definition module
 -------------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.data_structures.oval_definition
    :members:
    :undoc-members:
    :show-inheritance:
@@ -56,22 +88,38 @@
 ---------------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.data_structures.oval_result_eval
    :members:
    :undoc-members:
    :show-inheritance:
 
+openscap\_report.scap\_results\_parser.data\_structures.oval\_state module
+--------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.data_structures.oval_state
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 openscap\_report.scap\_results\_parser.data\_structures.oval\_test module
 -------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.data_structures.oval_test
    :members:
    :undoc-members:
    :show-inheritance:
 
+openscap\_report.scap\_results\_parser.data\_structures.profile\_info module
+----------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.data_structures.profile_info
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 openscap\_report.scap\_results\_parser.data\_structures.reference module
 ------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.data_structures.reference
    :members:
    :undoc-members:
    :show-inheritance:
@@ -88,22 +136,38 @@
 ---------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.data_structures.report
    :members:
    :undoc-members:
    :show-inheritance:
 
+openscap\_report.scap\_results\_parser.data\_structures.result\_of\_scan module
+-------------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.data_structures.result_of_scan
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 openscap\_report.scap\_results\_parser.data\_structures.rule module
 -------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.data_structures.rule
    :members:
    :undoc-members:
    :show-inheritance:
 
+openscap\_report.scap\_results\_parser.data\_structures.warning module
+----------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.data_structures.warning
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Module contents
 ---------------
 
 .. automodule:: openscap_report.scap_results_parser.data_structures
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.parsers.rst` & `openscap-report-0.2.4/docs/modules/openscap_report.scap_results_parser.parsers.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 openscap\_report.scap\_results\_parser.parsers package
 ======================================================
 
 Submodules
 ----------
 
+openscap\_report.scap\_results\_parser.parsers.cpe\_al\_parser module
+---------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.parsers.cpe_al_parser
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 openscap\_report.scap\_results\_parser.parsers.full\_text\_parser module
 ------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.parsers.full_text_parser
    :members:
    :undoc-members:
    :show-inheritance:
@@ -24,30 +32,54 @@
 ------------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.parsers.oval_definition_parser
    :members:
    :undoc-members:
    :show-inheritance:
 
+openscap\_report.scap\_results\_parser.parsers.oval\_object\_parser module
+--------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.parsers.oval_object_parser
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 openscap\_report.scap\_results\_parser.parsers.oval\_result\_parser module
 --------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.parsers.oval_result_parser
    :members:
    :undoc-members:
    :show-inheritance:
 
+openscap\_report.scap\_results\_parser.parsers.oval\_state\_parser module
+-------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.parsers.oval_state_parser
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 openscap\_report.scap\_results\_parser.parsers.oval\_test\_info\_parser module
 ------------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.parsers.oval_test_info_parser
    :members:
    :undoc-members:
    :show-inheritance:
 
+openscap\_report.scap\_results\_parser.parsers.profile\_info\_parser module
+---------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.parsers.profile_info_parser
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 openscap\_report.scap\_results\_parser.parsers.remediation\_parser module
 -------------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.parsers.remediation_parser
    :members:
    :undoc-members:
    :show-inheritance:
@@ -64,14 +96,30 @@
 ------------------------------------------------------------------
 
 .. automodule:: openscap_report.scap_results_parser.parsers.rule_parser
    :members:
    :undoc-members:
    :show-inheritance:
 
+openscap\_report.scap\_results\_parser.parsers.scan\_result\_parser module
+--------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.parsers.scan_result_parser
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+openscap\_report.scap\_results\_parser.parsers.shared\_static\_methods\_of\_parser module
+-----------------------------------------------------------------------------------------
+
+.. automodule:: openscap_report.scap_results_parser.parsers.shared_static_methods_of_parser
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Module contents
 ---------------
 
 .. automodule:: openscap_report.scap_results_parser.parsers
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `openscap-report-0.2.3/docs/modules/openscap_report.scap_results_parser.rst` & `openscap-report-0.2.4/docs/modules/openscap_report.scap_results_parser.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/cli.py` & `openscap-report-0.2.4/openscap_report/cli.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/debug_settings.py` & `openscap-report-0.2.4/openscap_report/debug_settings.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html.py` & `openscap-report-0.2.4/openscap_report/report_generators/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     @staticmethod
     @pass_context
     def include_file_in_base64(context, relative_path):
         real_path = Path(context.environment.loader.searchpath[0]) / relative_path
         if "RedHat" in relative_path:
             real_path = Path(relative_path)
         if not real_path.exists():
-            logging.warning("Please, install font: %s", real_path.name)
+            logging.info("Please, install font: %s", real_path.name)
             return Markup("NO-FONT-DATA")
         base64_data = None
         with open(real_path, "rb") as file_data:
             base64_data = (base64.b64encode(file_data.read())).decode('utf-8')
         return Markup(base64_data)
 
     @staticmethod
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/base_report.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/base_report.html`

 * *Files 15% similar despite different names*

```diff
@@ -41,24 +41,32 @@
                     <g transform="matrix(0.75266991,0,0,0.75266991,-17.752968,-104.57468)">
                         <path
                             d="m 24.7,173.5 c 0,-9 3.5,-17.5 9.9,-23.9 6.8,-6.8 15.7,-10.4 25,-10 8.6,0.3 16.9,3.9 22.9,9.8 6.4,6.4 9.9,14.9 10,23.8 0.1,9.1 -3.5,17.8 -10,24.3 -13.2,13.2 -34.7,13.1 -48,-0.1 -1.5,-1.5 -1.9,-4.2 0.2,-6.2 l 9,-9 c -2,-3.6 -4.9,-13.1 2.6,-20.7 7.6,-7.6 18.6,-6 24.4,-0.2 3.3,3.3 5.1,7.6 5.1,12.1 0.1,4.6 -1.8,9.1 -5.3,12.5 -4.2,4.2 -10.2,5.8 -16.1,4.4 -1.5,-0.4 -2.4,-1.9 -2.1,-3.4 0.4,-1.5 1.9,-2.4 3.4,-2.1 4.1,1 8,-0.1 10.9,-2.9 2.3,-2.3 3.6,-5.3 3.6,-8.4 0,0 0,-0.1 0,-0.1 0,-3 -1.3,-5.9 -3.5,-8.2 -3.9,-3.9 -11.3,-4.9 -16.5,0.2 -6.3,6.3 -1.6,14.1 -1.6,14.2 1.5,2.4 0.7,5 -0.9,6.3 l -8.4,8.4 c 9.9,8.9 27.2,11.2 39.1,-0.8 5.4,-5.4 8.4,-12.5 8.4,-20 0,-0.1 0,-0.2 0,-0.3 -0.1,-7.5 -3,-14.6 -8.4,-19.9 -5,-5 -11.9,-8 -19.1,-8.2 -7.8,-0.3 -15.2,2.7 -20.9,8.4 -8.7,8.7 -8.7,19 -7.9,24.3 0.3,2.4 1.1,4.9 2.2,7.3 0.6,1.4 0,3.1 -1.4,3.7 -1.4,0.6 -3.1,0 -3.7,-1.4 -1.3,-2.9 -2.2,-5.8 -2.6,-8.7 -0.3,-1.7 -0.4,-3.5 -0.4,-5.2 z"
                             style="fill:#0066CC" />
                     </g>
                 </svg>
                 &nbsp;&nbsp;&nbsp;
-                <h1 class="pf-c-title pf-m-4xl">OSCAP Scan Result</h1>
+                <h1 class="pf-c-title pf-m-4xl">{{ self.title() }}</h1>
             </div>
         </header>
         <main class="pf-c-page__main" tabindex="-1">
             <section class="pf-c-page__main-section pf-m-limit-width pf-m-align-center pf-m-no-fill">
                 <div class="pf-c-page__main-body">
                     {% block content%}
 
                     {% endblock %}
                 </div>
+                <div id="back-to-top-button" class="pf-c-back-to-top" style="visibility: hidden;">
+                    <a class="pf-c-button pf-m-primary" href="#top">
+                      Back to top
+                      <span class="pf-c-button__icon pf-m-end">
+                        <i class="fas fa-angle-up" aria-hidden="true"></i>
+                      </span>
+                    </a>
+                </div>
             </section>
             <footer class="pf-c-page__main-section pf-m-no-fill">
                 <div class="footer-content">
                     <div class="footer-logo">
                         <svg version="1.1" width="52" height="52" alt="Open SCAP logo" role="img">
                             <g transform="matrix(0.75266991,0,0,0.75266991,-17.752968,-104.57468)">
                                 <path
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 {# Copyright 2022, Red Hat, Inc. #} {# SPDX-License-Identifier: LGPL-2.1-or-
 later #}
 
 
  {% block patternfly_css %}{% endblock %} {% block style %}{% endblock %}
         
-****** OSCAP Scan Result ******
+****** {{ self.title() }} ******
 
 {% block content%} {% endblock %}
+Back_to_top
 
 
 *****  Generated by openscap-report *****
 
 {% block interactive_script %}{% endblock %} {% block
 oval_graph_generation_script %}{% endblock %} {%- if
 debug_setting.include_debug_script -%} {% block debug_script %}{% endblock %}
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/cpe_graph.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/cpe_graph.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/patternfly.css` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/css/patternfly.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/css/style.css` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/css/style.css`

 * *Files 20% similar despite different names*

```diff
@@ -170,46 +170,84 @@
     border-radius: 0px !important;
 }
 
 .cpe-label__content::before {
     border-radius: 0px !important;
 }
 
-.tooltip-box {
+.tooltip-box-right-side {
     visibility: hidden;
     position: absolute;
     top: 16%;
     left: 102%;
 }
 
-.tooltip-wrapper:hover .tooltip-box {
+.tooltip-wrapper:hover .tooltip-box-right-side {
     visibility: visible;
-    z-index: 10;
+    z-index: calc(var(--pf-c-tree-view--m-guides__list-item--ZIndex) + 1);
+}
+
+.tooltip-box-top-side {
+    visibility: hidden;
+    position: absolute;
+    top: -120%;
+    left: -185%;
+}
+
+#copy:active .tooltip-box-top-side {
+    visibility: visible;
+    z-index: calc(var(--pf-c-tree-view--m-guides__list-item--ZIndex) + 1);
+}
+
+.tooltip-wrapper:hover .tooltip-box-top-side {
+    visibility: visible;
+    z-index: calc(var(--pf-c-tree-view--m-guides__list-item--ZIndex) + 1);
 }
 
 .tooltip-wrapper {
     text-decoration: underline dotted;
 }
 
+.tooltip-box-top-side-oval-operator {
+    top: unset;
+    bottom: 24px;
+    left: 8px;
+    width: fit-content;
+}
+
+.tooltip-wrapper-oval-operator {
+    position: relative;
+}
+
 .tooltip-wrapper:hover {
     text-decoration: underline;
 }
 
-.tooltip__content-width {
-    width: 20vw;
+.tooltip__text-algin-justify {
     text-align: justify;
-    white-space: pre-line;
-    word-break: break-word;
-    hyphens: auto;
+}
+
+.tooltip__content-width-oval-operator {
+    width: 500px;
+}
+
+.pf-c-tooltip {
+    max-width: fit-content;
 }
 
 .clickable-element {
     text-decoration: underline dotted;
 }
 
 .clickable-element:hover {
     text-decoration: underline;
 }
 
 .remediation-clipboard-padding {
     padding-left: 0px !important;
 }
+
+@media screen and (max-width: 992px) {
+    .disable-scrollbar-for-low-resolution {
+        max-height: unset !important;
+    }
+}
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/evaluation_characteristics.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/evaluation_characteristics.html`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                 </li>
 
                 <li class="pf-c-data-list__item">
                     <div class="pf-c-data-list__item-row">
                         <div class="pf-c-data-list__item-content">
                             <div class="pf-c-data-list__cell"><b>Scanner:</b></div>
                             <div class="pf-c-data-list__cell">
-                                {{- report.scan_result.scanner -}} {{- report.scan_result.scanner_version -}}
+                                {{- report.scan_result.scanner -}}&nbsp;{{- report.scan_result.scanner_version -}}
                             </div>
                         </div>
                     </div>
                 </li>
 
                 <li class="pf-c-data-list__item">
                     <div class="pf-c-data-list__item-row">
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/debug_script.js` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/js/debug_script.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -135,8 +135,8 @@
 00000860: 772d 616c 6c2d 6f76 616c 2d74 6573 742d  w-all-oval-test-
 00000870: 6465 7461 696c 735d 6029 3b0a 2020 2020  details]`);.    
 00000880: 7d0a 2020 2020 7265 7475 726e 2062 7574  }.    return but
 00000890: 746f 6e2e 7061 7265 6e74 4e6f 6465 2e70  ton.parentNode.p
 000008a0: 6172 656e 744e 6f64 652e 7175 6572 7953  arentNode.queryS
 000008b0: 656c 6563 746f 7228 6062 7574 746f 6e5b  elector(`button[
 000008c0: 6964 3d73 686f 772d 616c 6c2d 7275 6c65  id=show-all-rule
-000008d0: 732d 6465 7461 696c 735d 6029 3b0a 7d    s-details]`);.}
+000008d0: 732d 6465 7461 696c 735d 6029 3b0a 7d0a  s-details]`);.}.
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/interactive_script.js` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/js/interactive_script.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -25,14 +25,15 @@
     return prefix + this.replace(/ /ug, "-").toLowerCase();
 };
 
 document.querySelector('main').addEventListener('scroll', () => {
     if ((window.innerHeight + window.scrollY) >= document.body.offsetHeight) {
         show_next_rules();
     }
+    document.getElementById('back-to-top-button').style.visibility = 'visible';
 }, false);
 
 function show_next_rules() {
     const next_five_rules = get_next_five_rules();
     next_five_rules.forEach(rule => {
         rule.classList.remove("hidden");
     });
@@ -125,8 +126,46 @@
     show_rule_detail(self.parentElement.previousSibling.firstChild);
 }
 
 const selector = ".pf-c-clipboard-copy__text";
 document.querySelectorAll("#copy").forEach(el => el.addEventListener('click', () => {
     const el_with_text = el.parentElement.parentElement.parentElement.querySelector(selector);
     navigator.clipboard.writeText(el_with_text.textContent);
-}));
+}));
+
+function clear_input(self) { // eslint-disable-line no-unused-vars
+    self.previousSibling.value = "";
+    search_rule(self.previousSibling);
+}
+
+document.querySelectorAll("#copy").forEach(el => el.appendChild(get_tooltip_copy_to_clipboard()));
+
+function get_tooltip_copy_to_clipboard() { // eslint-disable-line no-unused-vars
+    const div = document.createElement("div");
+
+    const tooltip_div = div.cloneNode();
+    tooltip_div.className = "pf-c-tooltip pf-m-top tooltip-box-top-side";
+    tooltip_div.setAttribute("role", "tooltip");
+
+    const tooltip_arrow_div = div.cloneNode();
+    tooltip_arrow_div.className = "pf-c-tooltip__arrow";
+    tooltip_div.appendChild(tooltip_arrow_div);
+
+    const tooltip_content_div = div.cloneNode();
+    tooltip_content_div.className = "pf-c-tooltip__content";
+    tooltip_content_div.textContent = `Copied to clipboard.`;
+    tooltip_div.appendChild(tooltip_content_div);
+    return tooltip_div;
+}
+
+function toogle_deselect_button(self) { // eslint-disable-line no-unused-vars
+    self.parentElement.parentElement.querySelectorAll('input[type="checkbox"]').forEach(e => {
+        if (self.textContent == 'Deselect all' && e.checked) {
+            e.onchange();
+            e.checked = !e.checked;
+        } else if (self.textContent == 'Select all' && !e.checked) {
+            e.onchange();
+            e.checked = !e.checked;
+        }
+    });
+    self.textContent = self.textContent == 'Deselect all' ? 'Select all' : 'Deselect all';
+}
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -56,14 +56,25 @@
     'fa-question-circle': 'fa-question-circle'
 };
 const COLOR_TRANSLATION = {
     'pf-m-green': '--pf-global--success-color--200',
     'pf-m-red': '--pf-global--danger-color--200',
     '': ''
 };
+const OVAL_OPERATOR_EXPLANATION = {
+    'AND': 'The AND operator produces a true result if every argument is true. If one or more arguments are false, the result of the AND is false. If one or more of the arguments are unknown, and if none of the arguments are false, then the AND operator produces a result of unknown.',
+    'OR': 'The OR operator produces a true result if one or more arguments is true. If every argument is false, the result of the OR is false. If one or more of the arguments are unknown and if none of arguments are true, then the OR operator produces a result of unknown.',
+    'XOR': 'XOR is defined to be true if an odd number of its arguments are true, and false otherwise. If any of the arguments are unknown, then the XOR operator produces a result of unknown.',
+    'ONE': 'The ONE operator produces a true result if one and only one argument is true. If there are more than argument is true (or if there are no true arguments), the result of the ONE is false. If one or more of the arguments are unknown, then the ONE operator produces a result of unknown.',
+    'NOT': 'NOT is negation, then the true result is false and the false result is true, all other results remain the same.'
+};
+const CPE_AL_OPERATOR_EXPLANATION = {
+    'AND': 'The AND operator produces a true result if every argument is true. If one or more arguments are false, the result of the AND is false.',
+    'OR': 'The OR operator produces a true result if one or more arguments is true. If every argument is false, the result of the OR is false.'
+};
 
 const DIV = document.createElement("div");
 const SPAN = document.createElement("span");
 
 const BUTTON = document.createElement("button");
 const ICON = document.createElement("i");
 const CODE = document.createElement("code");
@@ -224,15 +235,15 @@
         negate_icon
     } = get_colors_and_icons(node_data);
     const node = get_node(negate_color);
     node_text.appendChild(node);
     const html_icon = get_icon_as_html(negate_icon);
     node.appendChild(html_icon);
     if (node_data.negation) {
-        node.appendChild(get_bold_text("NOT"));
+        node.appendChild(get_operator_label_with_tooltip("NOT", OVAL_OPERATOR_EXPLANATION));
         html_icon.classList.add("icon-space");
     }
     return {
         node,
         color,
         icon
     };
@@ -244,15 +255,16 @@
         node_text
     } = get_operator_node();
     const {
         node,
         color,
         icon
     } = base_operator_node(node_data, node_text);
-    node.appendChild(get_bold_text(` ${node_data.node_type} `));
+
+    node.appendChild(get_operator_label_with_tooltip(node_data.node_type, CPE_AL_OPERATOR_EXPLANATION));
     node_text.appendChild(get_label(color, "CPE AL operator", undefined, "cpe-label", " cpe-label__content"));
     const span_space = SPAN.cloneNode();
     span_space.innerText = "\u00A0";
     node_text.appendChild(span_space);
     node_text.appendChild(get_label(color, node_data.value, get_icon_as_html(icon), "cpe-label", "cpe-label__content"));
     return operator_node;
 }
@@ -361,15 +373,15 @@
     } = get_colors_and_icons(node_data);
 
     const node = get_node(negate_color);
     node_text.appendChild(node);
     const html_icon = get_icon_as_html(negate_icon);
     node.appendChild(html_icon);
     if (node_data.negation) {
-        node.appendChild(get_bold_text("NOT"));
+        node.appendChild(get_operator_label_with_tooltip("NOT", OVAL_OPERATOR_EXPLANATION));
         html_icon.classList.add("icon-space");
     }
 
     const test_id = node_data.node_id.replace("oval:ssg-", "").replace(":tst:1", "");
     node.appendChild(get_bold_text(` ${test_id} `));
     node_text.appendChild(get_label(color, node_data.tag));
     node_text.appendChild(get_label(color, node_data.value, get_icon_as_html(icon)));
@@ -427,24 +439,24 @@
 
     const icon = ICON.cloneNode();
     icon.className = "fas fa-info-circle";
     icon.setAttribute("aria-hidden", "true");
     div.appendChild(icon);
 
     const tooltip_div = DIV.cloneNode();
-    tooltip_div.className = "pf-c-tooltip pf-m-right-top tooltip-box";
+    tooltip_div.className = "pf-c-tooltip pf-m-right-top tooltip-box-right-side";
     tooltip_div.setAttribute("role", "tooltip");
     div.appendChild(tooltip_div);
 
     const tooltip_arrow_div = DIV.cloneNode();
     tooltip_arrow_div.className = "pf-c-tooltip__arrow";
     tooltip_div.appendChild(tooltip_arrow_div);
 
     const tooltip_content_div = DIV.cloneNode();
-    tooltip_content_div.className = "pf-c-tooltip__content tooltip__content-width";
+    tooltip_content_div.className = "pf-c-tooltip__content tooltip__text-algin-justify";
     tooltip_content_div.textContent = text;
     tooltip_div.appendChild(tooltip_content_div);
 
     return div;
 }
 
 // eslint-disable-next-line max-params
@@ -521,26 +533,57 @@
 
     return {
         operator_node,
         node_text
     };
 }
 
+function add_tooltip_on_mouse_enter_to_oval_operator(self, text) { // eslint-disable-line no-unused-vars
+    const tooltip_div = DIV.cloneNode();
+    tooltip_div.className = "pf-c-tooltip pf-m-top-left tooltip-box-top-side tooltip-box-top-side-oval-operator";
+    tooltip_div.setAttribute("role", "tooltip");
+    self.appendChild(tooltip_div);
+
+    const tooltip_arrow_div = DIV.cloneNode();
+    tooltip_arrow_div.className = "pf-c-tooltip__arrow";
+    tooltip_div.appendChild(tooltip_arrow_div);
+
+    const tooltip_content_div = DIV.cloneNode();
+    tooltip_content_div.className = "pf-c-tooltip__content tooltip__text-algin-justify tooltip__content-width-oval-operator";
+    tooltip_content_div.textContent = text;
+    tooltip_div.appendChild(tooltip_content_div);
+}
+
+
+function remove_tooltip_on_mouse_leave_from_oval_operator(self) { // eslint-disable-line no-unused-vars
+    self.removeChild(self.lastChild);
+}
+
+function get_operator_label_with_tooltip(node_type, explanations) {
+    const span = SPAN.cloneNode();
+    span.className = "tooltip-wrapper tooltip-wrapper-oval-operator";
+    span.appendChild(get_bold_text(` ${node_type} `));
+
+    span.setAttribute("onmouseenter", `add_tooltip_on_mouse_enter_to_oval_operator(this, "${explanations[node_type]}")`);
+    span.setAttribute("onmouseleave", "remove_tooltip_on_mouse_leave_from_oval_operator(this)");
+    return span;
+}
+
 function get_OVAL_tree_operator_node(node_data) {
     const {
         operator_node,
         node_text
     } = get_operator_node();
     const {
         node,
         color,
         icon
     } = base_operator_node(node_data, node_text);
 
-    node.appendChild(get_bold_text(` ${node_data.node_type} `));
+    node.appendChild(get_operator_label_with_tooltip(node_data.node_type, OVAL_OPERATOR_EXPLANATION));
     node_text.appendChild(get_label(color, node_data.tag));
     node_text.appendChild(get_label(color, node_data.value, get_icon_as_html(icon)));
     node_text.appendChild(get_note(`\u00A0\u00A0${node_data.comment ? node_data.comment : ""}`));
 
     return operator_node;
 }
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/oval_definition_detail.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/oval_definition_detail.html`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     <th class="pf-m-fit-content" role="rowheader" scope="row"><b>Description:</b></th>
     <td role="cell">
         <div class="pf-l-flex pf-m-column"><div class="pf-l-flex__item">
         <p class="pf-c-table__text">{{ rule.oval_definition.description }}</p></div></div>
     </td>
 </tr>
 <tr role="row">
-    <th class="pf-m-fit-content" role="rowheader" scope="row"><b>Result explained:</b></th>
+    <th class="pf-m-fit-content" role="rowheader" scope="row"><b>Class explained:</b></th>
     <td role="cell">
         <div class="pf-l-flex pf-m-column"><div class="pf-l-flex__item">
         <p class="pf-c-table__text">{{ rule.oval_definition.get_oval_class_description() }}</p></div></div>
     </td>
 </tr>
 {% else %}
 <tr role="row">
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/oval_graph.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/oval_graph.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/remedations.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/remedations.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/rule_detail.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/rule_detail.html`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                     <div class="pf-l-flex pf-m-column"><div class="pf-l-flex__item">
                     <p class="pf-c-table__text">
                     <div>
                         {%- for identifier in rule.identifiers -%}
                         {%- if identifier.href -%}
                             <a href="{{ identifier.href | replace('&', ';') }}">{{ identifier.text }}</a>
                         {%- else -%}
-                            <a href="identifier_href_not_found">{{ identifier.text }}</a>
+                            <span>{{ identifier.text }}</span>
                         {%- endif -%}
                         {{- ", " if not loop.last else "" -}}
                         {%- endfor %}
                     </div>
                     </p>
                     </div></div>
                 </td>
@@ -143,15 +143,15 @@
                     <div class="pf-l-flex pf-m-column"><div class="pf-l-flex__item">
                     <p class="pf-c-table__text">
                     <div>
                         {%- for reference in rule.references -%}
                         {%- if reference.href -%}
                             <a href="{{ reference.href | replace('&', ';') }}">{{ reference.text }}</a>
                         {%- else -%}
-                            <a href="reference_href_not_found">{{ reference.text }}</a>
+                            <span>{{ reference.text }}</span>
                         {%- endif -%}
                         {{- ", " if not loop.last else "" -}}
                         {%- endfor -%}
                     </div>
                     </p>
                     </div></div>
                 </td>
```

#### html2text {}

```diff
@@ -16,19 +16,19 @@
                   { rule.severity }}  {% elif rule.result != "pass" and
 Severity:         rule.severity == "medium" %}  {{ rule.severity }}  {% elif
                   rule.result != "pass" and rule.severity == "high" %}  {
                   { rule.severity }}  {% else %}  {{ rule.severity }}  {% endif
                   %}
                   {%- for identifier in rule.identifiers -%} {%- if
 Identifiers:      identifier.href -%} {{_identifier.text_}} {%- else -%} {
-                  {_identifier.text_}} {%- endif -%} {{- ", " if not loop.last
+                  { identifier.text }} {%- endif -%} {{- ", " if not loop.last
                   else "" -}} {%- endfor %}
                   {%- for reference in rule.references -%} {%- if
 References:       reference.href -%} {{_reference.text_}} {%- else -%} {
-                  {_reference.text_}} {%- endif -%} {{- ", " if not loop.last
+                  { reference.text }} {%- endif -%} {{- ", " if not loop.last
                   else "" -}} {%- endfor -%}
 Description:      {{- rule.description | set_css_for_list -}}
 Rationale:        {{- rule.rationale | set_css_for_list -}}
                   {% for warning in rule.warnings %}
                   {{- warning.category | capitalize -}} warning
 Warnings:         {{- warning.text | set_css_for_list -}}
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/rule_results.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/rule_results.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/rules_overview.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/rules_overview.html`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                         </span>
                     {{- rule.result -}}
                     </span>
                 </span>
                 {% endif %}
             </td>
         </tr>
-        <tr class="pf-c-table__expandable-row" role="row">
+        <tr class="pf-c-table__expandable-row disable-scrollbar-for-low-resolution" role="row">
             <td role="cell" colspan="4">
                 <div class="pf-c-table__expandable-row-content">
                     {% include 'rule_detail.html' %}
                 </div>
             </td>
         </tr>
     </tbody>
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/score_bar.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/score_bar.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/search_input.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/search_input.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,90 @@
 {# Copyright 2022, Red Hat, Inc. #}
 {# SPDX-License-Identifier: LGPL-2.1-or-later #}
 <div class="pf-c-accordion pf-m-display-lg">
     <div class="pf-c-input-group">
         <input class="pf-c-form-control pf-m-search" oninput="search_rule(this)" type="search"
             placeholder="Search rule" id="input-search-rule" />
+        <button class="pf-c-button pf-m-control" type="button" aria-label="Clear" onclick="clear_input(this)">
+            <i class="fas fa-times fa-fw" aria-hidden="true"></i>
+        </button>
         <button class="pf-c-button pf-m-control" type="button" aria-expanded="true" aria-label="Advanced options"
             onclick="show_advanced_options(this);">
             <i class="fas fa-caret-right" aria-hidden="true"></i>
         </button>
     </div>
     <div class="pf-c-accordion__expanded-content" style="display: none;">
         <div class="pf-c-accordion__expanded-content-body">
             <br>
             <h3 class="pf-c-title pf-m-md">Advanced filtering options</h3>
             Filter by result:
             <div class="container">
+                <div>
+                    <button id="show-all-rules-details" class="pf-c-button pf-m-primary" type="button" onclick="toogle_deselect_button(this)">Deselect all</button>
+                </div>
                 <label class="pf-c-check" for="checkbox-result-pass">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-pass" onchange="toggle_rules('result', 'pass');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-pass" autocomplete="off" onchange="toggle_rules('result', 'pass');" checked/>
                     <span class="pf-c-check__label">Pass</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-result-fail">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-fail" onchange="toggle_rules('result', 'fail');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-fail" autocomplete="off" onchange="toggle_rules('result', 'fail');" checked/>
                     <span class="pf-c-check__label">Fail</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-result-not-checked">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-not-checked" onchange="toggle_rules('result', 'notchecked');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-not-checked" autocomplete="off" onchange="toggle_rules('result', 'notchecked');" checked/>
                     <span class="pf-c-check__label">Not checked</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-result-not-applicable">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-not-applicable" onchange="toggle_rules('result', 'notapplicable');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-not-applicable" autocomplete="off" onchange="toggle_rules('result', 'notapplicable');" checked/>
                     <span class="pf-c-check__label">Not applicable</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-result-fixed">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-fixed" onchange="toggle_rules('result', 'fixed');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-fixed" autocomplete="off" onchange="toggle_rules('result', 'fixed');" checked/>
                     <span class="pf-c-check__label">Fixed</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-result-error">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-error" onchange="toggle_rules('result', 'error');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-error" autocomplete="off" onchange="toggle_rules('result', 'error');" checked/>
                     <span class="pf-c-check__label">Error</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-fix-failed">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-fix-failed" onchange="toggle_rules('result', 'fix-failed');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-fix-failed" autocomplete="off" onchange="toggle_rules('result', 'fix-failed');" checked/>
                     <span class="pf-c-check__label">Fix failed</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-fix-unsuccessful">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-fix-unsuccessful" onchange="toggle_rules('result', 'fix-unsuccessful');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-fix-unsuccessful" autocomplete="off" onchange="toggle_rules('result', 'fix-unsuccessful');" checked/>
                     <span class="pf-c-check__label">Fix unsuccessful</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-result-informational">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-informational" onchange="toggle_rules('result', 'informational');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-informational" autocomplete="off" onchange="toggle_rules('result', 'informational');" checked/>
                     <span class="pf-c-check__label">Informational</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-result-unknown">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-unknown" onchange="toggle_rules('result', 'unknown');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-result-unknown" autocomplete="off" onchange="toggle_rules('result', 'unknown');" checked/>
                     <span class="pf-c-check__label">Unknown</span>
                 </label>
             </div>
             Filter by severity:
             <div class="container">
+                <div>
+                    <button id="show-all-rules-details" class="pf-c-button pf-m-primary" type="button" onclick="toogle_deselect_button(this)">Deselect all</button>
+                </div>
                 <label class="pf-c-check" for="checkbox-severity-high">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-severity-high" onchange="toggle_rules('severity', 'high');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-severity-high" autocomplete="off" onchange="toggle_rules('severity', 'high');" checked/>
                     <span class="pf-c-check__label">high</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-severity-medium">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-severity-medium" onchange="toggle_rules('severity', 'medium');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-severity-medium" autocomplete="off" onchange="toggle_rules('severity', 'medium');" checked/>
                     <span class="pf-c-check__label">Medium</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-severity-low">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-severity-low" onchange="toggle_rules('severity', 'low');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-severity-low" autocomplete="off" onchange="toggle_rules('severity', 'low');" checked/>
                     <span class="pf-c-check__label">Low</span>
                 </label>
                 <label class="pf-c-check" for="checkbox-severity-unknown">
-                    <input class="pf-c-check__input" type="checkbox" id="checkbox-severity-unknown" onchange="toggle_rules('severity', 'unknown');" checked/>
+                    <input class="pf-c-check__input" type="checkbox" id="checkbox-severity-unknown" autocomplete="off" onchange="toggle_rules('severity', 'unknown');" checked/>
                     <span class="pf-c-check__label">Unknown</span>
                 </label>
             </div>
             {%- if debug_setting.button_show_all_rules -%}
                 <br>
                 <div>
                     <button id="show-all-rules-details" class="pf-c-button pf-m-primary" type="button" onclick="show_all_rules_details(this)">Show all result details</button>
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/severity_of_failed_rules.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/severity_of_failed_rules.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/summary_banner.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/summary_banner.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/html_templates/template_report.html` & `openscap-report-0.2.4/openscap_report/report_generators/html_templates/template_report.html`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 
 {% block style %}
 <style>
     {%- include './css/style.css' -%}
 </style>
 {% endblock %}
 
-{% block title%}OpenSCAP Evaluation Report{% endblock %}
+{% block title%}SCAP Evaluation Report{% endblock %}
 
 {% block content %}
 
 {% if report.profile_info.title|length and report.profile_info.description|length -%}
-<h2 class="pf-c-title pf-m-3xl">About profile</h2>
+<h2 id="top" class="pf-c-title pf-m-3xl">About profile</h2>
 <br>
 {% include 'profile_info.html' %}
 <br>
 {%- endif -%}
 
 <h2 class="pf-c-title pf-m-3xl">Compliance and Scoring</h2>
 <br>
```

#### html2text {}

```diff
@@ -2,16 +2,16 @@
 later #} {% extends 'base_report.html' %} {% block interactive_script %}
  {% endblock %} {% block oval_graph_generation_script %}
  {% endblock %} {% block debug_script %}
  {% endblock %} {% block patternfly_css %} {% if debug_setting.use_online_css
 %}
  {% else %}
  {% endif %} {% endblock %} {% block style %}
- {% endblock %} {% block title%}OpenSCAP Evaluation Report{% endblock %} {%
-block content %} {% if report.profile_info.title|length and
+ {% endblock %} {% block title%}SCAP Evaluation Report{% endblock %} {% block
+content %} {% if report.profile_info.title|length and
 report.profile_info.description|length -%}
 ***** About profile *****
 
 {% include 'profile_info.html' %}
 {%- endif -%}
 ***** Compliance and Scoring *****
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/json.py` & `openscap-report-0.2.4/openscap_report/report_generators/json.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/old_style_html.py` & `openscap-report-0.2.4/openscap_report/report_generators/old_style_html.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-branding.xsl` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-branding.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-references.xsl` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-references.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report-impl.xsl` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-report-impl.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-report.xsl` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-report.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/openscap.css` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/openscap.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources/openscap.js` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources/openscap.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text*

 * *Files 0% similar despite different names*

```diff
@@ -574,8 +574,8 @@
 000023d0: 6f77 7329 2e65 6163 6828 6675 6e63 7469  ows).each(functi
 000023e0: 6f6e 2028 2920 7b0a 2020 2020 2020 2020  on () {.        
 000023f0: 2428 7468 6973 292e 6373 7328 2262 6163  $(this).css("bac
 00002400: 6b67 726f 756e 642d 636f 6c6f 7222 2c20  kground-color", 
 00002410: 6576 656e 203f 2022 2346 3946 3946 3922  even ? "#F9F9F9"
 00002420: 203a 2022 696e 6865 7269 7422 293b 0a20   : "inherit");. 
 00002430: 2020 2020 2020 2065 7665 6e20 3d20 2165         even = !e
-00002440: 7665 6e3b 0a20 2020 207d 293b 0a7d       ven;.    });.}
+00002440: 7665 6e3b 0a20 2020 207d 293b 0a7d 0a    ven;.    });.}.
```

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources-build.sh` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources-build.sh`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-resources.xsl` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-resources.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/report_generators/xsl/xccdf-share.xsl` & `openscap-report-0.2.4/openscap_report/report_generators/xsl/xccdf-share.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/__init__.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/group.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/group.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/json_transformation.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/json_transformation.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_definition.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_definition.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_node.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_node.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/oval_result_eval.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/oval_result_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/profile_info.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/profile_info.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/remediation.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/remediation.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/report.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/report.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/result_of_scan.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/result_of_scan.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/data_structures/rule.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/data_structures/rule.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/exceptions.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/namespaces.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/namespaces.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/__init__.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/cpe_al_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/cpe_al_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/full_text_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/full_text_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/group_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/group_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_definition_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_definition_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_object_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_object_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_result_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_result_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_state_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_state_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/oval_test_info_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/oval_test_info_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/profile_info_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/profile_info_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/remediation_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/remediation_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/report_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/report_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/rule_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/rule_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/scan_result_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/scan_result_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/scap_results_parser.py` & `openscap-report-0.2.4/openscap_report/scap_results_parser/scap_results_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/catalog.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/common/catalog.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xlink.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/common/xlink.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xml.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/common/xml.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd` & `openscap-report-0.2.4/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/openscap_report.egg-info/PKG-INFO` & `openscap-report-0.2.4/openscap_report.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openscap-report
-Version: 0.2.3
+Version: 0.2.4
 Summary: Tool for generating report from results of oscap scan.
 Home-page: https://github.com/OpenSCAP/oscap-report
 Author: Jan Rodak
 Author-email: jrodak@redhat.com
 License: LGPL-2.1 License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openscap-report-0.2.3/openscap_report.egg-info/SOURCES.txt` & `openscap-report-0.2.4/openscap_report.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/requirements.txt
 docs/exts/sphinxarg/__init__.py
 docs/exts/sphinxarg/ext.py
 docs/exts/sphinxarg/markdown.py
 docs/exts/sphinxarg/parser.py
 docs/manual/installation.rst
 docs/manual/report.rst
+docs/manual/test-suite.rst
 docs/manual/usage.rst
 docs/manual/assets/about_profile.png
 docs/manual/assets/compliance_and_scoring.png
 docs/manual/assets/cpe_aplicability_language.png
 docs/manual/assets/evaluation_characteristics.png
 docs/manual/assets/example_report.html
 docs/manual/assets/oval.gif
```

### Comparing `openscap-report-0.2.3/setup.py` & `openscap-report-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def get_long_description():
     with open("README.md", "r", encoding="utf-8") as readme_file:
         return readme_file.read()
 
 
 setup(name='openscap-report',
-      version='0.2.3',
+      version='0.2.4',
       description='Tool for generating report from results of oscap scan.',
       long_description=get_long_description(),
       long_description_content_type="text/markdown",
       url='https://github.com/OpenSCAP/oscap-report',
       author='Jan Rodak',
       author_email='jrodak@redhat.com',
       license='LGPL-2.1 License',
```

### Comparing `openscap-report-0.2.3/tests/constants.py` & `openscap-report-0.2.4/tests/constants.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/integration.fmf` & `openscap-report-0.2.4/tests/integration.fmf`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/integration_tests/test_basic_usage.py` & `openscap-report-0.2.4/tests/integration_tests/test_basic_usage.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/integration_tests/test_cli.py` & `openscap-report-0.2.4/tests/integration_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/integration_tests/test_json.py` & `openscap-report-0.2.4/tests/integration_tests/test_json.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/json_schema_of_report.json` & `openscap-report-0.2.4/tests/json_schema_of_report.json`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/smoke.sh` & `openscap-report-0.2.4/tests/smoke.sh`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf-container.xml` & `openscap-report-0.2.4/tests/test_data/arf-container.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf-dangling-reference-to.xml` & `openscap-report-0.2.4/tests/test_data/arf-dangling-reference-to.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf-report.xml` & `openscap-report-0.2.4/tests/test_data/arf-report.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf-with-removed-info.xml` & `openscap-report-0.2.4/tests/test_data/arf-with-removed-info.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf_cpe_check_os_platform.xml` & `openscap-report-0.2.4/tests/test_data/arf_cpe_check_os_platform.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf_multi_check.xml` & `openscap-report-0.2.4/tests/test_data/arf_multi_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf_no_system_data.xml` & `openscap-report-0.2.4/tests/test_data/arf_no_system_data.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf_rule_and_cpe_check.xml` & `openscap-report-0.2.4/tests/test_data/arf_rule_and_cpe_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf_simple_rule_fail.xml` & `openscap-report-0.2.4/tests/test_data/arf_simple_rule_fail.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/arf_simple_rule_pass.xml` & `openscap-report-0.2.4/tests/test_data/arf_simple_rule_pass.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/plant_catalog.xml` & `openscap-report-0.2.4/tests/test_data/plant_catalog.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt` & `openscap-report-0.2.4/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt` & `openscap-report-0.2.4/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt` & `openscap-report-0.2.4/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt` & `openscap-report-0.2.4/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/xccdf-report.xml` & `openscap-report-0.2.4/tests/test_data/xccdf-report.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/xccdf-with-removed-info.xml` & `openscap-report-0.2.4/tests/test_data/xccdf-with-removed-info.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/xccdf_multi_check.xml` & `openscap-report-0.2.4/tests/test_data/xccdf_multi_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/xccdf_no_system_data.xml` & `openscap-report-0.2.4/tests/test_data/xccdf_no_system_data.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/xccdf_rule_and_cpe_check.xml` & `openscap-report-0.2.4/tests/test_data/xccdf_rule_and_cpe_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/xccdf_simple_rule_fail.xml` & `openscap-report-0.2.4/tests/test_data/xccdf_simple_rule_fail.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_data/xccdf_simple_rule_pass.xml` & `openscap-report-0.2.4/tests/test_data/xccdf_simple_rule_pass.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/test_utils.py` & `openscap-report-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_cli.py` & `openscap-report-0.2.4/tests/unit_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_cpe_al_parser.py` & `openscap-report-0.2.4/tests/unit_tests/test_cpe_al_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_data_structure.py` & `openscap-report-0.2.4/tests/unit_tests/test_data_structure.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_debug_settings.py` & `openscap-report-0.2.4/tests/unit_tests/test_debug_settings.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_full_text_parser.py` & `openscap-report-0.2.4/tests/unit_tests/test_full_text_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_json_transitions.py` & `openscap-report-0.2.4/tests/unit_tests/test_json_transitions.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_oval_result_eval.py` & `openscap-report-0.2.4/tests/unit_tests/test_oval_result_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_oval_tree_eval.py` & `openscap-report-0.2.4/tests/unit_tests/test_oval_tree_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_scap_result_parser.py` & `openscap-report-0.2.4/tests/unit_tests/test_scap_result_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tests/unit_tests/test_shared_static_methods_of_parser.py` & `openscap-report-0.2.4/tests/unit_tests/test_shared_static_methods_of_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.3/tox.ini` & `openscap-report-0.2.4/tox.ini`

 * *Files identical despite different names*

