# Comparing `tmp/ansys_templates-0.9.0.tar.gz` & `tmp/ansys_templates-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_templates-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_templates-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_templates-0.9.0.tar` & `ansys_templates-1.0.0.tar`

### file list

```diff
@@ -1,276 +1,278 @@
--rw-r--r--   0        0        0     1091 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     9947 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/README.rst
--rw-r--r--   0        0        0     3122 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2266 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/__init__.py
--rw-r--r--   0        0        0     1284 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/__main__.py
--rw-r--r--   0        0        0     3776 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/cli.py
--rw-r--r--   0        0        0     1106 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/licenses/LICENSE_MIT
--rw-r--r--   0        0        0      199 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/licenses/__init__.py
--rw-r--r--   0        0        0     3894 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/paths.py
--rw-r--r--   0        0        0      398 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/python/common/cookiecutter.json
--rw-r--r--   0        0        0       86 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
--rw-r--r--   0        0        0      356 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
--rw-r--r--   0        0        0      265 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0       59 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
--rw-r--r--   0        0        0      418 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0      119 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
--rw-r--r--   0        0        0      594 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
--rw-r--r--   0        0        0     3713 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2779 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
--rw-r--r--   0        0        0     2987 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      764 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0     2689 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0      282 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1052 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
--rw-r--r--   0        0        0      657 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rwxr-xr-x   0        0        0     1026 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      969 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       63 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rwxr-xr-x   0        0        0     4076 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0      928 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
--rw-r--r--   0        0        0       11 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3414 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      196 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
--rw-r--r--   0        0        0       27 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0       81 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
--rw-r--r--   0        0        0       32 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0     1104 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      140 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     2377 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1087 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/cookiecutter.json
--rw-r--r--   0        0        0     2046 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3238 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     1187 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1134 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
--rw-r--r--   0        0        0      825 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1732 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/cookiecutter.json
--rw-r--r--   0        0        0     6017 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      161 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     2365 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2147 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     3177 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      655 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0   220746 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock
--rw-r--r--   0        0        0      199 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.toml
--rw-r--r--   0        0        0     4222 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    39004 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      421 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       50 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
--rw-r--r--   0        0        0       47 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0     6614 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/extract_system_hierarchy.py
--rw-r--r--   0        0        0     1360 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
--rw-r--r--   0        0        0      725 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      248 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
--rw-r--r--   0        0        0    12171 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
--rw-r--r--   0        0        0      922 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0      755 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
--rw-r--r--   0        0        0       41 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
--rw-r--r--   0        0        0     9913 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0       37 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
--rw-r--r--   0        0        0     2579 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py
--rw-r--r--   0        0        0     3687 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py
--rw-r--r--   0        0        0     3177 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py
--rw-r--r--   0        0        0     5284 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py
--rw-r--r--   0        0        0     1837 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py
--rw-r--r--   0        0        0     2482 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py
--rw-r--r--   0        0        0     5649 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py
--rw-r--r--   0        0        0     1753 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py
--rw-r--r--   0        0        0     4962 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py
--rw-r--r--   0        0        0     4954 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
--rw-r--r--   0        0        0     9719 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py
--rw-r--r--   0        0        0     3165 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py
--rw-r--r--   0        0        0     3676 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py
--rw-r--r--   0        0        0      960 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py
--rw-r--r--   0        0        0     3626 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py
--rw-r--r--   0        0        0      543 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py
--rw-r--r--   0        0        0      983 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py
--rw-r--r--   0        0        0     1372 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py
--rw-r--r--   0        0        0      296 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/result_files_page.py
--rw-r--r--   0        0        0      714 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py
--rw-r--r--   0        0        0      660 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py
--rw-r--r--   0        0        0      793 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py
--rw-r--r--   0        0        0      574 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py
--rw-r--r--   0        0        0       20 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1560 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
--rw-r--r--   0        0        0     2903 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
--rw-r--r--   0        0        0      800 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1132 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       49 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      111 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       21 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0     1461 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      997 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      186 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      687 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1558 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
--rw-r--r--   0        0        0     3070 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
--rw-r--r--   0        0        0      763 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1133 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       58 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      104 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       25 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
--rw-r--r--   0        0        0      621 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
--rw-r--r--   0        0        0      525 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
--rw-r--r--   0        0        0       21 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0       28 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1475 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0     1877 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      955 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     1062 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1557 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
--rw-r--r--   0        0        0     3055 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
--rw-r--r--   0        0        0      951 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1145 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      630 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
--rw-r--r--   0        0        0       44 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      116 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      265 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0      850 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1409 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      851 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0       23 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
--rw-r--r--   0        0        0      902 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
--rw-r--r--   0        0        0      408 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      641 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      961 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1556 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
--rw-r--r--   0        0        0     2831 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
--rw-r--r--   0        0        0      860 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1129 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0      445 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
--rw-r--r--   0        0        0      622 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
--rw-r--r--   0        0        0      184 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0     1458 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys/cookiecutter.json
--rw-r--r--   0        0        0     1110 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3398 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1540 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
--rw-r--r--   0        0        0     2619 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
--rw-r--r--   0        0        0     6537 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1879 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
--rw-r--r--   0        0        0     1010 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
--rw-r--r--   0        0        0      241 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0     1599 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
--rw-r--r--   0        0        0     1857 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
--rw-r--r--   0        0        0     1726 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
--rw-r--r--   0        0        0     4317 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
--rw-r--r--   0        0        0      975 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/cookiecutter.json
--rw-r--r--   0        0        0     1035 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3170 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      896 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      253 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1027 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/cookiecutter.json
--rw-r--r--   0        0        0     3166 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      161 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     2365 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1710 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     2701 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1545 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
--rw-r--r--   0        0        0      655 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0   198506 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock
--rw-r--r--   0        0        0     3782 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    35407 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      583 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       52 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
--rw-r--r--   0        0        0       51 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
--rw-r--r--   0        0        0       52 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      803 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      570 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
--rw-r--r--   0        0        0      274 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
--rw-r--r--   0        0        0      263 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
--rw-r--r--   0        0        0      922 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0      755 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
--rw-r--r--   0        0        0       18 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
--rw-r--r--   0        0        0   749872 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
--rw-r--r--   0        0        0     9913 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0       37 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
--rw-r--r--   0        0        0       18 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
--rw-r--r--   0        0        0     2030 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
--rw-r--r--   0        0        0     4700 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py
--rw-r--r--   0        0        0     5244 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
--rw-r--r--   0        0        0      593 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
--rw-r--r--   0        0        0       20 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     4035 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/testing.py
--rw-r--r--   0        0        0     6698 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/utils.py
--rw-r--r--   0        0        0    11425 1970-01-01 00:00:00.000000 ansys_templates-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-07-05 18:03:30.981319 ansys_templates-1.0.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     9947 2023-07-05 18:03:30.981319 ansys_templates-1.0.0/README.rst
+-rw-r--r--   0        0        0     3122 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2266 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/__init__.py
+-rw-r--r--   0        0        0     1284 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/__main__.py
+-rw-r--r--   0        0        0     3803 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/cli.py
+-rw-r--r--   0        0        0     1106 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/licenses/LICENSE_MIT
+-rw-r--r--   0        0        0      199 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/licenses/__init__.py
+-rw-r--r--   0        0        0     3894 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/paths.py
+-rw-r--r--   0        0        0      398 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/cookiecutter.json
+-rw-r--r--   0        0        0       86 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
+-rw-r--r--   0        0        0      356 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
+-rw-r--r--   0        0        0      265 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0       59 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
+-rw-r--r--   0        0        0      418 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      119 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     3713 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     2779 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2987 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      764 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      379 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/AUTHORS
+-rw-r--r--   0        0        0       11 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2689 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0      105 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      282 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1052 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
+-rw-r--r--   0        0        0      657 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rwxr-xr-x   0        0        0     1026 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      969 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       63 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rwxr-xr-x   0        0        0     4076 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0      928 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
+-rw-r--r--   0        0        0       11 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3414 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
+-rw-r--r--   0        0        0       27 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0       81 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
+-rw-r--r--   0        0        0       32 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0     1104 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      140 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     2377 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1087 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/doc_project/cookiecutter.json
+-rw-r--r--   0        0        0     2046 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3238 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     1187 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1134 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
+-rw-r--r--   0        0        0      825 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1434 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/cookiecutter.json
+-rw-r--r--   0        0        0     7450 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      161 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2147 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2819 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-07-05 18:03:30.985319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0   223733 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock
+-rw-r--r--   0        0        0      199 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.toml
+-rw-r--r--   0        0        0     3849 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38166 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       50 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0     3918 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py
+-rw-r--r--   0        0        0       47 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      959 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
+-rw-r--r--   0        0        0      725 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      248 2023-07-05 18:03:30.989319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
+-rw-r--r--   0        0        0    13429 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
+-rw-r--r--   0        0        0      922 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       41 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0     9913 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0     2579 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py
+-rw-r--r--   0        0        0     3687 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py
+-rw-r--r--   0        0        0     3177 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py
+-rw-r--r--   0        0        0     5284 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py
+-rw-r--r--   0        0        0     1837 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py
+-rw-r--r--   0        0        0     2482 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py
+-rw-r--r--   0        0        0     5649 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py
+-rw-r--r--   0        0        0     1753 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py
+-rw-r--r--   0        0        0     4962 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py
+-rw-r--r--   0        0        0     7522 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0     9107 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py
+-rw-r--r--   0        0        0     3165 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py
+-rw-r--r--   0        0        0     3676 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py
+-rw-r--r--   0        0        0      960 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py
+-rw-r--r--   0        0        0     3626 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py
+-rw-r--r--   0        0        0      618 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py
+-rw-r--r--   0        0        0      983 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py
+-rw-r--r--   0        0        0     1372 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py
+-rw-r--r--   0        0        0      296 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/result_files_page.py
+-rw-r--r--   0        0        0      714 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py
+-rw-r--r--   0        0        0      660 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py
+-rw-r--r--   0        0        0      793 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py
+-rw-r--r--   0        0        0      574 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py
+-rw-r--r--   0        0        0       20 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1560 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
+-rw-r--r--   0        0        0     2941 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      800 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1132 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       49 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      111 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       21 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0     1461 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      997 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      186 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      687 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1558 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
+-rw-r--r--   0        0        0     3108 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      763 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1133 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       58 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      104 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       25 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
+-rw-r--r--   0        0        0      621 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
+-rw-r--r--   0        0        0      525 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
+-rw-r--r--   0        0        0       21 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0     1877 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      955 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     1062 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1557 2023-07-05 18:03:30.993319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
+-rw-r--r--   0        0        0     3093 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      951 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1145 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      630 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
+-rw-r--r--   0        0        0       44 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      116 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      265 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0      850 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1409 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      851 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0       23 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
+-rw-r--r--   0        0        0      408 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      641 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      961 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1556 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
+-rw-r--r--   0        0        0     2869 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      860 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1129 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0      445 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
+-rw-r--r--   0        0        0      622 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
+-rw-r--r--   0        0        0      184 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0     1458 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys/cookiecutter.json
+-rw-r--r--   0        0        0     1148 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3398 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1540 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
+-rw-r--r--   0        0        0     2657 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     6537 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1879 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
+-rw-r--r--   0        0        0     1048 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      241 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0     1599 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
+-rw-r--r--   0        0        0     1857 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
+-rw-r--r--   0        0        0     1726 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
+-rw-r--r--   0        0        0     4317 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
+-rw-r--r--   0        0        0      975 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pybasic/cookiecutter.json
+-rw-r--r--   0        0        0     1073 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3170 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      896 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      253 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1063 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/cookiecutter.json
+-rw-r--r--   0        0        0     3318 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      161 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1710 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2701 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1567 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
+-rw-r--r--   0        0        0      655 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-07-05 18:03:30.997319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0   202408 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock
+-rw-r--r--   0        0        0     3863 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38166 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       52 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       51 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0       52 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      803 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      570 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
+-rw-r--r--   0        0        0      274 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
+-rw-r--r--   0        0        0      263 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
+-rw-r--r--   0        0        0      922 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       18 2023-07-05 18:03:31.001320 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0   749872 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
+-rw-r--r--   0        0        0     9913 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0       18 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
+-rw-r--r--   0        0        0     3490 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
+-rw-r--r--   0        0        0     4700 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py
+-rw-r--r--   0        0        0     5244 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0      593 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
+-rw-r--r--   0        0        0       20 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     4035 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/testing.py
+-rw-r--r--   0        0        0     6698 2023-07-05 18:03:31.005319 ansys_templates-1.0.0/src/ansys/templates/utils.py
+-rw-r--r--   0        0        0    11425 1970-01-01 00:00:00.000000 ansys_templates-1.0.0/PKG-INFO
```

### Comparing `ansys_templates-0.9.0/LICENSES/MIT.txt` & `ansys_templates-1.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/README.rst` & `ansys_templates-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/pyproject.toml` & `ansys_templates-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-templates"
-version = "0.9.0"
+version = "1.0.0"
 description = "Creates Python projects according to PyAnsys guidelines"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSES/MIT.txt"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -47,23 +47,23 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "importlib-metadata >=4.0",
-    "click>=7.0,<8.0.0",
+    "click>=7.0,<9.0.0",
     "cookiecutter>=2.1.0",
     "isort>=5.10.1",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.3.2",
-    "pytest-cov==4.0.0",
+    "pytest==7.4.0",
+    "pytest-cov==4.1.0",
 ]
 doc = [
     "ansys-sphinx-theme==0.9.9",
     "numpydoc==1.5.0",
     "sphinx==7.0.1",
     "sphinx-copybutton==0.5.2",
 ]
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/__init__.py` & `ansys_templates-1.0.0/src/ansys/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/__main__.py` & `ansys_templates-1.0.0/src/ansys/templates/__main__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/cli.py` & `ansys_templates-1.0.0/src/ansys/templates/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 @new.command()
 def pyace_grpc():
     """Create gRPC project initialized for any developer."""
     create_project("pyace-grpc")
 
 @new.command()
-@click.option('-f',  '--from', '_from' , help='From existing workflow.',
-              type=click.Choice(['opf'], case_sensitive=False))
+@click.option('-f',  '--from', '_from' , help='From existing optiSLang application archive (OWA).',
+              type=click.Choice(['owa'], case_sensitive=False))
 def solution(_from):
     """[Ansys Internal Use Only] Create a solution based on SAF."""
-    if _from == 'opf':
+    if _from == 'owa':
         create_project("osl-solution")
     else:
         create_project("solution")
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/licenses/LICENSE_MIT` & `ansys_templates-1.0.0/src/ansys/templates/licenses/LICENSE_MIT`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/paths.py` & `ansys_templates-1.0.0/src/ansys/templates/paths.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.0.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/doc_project/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-1.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.0.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import shutil
 import os
 from pathlib import Path
 from ansys.templates.utils import keep_files
+import zipfile
 
 
 DESIRED_STRUCTURE = [
     ".github/workflows/ci.yml",
     ".vscode/launch.json",
     "doc/source/_static/ansys-solutions-logo-black-background.png",
     "doc/source/_static/README.md",
@@ -16,16 +17,16 @@
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/styles/.gitignore",
     "doc/.vale.ini",
     "doc/make.bat",
     "doc/Makefile",
     "examples/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/assets/README.md",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/scripts/extract_system_hierarchy.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/scripts/README.md",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/osl_project_tree.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/utils.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/definition.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/monitoring_step.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/problem_setup_step.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/css/style.css",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/images/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/logos/ansys-solutions-horizontal-logo.png",
@@ -62,51 +63,86 @@
     "tests/conftest.py",
     ".codespell.exclude",
     ".codespell.ignore",
     ".env",
     ".flake8",
     ".gitignore",
     ".pre-commit-config.yaml",
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CODEOWNERS",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     "LICENSE.rst",
     "poetry.lock",
     "pyproject.toml",
     "README.rst",
     "setup_environment.py",
     "tox.ini"
 ]
 """A list holding all desired files to be included in the project."""
 
 ASSETS_DIRCTORY = Path(f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/assets/").absolute()
 
 
-def copy_file_to_assets_folder(file_path: str, destination: str):
+def unzip_archive(archive_path: Path, extract_path: Path) -> None:
+    """Unzip an archive."""
+
+    with zipfile.ZipFile(archive_path, "r") as zip_ref:
+        zip_ref.extractall(extract_path)
+
+
+def copy_file_to_assets_folder(file_path: str, destination: str) -> None:
     """Copy a file if it exists."""
 
     if not os.path.isabs(file_path):
         working_directory = os.path.dirname(os.getcwd())
         file_path = os.path.join(working_directory, file_path)
 
     if os.path.exists(file_path):
         shutil.copy(file_path, destination)
     else:
         print(f"Unable to find {file_path}.")
 
 
+def collect_files_with_extension(directory, extension):
+    """
+    Collects all files with the specified extension from a directory.
+    Args:
+        directory (str): The directory path.
+        extension (str): The desired file extension.
+    Returns:
+        list: A list of file names with the specified extension.
+    """
+    files_with_extension = [file for file in os.listdir(directory) if file.endswith(extension)]
+    return files_with_extension
+
+
 def main():
     """Entry point of the script."""
 
     keep_files(DESIRED_STRUCTURE)
 
-    if len("{{ cookiecutter.__optiSLang_project_file }}".replace(" ", "")):
-        copy_file_to_assets_folder("{{ cookiecutter.__optiSLang_project_file }}",  str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_project_file_name }}"))
-    if len("{{ cookiecutter.__optiSLang_properties_file }}".replace(" ", "")):
-        copy_file_to_assets_folder("{{ cookiecutter.__optiSLang_properties_file }}", str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_properties_file_name }}"))
-    if len("{{ cookiecutter.__optiSLang_metadata_file }}".replace(" ", "")):
-        copy_file_to_assets_folder("{{ cookiecutter.__optiSLang_metadata_file }}", str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_metadata_file_name }}"))
-
+    if len("{{ cookiecutter.__optiSLang_application_archive }}".replace(" ", "")):
+        unzip_archive("{{ cookiecutter.__optiSLang_application_archive }}", ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_application_archive_stem }}")
+        for file in ["metadata.json", "doc.md"]:
+            copy_file_to_assets_folder(
+                str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_application_archive_stem }}" / file),
+                str(ASSETS_DIRCTORY / file)
+            )
+        for extension in [".json", ".opf"]:
+            candidates = collect_files_with_extension(str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_application_archive_stem }}" / "custom_data"), extension)
+            if len(candidates) == 0:
+                raise Exception("The optiSLang application archive contains no project file (opf).")
+            elif len(candidates) > 1:
+                raise Exception("The optiSLang application archive contains multiple project files (opf).")
+            else:
+                candidate = "{{ cookiecutter.__optiSLang_application_archive_stem }}" + extension
+                copy_file_to_assets_folder(
+                    str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_application_archive_stem }}" / "custom_data" / candidates[0]),
+                    str(ASSETS_DIRCTORY / candidate)
+                )
+        shutil.rmtree(str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_application_archive_stem }}"))
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -96,20 +96,14 @@
 
 6. Configure the portal database:
 
   .. code:: bash
 
     poetry run configure-portal-database
 
-7. Run this command to extract the project tree (system hierarchy) from the optiSLang project file:
-
-  .. code:: bash
-
-    python src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/scripts/extract_system_hierarchy.py -p src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/assets/{{ cookiecutter.__optiSLang_project_file_name }}
-
 From now on, all the commands must be executed within the virtual environment.
 
 
 Start the solution
 ==================
 
 To start the solution run the following command anywhere in the project:
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,30 @@
 python-versions = ">=3.6"
 files = [
     {file = "alabaster-0.7.13-py3-none-any.whl", hash = "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3"},
     {file = "alabaster-0.7.13.tar.gz", hash = "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"},
 ]
 
 [[package]]
+name = "ansi2html"
+version = "1.8.0"
+description = ""
+category = "main"
+optional = false
+python-versions = ">=3.6"
+files = [
+    {file = "ansi2html-1.8.0-py3-none-any.whl", hash = "sha256:ef9cc9682539dbe524fbf8edad9c9462a308e04bce1170c32daa8fdfd0001785"},
+    {file = "ansi2html-1.8.0.tar.gz", hash = "sha256:38b82a298482a1fa2613f0f9c9beb3db72a8f832eeac58eb2e47bf32cd37f6d5"},
+]
+
+[package.extras]
+docs = ["Sphinx", "setuptools-scm", "sphinx-rtd-theme"]
+test = ["pytest", "pytest-cov"]
+
+[[package]]
 name = "ansys-api-platform-instancemanagement"
 version = "1.0.0b3"
 description = ""
 category = "main"
 optional = false
 python-versions = "*"
 files = [
@@ -183,68 +199,47 @@
 [package.source]
 type = "legacy"
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple"
 reference = "solutions-private-pypi"
 
 [[package]]
 name = "ansys-solutions-dash-lib"
-version = "0.3.0"
+version = "0.4.2"
 description = "A collection of functions and classes to design solution's frontend using Dash components."
 category = "main"
 optional = false
 python-versions = ">=3.8,<3.11"
 files = [
-    {file = "ansys-solutions-dash-lib-0.3.0.tar.gz", hash = "sha256:a2ce7ef96609d575e8b439eb3f7cc8a3039633cc7cf9f059cdea8510b616ee9a"},
-    {file = "ansys_solutions_dash_lib-0.3.0-py3-none-any.whl", hash = "sha256:fbacf674fceed9f31bfcd3affa47dcb9249b4235302057109773fc7cdff7f140"},
+    {file = "ansys_solutions_dash_lib-0.4.2-py3-none-any.whl", hash = "sha256:21bd1225591d290ff463602ff83c033bfe35fd7b4418db496654eb1c8e25084c"},
+    {file = "ansys_solutions_dash_lib-0.4.2.tar.gz", hash = "sha256:285ccf20b01e1de03ea288f2fced6bb16d6d1d8dc4a09d647626d57c551681df"},
 ]
 
 [package.dependencies]
 dash = ">=2.5,<3.0"
 dash_bootstrap_components = ">=1.3,<2.0"
 
 [package.source]
 type = "legacy"
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple"
 reference = "solutions-private-pypi"
 
 [[package]]
 name = "ansys-solutions-optislang-frontend-components"
-version = "0.1.dev3"
-description = ""
-category = "main"
-optional = false
-python-versions = ">=3.8,<3.11"
-files = [
-    {file = "ansys_solutions_optislang_frontend_components-0.1.dev3-py3-none-any.whl", hash = "sha256:8e82b5bb06e369a518bfe60872bbf9f03ed6811f3cf76cb9699c5ba771e8f7e1"},
-    {file = "ansys_solutions_optislang_frontend_components-0.1.dev3.tar.gz", hash = "sha256:a1146cb5c3473ebc7719d4c67eb61029ed512224c9dfa7356fd10451ee95759a"},
-]
-
-[package.dependencies]
-ansys-solutions-dash-lib = "0.3.0"
-ansys-solutions-optislang-parser = ">=0.1.dev1,<0.2"
-
-[package.source]
-type = "legacy"
-url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple"
-reference = "solutions-private-pypi"
-
-[[package]]
-name = "ansys-solutions-optislang-parser"
 version = "0.1.dev6"
 description = ""
 category = "main"
 optional = false
 python-versions = ">=3.8,<3.11"
 files = [
-    {file = "ansys_solutions_optislang_parser-0.1.dev6-py3-none-any.whl", hash = "sha256:f48ad3715f453f7ac3b3e95f06a73f88c095b79e314d2e6dfb5e1b3fa89e7140"},
-    {file = "ansys_solutions_optislang_parser-0.1.dev6.tar.gz", hash = "sha256:745f10c6f532a9dc4edeb08b7f9fe01dad3b4d2eb8af806c017e973e5263b4a0"},
+    {file = "ansys_solutions_optislang_frontend_components-0.1.dev6-py3-none-any.whl", hash = "sha256:0ca79c5f8fc799ac68723287e00ac0bd81ac1580908c312cf89698ea60c9cd3b"},
+    {file = "ansys_solutions_optislang_frontend_components-0.1.dev6.tar.gz", hash = "sha256:aa23ea70987986a8a38722bc53d6279db34073f7f4927a4e02c17b31f58ade3b"},
 ]
 
 [package.dependencies]
-ansys-optislang-core = ">=0.3,<0.4"
+ansys-solutions-dash-lib = "0.4.2"
 
 [package.source]
 type = "legacy"
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple"
 reference = "solutions-private-pypi"
 
 [[package]]
@@ -814,35 +809,40 @@
 ssh = ["bcrypt (>=3.1.5)"]
 test = ["hypothesis (>=1.11.4,!=3.79.2)", "iso8601", "pretend", "pytest (>=6.2.0)", "pytest-benchmark", "pytest-cov", "pytest-shard (>=0.1.2)", "pytest-subtests", "pytest-xdist", "pytz"]
 test-randomorder = ["pytest-randomly"]
 tox = ["tox"]
 
 [[package]]
 name = "dash"
-version = "2.10.2"
+version = "2.11.1"
 description = "A Python framework for building reactive web-apps. Developed by Plotly."
 category = "main"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "dash-2.10.2-py3-none-any.whl", hash = "sha256:f1b7132558bd2341e6cf7ca1e83e216d46bbb27a255ca962a0fa5561c6776953"},
-    {file = "dash-2.10.2.tar.gz", hash = "sha256:b99839890b44171da0e3668c2e607ef4b4f6948a6074c034693534ba52aa1d2b"},
+    {file = "dash-2.11.1-py3-none-any.whl", hash = "sha256:a5b55efc7f139538d95331fa0b5ee0d21600f7dafa9cce4fe4f887b773aba01a"},
+    {file = "dash-2.11.1.tar.gz", hash = "sha256:1acc4c634311cb306a1086fff315c1f2aaa3898bac362d93bc8db6b1a6474e5c"},
 ]
 
 [package.dependencies]
+ansi2html = "*"
 dash-core-components = "2.0.0"
 dash-html-components = "2.0.0"
 dash-table = "5.0.0"
 Flask = ">=1.0.4,<2.3.0"
+nest-asyncio = "*"
 plotly = ">=5.0.0"
+requests = "*"
+retrying = "*"
+typing-extensions = ">=4.1.1"
 Werkzeug = "<2.3.0"
 
 [package.extras]
 celery = ["celery[redis] (>=5.1.2)", "importlib-metadata (<5)", "redis (>=3.5.3)"]
-ci = ["black (==21.6b0)", "black (==22.3.0)", "dash-dangerously-set-inner-html", "dash-flow-example (==0.0.5)", "flake8 (==3.9.2)", "flaky (==3.7.0)", "flask-talisman (==1.0.0)", "isort (==4.3.21)", "mimesis", "mock (==4.0.3)", "numpy", "openpyxl", "orjson (==3.5.4)", "orjson (==3.6.7)", "pandas (==1.1.5)", "pandas (>=1.4.0)", "preconditions", "pyarrow", "pyarrow (<3)", "pylint (==2.13.5)", "pytest-mock", "pytest-rerunfailures", "pytest-sugar (==0.9.6)", "xlrd (<2)", "xlrd (>=2.0.1)"]
+ci = ["black (==21.6b0)", "black (==22.3.0)", "dash-dangerously-set-inner-html", "dash-flow-example (==0.0.5)", "flake8 (==3.9.2)", "flaky (==3.7.0)", "flask-talisman (==1.0.0)", "isort (==4.3.21)", "jupyterlab (<4.0.0)", "mimesis", "mock (==4.0.3)", "numpy", "openpyxl", "orjson (==3.5.4)", "orjson (==3.6.7)", "pandas (==1.1.5)", "pandas (>=1.4.0)", "preconditions", "pyarrow", "pyarrow (<3)", "pylint (==2.13.5)", "pytest-mock", "pytest-rerunfailures", "pytest-sugar (==0.9.6)", "xlrd (<2)", "xlrd (>=2.0.1)"]
 compress = ["flask-compress"]
 dev = ["PyYAML (>=5.4.1)", "coloredlogs (>=15.0.1)", "fire (>=0.4.0)"]
 diskcache = ["diskcache (>=5.2.1)", "multiprocess (>=0.70.12)", "psutil (>=5.8.0)"]
 testing = ["beautifulsoup4 (>=4.8.2)", "cryptography (<3.4)", "dash-testing-stub (>=0.0.2)", "lxml (>=4.6.2)", "multiprocess (>=0.70.12)", "percy (>=2.0.2)", "psutil (>=5.8.0)", "pytest (>=6.0.2)", "requests[security] (>=2.21.0)", "selenium (>=3.141.0,<=4.2.0)", "waitress (>=1.4.4)"]
 
 [[package]]
 name = "dash-bootstrap-components"
@@ -916,14 +916,29 @@
 python-versions = "*"
 files = [
     {file = "dash_iconify-0.1.2-py3-none-any.whl", hash = "sha256:9ab0eda19bb4514e177bf1f8f36947bb9e5b44aba6ce947f22a1cf0f1a45fc14"},
     {file = "dash_iconify-0.1.2.tar.gz", hash = "sha256:564774be6b11b0ac3a8999b7137c3d17a1d351d69b673aa313c7228eacc9d143"},
 ]
 
 [[package]]
+name = "dash-loading-spinners"
+version = "1.0.0"
+description = "Fun and funky loading spinners for your Dash apps"
+category = "main"
+optional = false
+python-versions = "*"
+files = [
+    {file = "dash_loading_spinners-1.0.0-py3-none-any.whl", hash = "sha256:7dd514f8acbc7e58f4b1e64110b022badee60248f18cc78233ee3c68e0716f14"},
+    {file = "dash_loading_spinners-1.0.0.tar.gz", hash = "sha256:bc759733fbd391f1d1c60dbd9e7e47a3eb33fe6d1778d4936307d9ccb5417565"},
+]
+
+[package.dependencies]
+dash = "*"
+
+[[package]]
 name = "dash-table"
 version = "5.0.0"
 description = "Dash table"
 category = "main"
 optional = false
 python-versions = "*"
 files = [
@@ -1028,22 +1043,22 @@
 files = [
     {file = "EditorConfig-0.12.3-py3-none-any.whl", hash = "sha256:6b0851425aa875b08b16789ee0eeadbd4ab59666e9ebe728e526314c4a2e52c1"},
     {file = "EditorConfig-0.12.3.tar.gz", hash = "sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.1.1"
+version = "1.1.2"
 description = "Backport of PEP 654 (exception groups)"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
-    {file = "exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
+    {file = "exceptiongroup-1.1.2-py3-none-any.whl", hash = "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"},
+    {file = "exceptiongroup-1.1.2.tar.gz", hash = "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "execnet"
@@ -1517,36 +1532,36 @@
 
 [package.dependencies]
 editorconfig = ">=0.12.2"
 six = ">=1.13.0"
 
 [[package]]
 name = "keyring"
-version = "23.13.1"
+version = "24.2.0"
 description = "Store and access your passwords safely."
 category = "dev"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "keyring-23.13.1-py3-none-any.whl", hash = "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd"},
-    {file = "keyring-23.13.1.tar.gz", hash = "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"},
+    {file = "keyring-24.2.0-py3-none-any.whl", hash = "sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6"},
+    {file = "keyring-24.2.0.tar.gz", hash = "sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509"},
 ]
 
 [package.dependencies]
 importlib-metadata = {version = ">=4.11.4", markers = "python_version < \"3.12\""}
 importlib-resources = {version = "*", markers = "python_version < \"3.9\""}
 "jaraco.classes" = "*"
 jeepney = {version = ">=0.4.2", markers = "sys_platform == \"linux\""}
 pywin32-ctypes = {version = ">=0.2.0", markers = "sys_platform == \"win32\""}
 SecretStorage = {version = ">=3.2", markers = "sys_platform == \"linux\""}
 
 [package.extras]
 completion = ["shtab"]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)"]
-testing = ["flake8 (<5)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
+testing = ["pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-ruff"]
 
 [[package]]
 name = "markdown-it-py"
 version = "3.0.0"
 description = "Python port of markdown-it. Markdown parsing, done right!"
 category = "dev"
 optional = false
@@ -1679,14 +1694,26 @@
 python-versions = ">=3.7"
 files = [
     {file = "more-itertools-9.1.0.tar.gz", hash = "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d"},
     {file = "more_itertools-9.1.0-py3-none-any.whl", hash = "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"},
 ]
 
 [[package]]
+name = "nest-asyncio"
+version = "1.5.6"
+description = "Patch asyncio to allow nested event loops"
+category = "main"
+optional = false
+python-versions = ">=3.5"
+files = [
+    {file = "nest_asyncio-1.5.6-py3-none-any.whl", hash = "sha256:b9a953fb40dceaa587d109609098db21900182b16440652454a146cffb06e8b8"},
+    {file = "nest_asyncio-1.5.6.tar.gz", hash = "sha256:d267cc1ff794403f7df692964d1d2a3fa9418ffea2a3f6859a439ff482fef290"},
+]
+
+[[package]]
 name = "networkx"
 version = "3.1"
 description = "Python package for creating and manipulating graphs and networks"
 category = "main"
 optional = false
 python-versions = ">=3.8"
 files = [
@@ -1699,48 +1726,48 @@
 developer = ["mypy (>=1.1)", "pre-commit (>=3.2)"]
 doc = ["nb2plots (>=0.6)", "numpydoc (>=1.5)", "pillow (>=9.4)", "pydata-sphinx-theme (>=0.13)", "sphinx (>=6.1)", "sphinx-gallery (>=0.12)", "texext (>=0.6.7)"]
 extra = ["lxml (>=4.6)", "pydot (>=1.4.2)", "pygraphviz (>=1.10)", "sympy (>=1.10)"]
 test = ["codecov (>=2.1)", "pytest (>=7.2)", "pytest-cov (>=4.0)"]
 
 [[package]]
 name = "numpy"
-version = "1.24.3"
+version = "1.24.4"
 description = "Fundamental package for array computing in Python"
 category = "main"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "numpy-1.24.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:3c1104d3c036fb81ab923f507536daedc718d0ad5a8707c6061cdfd6d184e570"},
-    {file = "numpy-1.24.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7"},
-    {file = "numpy-1.24.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8535303847b89aa6b0f00aa1dc62867b5a32923e4d1681a35b5eef2d9591a463"},
-    {file = "numpy-1.24.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2d926b52ba1367f9acb76b0df6ed21f0b16a1ad87c6720a1121674e5cf63e2b6"},
-    {file = "numpy-1.24.3-cp310-cp310-win32.whl", hash = "sha256:f21c442fdd2805e91799fbe044a7b999b8571bb0ab0f7850d0cb9641a687092b"},
-    {file = "numpy-1.24.3-cp310-cp310-win_amd64.whl", hash = "sha256:ab5f23af8c16022663a652d3b25dcdc272ac3f83c3af4c02eb8b824e6b3ab9d7"},
-    {file = "numpy-1.24.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:9a7721ec204d3a237225db3e194c25268faf92e19338a35f3a224469cb6039a3"},
-    {file = "numpy-1.24.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d6cc757de514c00b24ae8cf5c876af2a7c3df189028d68c0cb4eaa9cd5afc2bf"},
-    {file = "numpy-1.24.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:76e3f4e85fc5d4fd311f6e9b794d0c00e7002ec122be271f2019d63376f1d385"},
-    {file = "numpy-1.24.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a1d3c026f57ceaad42f8231305d4653d5f05dc6332a730ae5c0bea3513de0950"},
-    {file = "numpy-1.24.3-cp311-cp311-win32.whl", hash = "sha256:c91c4afd8abc3908e00a44b2672718905b8611503f7ff87390cc0ac3423fb096"},
-    {file = "numpy-1.24.3-cp311-cp311-win_amd64.whl", hash = "sha256:5342cf6aad47943286afa6f1609cad9b4266a05e7f2ec408e2cf7aea7ff69d80"},
-    {file = "numpy-1.24.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:7776ea65423ca6a15255ba1872d82d207bd1e09f6d0894ee4a64678dd2204078"},
-    {file = "numpy-1.24.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:ae8d0be48d1b6ed82588934aaaa179875e7dc4f3d84da18d7eae6eb3f06c242c"},
-    {file = "numpy-1.24.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ecde0f8adef7dfdec993fd54b0f78183051b6580f606111a6d789cd14c61ea0c"},
-    {file = "numpy-1.24.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4749e053a29364d3452c034827102ee100986903263e89884922ef01a0a6fd2f"},
-    {file = "numpy-1.24.3-cp38-cp38-win32.whl", hash = "sha256:d933fabd8f6a319e8530d0de4fcc2e6a61917e0b0c271fded460032db42a0fe4"},
-    {file = "numpy-1.24.3-cp38-cp38-win_amd64.whl", hash = "sha256:56e48aec79ae238f6e4395886b5eaed058abb7231fb3361ddd7bfdf4eed54289"},
-    {file = "numpy-1.24.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4719d5aefb5189f50887773699eaf94e7d1e02bf36c1a9d353d9f46703758ca4"},
-    {file = "numpy-1.24.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187"},
-    {file = "numpy-1.24.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ea8282b9bcfe2b5e7d491d0bf7f3e2da29700cec05b49e64d6246923329f2b02"},
-    {file = "numpy-1.24.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4"},
-    {file = "numpy-1.24.3-cp39-cp39-win32.whl", hash = "sha256:784c6da1a07818491b0ffd63c6bbe5a33deaa0e25a20e1b3ea20cf0e43f8046c"},
-    {file = "numpy-1.24.3-cp39-cp39-win_amd64.whl", hash = "sha256:d5036197ecae68d7f491fcdb4df90082b0d4960ca6599ba2659957aafced7c17"},
-    {file = "numpy-1.24.3-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:352ee00c7f8387b44d19f4cada524586f07379c0d49270f87233983bc5087ca0"},
-    {file = "numpy-1.24.3-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812"},
-    {file = "numpy-1.24.3-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:35400e6a8d102fd07c71ed7dcadd9eb62ee9a6e84ec159bd48c28235bbb0f8e4"},
-    {file = "numpy-1.24.3.tar.gz", hash = "sha256:ab344f1bf21f140adab8e47fdbc7c35a477dc01408791f8ba00d018dd0bc5155"},
+    {file = "numpy-1.24.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c0bfb52d2169d58c1cdb8cc1f16989101639b34c7d3ce60ed70b19c63eba0b64"},
+    {file = "numpy-1.24.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ed094d4f0c177b1b8e7aa9cba7d6ceed51c0e569a5318ac0ca9a090680a6a1b1"},
+    {file = "numpy-1.24.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:79fc682a374c4a8ed08b331bef9c5f582585d1048fa6d80bc6c35bc384eee9b4"},
+    {file = "numpy-1.24.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7ffe43c74893dbf38c2b0a1f5428760a1a9c98285553c89e12d70a96a7f3a4d6"},
+    {file = "numpy-1.24.4-cp310-cp310-win32.whl", hash = "sha256:4c21decb6ea94057331e111a5bed9a79d335658c27ce2adb580fb4d54f2ad9bc"},
+    {file = "numpy-1.24.4-cp310-cp310-win_amd64.whl", hash = "sha256:b4bea75e47d9586d31e892a7401f76e909712a0fd510f58f5337bea9572c571e"},
+    {file = "numpy-1.24.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:f136bab9c2cfd8da131132c2cf6cc27331dd6fae65f95f69dcd4ae3c3639c810"},
+    {file = "numpy-1.24.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:e2926dac25b313635e4d6cf4dc4e51c8c0ebfed60b801c799ffc4c32bf3d1254"},
+    {file = "numpy-1.24.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:222e40d0e2548690405b0b3c7b21d1169117391c2e82c378467ef9ab4c8f0da7"},
+    {file = "numpy-1.24.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7215847ce88a85ce39baf9e89070cb860c98fdddacbaa6c0da3ffb31b3350bd5"},
+    {file = "numpy-1.24.4-cp311-cp311-win32.whl", hash = "sha256:4979217d7de511a8d57f4b4b5b2b965f707768440c17cb70fbf254c4b225238d"},
+    {file = "numpy-1.24.4-cp311-cp311-win_amd64.whl", hash = "sha256:b7b1fc9864d7d39e28f41d089bfd6353cb5f27ecd9905348c24187a768c79694"},
+    {file = "numpy-1.24.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1452241c290f3e2a312c137a9999cdbf63f78864d63c79039bda65ee86943f61"},
+    {file = "numpy-1.24.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:04640dab83f7c6c85abf9cd729c5b65f1ebd0ccf9de90b270cd61935eef0197f"},
+    {file = "numpy-1.24.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a5425b114831d1e77e4b5d812b69d11d962e104095a5b9c3b641a218abcc050e"},
+    {file = "numpy-1.24.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dd80e219fd4c71fc3699fc1dadac5dcf4fd882bfc6f7ec53d30fa197b8ee22dc"},
+    {file = "numpy-1.24.4-cp38-cp38-win32.whl", hash = "sha256:4602244f345453db537be5314d3983dbf5834a9701b7723ec28923e2889e0bb2"},
+    {file = "numpy-1.24.4-cp38-cp38-win_amd64.whl", hash = "sha256:692f2e0f55794943c5bfff12b3f56f99af76f902fc47487bdfe97856de51a706"},
+    {file = "numpy-1.24.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:2541312fbf09977f3b3ad449c4e5f4bb55d0dbf79226d7724211acc905049400"},
+    {file = "numpy-1.24.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:9667575fb6d13c95f1b36aca12c5ee3356bf001b714fc354eb5465ce1609e62f"},
+    {file = "numpy-1.24.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f3a86ed21e4f87050382c7bc96571755193c4c1392490744ac73d660e8f564a9"},
+    {file = "numpy-1.24.4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d11efb4dbecbdf22508d55e48d9c8384db795e1b7b51ea735289ff96613ff74d"},
+    {file = "numpy-1.24.4-cp39-cp39-win32.whl", hash = "sha256:6620c0acd41dbcb368610bb2f4d83145674040025e5536954782467100aa8835"},
+    {file = "numpy-1.24.4-cp39-cp39-win_amd64.whl", hash = "sha256:befe2bf740fd8373cf56149a5c23a0f601e82869598d41f8e188a0e9869926f8"},
+    {file = "numpy-1.24.4-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:31f13e25b4e304632a4619d0e0777662c2ffea99fcae2029556b17d8ff958aef"},
+    {file = "numpy-1.24.4-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:95f7ac6540e95bc440ad77f56e520da5bf877f87dca58bd095288dce8940532a"},
+    {file = "numpy-1.24.4-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:e98f220aa76ca2a977fe435f5b04d7b3470c0a2e6312907b37ba6068f26787f2"},
+    {file = "numpy-1.24.4.tar.gz", hash = "sha256:80f5e3a4e498641401868df4208b74581206afbee7cf7b8329daae82676d9463"},
 ]
 
 [[package]]
 name = "numpy"
 version = "1.25.0"
 description = "Fundamental package for array computing in Python"
 category = "main"
@@ -2103,58 +2130,58 @@
 files = [
     {file = "packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {file = "packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 
 [[package]]
 name = "pandas"
-version = "2.0.2"
+version = "2.0.3"
 description = "Powerful data structures for data analysis, time series, and statistics"
 category = "main"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "pandas-2.0.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:9ebb9f1c22ddb828e7fd017ea265a59d80461d5a79154b49a4207bd17514d122"},
-    {file = "pandas-2.0.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:1eb09a242184092f424b2edd06eb2b99d06dc07eeddff9929e8667d4ed44e181"},
-    {file = "pandas-2.0.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c7319b6e68de14e6209460f72a8d1ef13c09fb3d3ef6c37c1e65b35d50b5c145"},
-    {file = "pandas-2.0.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dd46bde7309088481b1cf9c58e3f0e204b9ff9e3244f441accd220dd3365ce7c"},
-    {file = "pandas-2.0.2-cp310-cp310-win32.whl", hash = "sha256:51a93d422fbb1bd04b67639ba4b5368dffc26923f3ea32a275d2cc450f1d1c86"},
-    {file = "pandas-2.0.2-cp310-cp310-win_amd64.whl", hash = "sha256:66d00300f188fa5de73f92d5725ced162488f6dc6ad4cecfe4144ca29debe3b8"},
-    {file = "pandas-2.0.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:02755de164da6827764ceb3bbc5f64b35cb12394b1024fdf88704d0fa06e0e2f"},
-    {file = "pandas-2.0.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:0a1e0576611641acde15c2322228d138258f236d14b749ad9af498ab69089e2d"},
-    {file = "pandas-2.0.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a6b5f14cd24a2ed06e14255ff40fe2ea0cfaef79a8dd68069b7ace74bd6acbba"},
-    {file = "pandas-2.0.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50e451932b3011b61d2961b4185382c92cc8c6ee4658dcd4f320687bb2d000ee"},
-    {file = "pandas-2.0.2-cp311-cp311-win32.whl", hash = "sha256:7b21cb72958fc49ad757685db1919021d99650d7aaba676576c9e88d3889d456"},
-    {file = "pandas-2.0.2-cp311-cp311-win_amd64.whl", hash = "sha256:c4af689352c4fe3d75b2834933ee9d0ccdbf5d7a8a7264f0ce9524e877820c08"},
-    {file = "pandas-2.0.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:69167693cb8f9b3fc060956a5d0a0a8dbfed5f980d9fd2c306fb5b9c855c814c"},
-    {file = "pandas-2.0.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:30a89d0fec4263ccbf96f68592fd668939481854d2ff9da709d32a047689393b"},
-    {file = "pandas-2.0.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a18e5c72b989ff0f7197707ceddc99828320d0ca22ab50dd1b9e37db45b010c0"},
-    {file = "pandas-2.0.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7376e13d28eb16752c398ca1d36ccfe52bf7e887067af9a0474de6331dd948d2"},
-    {file = "pandas-2.0.2-cp38-cp38-win32.whl", hash = "sha256:6d6d10c2142d11d40d6e6c0a190b1f89f525bcf85564707e31b0a39e3b398e08"},
-    {file = "pandas-2.0.2-cp38-cp38-win_amd64.whl", hash = "sha256:e69140bc2d29a8556f55445c15f5794490852af3de0f609a24003ef174528b79"},
-    {file = "pandas-2.0.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:b42b120458636a981077cfcfa8568c031b3e8709701315e2bfa866324a83efa8"},
-    {file = "pandas-2.0.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f908a77cbeef9bbd646bd4b81214cbef9ac3dda4181d5092a4aa9797d1bc7774"},
-    {file = "pandas-2.0.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:713f2f70abcdade1ddd68fc91577cb090b3544b07ceba78a12f799355a13ee44"},
-    {file = "pandas-2.0.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cf3f0c361a4270185baa89ec7ab92ecaa355fe783791457077473f974f654df5"},
-    {file = "pandas-2.0.2-cp39-cp39-win32.whl", hash = "sha256:598e9020d85a8cdbaa1815eb325a91cfff2bb2b23c1442549b8a3668e36f0f77"},
-    {file = "pandas-2.0.2-cp39-cp39-win_amd64.whl", hash = "sha256:77550c8909ebc23e56a89f91b40ad01b50c42cfbfab49b3393694a50549295ea"},
-    {file = "pandas-2.0.2.tar.gz", hash = "sha256:dd5476b6c3fe410ee95926873f377b856dbc4e81a9c605a0dc05aaccc6a7c6c6"},
+    {file = "pandas-2.0.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e4c7c9f27a4185304c7caf96dc7d91bc60bc162221152de697c98eb0b2648dd8"},
+    {file = "pandas-2.0.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:f167beed68918d62bffb6ec64f2e1d8a7d297a038f86d4aed056b9493fca407f"},
+    {file = "pandas-2.0.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ce0c6f76a0f1ba361551f3e6dceaff06bde7514a374aa43e33b588ec10420183"},
+    {file = "pandas-2.0.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ba619e410a21d8c387a1ea6e8a0e49bb42216474436245718d7f2e88a2f8d7c0"},
+    {file = "pandas-2.0.3-cp310-cp310-win32.whl", hash = "sha256:3ef285093b4fe5058eefd756100a367f27029913760773c8bf1d2d8bebe5d210"},
+    {file = "pandas-2.0.3-cp310-cp310-win_amd64.whl", hash = "sha256:9ee1a69328d5c36c98d8e74db06f4ad518a1840e8ccb94a4ba86920986bb617e"},
+    {file = "pandas-2.0.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:b084b91d8d66ab19f5bb3256cbd5ea661848338301940e17f4492b2ce0801fe8"},
+    {file = "pandas-2.0.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:37673e3bdf1551b95bf5d4ce372b37770f9529743d2498032439371fc7b7eb26"},
+    {file = "pandas-2.0.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b9cb1e14fdb546396b7e1b923ffaeeac24e4cedd14266c3497216dd4448e4f2d"},
+    {file = "pandas-2.0.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d9cd88488cceb7635aebb84809d087468eb33551097d600c6dad13602029c2df"},
+    {file = "pandas-2.0.3-cp311-cp311-win32.whl", hash = "sha256:694888a81198786f0e164ee3a581df7d505024fbb1f15202fc7db88a71d84ebd"},
+    {file = "pandas-2.0.3-cp311-cp311-win_amd64.whl", hash = "sha256:6a21ab5c89dcbd57f78d0ae16630b090eec626360085a4148693def5452d8a6b"},
+    {file = "pandas-2.0.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:9e4da0d45e7f34c069fe4d522359df7d23badf83abc1d1cef398895822d11061"},
+    {file = "pandas-2.0.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:32fca2ee1b0d93dd71d979726b12b61faa06aeb93cf77468776287f41ff8fdc5"},
+    {file = "pandas-2.0.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:258d3624b3ae734490e4d63c430256e716f488c4fcb7c8e9bde2d3aa46c29089"},
+    {file = "pandas-2.0.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9eae3dc34fa1aa7772dd3fc60270d13ced7346fcbcfee017d3132ec625e23bb0"},
+    {file = "pandas-2.0.3-cp38-cp38-win32.whl", hash = "sha256:f3421a7afb1a43f7e38e82e844e2bca9a6d793d66c1a7f9f0ff39a795bbc5e02"},
+    {file = "pandas-2.0.3-cp38-cp38-win_amd64.whl", hash = "sha256:69d7f3884c95da3a31ef82b7618af5710dba95bb885ffab339aad925c3e8ce78"},
+    {file = "pandas-2.0.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:5247fb1ba347c1261cbbf0fcfba4a3121fbb4029d95d9ef4dc45406620b25c8b"},
+    {file = "pandas-2.0.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:81af086f4543c9d8bb128328b5d32e9986e0c84d3ee673a2ac6fb57fd14f755e"},
+    {file = "pandas-2.0.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1994c789bf12a7c5098277fb43836ce090f1073858c10f9220998ac74f37c69b"},
+    {file = "pandas-2.0.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5ec591c48e29226bcbb316e0c1e9423622bc7a4eaf1ef7c3c9fa1a3981f89641"},
+    {file = "pandas-2.0.3-cp39-cp39-win32.whl", hash = "sha256:04dbdbaf2e4d46ca8da896e1805bc04eb85caa9a82e259e8eed00254d5e0c682"},
+    {file = "pandas-2.0.3-cp39-cp39-win_amd64.whl", hash = "sha256:1168574b036cd8b93abc746171c9b4f1b83467438a5e45909fed645cf8692dbc"},
+    {file = "pandas-2.0.3.tar.gz", hash = "sha256:c02f372a88e0d17f36d3093a644c73cfc1788e876a7c4bcb4020a77512e2043c"},
 ]
 
 [package.dependencies]
 numpy = [
     {version = ">=1.20.3", markers = "python_version < \"3.10\""},
     {version = ">=1.21.0", markers = "python_version >= \"3.10\""},
 ]
 python-dateutil = ">=2.8.2"
 pytz = ">=2020.1"
 tzdata = ">=2022.1"
 
 [package.extras]
-all = ["PyQt5 (>=5.15.1)", "SQLAlchemy (>=1.4.16)", "beautifulsoup4 (>=4.9.3)", "bottleneck (>=1.3.2)", "brotlipy (>=0.7.0)", "fastparquet (>=0.6.3)", "fsspec (>=2021.07.0)", "gcsfs (>=2021.07.0)", "html5lib (>=1.1)", "hypothesis (>=6.34.2)", "jinja2 (>=3.0.0)", "lxml (>=4.6.3)", "matplotlib (>=3.6.1)", "numba (>=0.53.1)", "numexpr (>=2.7.3)", "odfpy (>=1.4.1)", "openpyxl (>=3.0.7)", "pandas-gbq (>=0.15.0)", "psycopg2 (>=2.8.6)", "pyarrow (>=7.0.0)", "pymysql (>=1.0.2)", "pyreadstat (>=1.1.2)", "pytest (>=7.0.0)", "pytest-asyncio (>=0.17.0)", "pytest-xdist (>=2.2.0)", "python-snappy (>=0.6.0)", "pyxlsb (>=1.0.8)", "qtpy (>=2.2.0)", "s3fs (>=2021.08.0)", "scipy (>=1.7.1)", "tables (>=3.6.1)", "tabulate (>=0.8.9)", "xarray (>=0.21.0)", "xlrd (>=2.0.1)", "xlsxwriter (>=1.4.3)", "zstandard (>=0.15.2)"]
+all = ["PyQt5 (>=5.15.1)", "SQLAlchemy (>=1.4.16)", "beautifulsoup4 (>=4.9.3)", "bottleneck (>=1.3.2)", "brotlipy (>=0.7.0)", "fastparquet (>=0.6.3)", "fsspec (>=2021.07.0)", "gcsfs (>=2021.07.0)", "html5lib (>=1.1)", "hypothesis (>=6.34.2)", "jinja2 (>=3.0.0)", "lxml (>=4.6.3)", "matplotlib (>=3.6.1)", "numba (>=0.53.1)", "numexpr (>=2.7.3)", "odfpy (>=1.4.1)", "openpyxl (>=3.0.7)", "pandas-gbq (>=0.15.0)", "psycopg2 (>=2.8.6)", "pyarrow (>=7.0.0)", "pymysql (>=1.0.2)", "pyreadstat (>=1.1.2)", "pytest (>=7.3.2)", "pytest-asyncio (>=0.17.0)", "pytest-xdist (>=2.2.0)", "python-snappy (>=0.6.0)", "pyxlsb (>=1.0.8)", "qtpy (>=2.2.0)", "s3fs (>=2021.08.0)", "scipy (>=1.7.1)", "tables (>=3.6.1)", "tabulate (>=0.8.9)", "xarray (>=0.21.0)", "xlrd (>=2.0.1)", "xlsxwriter (>=1.4.3)", "zstandard (>=0.15.2)"]
 aws = ["s3fs (>=2021.08.0)"]
 clipboard = ["PyQt5 (>=5.15.1)", "qtpy (>=2.2.0)"]
 compression = ["brotlipy (>=0.7.0)", "python-snappy (>=0.6.0)", "zstandard (>=0.15.2)"]
 computation = ["scipy (>=1.7.1)", "xarray (>=0.21.0)"]
 excel = ["odfpy (>=1.4.1)", "openpyxl (>=3.0.7)", "pyxlsb (>=1.0.8)", "xlrd (>=2.0.1)", "xlsxwriter (>=1.4.3)"]
 feather = ["pyarrow (>=7.0.0)"]
 fss = ["fsspec (>=2021.07.0)"]
@@ -2165,15 +2192,15 @@
 output-formatting = ["jinja2 (>=3.0.0)", "tabulate (>=0.8.9)"]
 parquet = ["pyarrow (>=7.0.0)"]
 performance = ["bottleneck (>=1.3.2)", "numba (>=0.53.1)", "numexpr (>=2.7.1)"]
 plot = ["matplotlib (>=3.6.1)"]
 postgresql = ["SQLAlchemy (>=1.4.16)", "psycopg2 (>=2.8.6)"]
 spss = ["pyreadstat (>=1.1.2)"]
 sql-other = ["SQLAlchemy (>=1.4.16)"]
-test = ["hypothesis (>=6.34.2)", "pytest (>=7.0.0)", "pytest-asyncio (>=0.17.0)", "pytest-xdist (>=2.2.0)"]
+test = ["hypothesis (>=6.34.2)", "pytest (>=7.3.2)", "pytest-asyncio (>=0.17.0)", "pytest-xdist (>=2.2.0)"]
 xml = ["lxml (>=4.6.3)"]
 
 [[package]]
 name = "pep517"
 version = "0.13.0"
 description = "Wrappers to build Python packages using PEP 517 hooks"
 category = "dev"
@@ -2212,22 +2239,22 @@
 ]
 
 [package.extras]
 testing = ["pytest", "pytest-cov"]
 
 [[package]]
 name = "platformdirs"
-version = "3.6.0"
+version = "3.8.0"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-3.6.0-py3-none-any.whl", hash = "sha256:ffa199e3fbab8365778c4a10e1fbf1b9cd50707de826eb304b50e57ec0cc8d38"},
-    {file = "platformdirs-3.6.0.tar.gz", hash = "sha256:57e28820ca8094678b807ff529196506d7a21e17156cb1cddb3e74cebce54640"},
+    {file = "platformdirs-3.8.0-py3-none-any.whl", hash = "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"},
+    {file = "platformdirs-3.8.0.tar.gz", hash = "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc"},
 ]
 
 [package.extras]
 docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
@@ -2244,22 +2271,22 @@
 
 [package.dependencies]
 packaging = "*"
 tenacity = ">=6.2.0"
 
 [[package]]
 name = "pluggy"
-version = "1.0.0"
+version = "1.2.0"
 description = "plugin and hook calling mechanisms for python"
 category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
-    {file = "pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
+    {file = "pluggy-1.2.0-py3-none-any.whl", hash = "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849"},
+    {file = "pluggy-1.2.0.tar.gz", hash = "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"},
 ]
 
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
@@ -2356,56 +2383,56 @@
 files = [
     {file = "pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
     {file = "pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
 ]
 
 [[package]]
 name = "pydantic"
-version = "1.10.9"
+version = "1.10.11"
 description = "Data validation and settings management using python type hints"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pydantic-1.10.9-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e692dec4a40bfb40ca530e07805b1208c1de071a18d26af4a2a0d79015b352ca"},
-    {file = "pydantic-1.10.9-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:3c52eb595db83e189419bf337b59154bdcca642ee4b2a09e5d7797e41ace783f"},
-    {file = "pydantic-1.10.9-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:939328fd539b8d0edf244327398a667b6b140afd3bf7e347cf9813c736211896"},
-    {file = "pydantic-1.10.9-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b48d3d634bca23b172f47f2335c617d3fcb4b3ba18481c96b7943a4c634f5c8d"},
-    {file = "pydantic-1.10.9-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:f0b7628fb8efe60fe66fd4adadd7ad2304014770cdc1f4934db41fe46cc8825f"},
-    {file = "pydantic-1.10.9-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:e1aa5c2410769ca28aa9a7841b80d9d9a1c5f223928ca8bec7e7c9a34d26b1d4"},
-    {file = "pydantic-1.10.9-cp310-cp310-win_amd64.whl", hash = "sha256:eec39224b2b2e861259d6f3c8b6290d4e0fbdce147adb797484a42278a1a486f"},
-    {file = "pydantic-1.10.9-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:d111a21bbbfd85c17248130deac02bbd9b5e20b303338e0dbe0faa78330e37e0"},
-    {file = "pydantic-1.10.9-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:2e9aec8627a1a6823fc62fb96480abe3eb10168fd0d859ee3d3b395105ae19a7"},
-    {file = "pydantic-1.10.9-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:07293ab08e7b4d3c9d7de4949a0ea571f11e4557d19ea24dd3ae0c524c0c334d"},
-    {file = "pydantic-1.10.9-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7ee829b86ce984261d99ff2fd6e88f2230068d96c2a582f29583ed602ef3fc2c"},
-    {file = "pydantic-1.10.9-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:4b466a23009ff5cdd7076eb56aca537c745ca491293cc38e72bf1e0e00de5b91"},
-    {file = "pydantic-1.10.9-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:7847ca62e581e6088d9000f3c497267868ca2fa89432714e21a4fb33a04d52e8"},
-    {file = "pydantic-1.10.9-cp311-cp311-win_amd64.whl", hash = "sha256:7845b31959468bc5b78d7b95ec52fe5be32b55d0d09983a877cca6aedc51068f"},
-    {file = "pydantic-1.10.9-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:517a681919bf880ce1dac7e5bc0c3af1e58ba118fd774da2ffcd93c5f96eaece"},
-    {file = "pydantic-1.10.9-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:67195274fd27780f15c4c372f4ba9a5c02dad6d50647b917b6a92bf00b3d301a"},
-    {file = "pydantic-1.10.9-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2196c06484da2b3fded1ab6dbe182bdabeb09f6318b7fdc412609ee2b564c49a"},
-    {file = "pydantic-1.10.9-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:6257bb45ad78abacda13f15bde5886efd6bf549dd71085e64b8dcf9919c38b60"},
-    {file = "pydantic-1.10.9-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3283b574b01e8dbc982080d8287c968489d25329a463b29a90d4157de4f2baaf"},
-    {file = "pydantic-1.10.9-cp37-cp37m-win_amd64.whl", hash = "sha256:5f8bbaf4013b9a50e8100333cc4e3fa2f81214033e05ac5aa44fa24a98670a29"},
-    {file = "pydantic-1.10.9-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:b9cd67fb763248cbe38f0593cd8611bfe4b8ad82acb3bdf2b0898c23415a1f82"},
-    {file = "pydantic-1.10.9-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f50e1764ce9353be67267e7fd0da08349397c7db17a562ad036aa7c8f4adfdb6"},
-    {file = "pydantic-1.10.9-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:73ef93e5e1d3c8e83f1ff2e7fdd026d9e063c7e089394869a6e2985696693766"},
-    {file = "pydantic-1.10.9-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:128d9453d92e6e81e881dd7e2484e08d8b164da5507f62d06ceecf84bf2e21d3"},
-    {file = "pydantic-1.10.9-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ad428e92ab68798d9326bb3e5515bc927444a3d71a93b4a2ca02a8a5d795c572"},
-    {file = "pydantic-1.10.9-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:fab81a92f42d6d525dd47ced310b0c3e10c416bbfae5d59523e63ea22f82b31e"},
-    {file = "pydantic-1.10.9-cp38-cp38-win_amd64.whl", hash = "sha256:963671eda0b6ba6926d8fc759e3e10335e1dc1b71ff2a43ed2efd6996634dafb"},
-    {file = "pydantic-1.10.9-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:970b1bdc6243ef663ba5c7e36ac9ab1f2bfecb8ad297c9824b542d41a750b298"},
-    {file = "pydantic-1.10.9-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:7e1d5290044f620f80cf1c969c542a5468f3656de47b41aa78100c5baa2b8276"},
-    {file = "pydantic-1.10.9-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:83fcff3c7df7adff880622a98022626f4f6dbce6639a88a15a3ce0f96466cb60"},
-    {file = "pydantic-1.10.9-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0da48717dc9495d3a8f215e0d012599db6b8092db02acac5e0d58a65248ec5bc"},
-    {file = "pydantic-1.10.9-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:0a2aabdc73c2a5960e87c3ffebca6ccde88665616d1fd6d3db3178ef427b267a"},
-    {file = "pydantic-1.10.9-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:9863b9420d99dfa9c064042304868e8ba08e89081428a1c471858aa2af6f57c4"},
-    {file = "pydantic-1.10.9-cp39-cp39-win_amd64.whl", hash = "sha256:e7c9900b43ac14110efa977be3da28931ffc74c27e96ee89fbcaaf0b0fe338e1"},
-    {file = "pydantic-1.10.9-py3-none-any.whl", hash = "sha256:6cafde02f6699ce4ff643417d1a9223716ec25e228ddc3b436fe7e2d25a1f305"},
-    {file = "pydantic-1.10.9.tar.gz", hash = "sha256:95c70da2cd3b6ddf3b9645ecaa8d98f3d80c606624b6d245558d202cd23ea3be"},
+    {file = "pydantic-1.10.11-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:ff44c5e89315b15ff1f7fdaf9853770b810936d6b01a7bcecaa227d2f8fe444f"},
+    {file = "pydantic-1.10.11-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:a6c098d4ab5e2d5b3984d3cb2527e2d6099d3de85630c8934efcfdc348a9760e"},
+    {file = "pydantic-1.10.11-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:16928fdc9cb273c6af00d9d5045434c39afba5f42325fb990add2c241402d151"},
+    {file = "pydantic-1.10.11-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0588788a9a85f3e5e9ebca14211a496409cb3deca5b6971ff37c556d581854e7"},
+    {file = "pydantic-1.10.11-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:e9baf78b31da2dc3d3f346ef18e58ec5f12f5aaa17ac517e2ffd026a92a87588"},
+    {file = "pydantic-1.10.11-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:373c0840f5c2b5b1ccadd9286782852b901055998136287828731868027a724f"},
+    {file = "pydantic-1.10.11-cp310-cp310-win_amd64.whl", hash = "sha256:c3339a46bbe6013ef7bdd2844679bfe500347ac5742cd4019a88312aa58a9847"},
+    {file = "pydantic-1.10.11-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:08a6c32e1c3809fbc49debb96bf833164f3438b3696abf0fbeceb417d123e6eb"},
+    {file = "pydantic-1.10.11-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:a451ccab49971af043ec4e0d207cbc8cbe53dbf148ef9f19599024076fe9c25b"},
+    {file = "pydantic-1.10.11-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5b02d24f7b2b365fed586ed73582c20f353a4c50e4be9ba2c57ab96f8091ddae"},
+    {file = "pydantic-1.10.11-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3f34739a89260dfa420aa3cbd069fbcc794b25bbe5c0a214f8fb29e363484b66"},
+    {file = "pydantic-1.10.11-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:e297897eb4bebde985f72a46a7552a7556a3dd11e7f76acda0c1093e3dbcf216"},
+    {file = "pydantic-1.10.11-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:d185819a7a059550ecb85d5134e7d40f2565f3dd94cfd870132c5f91a89cf58c"},
+    {file = "pydantic-1.10.11-cp311-cp311-win_amd64.whl", hash = "sha256:4400015f15c9b464c9db2d5d951b6a780102cfa5870f2c036d37c23b56f7fc1b"},
+    {file = "pydantic-1.10.11-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:2417de68290434461a266271fc57274a138510dca19982336639484c73a07af6"},
+    {file = "pydantic-1.10.11-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:331c031ba1554b974c98679bd0780d89670d6fd6f53f5d70b10bdc9addee1713"},
+    {file = "pydantic-1.10.11-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8268a735a14c308923e8958363e3a3404f6834bb98c11f5ab43251a4e410170c"},
+    {file = "pydantic-1.10.11-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:44e51ba599c3ef227e168424e220cd3e544288c57829520dc90ea9cb190c3248"},
+    {file = "pydantic-1.10.11-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d7781f1d13b19700b7949c5a639c764a077cbbdd4322ed505b449d3ca8edcb36"},
+    {file = "pydantic-1.10.11-cp37-cp37m-win_amd64.whl", hash = "sha256:7522a7666157aa22b812ce14c827574ddccc94f361237ca6ea8bb0d5c38f1629"},
+    {file = "pydantic-1.10.11-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:bc64eab9b19cd794a380179ac0e6752335e9555d214cfcb755820333c0784cb3"},
+    {file = "pydantic-1.10.11-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:8dc77064471780262b6a68fe67e013298d130414d5aaf9b562c33987dbd2cf4f"},
+    {file = "pydantic-1.10.11-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fe429898f2c9dd209bd0632a606bddc06f8bce081bbd03d1c775a45886e2c1cb"},
+    {file = "pydantic-1.10.11-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:192c608ad002a748e4a0bed2ddbcd98f9b56df50a7c24d9a931a8c5dd053bd3d"},
+    {file = "pydantic-1.10.11-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ef55392ec4bb5721f4ded1096241e4b7151ba6d50a50a80a2526c854f42e6a2f"},
+    {file = "pydantic-1.10.11-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:41e0bb6efe86281623abbeeb0be64eab740c865388ee934cd3e6a358784aca6e"},
+    {file = "pydantic-1.10.11-cp38-cp38-win_amd64.whl", hash = "sha256:265a60da42f9f27e0b1014eab8acd3e53bd0bad5c5b4884e98a55f8f596b2c19"},
+    {file = "pydantic-1.10.11-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:469adf96c8e2c2bbfa655fc7735a2a82f4c543d9fee97bd113a7fb509bf5e622"},
+    {file = "pydantic-1.10.11-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:e6cbfbd010b14c8a905a7b10f9fe090068d1744d46f9e0c021db28daeb8b6de1"},
+    {file = "pydantic-1.10.11-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:abade85268cc92dff86d6effcd917893130f0ff516f3d637f50dadc22ae93999"},
+    {file = "pydantic-1.10.11-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e9738b0f2e6c70f44ee0de53f2089d6002b10c33264abee07bdb5c7f03038303"},
+    {file = "pydantic-1.10.11-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:787cf23e5a0cde753f2eabac1b2e73ae3844eb873fd1f5bdbff3048d8dbb7604"},
+    {file = "pydantic-1.10.11-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:174899023337b9fc685ac8adaa7b047050616136ccd30e9070627c1aaab53a13"},
+    {file = "pydantic-1.10.11-cp39-cp39-win_amd64.whl", hash = "sha256:1954f8778489a04b245a1e7b8b22a9d3ea8ef49337285693cf6959e4b757535e"},
+    {file = "pydantic-1.10.11-py3-none-any.whl", hash = "sha256:008c5e266c8aada206d0627a011504e14268a62091450210eda7c07fabe6963e"},
+    {file = "pydantic-1.10.11.tar.gz", hash = "sha256:f66d479cf7eb331372c470614be6511eae96f1f120344c25f3f9bb59fb1b5528"},
 ]
 
 [package.dependencies]
 typing-extensions = ">=4.2.0"
 
 [package.extras]
 dotenv = ["python-dotenv (>=0.10.4)"]
@@ -2498,14 +2525,36 @@
     {file = "pyobjc_framework_Cocoa-9.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:b236bb965e41aeb2e215d4e98a5a230d4b63252c6d26e00924ea2e69540a59d6"},
 ]
 
 [package.dependencies]
 pyobjc-core = ">=9.2"
 
 [[package]]
+name = "pyobjc-framework-security"
+version = "9.2"
+description = "Wrappers for the framework Security on macOS"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "pyobjc-framework-Security-9.2.tar.gz", hash = "sha256:8d4f7a22db2fe666c7bff4a5825b49d2345e9a8d96ea085f1a614ad9a559b4e5"},
+    {file = "pyobjc_framework_Security-9.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:06137e1dd28af61f9966e1dfddba4ff7dc25d3d77f49f9af47bb4791492e58ce"},
+    {file = "pyobjc_framework_Security-9.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:ca272397da447897d73e1b72ae0acddadfefbb575e452b85028b2d7ae13b0fc7"},
+    {file = "pyobjc_framework_Security-9.2-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:f9cfb6c44cefe7d6456ddfdda569867254a271d8fef10500e86456a105e255b9"},
+    {file = "pyobjc_framework_Security-9.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:3d627e92688dfb31a0399f12283256717e5a1bd05b2abfd8b470621f955995a3"},
+    {file = "pyobjc_framework_Security-9.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0f9435986f7cf74d22a2920a5d85d922e24caa3b5b2911fb6d07c3b89f9973f9"},
+    {file = "pyobjc_framework_Security-9.2-cp38-cp38-macosx_11_0_universal2.whl", hash = "sha256:aa18fbb458edf04b0c34d13443a4665aeff4ae90ee644f008cd58146740f166d"},
+    {file = "pyobjc_framework_Security-9.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:8be7f51fc483532100853a570d62570f553fce5d7e101a572ad70198acfc9a8e"},
+]
+
+[package.dependencies]
+pyobjc-core = ">=9.2"
+pyobjc-framework-Cocoa = ">=9.2"
+
+[[package]]
 name = "pyobjc-framework-webkit"
 version = "9.2"
 description = "Wrappers for the framework WebKit on macOS"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -2552,22 +2601,22 @@
 ]
 
 [package.dependencies]
 pywin32 = {version = "*", markers = "platform_system == \"Windows\""}
 
 [[package]]
 name = "pytest"
-version = "7.3.2"
+version = "7.4.0"
 description = "pytest: simple powerful testing with Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pytest-7.3.2-py3-none-any.whl", hash = "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295"},
-    {file = "pytest-7.3.2.tar.gz", hash = "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"},
+    {file = "pytest-7.4.0-py3-none-any.whl", hash = "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32"},
+    {file = "pytest-7.4.0.tar.gz", hash = "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "sys_platform == \"win32\""}
 exceptiongroup = {version = ">=1.0.0rc8", markers = "python_version < \"3.11\""}
 iniconfig = "*"
 packaging = "*"
@@ -2792,36 +2841,38 @@
 files = [
     {file = "pytz-2023.3-py2.py3-none-any.whl", hash = "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"},
     {file = "pytz-2023.3.tar.gz", hash = "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588"},
 ]
 
 [[package]]
 name = "pywebview"
-version = "4.1"
-description = "Build GUI for your Python program with JavaScript, HTML, and CSS."
+version = "4.2.2"
+description = "Build GUI for your Python program with JavaScript, HTML, and CSS"
 category = "main"
 optional = false
-python-versions = "*"
+python-versions = ">=3.7"
 files = [
-    {file = "pywebview-4.1-py3-none-any.whl", hash = "sha256:d4945c3be285b1046f812032fff882cf640547b63be132016730ad5a11153304"},
-    {file = "pywebview-4.1.tar.gz", hash = "sha256:62efa24fff0b35fb8028556b6d44fc1c698a1deefa8df2c5557909af54679450"},
+    {file = "pywebview-4.2.2-py3-none-any.whl", hash = "sha256:1db26c0fcf9e856195467464b2a3e00189d231457189a102747d4a8694c974e4"},
+    {file = "pywebview-4.2.2.tar.gz", hash = "sha256:85be4215cd65ceacca5c7faef9d271e10bfe3ca25d2498c1c6d2e59a4d56e86c"},
 ]
 
 [package.dependencies]
 bottle = "*"
 proxy-tools = "*"
 pyobjc-core = {version = "*", markers = "sys_platform == \"darwin\""}
 pyobjc-framework-Cocoa = {version = "*", markers = "sys_platform == \"darwin\""}
+pyobjc-framework-security = {version = "*", markers = "sys_platform == \"darwin\""}
 pyobjc-framework-WebKit = {version = "*", markers = "sys_platform == \"darwin\""}
 pythonnet = {version = "*", markers = "sys_platform == \"win32\""}
 QtPy = {version = "*", markers = "sys_platform == \"openbsd6\""}
+typing-extensions = "*"
 
 [package.extras]
 cef = ["cefpython3"]
-gtk = ["PyGObject"]
+gtk = ["PyGObject", "PyGObject-stubs"]
 pyside2 = ["PySide2", "QtPy"]
 pyside6 = ["PySide6", "QtPy"]
 qt = ["PyQt5", "QtPy", "pyqtwebengine"]
 
 [[package]]
 name = "pywin32"
 version = "306"
@@ -2844,22 +2895,22 @@
     {file = "pywin32-306-cp38-cp38-win_amd64.whl", hash = "sha256:e8ac1ae3601bee6ca9f7cb4b5363bf1c0badb935ef243c4733ff9a393b1690c0"},
     {file = "pywin32-306-cp39-cp39-win32.whl", hash = "sha256:e25fd5b485b55ac9c057f67d94bc203f3f6595078d1fb3b458c9c28b7153a802"},
     {file = "pywin32-306-cp39-cp39-win_amd64.whl", hash = "sha256:39b61c15272833b5c329a2989999dcae836b1eed650252ab1b7bfbe1d59f30f4"},
 ]
 
 [[package]]
 name = "pywin32-ctypes"
-version = "0.2.1"
+version = "0.2.2"
 description = "A (partial) reimplementation of pywin32 using ctypes/cffi"
 category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "pywin32-ctypes-0.2.1.tar.gz", hash = "sha256:934a2def1e5cbc472b2b6bf80680c0f03cd87df65dfd58bfd1846969de095b03"},
-    {file = "pywin32_ctypes-0.2.1-py3-none-any.whl", hash = "sha256:b9a53ef754c894a525469933ab2a447c74ec1ea6b9d2ef446f40ec50d3dcec9f"},
+    {file = "pywin32-ctypes-0.2.2.tar.gz", hash = "sha256:3426e063bdd5fd4df74a14fa3cf80a0b42845a87e1d1e81f6549f9daec593a60"},
+    {file = "pywin32_ctypes-0.2.2-py3-none-any.whl", hash = "sha256:bf490a1a709baf35d688fe0ecf980ed4de11d2b3e37b51e5442587a75d9957e7"},
 ]
 
 [[package]]
 name = "pyyaml"
 version = "6.0"
 description = "YAML parser and emitter for Python"
 category = "main"
@@ -2924,22 +2975,22 @@
 packaging = "*"
 
 [package.extras]
 test = ["pytest (>=6,!=7.0.0,!=7.0.1)", "pytest-cov (>=3.0.0)", "pytest-qt"]
 
 [[package]]
 name = "readme-renderer"
-version = "37.3"
+version = "40.0"
 description = "readme_renderer is a library for rendering \"readme\" descriptions for Warehouse"
 category = "dev"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "readme_renderer-37.3-py3-none-any.whl", hash = "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"},
-    {file = "readme_renderer-37.3.tar.gz", hash = "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273"},
+    {file = "readme_renderer-40.0-py3-none-any.whl", hash = "sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a"},
+    {file = "readme_renderer-40.0.tar.gz", hash = "sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4"},
 ]
 
 [package.dependencies]
 bleach = ">=2.1.0"
 docutils = ">=0.13.1"
 Pygments = ">=2.5.1"
 
@@ -2980,14 +3031,29 @@
     {file = "requests_toolbelt-1.0.0-py2.py3-none-any.whl", hash = "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"},
 ]
 
 [package.dependencies]
 requests = ">=2.0.1,<3.0.0"
 
 [[package]]
+name = "retrying"
+version = "1.3.4"
+description = "Retrying"
+category = "main"
+optional = false
+python-versions = "*"
+files = [
+    {file = "retrying-1.3.4-py3-none-any.whl", hash = "sha256:8cc4d43cb8e1125e0ff3344e9de678fefd85db3b750b81b2240dc0183af37b35"},
+    {file = "retrying-1.3.4.tar.gz", hash = "sha256:345da8c5765bd982b1d1915deb9102fd3d1f7ad16bd84a9700b85f64d24e8f3e"},
+]
+
+[package.dependencies]
+six = ">=1.7.0"
+
+[[package]]
 name = "rfc3986"
 version = "1.5.0"
 description = "Validating URI References per RFC 3986"
 category = "main"
 optional = false
 python-versions = "*"
 files = [
@@ -3345,61 +3411,61 @@
 
 [package.extras]
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sqlalchemy"
-version = "2.0.16"
+version = "2.0.17"
 description = "Database Abstraction Library"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:7641f6ed2682de84d77c4894cf2e43700f3cf7a729361d7f9cac98febf3d8614"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8d3cbdb2f07fb0e4b897dc1df39166735e194fb946f28f26f4c9f9801c8b24f7"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a08a791c75d6154d46914d1e23bd81d9455f2950ec1de81f2723848c593d2c8b"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:91eb8f89fcce8f709f8a4d65d265bc48a80264ee14c7c9e955f3222f19b4b39c"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:fc1dae11bd5167f9eb53b3ccad24a79813004612141e76de21cf4c028dc30b34"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b2801f85c5c0293aa710f8aa5262c707a83c1c203962ae5a22b4d9095e71aa9d"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-win32.whl", hash = "sha256:c5e333b81fe10d14efebd4e9429b7bb865ed9463ca8bef07a7136dfa1fd4a37b"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-win_amd64.whl", hash = "sha256:f387b496a4c9474d8580195bb2660264a3f295a04d3a9d00f4fa15e9e597427e"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:7be04dbe3470fe8dd332fdb48c979887c381ef6c635eddf2dec43d2766111be4"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f2938edc512dd1fa48653e14c1655ab46144d4450f0e6b33da7acd8ba77fbfd7"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a5a2856e12cf5f54301ddf043bcbf0552561d61555e1bcf348b63f42b8e1eec2"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:90d320fde566b864adbc19abb40ecb80f4e25d6f084639969bb972d5cca16858"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:6e85e315725807c127ad8ba3d628fdb861cf9ebfb0e10c39a97c01e257cdd71b"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:63ea36c08792a7a8a08958bc806ecff6b491386feeaf14607c3d9d2d9325e67f"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-win32.whl", hash = "sha256:bdaf89dd82f4a0e1b8b5ffc9cdc0c9551be6175f7eee5af6a838e92ba2e57100"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-win_amd64.whl", hash = "sha256:5a934eff1a2882137be3384826f997db8441d43b61fda3094923e69fffe474be"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:fbcc51fdbc89fafe4f4fe66f59372a8be88ded04de34ef438ab04f980beb12d4"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ff6496ad5e9dc8baeb93a151cc2f599d01e5f8928a2aaf0b09a06428fdbaf553"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8d6ef848e5afcd1bda3e9a843751f845c0ca888b61e669237680e913d84ec206"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:3ef876615ff4b53e2033022195830ec4941a6e21068611f8d77de60203b90a98"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:8544c6e62eacb77d5106e2055ef10f2407fc0dbd547e879f8745b2032eefd2bc"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-win32.whl", hash = "sha256:2f3b6c31b915159b96b68372212fa77f69230b0a32acab40cf539d2823954f5a"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-win_amd64.whl", hash = "sha256:d0c96592f54edd571e00ba6b1ed5df8263328ca1da9e78088c0ebc93c2e6562c"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:a2e9f50a906d0b81292576a9fb458f8cace904c81a67088f4a2ca9ff2856f55d"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:dc97238fa44be86971270943a0c21c19ce18b8d1596919048e57912e8abc02cc"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0db6734cb5644c55d0262a813b764c6e2cda1e66e939a488b3d6298cdc7344c2"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:131f0c894c6572cb1bdcf97c92d999d3128c4ff1ca13061296057072f61afe13"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:f662cf69484c59f8a3435902c40dfc34d86050bdb15e23d437074ce9f153306b"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:b72f4e4def50414164a1d899f2ce4e782a029fad0ed5585981d1611e8ae29a74"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-win32.whl", hash = "sha256:0e4645b260cfe375a0603aa117f0a47680864cf37833129da870919e88b08d8f"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-win_amd64.whl", hash = "sha256:f409f35a0330ab0cb18ece736b86d8b8233c64f4461fcb10993f67afc0ac7e5a"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:e19546924f0cf2ec930d1faf318b7365e5827276410a513340f31a2b423e96a4"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:ce1fc3f64fd42d5f763d6b83651471f32920338a1ba107a3186211474861af57"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8e2569dac4e3cb85365b91ab569d06a221e0e17e65ce59949d00c3958946282b"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:61f2035dea56ff1a429077e481496f813378beb02b823d2e3e7eb05bc1a7a8ca"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:81d867c1be5abd49f7e547c108391f371a9d980ba7ec34666c50d683f782b754"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:2de1477af7f48c633b8ecb88245aedd811dca88e88aee9e9d787b388abe74c44"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-win32.whl", hash = "sha256:5e8522b49e0e640287308b68f71cc338446bbe1c226c8f81743baa91b0246e92"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-win_amd64.whl", hash = "sha256:43e69c8c1cea0188b7094e22fb93ae1a1890aac748628b7e925024a206f75368"},
-    {file = "SQLAlchemy-2.0.16-py3-none-any.whl", hash = "sha256:53081c6fce0d49bb36d05f12dc87e008c9b0df58a163b792c5fc4ac638925f98"},
-    {file = "SQLAlchemy-2.0.16.tar.gz", hash = "sha256:1e2caba78e7d1f5003e88817b7a1754d4e58f4a8f956dc423bf8e304c568ab09"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:04383f1e3452f6739084184e427e9d5cb4e68ddc765d52157bf5ef30d5eca14f"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:724355973297bbe547f3eb98b46ade65a67a3d5a6303f17ab59a2dc6fb938943"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cf07ff9920cb3ca9d73525dfd4f36ddf9e1a83734ea8b4f724edfd9a2c6e82d9"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f2f389f77c68dc22cb51f026619291c4a38aeb4b7ecb5f998fd145b2d81ca513"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ba03518e64d86f000dc24ab3d3a1aa876bcbaa8aa15662ac2df5e81537fa3394"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:218fb20c01e95004f50a3062bf4c447dcb360cab8274232f31947e254f118298"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-win32.whl", hash = "sha256:b47be4c6281a86670ea5cfbbbe6c3a65366a8742f5bc8b986f790533c60b5ddb"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-win_amd64.whl", hash = "sha256:74ddcafb6488f382854a7da851c404c394be3729bb3d91b02ad86c5458140eff"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:51736cfb607cf4e8fafb693906f9bc4e5ee55be0b096d44bd7f20cd8489b8571"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8741d3d401383e54b2aada37cbd10f55c5d444b360eae3a82f74a2be568a7710"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ead58cae2a089eee1b0569060999cb5f2b2462109498a0937cc230a7556945a1"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5f40e3a7d0a464f1c8593f2991e5520b2f5b26da24e88000bbd4423f86103d4f"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:21583808d37f126a647652c90332ac1d3a102edf3c94bcc3319edcc0ea2300cc"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:f593170fc09c5abb1205a738290b39532f7380094dc151805009a07ae0e85330"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-win32.whl", hash = "sha256:b0eaf82cc844f6b46defe15ad243ea00d1e39ed3859df61130c263dc7204da6e"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-win_amd64.whl", hash = "sha256:1822620c89779b85f7c23d535c8e04b79c517739ae07aaed48c81e591ed5498e"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:2269b1f9b8be47e52b70936069a25a3771eff53367aa5cc59bb94f28a6412e13"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:48111d56afea5699bab72c38ec95561796b81befff9e13d1dd5ce251ab25f51d"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:28da17059ecde53e2d10ba813d38db942b9f6344360b2958b25872d5cb729d35"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:48b40dc2895841ea89d89df9eb3ac69e2950a659db20a369acf4259f68e6dc1f"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:7f31d4e7ca1dd8ca5a27fd5eaa0f9e2732fe769ff7dd35bf7bba179597e4df07"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-win32.whl", hash = "sha256:7830e01b02d440c27f2a5be68296e74ccb55e6a5b5962ffafd360b98930b2e5e"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-win_amd64.whl", hash = "sha256:234678ed6576531b8e4be255b980f20368bf07241a2e67b84e6b0fe679edb9c4"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2c6ff5767d954f6091113fedcaaf49cdec2197ae4c5301fe83d5ae4393c82f33"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:aa995b21f853864996e4056d9fde479bcecf8b7bff4beb3555eebbbba815f35d"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:125f9f7e62ddf8b590c069729080ffe18b68a20d9882eb0947f72e06274601d7"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b114a16bc03dfe20b625062e456affd7b9938286e05a3f904a025b9aacc29dd4"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:cf175d26f6787cce30fe6c04303ca0aeeb0ad40eeb22e3391f24b32ec432a1e1"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:e2d5c3596254cf1a96474b98e7ce20041c74c008b0f101c1cb4f8261cb77c6d3"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-win32.whl", hash = "sha256:513411d73503a6fc5804f01fae3b3d44f267c1b3a06cfeac02e9286a7330e857"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-win_amd64.whl", hash = "sha256:40a3dc52b2b16f08b5c16b9ee7646329e4b3411e9280e5e8d57b19eaa51cbef4"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:e3189432db2f5753b4fde1aa90a61c69976f4e7e31d1cf4611bfe3514ed07478"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:6150560fcffc6aee5ec9a97419ac768c7a9f56baf7a7eb59cb4b1b6a4d463ad9"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:910d45bf3673f0e4ef13858674bd23cfdafdc8368b45b948bf511797dbbb401d"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d0aeb3afaa19f187a70fa592fbe3c20a056b57662691fd3abf60f016aa5c1848"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:36a87e26fe8fa8c466fae461a8fcb780d0a1cbf8206900759fc6fe874475a3ce"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:e3a6b2788f193756076061626679c5c5a6d600ddf8324f986bc72004c3e9d92e"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-win32.whl", hash = "sha256:af7e2ba75bf84b64adb331918188dda634689a2abb151bc1a583e488363fd2f8"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-win_amd64.whl", hash = "sha256:394ac3adf3676fad76d4b8fcecddf747627f17f0738dc94bac15f303d05b03d4"},
+    {file = "SQLAlchemy-2.0.17-py3-none-any.whl", hash = "sha256:cc9c2630c423ac4973492821b2969f5fe99d9736f3025da670095668fbfcd4d5"},
+    {file = "SQLAlchemy-2.0.17.tar.gz", hash = "sha256:e186e9e95fb5d993b075c33fe4f38a22105f7ce11cecb5c17b5618181e356702"},
 ]
 
 [package.dependencies]
 greenlet = {version = "!=0.4.17", markers = "platform_machine == \"aarch64\" or platform_machine == \"ppc64le\" or platform_machine == \"x86_64\" or platform_machine == \"amd64\" or platform_machine == \"AMD64\" or platform_machine == \"win32\" or platform_machine == \"WIN32\""}
 typing-extensions = ">=4.2.0"
 
 [package.extras]
@@ -3482,22 +3548,22 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tox"
-version = "4.6.2"
+version = "4.6.3"
 description = "tox is a generic virtualenv management and test command line tool"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "tox-4.6.2-py3-none-any.whl", hash = "sha256:52241851a7b0cd7de07d6ef067a13b092d2a4f82fe9048efb2444aed1708d713"},
-    {file = "tox-4.6.2.tar.gz", hash = "sha256:58c7c2acce2f3d44cd1b359349557162336288ecf19ef53ccda89c9cee0ad9c4"},
+    {file = "tox-4.6.3-py3-none-any.whl", hash = "sha256:2946a0bb38924c3a9f9575c7fb4ca1f4c11a7c69c61592f176778892155cb50c"},
+    {file = "tox-4.6.3.tar.gz", hash = "sha256:9e2c5091a117d03b583c57c4c40aecd068099c17d40520e7b165e85c19334534"},
 ]
 
 [package.dependencies]
 cachetools = ">=5.3.1"
 chardet = ">=5.1"
 colorama = ">=0.4.6"
 filelock = ">=3.12.2"
@@ -3533,22 +3599,22 @@
 requests-toolbelt = ">=0.8.0,<0.9.0 || >0.9.0"
 rfc3986 = ">=1.4.0"
 rich = ">=12.0.0"
 urllib3 = ">=1.26.0"
 
 [[package]]
 name = "typing-extensions"
-version = "4.6.3"
+version = "4.7.1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "typing_extensions-4.6.3-py3-none-any.whl", hash = "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26"},
-    {file = "typing_extensions-4.6.3.tar.gz", hash = "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"},
+    {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
+    {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 
 [[package]]
 name = "tzdata"
 version = "2023.3"
 description = "Provider of IANA time zone data"
 category = "main"
@@ -3762,8 +3828,8 @@
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = ">=3.8, <3.11"
-content-hash = "e2f8066e407a360c95ef8f8091de8a5fd822ee68e39d62e689abf9962af04f59"
+content-hash = "836ee2c76be8bd44c23a9a94487321beb7546e57c654f8d5de82ed17d1be1978"
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 [build-system]
 requires = ["poetry-core>=1.0.0,<1.3.0", "setuptools>=65.0"]
 build-backend = "poetry.core.masonry.api"
 
-# The following lines were added to enforce the poetry version needed for the project.
-# It will be read by the setup_environment.py script to install this version.
 [build-system-requirements]
-build-system-version = "1.4.2"
+build-system-version = "1.5.2"
 
 [tool.poetry]
 name = "{{cookiecutter.__pkg_name}}"
 version = "{{cookiecutter.__version}}"
 description = "{{cookiecutter.__short_description}}"
 license = "Proprietary"
 authors = ["ANSYS, Inc. <solution-applications.maintainers@ansys.com>"]
@@ -32,72 +30,73 @@
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [[tool.poetry.source]]
 name = "solutions-private-pypi"
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple/"
-default = false
-secondary = true
+priority = "supplemental"
 
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
+
+# Main dependencies
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 ansys-dash-treeview = {version = "0.0.1.dev0", source = "solutions-private-pypi"}
-ansys-optislang-core = "^0.3.0"
-ansys-saf-glow = {version = "0.3.dev4", source = "solutions-private-pypi"}
+ansys-saf-glow = {version = "0.3.dev4", source = "solutions-private-pypi" }
 ansys-saf-portal = {version = "0.2.0", source = "solutions-private-pypi"}
-ansys-solutions-dash-lib = {version = "^0.3.0", source = "solutions-private-pypi"}
-ansys-solutions-products-ecosystem = {version = "^0.1.dev0", source = "solutions-private-pypi"}
-ansys-solutions-optislang-parser = {version = "^0.1.dev6", source = "solutions-private-pypi"}
-ansys-solutions-optislang-frontend-components = {version = "^0.1.dev3", source = "solutions-private-pypi"}
-optislang-dash-lib = {version = "^0.2.1", source = "solutions-private-pypi"}
-dash = "^2.6"
-dash_bootstrap_components = "^1.2"
-dash-extensions = "^0.1"
-dash-iconify = "^0.1"
-dash-uploader = "^0.6"
-pandas = "^2.0.0"
+ansys-solutions-dash-lib = {version = "^0.4", source = "solutions-private-pypi"}
+{% if cookiecutter.with_dash_ui == "yes" %}
+dash = {version = "^2.6"}
+dash_bootstrap_components = {version = "^1.2"}
+dash-extensions = {version = "^0.1"}
+dash-iconify = {version = "^0.1"}
+dash-uploader = {version = "^0.6"}
+{% endif %}
 
+# Optional documentation dependencies
 [tool.poetry.group.doc]
 optional = true
 [tool.poetry.group.doc.dependencies]
 ansys-sphinx-theme = {version = "^0.8.0"}
 numpydoc = {version = "^1.4.0"}
 sphinx = {version = "5.1.0"}
 sphinx-copybutton = {version = "^0.5.1"}
 sphinx_design = {version = "^0.3.0"}
 sphinx_code_tabs = {version = "^0.5.3"}
 sphinx-gallery = {version = "^0.11.1"}
 sphinx_mdinclude= {version = "^0.5.3"}
 sphinx-tabs = {version = ">=1.2.1,<3.5.0"}
-toml = {version = "^0.10.2"} # Needed by conf.py
-tox = {version = "^4.4.11"}
+toml = {version = "^0.10.0"} # Needed by conf.py
 
+# Optional testing dependencies
 [tool.poetry.group.tests]
 optional = true
 [tool.poetry.group.tests.dependencies]
 coverage = {version = "^6.4.1"}
 filelock = {version = "^3.8.0"}
 mock = {version = "^4.0.3"}
 pytest = {version = "^7.1.2"}
 pytest-cov = {version = "^3.0.0"}
 pytest-dependency = {version = "^0.5.1"}
 pytest-flakes = {version = "^4.0.5"}
 pytest-pep8 = {version = "*"}
 pytest-pythonpath = {version = "*"}
 pytest-xdist = {version = "^3.0.2"}
 pytest-mock = {version = "*"}
-tox = {version = "^4.4.11"}
+tox = {version = "^4.4.0"}
 
+# Optional build requirements
 [tool.poetry.group.build]
 optional = true
 [tool.poetry.group.build.dependencies]
 build = {version = "^0.8.0"}
 twine = {version = "^4.0.1"}
-tox = {version = "^4.4.11"}
 
 [tool.poetry.plugins."console_scripts"]
 {{ cookiecutter.__solution_name_slug }}_main = "ansys.solutions.{{ cookiecutter.__solution_name_slug }}.main:main"
 
 [tool.black]
 line-length = {{ cookiecutter.__max_linelength }}
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
-# CAPTURED v0.4.0 from:
+# CAPTURED v0.5.1 on 7/4/23 from:
 # https://github.com/Solution-Applications/common-files/blob/v0.4.0/setup-environment/setup_environment.py
 
 """
 A Python script to automate the setup of the Python ecosystem of a project.
 
 Prerequisites
 -------------
 
-1. This script needs to be executed at project's root.
+1. The following packages are required:
+    * packaging
+    * toml
 
-2. Currently, this code only supports:
+2. This script needs to be executed at project's root.
+
+3. Currently, this code only supports:
     * ``windows`` as operating system
-    * ``poetry`` and ``flit`` as dependency management systems
+    * ``poetry`` as dependency management system
     * projects without dependency management systems
     * ``poetry`` 1.2 to latest.
 
-3. The following project structure is expected for projects without a dependency management system:
+4. The following project structure is expected for projects without a dependency management system:
     project-name
     ├──requirements/                    # Folder containing the optional group of dependencies.
     │  ├── requirements_doc.txt         # Requirements file associated to the documentation group.
     │  ├── requirements_tests.txt       # Requirements file associated to the tests group.
     │  ├── requirements_style.txt       # Requirements file associated to the style group.
     │  └── requirements_build.txt       # Requirements file associated to the build group.
 
-4. The following project structure is expected for projects with a dependency management system:
+5. The following project structure is expected for projects with a dependency management system:
     project-name
     └── pyproject.toml                  # Configuration of the build system.
 
 The following packages are needed on top of the standard Python configuration: ``toml`` and ``packaging``.
 
 Usage
 -----
@@ -111,39 +115,52 @@
 import re
 import shutil
 import subprocess
 import sys
 import textwrap
 import time
 
-from packaging.markers import Marker
-import toml
+try:
+    from packaging.markers import Marker
+except:
+    sys.exit("Process stopped. The `packaging` library is missing. Install with: `pip install packaging`.")
+try:
+    import toml
+except:
+    sys.exit("Process stopped. The `toml` library is missing. Install with: `pip install toml`.")
 
 # =================================================== [Variables] =================================================== #
 
-SUPPORTED_DEPENDENCY_MANAGERS = {
-    "poetry": {
+DEPENDENCY_MANAGER_PATHS = {
+    "win32": {
+        "poetry_python_executable": Path(".poetry").absolute() / ".venv" / "Scripts" / "python.exe",
+        "build_sys_exec": Path(".poetry").absolute() / ".venv" / "Scripts" / "poetry.exe",
+        "dep_bin_venv_path": Path(".venv").absolute() / "Scripts" / "poetry.exe",
+        "python_executable": Path(".venv").absolute() / "Scripts" / "python.exe",
+        "shell": True,
+    },
+    "linux": {
+        "poetry_python_executable": Path(".poetry").absolute() / ".venv" / "bin" / "python",
+        "build_sys_exec": Path(".poetry").absolute() / ".venv" / "bin" / "poetry",
+        "dep_bin_venv_path": Path(".venv").absolute() / "bin" / "poetry",
+        "python_executable": Path(".venv").absolute() / "bin" / "python",
+        "shell": False,
+    },
+    "common": {
         "configuration_file": "pyproject.toml",
         "build_backend": "poetry.core.masonry.api",
         "required_venv_name": ".venv",
         "lock_file": "poetry.lock",
-        "cache_folder": ".poetry\.cache",
-        "build_system_venv": ".poetry\.venv",
-    },
-    "flit": {
-        "configuration_file": "pyproject.toml",
-        "build_backend": "flit_core.buildapi",
-        "required_venv_name": None,
-        "lock_file": None,
-        "cache_folder": ".flit/.cache",
-        "build_system_venv": ".flit/.venv",
+        "build_system_venv": Path(".poetry") / ".venv",
+        "cache_folder": Path(".poetry").absolute() / ".cache",
     },
 }
 
-STANDARD_OPTIONAL_DEPENDENCY_GROUPS = ["doc", "tests", "build", "style", "external"]
+configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
+STANDARD_OPTIONAL_DEPENDENCY_GROUPS = [group for group in configuration["tool"]["poetry"]["group"].keys()]
 
 # =================================================== [Functions] =================================================== #
 
 # Console prints ----------------------------------------------------------------------------------------------------
 
 
 def print_main_header(text: str, max_length: int = 100) -> None:
@@ -196,134 +213,108 @@
     for dependency_group in STANDARD_OPTIONAL_DEPENDENCY_GROUPS:
         print_input_value(
             f"{dependency_group} dependencies",
             "yes" if dependency_group in args.dependencies else "no",
             separator=":",
             separator_position=37,
         )
-    if args.build_system and args.extra_dependencies:
+    if args.extra_dependencies:
         for dependency_group in args.extra_dependencies:
             print_input_value(
                 f"{dependency_group} dependencies",
                 "yes",
                 separator=":",
                 separator_position=37,
             )
-    print(f"Dependency management system         : {args.build_system}")
+    print(f"Dependency management system         : poetry")
     print(f"Dependency management system version : {args.build_system_version}")
     print(f"Credentials management               : {args.credentials_management_method}")
     print()
 
 
 # Checks ------------------------------------------------------------------------------------------------------------
 
 
-def check_dependency_management_system() -> str:
-    """Check if a dependency management system is available at project root."""
-
-    for dms_name in SUPPORTED_DEPENDENCY_MANAGERS.keys():
-        if os.path.exists(SUPPORTED_DEPENDENCY_MANAGERS[dms_name]["configuration_file"]):
-            dms_configuration = toml.load(SUPPORTED_DEPENDENCY_MANAGERS[dms_name]["configuration_file"])
-            if (
-                dms_configuration["build-system"]["build-backend"]
-                == SUPPORTED_DEPENDENCY_MANAGERS[dms_name]["build_backend"]
-            ):
-                return dms_name
-
-
 def check_virtual_environment_name(args: object) -> None:
     """Check if the virtual environment name is consistent with the build system expectations."""
 
-    if args.build_system:
-        if SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["required_venv_name"]:
-            if SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["required_venv_name"] != args.venv_name:
-                old_name = args.venv_name
-                args.venv_name = SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["required_venv_name"]
-                print(
-                    f"Warning: {args.build_system} expects the name of the virtual environment name to be"
-                    f" {args.venv_name}. {old_name} is replaced by {args.venv_name}."
-                )
+    if DEPENDENCY_MANAGER_PATHS["common"]["required_venv_name"] != args.venv_name:
+        old_name = args.venv_name
+        args.venv_name = DEPENDENCY_MANAGER_PATHS["common"]["required_venv_name"]
+        print(
+            f"Warning: poetry expects the name of the virtual environment name to be"
+            f" {args.venv_name}. {old_name} is replaced by {args.venv_name}."
+        )
 
 
 def check_python_version(args: object) -> None:
     """
     Check if the version of the current Python interpreter is consistent with the python version specifications
     from the build system.
     """
 
-    if args.build_system:
-        # Initialize lower/upper versions
-        lower_version, upper_version, lower_bound_symbol, upper_bound_symbol = None, None, None, None
-        lower_specification, upper_specification, single_specification = None, None, None
-        # Read TOML
-        configuration = toml.load(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["configuration_file"])
-        # Read Python version constraint
-        python_compatibility = ""
-        if args.build_system == "poetry":
-            python_compatibility = configuration["tool"][args.build_system]["dependencies"]["python"].replace(" ", "")
-        elif args.build_system == "flit":
-            python_compatibility = configuration["project"]["requires-python"].replace(" ", "")
-        # Split lower/upper version constraint
-        if "," in python_compatibility:
-            lower_specification, upper_specification = (
-                python_compatibility.split(",")[0],
-                python_compatibility.split(",")[1],
-            )
+    # Initialize lower/upper versions
+    lower_version, upper_version, lower_bound_symbol, upper_bound_symbol = None, None, None, None
+    lower_specification, upper_specification, single_specification = None, None, None
+    # Read TOML
+    configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
+    # Read Python version constraint
+    python_compatibility = configuration["tool"]["poetry"]["dependencies"]["python"].replace(" ", "")
+    # Split lower/upper version constraint
+    if "," in python_compatibility:
+        lower_specification, upper_specification = (
+            python_compatibility.split(",")[0],
+            python_compatibility.split(",")[1],
+        )
+    else:
+        if python_compatibility.startswith(">"):
+            lower_specification, upper_specification = python_compatibility, None
+        elif python_compatibility.startswith("<"):
+            lower_specification, upper_specification = None, python_compatibility
         else:
-            if python_compatibility.startswith(">"):
-                lower_specification, upper_specification = python_compatibility, None
-            elif python_compatibility.startswith("<"):
-                lower_specification, upper_specification = None, python_compatibility
-            else:
-                single_specification = python_compatibility
-        # Process lower constraint
-        if lower_specification:
-            lower_version = get_version_from_python_specification(lower_specification)
-            lower_bound_symbol = get_sign_from_python_specification(lower_specification)
-            marker = Marker(f"python_full_version {lower_bound_symbol} '{lower_version}'")
-            if not marker.evaluate():
-                raise Exception(f"Python version must be {lower_bound_symbol} {lower_version}.")
-        # Process upper constraint
-        if upper_specification:
-            upper_version = get_version_from_python_specification(upper_specification)
-            upper_bound_symbol = get_sign_from_python_specification(upper_specification)
-            marker = Marker(f"python_full_version {upper_bound_symbol} '{upper_version}'")
-            if not marker.evaluate():
-                raise Exception(f"Python version must be {upper_bound_symbol} {upper_version}.")
-        # Process single
-        if single_specification:
-            version = get_version_from_python_specification(single_specification)
-            sign = get_sign_from_python_specification(single_specification)
-            if sign != "==":
-                raise Exception("Unable to interpret python version specification.")
-            marker = Marker(f"python_full_version {sign} '{version}'")
-            if not marker.evaluate():
-                raise Exception(f"Python version must be equal to {version}.")
+            single_specification = python_compatibility
+    # Process lower constraint
+    if lower_specification:
+        lower_version = get_version_from_python_specification(lower_specification)
+        lower_bound_symbol = get_sign_from_python_specification(lower_specification)
+        marker = Marker(f"python_full_version {lower_bound_symbol} '{lower_version}'")
+        if not marker.evaluate():
+            raise Exception(f"Python version must be {lower_bound_symbol} {lower_version}.")
+    # Process upper constraint
+    if upper_specification:
+        upper_version = get_version_from_python_specification(upper_specification)
+        upper_bound_symbol = get_sign_from_python_specification(upper_specification)
+        marker = Marker(f"python_full_version {upper_bound_symbol} '{upper_version}'")
+        if not marker.evaluate():
+            raise Exception(f"Python version must be {upper_bound_symbol} {upper_version}.")
+    # Process single
+    if single_specification:
+        version = get_version_from_python_specification(single_specification)
+        sign = get_sign_from_python_specification(single_specification)
+        if sign != "==":
+            raise Exception("Unable to interpret python version specification.")
+        marker = Marker(f"python_full_version {sign} '{version}'")
+        if not marker.evaluate():
+            raise Exception(f"Python version must be equal to {version}.")
 
 
 def check_existing_install(args: object) -> str:
     """Check if an install exists already."""
 
     return os.path.isdir(args.venv_name)
 
 
 def check_inputs(args: object) -> None:
     """Check inputs consistency."""
-
-    # Check platform
-    if sys.platform != "win32":
-        raise Exception("Only Windows operating systems are supported.")
     # Rework dependencies argument if all option is selected
     if "all" in args.dependencies:
         args.install_all = True
         args.dependencies = STANDARD_OPTIONAL_DEPENDENCY_GROUPS + ["run"]
     else:
         args.install_all = False
-    # Check if a dependency management system is declared
-    args.build_system = check_dependency_management_system()
     # Check virtual environment name
     check_virtual_environment_name(args)
     # Check python version
     check_python_version(args)
     # Check if an install already exists
     args.has_install = check_existing_install(args)
 
@@ -363,29 +354,30 @@
 def get_python_version() -> None:
     """Get Python version."""
 
     return f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
 
 
 def set_pip_command(
-    package_name: str,
     package_version: str = "*",
     method: str = "install",
     pypi_url: str = "https://pypi.org/simple",
     private_pypi_token_name: str = "",
     no_deps: bool = False,
     python_executable: str = sys.executable,
 ) -> str:
     """Make pip command."""
 
-    # Set command
-    command = f"{python_executable} -m pip {method} {package_name}"
+    package_name = "poetry"
+
     # Add package version if specified
     if package_version != "*":
-        command += f"=={package_version}"
+        package_name += f"=={package_version}"
+    # Set command
+    command = [python_executable, "-m", "pip", method, package_name]
     # Add part related to private PyPI source
     if pypi_url != "https://pypi.org/simple":
         # Check if token is available
         if private_pypi_token_name is None:
             raise Exception(f"No token specified for private PyPI server {pypi_url}.")
         # Check if the environment variable associated to the private PyPI token exists
         private_pypi_token = os.getenv(private_pypi_token_name)
@@ -399,29 +391,26 @@
     if no_deps:
         command += " --no-deps"
 
     return command
 
 
 def get_python_package(
-    package_name: str,
     package_version: str = "*",
     method: str = "install",
     pypi_url: str = "https://pypi.org/simple",
     private_pypi_token_name: str = "",
     no_deps: bool = False,
     python_executable: str = sys.executable,
 ) -> None:
     """
     Install or download a python package using PIP.
 
     Parameters
     ----------
-    package_name : str
-        Name of the package.
     package_version : str
         Version of the package.
     method : str
         Get method: ``download`` or ``install``
     pypi_url : str
         URL of the PyPI server.
     private_pypi_token_name : str
@@ -432,73 +421,78 @@
     Returns
     -------
     None
     """
 
     # Set pip command
     command = set_pip_command(
-        package_name=package_name,
         package_version=package_version,
         method=method,
         pypi_url=pypi_url,
         private_pypi_token_name=private_pypi_token_name,
         no_deps=no_deps,
         python_executable=python_executable,
     )
     # Run pip command
-    process = subprocess.run(command.split(), check=False, shell=True, capture_output=True, text=True)
+    process = subprocess.run(
+        command, check=False, shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"], capture_output=True, text=True
+    )
     if process.returncode != 0:
         print(process.stdout)
         print(process.stderr)
         raise Exception("Command failed with error.")
 
 
 def get_python_package_versions(
-    package_name: str,
     pypi_url: str = "https://pypi.org/simple",
     private_pypi_token_name: str = "",
     python_executable: str = sys.executable,
 ) -> None:
     """Get available versions of a package."""
 
     # Set pip command
     command = set_pip_command(
-        package_name=package_name,
         package_version="x",
         pypi_url=pypi_url,
         private_pypi_token_name=private_pypi_token_name,
         python_executable=python_executable,
     )
     # Run pip command
-    process = subprocess.run(command.split(), check=False, shell=True, capture_output=True, text=True)
+    process = subprocess.run(
+        command, check=False, shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"], capture_output=True, text=True
+    )
     if process.returncode == 0:
         print(command)
         raise Exception("This command should have failed. There is something wrong.")
     else:
         return extract_substring_between_markers(process.stderr, "(from versions:", ")").replace(" ", "").split(",")
 
 
 def upgrade_pip(python_executable: str = sys.executable) -> None:
     """Upgrade to latest PIP version in the virtual environment."""
 
     print("Upgrade to latest pip version")
     subprocess.run(
         [python_executable, "-m", "pip", "install", "--upgrade", "pip"],
         check=True,
-        shell=True,
+        shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
     )
     print()
 
 
 def create_virtual_environment(args: object, venv: str = ".venv") -> None:
     """Create a virtual environment."""
 
     print("Create virtual environment")
     if not args.has_install or args.force_clear or args.force_clear_all:
-        subprocess.run([sys.executable, "-m", "venv", venv], check=True, shell=True)
+        if sys.platform == "linux":
+            subprocess.run(["sudo", "apt-get", "install", "-y", "python3-venv"], check=True)
+        subprocess.run(
+            [sys.executable, "-m", "venv", venv], check=True, shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"]
+        )
     else:
         print("Skipped")
     print()
 
 
 # Dependency Management System (Build System) -----------------------------------------------------------------------
 
@@ -529,150 +523,131 @@
         sign = "=="
     return sign
 
 
 def get_build_system_version(args: object) -> str:
     """Assign build system version."""
 
-    if args.build_system:
-        if not args.has_install or args.force_clear or args.force_clear_all:
-            configuration = toml.load(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["configuration_file"])
-            if "build-system-requirements" in configuration.keys():
-                if (
-                    args.build_system_version == "*"
-                    and "build-system-version" in configuration["build-system-requirements"]
-                ):
-                    args.build_system_version = configuration["build-system-requirements"]["build-system-version"]
-            else:
-                args.build_system_version = get_python_package_versions(args.build_system)[-1]
+    if not args.has_install or args.force_clear or args.force_clear_all:
+        configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
+        if "build-system-requirements" in configuration.keys():
+            if (
+                args.build_system_version == "*"
+                and "build-system-version" in configuration["build-system-requirements"]
+            ):
+                args.build_system_version = configuration["build-system-requirements"]["build-system-version"]
+        else:
+            args.build_system_version = get_python_package_versions()[-1]
 
 
 def install_build_system(args: object) -> None:
     """Install build system."""
 
     print("Install dependency management system.")
-    if args.build_system:
-        if not args.has_install or args.force_clear or args.force_clear_all:
-            configuration = toml.load(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["configuration_file"])
-            if (
-                args.build_system_version == "*"
-                and "build-system-version" in configuration["build-system-requirements"]
-            ):
-                args.build_system_version = configuration["build-system-requirements"]["build-system-version"]
-            if args.build_system == "poetry":
-                create_virtual_environment(
-                    args, venv=SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["build_system_venv"]
-                )
-                upgrade_pip(
-                    python_executable=(
-                        rf".\{SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]['build_system_venv']}\Scripts\python"
-                    )
-                )
-                get_python_package(
-                    args.build_system,
-                    args.build_system_version,
-                    method="install",
-                    python_executable=(
-                        rf".\{SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]['build_system_venv']}\Scripts\python"
-                    ),
-                )
-            else:
-                get_python_package(
-                    args.build_system,
-                    args.build_system_version,
-                    method="install",
-                    python_executable=rf".\{args.venv_name}\Scripts\python",
-                    verbose=args.verbose,
-                )
-            print()
-            # Create a file symbolic link from the virtual environment (.venv) that the build system (poetry) manages
-            # to the build system executable (poetry.exe) in the poetry virtual environment (.poetry/.venv).  This
-            # ensures that the correct poetry is accessible when the managed virtual environment is activated
-            build_system_executable = (
-                rf".\{SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]['build_system_venv']}"
-                rf"\Scripts\{args.build_system}.exe"
-            )
-            if os.path.exists(build_system_executable):
+    if not args.has_install or args.force_clear or args.force_clear_all:
+        configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
+        if args.build_system_version == "*" and "build-system-version" in configuration["build-system-requirements"]:
+            args.build_system_version = configuration["build-system-requirements"]["build-system-version"]
+
+        create_virtual_environment(args, venv=DEPENDENCY_MANAGER_PATHS["common"]["build_system_venv"])
+        upgrade_pip(python_executable=DEPENDENCY_MANAGER_PATHS[sys.platform]["poetry_python_executable"])
+        get_python_package(
+            args.build_system_version,
+            method="install",
+            python_executable=DEPENDENCY_MANAGER_PATHS[sys.platform]["poetry_python_executable"],
+        )
+        print()
+        # Create a file symbolic link from the virtual environment (.venv) that the build system (poetry) manages
+        # to the build system executable (poetry.exe) in the poetry virtual environment (.poetry/.venv).  This
+        # ensures that the correct poetry is accessible when the managed virtual environment is activated
+        build_system_executable = DEPENDENCY_MANAGER_PATHS[sys.platform]["build_sys_exec"]
+        if os.path.exists(build_system_executable):
+            if sys.platform == "win32":
                 subprocess.run(
                     [
                         "powershell",
                         "-Command",
                         "New-Item",
                         "-ItemType",
                         "SymbolicLink",
                         "-Path",
-                        rf".\{args.venv_name}\Scripts\{args.build_system}.exe",
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["dep_bin_venv_path"],
                         "-Target",
                         build_system_executable,
                     ]
                 )
-            return
+            elif sys.platform == "linux":
+                subprocess.run(
+                    [
+                        "ln",
+                        "-sf",
+                        build_system_executable,
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["dep_bin_venv_path"],
+                    ]
+                )
+        return
     print("Skipped")
     print()
 
 
 def configure_build_system(args: object) -> None:
     """Configure the build system to enable connection to private sources."""
 
     print("Configure dependency management system.")
-    if args.build_system:
-        if not args.has_install or args.force_clear or args.force_clear_all:
-            if args.build_system == "poetry":
-                configure_poetry(
-                    SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["build_system_venv"],
-                    args.credentials_management_method,
-                )
-                print()
-            return
+    if not args.has_install or args.force_clear or args.force_clear_all:
+        configure_poetry(
+            DEPENDENCY_MANAGER_PATHS["common"]["build_system_venv"],
+            args.credentials_management_method,
+        )
+        print()
+        return
     print("Skipped")
     print()
 
 
 def configure_poetry(venv_name: str, credentials_management_method: str) -> None:
     """Configure Poetry."""
-
+    poetry_executable = DEPENDENCY_MANAGER_PATHS[sys.platform]["dep_bin_venv_path"]
     # Get list of private sources
     private_sources = get_private_sources("pyproject.toml")
     # Turn-on in-project
-    subprocess.run([rf".\{venv_name}\Scripts\poetry", "config", "virtualenvs.create", "false", "--local"], check=True)
+    subprocess.run([poetry_executable, "config", "virtualenvs.create", "false", "--local"], check=True)
     # Turn-off virtual environment creation
-    subprocess.run(
-        [rf".\{venv_name}\Scripts\poetry", "config", "virtualenvs.in-project", "true", "--local"], check=True
-    )
+    subprocess.run([poetry_executable, "config", "virtualenvs.in-project", "true", "--local"], check=True)
     # Turn-on poetry cache
     subprocess.run(
         [
-            rf".\{venv_name}\Scripts\poetry",
+            poetry_executable,
             "config",
             "cache-dir",
-            SUPPORTED_DEPENDENCY_MANAGERS["poetry"]["cache_folder"],
+            DEPENDENCY_MANAGER_PATHS["common"]["cache_folder"],
             "--local",
         ],
         check=True,
     )
     # Turn-on in-project
-    subprocess.run([rf".\{venv_name}\Scripts\poetry", "config", "virtualenvs.create", "false", "--local"], check=True)
+    subprocess.run([poetry_executable, "config", "virtualenvs.create", "false", "--local"], check=True)
     # Declare credentials for private sources
     for source in private_sources:
         print(f"Declare credentials for {source['name']}")
         if source["name"].lower() == "pypi":
             continue
         elif source["url"] == "https://pkgs.dev.azure.com/pyansys/_packaging/pyansys/pypi/simple/":
             token = os.environ["PYANSYS_PRIVATE_PYPI_PAT"]
         elif source["url"] == "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple/":
             token = os.environ["SOLUTIONS_PRIVATE_PYPI_PAT"]
         else:
             raise Exception(f"Unknown private source {source['name']} with url {source['url']}.")
         # Store credentials
         if credentials_management_method == "keyring":
             # Declare source URL
-            command_line = f"{venv_name}/Scripts/poetry config repositories.{source['name']} {source['url']} --local"
+            command_line = [poetry_executable, "config", f"repositories.{source['name']}", source["url"], "--local"]
             subprocess.run(command_line, check=True)
             # Declare source credentials
-            command_line = f"{venv_name}/Scripts/poetry config http-basic.{source['name']} PAT {token} --local"
+            command_line = [poetry_executable, "config", f"http-basic.{source['name']}", "PAT", token, "--local"]
             subprocess.run(command_line, check=True)
         elif credentials_management_method == "environment-variables":
             # Format source name to comply with Poetry environment variable syntax
             source_name = source["name"].upper().replace("-", "_")
             # Create Poetry environment variable
             os.environ[f"POETRY_HTTP_BASIC_{source_name}_USERNAME"] = "PAT"
             os.environ[f"POETRY_HTTP_BASIC_{source_name}_PASSWORD"] = token
@@ -785,135 +760,143 @@
     print("Clear workspace")
     if args.force_clear or args.force_clear_all:
         # Remove virtual environment
         if os.path.isdir(args.venv_name):
             print(f"Delete existing virtual environment {args.venv_name}.")
             shutil.rmtree(args.venv_name)
         # Remove poetry virtual environment
-        if os.path.isdir(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["build_system_venv"]):
+        if os.path.isdir(DEPENDENCY_MANAGER_PATHS["common"]["build_system_venv"]):
             print("Delete existing poetry virtual environment")
-            shutil.rmtree(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["build_system_venv"])
+            shutil.rmtree(DEPENDENCY_MANAGER_PATHS["common"]["build_system_venv"])
         # Remove poetry cache
-        if os.path.isdir(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["cache_folder"]):
+        if os.path.isdir(DEPENDENCY_MANAGER_PATHS["common"]["cache_folder"]):
             print("Delete existing poetry cache")
-            shutil.rmtree(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["cache_folder"])
+            shutil.rmtree(DEPENDENCY_MANAGER_PATHS["common"]["cache_folder"])
         if args.force_clear_all:
             # Remove lock file
-            if args.build_system:
-                if SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["lock_file"]:
-                    if os.path.isfile(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["lock_file"]):
-                        print("Delete existing poetry lock file")
-                        os.remove(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["lock_file"])
+            if DEPENDENCY_MANAGER_PATHS["common"]["lock_file"]:
+                if os.path.isfile(DEPENDENCY_MANAGER_PATHS["common"]["lock_file"]):
+                    print("Delete existing poetry lock file")
+                    os.remove(DEPENDENCY_MANAGER_PATHS["common"]["lock_file"])
     else:
         print("Skipped")
     print()
 
 
 def install_production_dependencies(args: object) -> None:
     """Install the package (mandatory requirements only)."""
 
     print("Install production dependencies")
-    if args.build_system and "run" in args.dependencies:
-        if args.build_system == "poetry":
-            subprocess.run(
-                [
-                    rf".\{SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]['build_system_venv']}\Scripts\poetry",
-                    "install",
-                    "-vv",
-                ],
-                check=True,
-                shell=True,
-            )
-        elif args.build_system == "flit":
-            subprocess.run([rf".\{args.venv_name}\Scripts\flit", "install"], check=True, shell=True)
+    if "run" in args.dependencies:
+        subprocess.run(
+            [
+                DEPENDENCY_MANAGER_PATHS[sys.platform]["build_sys_exec"],
+                "install",
+                "-vv",
+            ],
+            check=True,
+            shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
+        )
         print()
         return
     print("Skipped")
     print()
 
 
 def install_optional_dependencies(args: object) -> None:
     """Install optional requirements (doc, tests, build or style)."""
 
-    # Load configuration file if a dependency management system is available
-    if args.build_system:
-        configuration = toml.load(SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]["configuration_file"])
-    else:
-        configuration = {}
+    # Load configuration file
+    configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
     # Install standard optional dependency groups
     for dependency_group in STANDARD_OPTIONAL_DEPENDENCY_GROUPS:
         print(f"Install {dependency_group} dependencies")
         if dependency_group in args.dependencies:
             # Install dependency group in the configuration file of the build system
-            if args.build_system:
-                has_dependency_group = check_dependency_group(dependency_group, configuration)
-                if has_dependency_group:
-                    print("Installing from build system configuration file.")
-                    subprocess.run(
-                        [
-                            (
-                                rf".\{SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]['build_system_venv']}"
-                                r"\Scripts\poetry"
-                            ),
-                            "install",
-                            "--only",
-                            dependency_group,
-                            "-vv",
-                        ],
-                        check=True,
-                        shell=True,
-                    )
-                    print()
-                    continue
+            has_dependency_group = check_dependency_group(dependency_group, configuration)
+            if has_dependency_group:
+                print("Installing from build system configuration file.")
+                subprocess.run(
+                    [
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["build_sys_exec"],
+                        "install",
+                        "--only",
+                        dependency_group,
+                        "-vv",
+                    ],
+                    check=True,
+                    shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
+                )
+                print()
+                continue
             # Alternatively search dependency group in the requirements folder
             requirements_file = os.path.join("requirements", f"requirements_{dependency_group}.txt")
             if os.path.exists(requirements_file):
                 print("Installing from requirements file.")
                 subprocess.run(
                     [
-                        rf".\{SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]['build_system_venv']}\Scripts\python",
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["poetry_python_executable"],
                         "-m",
                         "poetry",
                         "run",
                         "pip",
                         "install",
                         "-r",
                         requirements_file,
                         "--no-warn-conflicts",
                     ],
                     check=True,
-                    shell=True,
+                    shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
                 )
                 print()
                 continue
         print("Skipped")
         print()
     # Install extra optional dependency groups
-    if args.build_system and args.extra_dependencies:
+    if args.extra_dependencies:
         for dependency_group in args.extra_dependencies:
             print(f"Install {dependency_group} dependencies")
             has_dependency_group = check_dependency_group(dependency_group, configuration)
             if has_dependency_group:
                 subprocess.run(
                     [
-                        rf".\{SUPPORTED_DEPENDENCY_MANAGERS[args.build_system]['build_system_venv']}\Scripts\poetry",
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["build_sys_exec"],
                         "install",
                         "--only",
                         dependency_group,
                         "-vv",
                     ],
                     check=True,
-                    shell=True,
+                    shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
                 )
             else:
                 print(f"No dependency group named {dependency_group}.")
                 print("Skipped")
             print()
 
 
+def install_dotnet_linux_dependencies():
+    print("Install dotnet dependencies")
+    if sys.platform == "linux":
+        subprocess.run(
+            'set -xe \
+            && wget https://dot.net/v1/dotnet-install.sh \
+            && chmod +x dotnet-install.sh \
+            && ./dotnet-install.sh --install-dir /home/$USER/.dotnet --version 3.1.0 --runtime aspnetcore \
+            && grep -qxF "DOTNET_ROOT=/home/$USER/.dotnet" /home/$USER/.bash_profile \
+            || echo DOTNET_ROOT=/home/$USER/.dotnet >> /home/$USER/.bash_profile \
+            && grep -qxF "PATH=\$PATH:/home/$USER/.dotnet" /home/$USER/.bash_profile \
+            || echo "PATH=\$PATH:/home/$USER/.dotnet" >> /home/$USER/.bash_profile \
+            && echo "\nsource /home/$USER/.bash_profile" >> ./.venv/bin/activate \
+            && rm dotnet-install.sh',
+            check=True,
+            shell=True,
+        )
+
+
 def main() -> None:
     """Sequence of operations leading to the complete Python ecosystem."""
 
     # Start timer
     time_on = time.time()
     # Get current working directory
     working_directory = os.getcwd()
@@ -947,15 +930,15 @@
 
     # Setup virtual environment ---------------------------------------------------------------------------------------
 
     print_section_header("Setup virtual environment", max_length=100)
 
     create_virtual_environment(args)
 
-    upgrade_pip(python_executable=rf".\{args.venv_name}\Scripts\python")
+    upgrade_pip(python_executable=DEPENDENCY_MANAGER_PATHS[sys.platform]["python_executable"])
 
     # Setup dependency management system ------------------------------------------------------------------------------
 
     print_section_header("Setup dependency management system", max_length=100)
 
     install_build_system(args)
 
@@ -965,24 +948,27 @@
 
     print_section_header("Install dependencies", max_length=100)
 
     install_production_dependencies(args)
 
     install_optional_dependencies(args)
 
+    install_dotnet_linux_dependencies()
+
     # Back to current working directory
     os.chdir(working_directory)
 
     # Compute execution time
     elapsed_time = (time.time() - time_on) / 60  # in minutes
 
     print("You are all set!")
     print("Navigate to project root and activate your environment with one these commands:")
     print(rf"   - For Windows CMD       : {args.venv_name}\Scripts\activate.bat")
     print(rf"   - For Windows Powershell: {args.venv_name}\Scripts\Activate.ps1")
+    print(rf"   - For Ubuntu            : source {args.venv_name}/bin/activate")
     print("Enjoy!")
     print()
     print("Execution time: %.1f minutes." % (elapsed_time))
     print()
 
 
 # =================================================== [Execution] =================================================== #
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,36 @@
 
 """Backend of the problem setup step."""
 
 import json
 from pathlib import Path
 import platform
 import time
+from typing import List
+import subprocess
+import sys
 
 from ansys.optislang.core import Optislang, logging
-from ansys.saf.glow.solution import FileReference, StepModel, StepSpec, long_running, transaction
-from ansys.solutions.optislang.parser.project_properties import (
-    ProjectProperties,
-    apply_placeholders_to_properties_file,
-    write_properties_file,
-)
+from ansys.saf.glow.solution import FileReference, AssetFileReference, StepModel, StepSpec, long_running, transaction
+from ansys.solutions.optislang.frontend_components.project_properties import ProjectProperties, write_properties_file, apply_placeholders_to_properties_file
 from ansys.solutions.products_ecosystem.controller import AnsysProductsEcosystemController
 from ansys.solutions.products_ecosystem.utils import convert_to_long_version
 
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.model.utils import read_system_hierarchy
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.model.osl_project_tree import dump_project_state, get_project_tree, get_node_list, get_step_list
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.monitoring import _get_actor_hids, read_optislang_logs
 
 
 class ProblemSetupStep(StepModel):
     """Step model of the problem setup step."""
 
     # Parameters ------------------------------------------------------------------------------------------------------
 
     # Frontend persistence
     ansys_ecosystem_ready: bool = False
     optislang_solve_status: str = "initial"  # initial, processing, finished, stopped, aborted, idle
-    placeholder_values: dict = {}
-    placeholder_definitions: dict = {}
     ui_placeholders: dict = {}
     app_metadata: dict = {}
     analysis_running: bool = False
 
     # Backend data model
     tcp_server_host: str = "127.0.0.1"
     tcp_server_port: int = None
@@ -45,82 +42,99 @@
             "compatible_versions": [],
             "selected_version": None,
             "alert_message": "OptiSLang install not checked.",
             "alert_color": "warning",
             "alias": "optiSLang",
         }
     }
-    system_hierarchy: dict = {}
+    step_list: list = []
+    node_list: list = []
+    placeholders: dict = {}
+    registered_files: List = []
+    settings: dict = {}
+    parameter_manager: dict = {}
+    criteria: dict = {}
     project_status_info: dict = {}
     actors_info: dict = {}
     actors_status_info: dict = {}
     results_files: dict = {}
     tcp_server_stopped_states = ["idle", "finished", "stopped", "aborted"]
     optislang_logs: list = []
     optislang_log_level: str = "DEBUG"
+    project_initialized: bool = False
+    has_project_state: bool = False
 
     # File storage ----------------------------------------------------------------------------------------------------
 
     # Inputs
-    project_file: FileReference = FileReference("Problem_Setup/{{ cookiecutter.__optiSLang_project_file_name }}")
-    properties_file: FileReference = FileReference("Problem_Setup/{{ cookiecutter.__optiSLang_properties_file_name }}")
-    metadata_file: FileReference = FileReference("Problem_Setup/metadata_file.json")
-    system_hierarchy_file: FileReference = FileReference("Problem_Setup/system_hierarchy.json")
+    project_file: FileReference = FileReference("Problem_Setup/{{ cookiecutter.__optiSLang_application_archive_stem }}.opf")
+    properties_file: FileReference = FileReference("Problem_Setup/{{ cookiecutter.__optiSLang_application_archive_stem }}.json")
+    metadata_file: FileReference = FileReference("Problem_Setup/metadata.json")
+    project_state_file: FileReference = FileReference("Problem_Setup/project_state.json")
 
     # Outputs
     working_properties_file: FileReference = FileReference("Problem_Setup/working_properties_file.json")
     server_info_file: FileReference = FileReference("Problem_Setup/server_info.ini")
     optislang_log_file: FileReference = FileReference("Problem_Setup/pyoptislang.log")
 
     # Methods ---------------------------------------------------------------------------------------------------------
 
-    @transaction(self=StepSpec(download=["properties_file"], upload=["placeholder_values", "placeholder_definitions"]))
-    def get_default_placeholder_values(self) -> None:
-        """Get placeholder values and definitions using the ProjectProperties class."""
-        pp = ProjectProperties()
-        pp.read_file(self.properties_file.path)
-        placeholders = pp.get_properties()["placeholders"]
-        self.placeholder_values = placeholders.get("placeholder_values")
-        self.placeholder_definitions = placeholders.get("placeholder_definitions")
+    @transaction(
+        self=StepSpec(
+            upload=["has_project_state"]
+        )
+    )
+    def generate_project_state(self) -> None:
+        """Generate a project state from an optiSLang opf file."""
 
-    @transaction(self=StepSpec(download=["properties_file", "ui_placeholders"], upload=["working_properties_file"]))
-    def write_updated_properties_file(self) -> None:
-        properties = apply_placeholders_to_properties_file(self.ui_placeholders, self.properties_file.path)
-        write_properties_file(properties, Path(self.working_properties_file.path))
+        project_file = Path(__file__).absolute().parent.parent / "model" / "assets" / "{{ cookiecutter.__optiSLang_application_archive_stem }}.opf"
+
+        dump_project_state(project_file, Path(project_file).parent / "project_state.json")
+
+        self.has_project_state = True
 
     @transaction(
         self=StepSpec(
-            upload=["project_file", "properties_file", "metadata_file", "system_hierarchy_file"]
+            download=["project_state_file"],
+            upload=["step_list", "node_list"]
+        )
+    )
+    def read_project_tree(self) -> None:
+        """Read project tree from optiSLang project state file."""
+
+        project_tree = get_project_tree(self.project_state_file.path)
+        self.step_list = get_step_list(project_tree)
+        self.node_list = get_node_list(project_tree)
+
+    @transaction(
+        self=StepSpec(
+            upload=[
+                "project_file",
+                "properties_file",
+                "metadata_file",
+                "project_state_file",
+            ]
         )
     )
     def upload_bulk_files_to_project_directory(self) -> None:
         """Upload bulk files to project directory."""
 
-        original_project_file = Path(__file__).parent.absolute().parent / "model" / "assets" / "{{ cookiecutter.__optiSLang_project_file_name }}"
+        original_project_file = Path(__file__).parent.absolute().parent / "model" / "assets" / "{{ cookiecutter.__optiSLang_application_archive_stem }}.opf"
         self.project_file.write_bytes(original_project_file.read_bytes())
 
         original_properties_file = (
-            Path(__file__).parent.absolute().parent / "model" / "assets" / "{{ cookiecutter.__optiSLang_properties_file_name }}"
+            Path(__file__).parent.absolute().parent / "model" / "assets" / "{{ cookiecutter.__optiSLang_application_archive_stem }}.json"
         )
         self.properties_file.write_bytes(original_properties_file.read_bytes())
 
         original_metadata_file = Path(__file__).parent.absolute().parent / "model" / "assets" / "metadata.json"
         self.metadata_file.write_bytes(original_metadata_file.read_bytes())
 
-        original_system_hierarchy_file = (
-            Path(__file__).parent.absolute().parent / "model" / "assets" / "system_hierarchy.json"
-        )
-        self.system_hierarchy_file.write_bytes(original_system_hierarchy_file.read_bytes())
-
-    @transaction(self=StepSpec(download=["metadata_file"], upload=["app_metadata"]))
-    def get_app_metadata(self) -> None:
-        """Read OWA metadata file."""
-
-        with open(self.metadata_file.path) as f:
-            self.app_metadata = json.load(f)
+        original_project_state_file = Path(__file__).parent.absolute().parent / "model" / "assets" / "project_state.json"
+        self.project_state_file.write_bytes(original_project_state_file.read_bytes())
 
     @transaction(
         self=StepSpec(
             upload=["ansys_ecosystem", "ansys_ecosystem_ready"],
         )
     )
     def check_ansys_ecosystem(self) -> None:
@@ -169,22 +183,51 @@
                     alert_message += f" {convert_to_long_version(compatible_version)}"
                 alert_message += ".\n"
                 alert_message += "Selected version is %s." % (self.ansys_ecosystem[product_name]["selected_version"])
                 alert_color = "success"
             self.ansys_ecosystem[product_name]["alert_message"] = alert_message
             self.ansys_ecosystem[product_name]["alert_color"] = alert_color
 
+    @transaction(self=StepSpec(download=["properties_file"], upload=["placeholders", "registered_files", "settings", "parameter_manager", "criteria"]))
+    def get_default_placeholder_values(self):
+        """Get placeholder values and definitions using the ProjectProperties class."""
+
+        pp = ProjectProperties()
+        pp.read_file(self.properties_file.path)
+        self.placeholders = pp._placeholders
+        self.registered_files = pp._registered_files
+        self.settings = pp._settings
+        self.parameter_manager = pp._parameter_manager
+        self.criteria = pp._criteria
+
+    @transaction(self=StepSpec(download=["properties_file", "ui_placeholders"], upload=["working_properties_file"]))
+    def write_updated_properties_file(self) -> None:
+        properties = apply_placeholders_to_properties_file(self.ui_placeholders, self.properties_file.path)
+        write_properties_file(properties, Path(self.working_properties_file.path))
+
+    @transaction(
+        self=StepSpec(
+            download=["metadata_file"],
+            upload=["app_metadata"]
+        )
+    )
+    def get_app_metadata(self) -> None:
+        """Read OWA metadata file."""
+
+        with open(self.metadata_file.path) as f:
+            self.app_metadata = json.load(f)
+
     @transaction(
         self=StepSpec(
             download=[
                 "project_file",
                 "working_properties_file",
-                "system_hierarchy_file",
                 "tcp_server_stopped_states",
                 "optislang_log_level",
+                "node_list",
             ],
             upload=[
                 "optislang_solve_status",
                 "server_info_file",
                 "actors_info",
                 "actors_status_info",
                 "tcp_server_port",
@@ -195,16 +238,14 @@
             ],
         )
     )
     @long_running
     def start_analysis(self) -> None:
         """Start optiSLang and run the project."""
 
-        self.system_hierarchy = read_system_hierarchy(self.system_hierarchy_file.path)
-
         osl_logger = logging.OslLogger(
             loglevel=self.optislang_log_level,
             log_to_file=True,
             logfile_name=self.optislang_log_file.path,
             log_to_stdout=True,
         )
 
@@ -235,15 +276,15 @@
 
         while True:
             # Get project status info
             self.project_status_info = osl.get_osl_server().get_full_project_status_info()
             # Read pyoptislang logs
             self.optislang_logs = read_optislang_logs(self.optislang_log_file.path)
             # Get actor status info
-            for node_info in self.system_hierarchy:
+            for node_info in self.node_list:
                 self.actors_info[node_info["uid"]] = osl.get_osl_server().get_actor_info(node_info["uid"])
                 node_hids = _get_actor_hids(osl.get_osl_server().get_actor_states(node_info["uid"]))
                 if len(node_hids):
                     self.actors_status_info[node_info["uid"]] = []
                     for hid in node_hids:
                         self.actors_status_info[node_info["uid"]].append(
                             osl.get_osl_server().get_actor_status_info(node_info["uid"], hid)
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,74 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Initialization of the frontend layout across all the steps."""
 
+
 from ansys.saf.glow.client.dashclient import DashClient
 from ansys_dash_treeview import AnsysDashTreeview
 import dash_bootstrap_components as dbc
 from dash_extensions.enrich import Input, Output, callback, callback_context, dcc, html
 from dash_iconify import DashIconify
 
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import {{ cookiecutter.__solution_definition_name }}
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.pages import monitoring_page, problem_setup_page
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.common_functions import extract_dict_by_key, read_system_hierarchy
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import (
+    {{ cookiecutter.__solution_definition_name }},
+)
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.pages import intro_page, first_page, second_page
 
-step_list = read_system_hierarchy()
+step_list = [
+    {
+        "key": "intro_step",
+        "text": "Introduction",
+        "depth": 0,
+    },
+    {
+        "key": "first_step",
+        "text": "First Step",
+        "depth": 0,
+    },
+    {
+        "key": "second_step",
+        "text": "Second Step",
+        "depth": 0,
+    }
+]
 
 
 layout = html.Div(
     [
-        dcc.Location(id="url", refresh=False),  # represents the browser address bar and doesn't render anything
+        dcc.Location(id="url", refresh=False), # represents the browser address bar and doesn't render anything
         dbc.Stack(
             [
                 html.Div(
-                    [html.Img(src=r"/assets/logos/ansys-solutions-horizontal-logo.png", style={"width": "80%"})],
+                    [
+                        html.Img(
+                        src = r"/assets/logos/ansys-solutions-horizontal-logo.png",
+                        style={'width': '80%'}
+                    )
+                    ],
                 ),
                 html.Div(
                     [
                         dbc.Button(
                             "Project Name:",
-                            id="project-name",
-                            disabled=True,
+                            id = "project-name",
+                            disabled = True,
                             style={
                                 "color": "rgba(0, 0, 0, 1)",
                                 "background-color": "rgba(255, 255, 255, 1)",
-                                "border-color": "rgba(0, 0, 0, 1)",
+                                "border-color": "rgba(0, 0, 0, 1)"
                             },
                         )
                     ],
                     className="ms-auto",
                 ),
                 html.Div(id="return-to-portal"),
             ],
-            direction="horizontal",
-            gap=3,
+            direction = "horizontal",
+            gap = 3,
         ),
         html.Br(),
         dbc.Row(
             [
                 dbc.Col(
                     AnsysDashTreeview(
                         id="navigation_tree",
@@ -55,15 +78,21 @@
                             DashIconify(icon="bi:caret-down-square-fill"),
                         ],
                         style={"showButtons": True, "focusColor": "#ffb71b", "itemHeight": "32"},  # Ansys gold
                     ),
                     width=2,
                     style={"background-color": "rgba(242, 242, 242, 0.6)"},  # Ansys grey
                 ),
-                dbc.Col(html.Div(id="page-content", style={"padding-right": "1%"}), width=10),
+                dbc.Col(
+                    html.Div(
+                        id="page-content",
+                        style={"padding-right": "1%"}
+                    ),
+                    width=10
+                ),
             ],
         ),
     ]
 )
 
 
 @callback(
@@ -75,61 +104,55 @@
     portal_ui_url = DashClient.get_portal_ui_url()
     children = (
         []
         if portal_ui_url is None
         else [
             dbc.Button(
                 "Back to Projects",
-                id="return-to-portal",
-                className="me-2",
-                n_clicks=0,
-                href=portal_ui_url,
-                style={"background-color": "rgba(0, 0, 0, 1)", "border-color": "rgba(0, 0, 0, 1)"},
+                id = "return-to-portal",
+                className = "me-2",
+                n_clicks = 0,
+                href = portal_ui_url,
+                style = {"background-color": "rgba(0, 0, 0, 1)", "border-color": "rgba(0, 0, 0, 1)"},
             )
         ]
     )
     return children
 
 
 @callback(
     Output("project-name", "children"),
     Input("url", "pathname"),
 )
 def display_poject_name(pathname):
     """Display current project name."""
-    project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
+    project = DashClient[{{cookiecutter.__solution_definition_name}}].get_project(pathname)
     return f"Project Name: {project.project_display_name}"
 
 
+# this callback is essential for initializing the step based on the persisted
+# state of the project when the browser first displays the project to the user
+# given the project's URL
 @callback(
     Output("page-content", "children"),
     [
         Input("url", "pathname"),
         Input("navigation_tree", "focus"),
     ],
     prevent_initial_call=True,
 )
 def display_page(pathname, value):
-    """
-    Display page content.
-
-    this callback is essential for initializing the step based on the persisted
-    state of the project when the browser first displays the project to the user
-    given the project's URL
-    """
-
+    """Display page content."""
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     triggered_id = callback_context.triggered[0]["prop_id"].split(".")[0]
-
     if triggered_id == "url":
-        return problem_setup_page.layout(project.steps.problem_setup_step)
+        return intro_page.layout(project.steps.intro_step)
     if triggered_id == "navigation_tree":
         if value is None:
             page_layout = html.H1("Welcome!")
-        elif value == "problem_setup_step":
-            page_layout = problem_setup_page.layout(project.steps.problem_setup_step)
-        else:
-            node_info = extract_dict_by_key(step_list, "key", value, expect_unique=True)
-            page_layout = monitoring_page.layout(
-                project.steps.problem_setup_step, project.steps.monitoring_step, node_info
-            )
+        elif value == "intro_step":
+            page_layout = intro_page.layout(project.steps.intro_step)
+        elif value == "first_step":
+            page_layout = first_page.layout(project.steps.first_step)
+        elif value == "second_step":
+            page_layout = second_page.layout(project.steps.second_step)
         return page_layout
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,52 +3,34 @@
 """Frontend of the problem setup step."""
 
 import time
 
 from ansys.saf.glow.client.dashclient import DashClient
 from ansys.saf.glow.solution import MethodStatus
 from ansys.solutions.dash_components.table import InputRow
-from ansys.solutions.optislang.frontend_components.placeholder_table import PlaceholderTable
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 from dash_extensions.enrich import Input, Output, State, callback, dcc, html
+from ansys.solutions.optislang.frontend_components.load_sections import to_dash_sections
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import {{ cookiecutter.__solution_definition_name }}
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.problem_setup_step import ProblemSetupStep
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.alerts import update_alerts
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.placeholders import update_placeholders
 
 
 def layout(problem_setup_step: ProblemSetupStep) -> html.Div:
     """Layout of the problem setup step."""
 
     # Upload placeholders and assets
-    if problem_setup_step.placeholder_values == {}:
-        problem_setup_step.upload_bulk_files_to_project_directory()
-        problem_setup_step.get_app_metadata()
+    if problem_setup_step.placeholders == {}:
         problem_setup_step.get_default_placeholder_values()
-        problem_setup_step.ui_placeholders = problem_setup_step.placeholder_values
+        problem_setup_step.ui_placeholders = problem_setup_step.placeholders
 
-    # Placeholder card for displaying parameters defined in the <project_name>.json
-    placeholder_card = dbc.Accordion(
-        [
-            dbc.AccordionItem(
-                [
-                    html.Div(
-                        id="placeholder_table",
-                        children=PlaceholderTable(
-                            problem_setup_step.ui_placeholders, problem_setup_step.placeholder_definitions
-                        ).create(),
-                    ),
-                ],
-                title="Placeholders",
-                item_id="parameter_placeholders",
-            )
-        ]
-    )
+    project_properties_sections = to_dash_sections(problem_setup_step.placeholders, problem_setup_step.registered_files)
 
     return html.Div(
         [
             # Header
             html.H1(
                 problem_setup_step.app_metadata["title"].strip().title(),
                 className="display-3",
@@ -75,46 +57,42 @@
                         ],
                         width=12,
                     )
                 ]
             ),
             html.Br(),
             # Input form
-            dbc.Row(
-                [
-                    placeholder_card,
-                ],
-            ),
+            dbc.Row(project_properties_sections),
             dbc.Row(
                 [
                     dbc.Accordion(
                         [
                             dbc.AccordionItem(
                                 [
-                                    InputRow(
-                                        "button",
-                                        "check_ansys_ecosystem",
-                                        "Check Ansys ecosystem",
-                                        disabled=False,
-                                        label_width=2,
-                                        value_width=4,
-                                        unit_width=1,
-                                        description_width=4,
-                                        class_name="button",
-                                    ).get(),
-                                    dcc.Loading(
-                                        type="circle",
-                                        fullscreen=True,
-                                        color="#ffb71b",
-                                        style={
-                                            "background-color": "rgba(55, 58, 54, 0.1)",
-                                        },
-                                        children=html.Div(id="wait_ecosystem_ckeck"),
-                                    ),
-                                    html.Br(),
+                                    # InputRow(
+                                    #     "button",
+                                    #     "check_ansys_ecosystem",
+                                    #     "Check Ansys ecosystem",
+                                    #     disabled=False,
+                                    #     label_width=2,
+                                    #     value_width=4,
+                                    #     unit_width=1,
+                                    #     description_width=4,
+                                    #     class_name="button",
+                                    # ).get(),
+                                    # dcc.Loading(
+                                    #     type="circle",
+                                    #     fullscreen=True,
+                                    #     color="#ffb71b",
+                                    #     style={
+                                    #         "background-color": "rgba(55, 58, 54, 0.1)",
+                                    #     },
+                                    #     children=html.Div(id="wait_ecosystem_ckeck"),
+                                    # ),
+                                    # html.Br(),
                                     InputRow(
                                         "button",
                                         "start_analysis",
                                         "Start analysis",
                                         disabled=True
                                         if problem_setup_step.analysis_running
                                         or not problem_setup_step.ansys_ecosystem_ready
@@ -160,53 +138,53 @@
     )
     def toggle_popover(n_clicks, is_open):
         if n_clicks:
             return not is_open
         return is_open
 
 
-@callback(
-    Output("alert_messages", "children"),
-    Output("wait_ecosystem_ckeck", "children"),
-    Output("start_analysis", "disabled"),
-    Input("check_ansys_ecosystem", "n_clicks"),
-    State("url", "pathname"),
-    prevent_initial_call=True,
-)
-def check_ansys_ecosystem(n_clicks, pathname):
-    """Start OptiSLang and run the simulation. Wait for the process to complete."""
-
-    project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
-    problem_setup_step = project.steps.problem_setup_step
-
-    if n_clicks:
-        problem_setup_step.check_ansys_ecosystem()
-        return update_alerts(problem_setup_step), True, False if problem_setup_step.ansys_ecosystem_ready else True
-    else:
-        raise PreventUpdate
+# @callback(
+#     Output("alert_messages", "children"),
+#     Output("wait_ecosystem_ckeck", "children"),
+#     Output("start_analysis", "disabled"),
+#     Input("check_ansys_ecosystem", "n_clicks"),
+#     State("url", "pathname"),
+#     prevent_initial_call=True,
+# )
+# def check_ansys_ecosystem(n_clicks, pathname):
+#     """Start optiSLang and run the simulation. Wait for the process to complete."""
+
+#     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
+#     problem_setup_step = project.steps.problem_setup_step
+
+#     if n_clicks:
+#         problem_setup_step.check_ansys_ecosystem()
+#         return update_alerts(problem_setup_step), True, False if problem_setup_step.ansys_ecosystem_ready else True
+#     else:
+#         raise PreventUpdate
 
 
 @callback(
     Output("alert_messages", "children"),
     Output("wait_start_analysis", "children"),
     Output("start_analysis", "disabled"),
     Input("start_analysis", "n_clicks"),
-    [State("placeholder_table", "children")],
+    [State("table-placeholders", "children")],
     State("url", "pathname"),
     prevent_initial_call=True,
 )
 def start_analysis(n_clicks, table_children, pathname):
-    """Start OptiSLang and run the simulation. Wait for the process to complete."""
+    """Start optiSLang and run the simulation. Wait for the process to complete."""
 
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     problem_setup_step = project.steps.problem_setup_step
 
     if n_clicks:
         # Update project properties file prior to the solve
-        problem_setup_step.ui_placeholders = update_placeholders(table_children, problem_setup_step.placeholder_values)
+        problem_setup_step.ui_placeholders = update_placeholders(table_children, problem_setup_step.placeholders)
         problem_setup_step.write_updated_properties_file()
         # Start analysis
         problem_setup_step.start_analysis()
         # Lock start analysis
         problem_setup_step.analysis_running = True
         # Wait until the analysis effectively starts
         while problem_setup_step.optislang_solve_status == "initial":
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,10 +4,12 @@
 def update_placeholders(ui_values: list, placeholders: dict) -> dict:
     """Information needed."""
 
     updated_dict = {}
     for row in ui_values[1:]:
         parameter_name = row["props"]["children"][0]["props"]["children"]["props"]["children"]
         input_value = row["props"]["children"][1]["props"]["children"]["props"]["value"]
-        if parameter_name in placeholders:
+
+        placeholder_values = placeholders.get("placeholder_values")
+        if parameter_name in placeholder_values:
             updated_dict[parameter_name] = input_value
     return updated_dict
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.0.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from pathlib import Path
 
 import isort
 
 from ansys.templates.utils import keep_files
 
 DESIRED_STRUCTURE = [
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from pathlib import Path
 
 import isort
 
 from ansys.templates.utils import keep_files
 
 DESIRED_STRUCTURE = [
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from pathlib import Path
 
 import isort
 
 from ansys.templates.utils import keep_files
 
 DESIRED_STRUCTURE = [
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from pathlib import Path
 
 import isort
 
 from ansys.templates.utils import keep_files
 
 DESIRED_STRUCTURE = [
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 DESIRED_STRUCTURE = [
     ".coveragerc",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     ".pre-commit-config.yaml",
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 
 from ansys.templates.utils import keep_files, remove_file
 
 ALLOWED_BUILD_SYSTEMS = ["flit", "poetry", "setuptools"]
 """A list of all allowed build systems by the template."""
 
 DESIRED_STRUCTURE = [
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 from ansys.templates.utils import keep_files
 
 ALLOWED_BUILD_SYSTEMS = ["flit"]
 """A list of all allowed build systems by the template."""
 
 DESIRED_STRUCTURE = [
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     ".flake8",
     ".github/workflows/build_and_test_library.yml",
     ".github/workflows/generate_library.yml",
     ".github/dependabot.yml",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml` & `ansys_templates-1.0.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pybasic/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/pybasic/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from ansys.templates.utils import keep_files
 
 
 DESIRED_STRUCTURE = [
     ".coveragerc",
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     "doc/Makefile",
     "doc/make.bat",
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-1.0.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/cookiecutter.json` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/cookiecutter.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9565217391304348%*

 * *Differences: {"'__project_name_slug'": '"{{ cookiecutter.project_name.lower().replace(\'_\', \'-\').replace(\' '*

 * *                          '\', \'-\') }}"',*

 * * "'__solution_name_slug'": '"{{ cookiecutter.solution_name.lower().replace(\'-\', '*

 * *                           '\'_\').replace(\' \', \'_\') }}"'}*

```diff
@@ -5,20 +5,20 @@
     "__library_name_slug": "",
     "__logo": "solutions",
     "__logo_color": "black",
     "__max_linelength": "120",
     "__pkg_name": "ansys-solutions-{{ cookiecutter.solution_name.lower().replace('_', '-') }}",
     "__pkg_namespace": "ansys.solutions.{{ cookiecutter.__project_name_slug }}",
     "__product_name_slug": "",
-    "__project_name_slug": "{{ cookiecutter.project_name.lower().replace('_', '-') }}",
+    "__project_name_slug": "{{ cookiecutter.project_name.lower().replace('_', '-').replace(' ', '-') }}",
     "__repository_url": "",
     "__requires_python": "3.8",
     "__short_description": "",
     "__solution_definition_name": "{{ cookiecutter.__solution_name_slug.title() }}Solution",
-    "__solution_name_slug": "{{ cookiecutter.solution_name.lower().replace('-', '_') }}",
+    "__solution_name_slug": "{{ cookiecutter.solution_name.lower().replace('-', '_').replace(' ', '_') }}",
     "__template_name": "solution",
     "__version": "0.1.dev0",
     "_copy_without_render": [
         "*.html"
     ],
     "project_name": "my-solution",
     "solution_display_name": "My Solution",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/hooks/post_gen_project.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/hooks/post_gen_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,31 +31,34 @@
     "tests/conftest.py",
     ".codespell.exclude",
     ".codespell.ignore",
     ".env",
     ".flake8",
     ".gitignore",
     ".pre-commit-config.yaml",
+    "AUTHORS",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CODEOWNERS",
     "CONTRIBUTING.md",
+    "CONTRIBUTORS.md",
     "LICENSE.rst",
     "poetry.lock",
     "pyproject.toml",
     "README.rst",
     "setup_environment.py",
     "tox.ini",
     ".env"
 ]
 """A list holding all desired files to be included in the project."""
 
 UI_STRUCTURE = [
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/css/style.css",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/images/README.md",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/images/solution-workflow-sketch.png",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/logos/ansys-solutions-horizontal-logo.png",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/scripts/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/first_page.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/intro_page.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/second_page.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/page.py",
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       - 6379:6379
     networks:
       - rep-obs
     extra_hosts:
       - "host.docker.internal:host-gateway"
 
   tracelens:
-    image: docker.io/rogeralsing/tracelens:amd64
+    image: azwepsifujiaksacr.azurecr.io/ansys/md1-obs/tracelens:latest
     ports:
       - 5000:5001
       - 4317:4317
     environment:
       - PlantUml__RemoteUrl=http://host.docker.internal:8082
       - Redis__Server=host.docker.internal
     networks:
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,29 @@
 python-versions = ">=3.6"
 files = [
     {file = "alabaster-0.7.13-py3-none-any.whl", hash = "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3"},
     {file = "alabaster-0.7.13.tar.gz", hash = "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"},
 ]
 
 [[package]]
+name = "ansi2html"
+version = "1.8.0"
+description = ""
+optional = false
+python-versions = ">=3.6"
+files = [
+    {file = "ansi2html-1.8.0-py3-none-any.whl", hash = "sha256:ef9cc9682539dbe524fbf8edad9c9462a308e04bce1170c32daa8fdfd0001785"},
+    {file = "ansi2html-1.8.0.tar.gz", hash = "sha256:38b82a298482a1fa2613f0f9c9beb3db72a8f832eeac58eb2e47bf32cd37f6d5"},
+]
+
+[package.extras]
+docs = ["Sphinx", "setuptools-scm", "sphinx-rtd-theme"]
+test = ["pytest", "pytest-cov"]
+
+[[package]]
 name = "ansys-api-platform-instancemanagement"
 version = "1.0.0b3"
 description = ""
 optional = false
 python-versions = "*"
 files = [
     {file = "ansys_api_platform_instancemanagement-1.0.0b3-py3-none-any.whl", hash = "sha256:fecd45064e7a0ddecd1c9301c39cb6c662094838d63afdd7cc32b369a16b9723"},
@@ -153,14 +168,34 @@
 
 [package.source]
 type = "legacy"
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple"
 reference = "solutions-private-pypi"
 
 [[package]]
+name = "ansys-solutions-dash-lib"
+version = "0.4.2"
+description = "A collection of functions and classes to design solution's frontend using Dash components."
+optional = false
+python-versions = ">=3.8,<3.11"
+files = [
+    {file = "ansys_solutions_dash_lib-0.4.2-py3-none-any.whl", hash = "sha256:21bd1225591d290ff463602ff83c033bfe35fd7b4418db496654eb1c8e25084c"},
+    {file = "ansys_solutions_dash_lib-0.4.2.tar.gz", hash = "sha256:285ccf20b01e1de03ea288f2fced6bb16d6d1d8dc4a09d647626d57c551681df"},
+]
+
+[package.dependencies]
+dash = ">=2.5,<3.0"
+dash_bootstrap_components = ">=1.3,<2.0"
+
+[package.source]
+type = "legacy"
+url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple"
+reference = "solutions-private-pypi"
+
+[[package]]
 name = "ansys-sphinx-theme"
 version = "0.8.2"
 description = "A theme devised by ANSYS, Inc. for Sphinx documentation."
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "ansys-sphinx-theme-0.8.2.tar.gz", hash = "sha256:eddff4954318e0cf924771d93bc128219669ecff0ddfb1d8d7d6c00f82b5771d"},
@@ -684,34 +719,39 @@
 ssh = ["bcrypt (>=3.1.5)"]
 test = ["hypothesis (>=1.11.4,!=3.79.2)", "iso8601", "pretend", "pytest (>=6.2.0)", "pytest-benchmark", "pytest-cov", "pytest-shard (>=0.1.2)", "pytest-subtests", "pytest-xdist", "pytz"]
 test-randomorder = ["pytest-randomly"]
 tox = ["tox"]
 
 [[package]]
 name = "dash"
-version = "2.10.2"
+version = "2.11.1"
 description = "A Python framework for building reactive web-apps. Developed by Plotly."
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "dash-2.10.2-py3-none-any.whl", hash = "sha256:f1b7132558bd2341e6cf7ca1e83e216d46bbb27a255ca962a0fa5561c6776953"},
-    {file = "dash-2.10.2.tar.gz", hash = "sha256:b99839890b44171da0e3668c2e607ef4b4f6948a6074c034693534ba52aa1d2b"},
+    {file = "dash-2.11.1-py3-none-any.whl", hash = "sha256:a5b55efc7f139538d95331fa0b5ee0d21600f7dafa9cce4fe4f887b773aba01a"},
+    {file = "dash-2.11.1.tar.gz", hash = "sha256:1acc4c634311cb306a1086fff315c1f2aaa3898bac362d93bc8db6b1a6474e5c"},
 ]
 
 [package.dependencies]
+ansi2html = "*"
 dash-core-components = "2.0.0"
 dash-html-components = "2.0.0"
 dash-table = "5.0.0"
 Flask = ">=1.0.4,<2.3.0"
+nest-asyncio = "*"
 plotly = ">=5.0.0"
+requests = "*"
+retrying = "*"
+typing-extensions = ">=4.1.1"
 Werkzeug = "<2.3.0"
 
 [package.extras]
 celery = ["celery[redis] (>=5.1.2)", "importlib-metadata (<5)", "redis (>=3.5.3)"]
-ci = ["black (==21.6b0)", "black (==22.3.0)", "dash-dangerously-set-inner-html", "dash-flow-example (==0.0.5)", "flake8 (==3.9.2)", "flaky (==3.7.0)", "flask-talisman (==1.0.0)", "isort (==4.3.21)", "mimesis", "mock (==4.0.3)", "numpy", "openpyxl", "orjson (==3.5.4)", "orjson (==3.6.7)", "pandas (==1.1.5)", "pandas (>=1.4.0)", "preconditions", "pyarrow", "pyarrow (<3)", "pylint (==2.13.5)", "pytest-mock", "pytest-rerunfailures", "pytest-sugar (==0.9.6)", "xlrd (<2)", "xlrd (>=2.0.1)"]
+ci = ["black (==21.6b0)", "black (==22.3.0)", "dash-dangerously-set-inner-html", "dash-flow-example (==0.0.5)", "flake8 (==3.9.2)", "flaky (==3.7.0)", "flask-talisman (==1.0.0)", "isort (==4.3.21)", "jupyterlab (<4.0.0)", "mimesis", "mock (==4.0.3)", "numpy", "openpyxl", "orjson (==3.5.4)", "orjson (==3.6.7)", "pandas (==1.1.5)", "pandas (>=1.4.0)", "preconditions", "pyarrow", "pyarrow (<3)", "pylint (==2.13.5)", "pytest-mock", "pytest-rerunfailures", "pytest-sugar (==0.9.6)", "xlrd (<2)", "xlrd (>=2.0.1)"]
 compress = ["flask-compress"]
 dev = ["PyYAML (>=5.4.1)", "coloredlogs (>=15.0.1)", "fire (>=0.4.0)"]
 diskcache = ["diskcache (>=5.2.1)", "multiprocess (>=0.70.12)", "psutil (>=5.8.0)"]
 testing = ["beautifulsoup4 (>=4.8.2)", "cryptography (<3.4)", "dash-testing-stub (>=0.0.2)", "lxml (>=4.6.2)", "multiprocess (>=0.70.12)", "percy (>=2.0.2)", "psutil (>=5.8.0)", "pytest (>=6.0.2)", "requests[security] (>=2.21.0)", "selenium (>=3.141.0,<=4.2.0)", "waitress (>=1.4.4)"]
 
 [[package]]
 name = "dash-bootstrap-components"
@@ -885,21 +925,21 @@
 files = [
     {file = "EditorConfig-0.12.3-py3-none-any.whl", hash = "sha256:6b0851425aa875b08b16789ee0eeadbd4ab59666e9ebe728e526314c4a2e52c1"},
     {file = "EditorConfig-0.12.3.tar.gz", hash = "sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.1.1"
+version = "1.1.2"
 description = "Backport of PEP 654 (exception groups)"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
-    {file = "exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
+    {file = "exceptiongroup-1.1.2-py3-none-any.whl", hash = "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"},
+    {file = "exceptiongroup-1.1.2.tar.gz", hash = "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "execnet"
@@ -1351,35 +1391,35 @@
 
 [package.dependencies]
 editorconfig = ">=0.12.2"
 six = ">=1.13.0"
 
 [[package]]
 name = "keyring"
-version = "23.13.1"
+version = "24.2.0"
 description = "Store and access your passwords safely."
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "keyring-23.13.1-py3-none-any.whl", hash = "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd"},
-    {file = "keyring-23.13.1.tar.gz", hash = "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"},
+    {file = "keyring-24.2.0-py3-none-any.whl", hash = "sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6"},
+    {file = "keyring-24.2.0.tar.gz", hash = "sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509"},
 ]
 
 [package.dependencies]
 importlib-metadata = {version = ">=4.11.4", markers = "python_version < \"3.12\""}
 importlib-resources = {version = "*", markers = "python_version < \"3.9\""}
 "jaraco.classes" = "*"
 jeepney = {version = ">=0.4.2", markers = "sys_platform == \"linux\""}
 pywin32-ctypes = {version = ">=0.2.0", markers = "sys_platform == \"win32\""}
 SecretStorage = {version = ">=3.2", markers = "sys_platform == \"linux\""}
 
 [package.extras]
 completion = ["shtab"]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)"]
-testing = ["flake8 (<5)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
+testing = ["pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-ruff"]
 
 [[package]]
 name = "markdown-it-py"
 version = "3.0.0"
 description = "Python port of markdown-it. Markdown parsing, done right!"
 optional = false
 python-versions = ">=3.8"
@@ -1506,14 +1546,25 @@
 python-versions = ">=3.7"
 files = [
     {file = "more-itertools-9.1.0.tar.gz", hash = "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d"},
     {file = "more_itertools-9.1.0-py3-none-any.whl", hash = "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"},
 ]
 
 [[package]]
+name = "nest-asyncio"
+version = "1.5.6"
+description = "Patch asyncio to allow nested event loops"
+optional = false
+python-versions = ">=3.5"
+files = [
+    {file = "nest_asyncio-1.5.6-py3-none-any.whl", hash = "sha256:b9a953fb40dceaa587d109609098db21900182b16440652454a146cffb06e8b8"},
+    {file = "nest_asyncio-1.5.6.tar.gz", hash = "sha256:d267cc1ff794403f7df692964d1d2a3fa9418ffea2a3f6859a439ff482fef290"},
+]
+
+[[package]]
 name = "networkx"
 version = "3.1"
 description = "Python package for creating and manipulating graphs and networks"
 optional = false
 python-versions = ">=3.8"
 files = [
     {file = "networkx-3.1-py3-none-any.whl", hash = "sha256:4f33f68cb2afcf86f28a45f43efc27a9386b535d567d2127f8f61d51dec58d36"},
@@ -1861,21 +1912,21 @@
 ]
 
 [package.extras]
 testing = ["pytest", "pytest-cov"]
 
 [[package]]
 name = "platformdirs"
-version = "3.6.0"
+version = "3.8.0"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-3.6.0-py3-none-any.whl", hash = "sha256:ffa199e3fbab8365778c4a10e1fbf1b9cd50707de826eb304b50e57ec0cc8d38"},
-    {file = "platformdirs-3.6.0.tar.gz", hash = "sha256:57e28820ca8094678b807ff529196506d7a21e17156cb1cddb3e74cebce54640"},
+    {file = "platformdirs-3.8.0-py3-none-any.whl", hash = "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"},
+    {file = "platformdirs-3.8.0.tar.gz", hash = "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc"},
 ]
 
 [package.extras]
 docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
@@ -1891,21 +1942,21 @@
 
 [package.dependencies]
 packaging = "*"
 tenacity = ">=6.2.0"
 
 [[package]]
 name = "pluggy"
-version = "1.0.0"
+version = "1.2.0"
 description = "plugin and hook calling mechanisms for python"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
-    {file = "pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
+    {file = "pluggy-1.2.0-py3-none-any.whl", hash = "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849"},
+    {file = "pluggy-1.2.0.tar.gz", hash = "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"},
 ]
 
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
@@ -1997,55 +2048,55 @@
 files = [
     {file = "pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
     {file = "pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
 ]
 
 [[package]]
 name = "pydantic"
-version = "1.10.9"
+version = "1.10.10"
 description = "Data validation and settings management using python type hints"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pydantic-1.10.9-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e692dec4a40bfb40ca530e07805b1208c1de071a18d26af4a2a0d79015b352ca"},
-    {file = "pydantic-1.10.9-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:3c52eb595db83e189419bf337b59154bdcca642ee4b2a09e5d7797e41ace783f"},
-    {file = "pydantic-1.10.9-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:939328fd539b8d0edf244327398a667b6b140afd3bf7e347cf9813c736211896"},
-    {file = "pydantic-1.10.9-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b48d3d634bca23b172f47f2335c617d3fcb4b3ba18481c96b7943a4c634f5c8d"},
-    {file = "pydantic-1.10.9-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:f0b7628fb8efe60fe66fd4adadd7ad2304014770cdc1f4934db41fe46cc8825f"},
-    {file = "pydantic-1.10.9-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:e1aa5c2410769ca28aa9a7841b80d9d9a1c5f223928ca8bec7e7c9a34d26b1d4"},
-    {file = "pydantic-1.10.9-cp310-cp310-win_amd64.whl", hash = "sha256:eec39224b2b2e861259d6f3c8b6290d4e0fbdce147adb797484a42278a1a486f"},
-    {file = "pydantic-1.10.9-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:d111a21bbbfd85c17248130deac02bbd9b5e20b303338e0dbe0faa78330e37e0"},
-    {file = "pydantic-1.10.9-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:2e9aec8627a1a6823fc62fb96480abe3eb10168fd0d859ee3d3b395105ae19a7"},
-    {file = "pydantic-1.10.9-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:07293ab08e7b4d3c9d7de4949a0ea571f11e4557d19ea24dd3ae0c524c0c334d"},
-    {file = "pydantic-1.10.9-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7ee829b86ce984261d99ff2fd6e88f2230068d96c2a582f29583ed602ef3fc2c"},
-    {file = "pydantic-1.10.9-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:4b466a23009ff5cdd7076eb56aca537c745ca491293cc38e72bf1e0e00de5b91"},
-    {file = "pydantic-1.10.9-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:7847ca62e581e6088d9000f3c497267868ca2fa89432714e21a4fb33a04d52e8"},
-    {file = "pydantic-1.10.9-cp311-cp311-win_amd64.whl", hash = "sha256:7845b31959468bc5b78d7b95ec52fe5be32b55d0d09983a877cca6aedc51068f"},
-    {file = "pydantic-1.10.9-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:517a681919bf880ce1dac7e5bc0c3af1e58ba118fd774da2ffcd93c5f96eaece"},
-    {file = "pydantic-1.10.9-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:67195274fd27780f15c4c372f4ba9a5c02dad6d50647b917b6a92bf00b3d301a"},
-    {file = "pydantic-1.10.9-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2196c06484da2b3fded1ab6dbe182bdabeb09f6318b7fdc412609ee2b564c49a"},
-    {file = "pydantic-1.10.9-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:6257bb45ad78abacda13f15bde5886efd6bf549dd71085e64b8dcf9919c38b60"},
-    {file = "pydantic-1.10.9-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3283b574b01e8dbc982080d8287c968489d25329a463b29a90d4157de4f2baaf"},
-    {file = "pydantic-1.10.9-cp37-cp37m-win_amd64.whl", hash = "sha256:5f8bbaf4013b9a50e8100333cc4e3fa2f81214033e05ac5aa44fa24a98670a29"},
-    {file = "pydantic-1.10.9-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:b9cd67fb763248cbe38f0593cd8611bfe4b8ad82acb3bdf2b0898c23415a1f82"},
-    {file = "pydantic-1.10.9-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f50e1764ce9353be67267e7fd0da08349397c7db17a562ad036aa7c8f4adfdb6"},
-    {file = "pydantic-1.10.9-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:73ef93e5e1d3c8e83f1ff2e7fdd026d9e063c7e089394869a6e2985696693766"},
-    {file = "pydantic-1.10.9-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:128d9453d92e6e81e881dd7e2484e08d8b164da5507f62d06ceecf84bf2e21d3"},
-    {file = "pydantic-1.10.9-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ad428e92ab68798d9326bb3e5515bc927444a3d71a93b4a2ca02a8a5d795c572"},
-    {file = "pydantic-1.10.9-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:fab81a92f42d6d525dd47ced310b0c3e10c416bbfae5d59523e63ea22f82b31e"},
-    {file = "pydantic-1.10.9-cp38-cp38-win_amd64.whl", hash = "sha256:963671eda0b6ba6926d8fc759e3e10335e1dc1b71ff2a43ed2efd6996634dafb"},
-    {file = "pydantic-1.10.9-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:970b1bdc6243ef663ba5c7e36ac9ab1f2bfecb8ad297c9824b542d41a750b298"},
-    {file = "pydantic-1.10.9-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:7e1d5290044f620f80cf1c969c542a5468f3656de47b41aa78100c5baa2b8276"},
-    {file = "pydantic-1.10.9-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:83fcff3c7df7adff880622a98022626f4f6dbce6639a88a15a3ce0f96466cb60"},
-    {file = "pydantic-1.10.9-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0da48717dc9495d3a8f215e0d012599db6b8092db02acac5e0d58a65248ec5bc"},
-    {file = "pydantic-1.10.9-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:0a2aabdc73c2a5960e87c3ffebca6ccde88665616d1fd6d3db3178ef427b267a"},
-    {file = "pydantic-1.10.9-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:9863b9420d99dfa9c064042304868e8ba08e89081428a1c471858aa2af6f57c4"},
-    {file = "pydantic-1.10.9-cp39-cp39-win_amd64.whl", hash = "sha256:e7c9900b43ac14110efa977be3da28931ffc74c27e96ee89fbcaaf0b0fe338e1"},
-    {file = "pydantic-1.10.9-py3-none-any.whl", hash = "sha256:6cafde02f6699ce4ff643417d1a9223716ec25e228ddc3b436fe7e2d25a1f305"},
-    {file = "pydantic-1.10.9.tar.gz", hash = "sha256:95c70da2cd3b6ddf3b9645ecaa8d98f3d80c606624b6d245558d202cd23ea3be"},
+    {file = "pydantic-1.10.10-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:adad1ee4ab9888f12dac2529276704e719efcf472e38df7813f5284db699b4ec"},
+    {file = "pydantic-1.10.10-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:7a7db03339893feef2092ff7b1afc9497beed15ebd4af84c3042a74abce02d48"},
+    {file = "pydantic-1.10.10-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:67b3714b97ff84b2689654851c2426389bcabfac9080617bcf4306c69db606f6"},
+    {file = "pydantic-1.10.10-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:edfdf0a5abc5c9bf2052ebaec20e67abd52e92d257e4f2d30e02c354ed3e6030"},
+    {file = "pydantic-1.10.10-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:20a3b30fd255eeeb63caa9483502ba96b7795ce5bf895c6a179b3d909d9f53a6"},
+    {file = "pydantic-1.10.10-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:db4c7f7e60ca6f7d6c1785070f3e5771fcb9b2d88546e334d2f2c3934d949028"},
+    {file = "pydantic-1.10.10-cp310-cp310-win_amd64.whl", hash = "sha256:a2d5be50ac4a0976817144c7d653e34df2f9436d15555189f5b6f61161d64183"},
+    {file = "pydantic-1.10.10-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:566a04ba755e8f701b074ffb134ddb4d429f75d5dced3fbd829a527aafe74c71"},
+    {file = "pydantic-1.10.10-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f79db3652ed743309f116ba863dae0c974a41b688242482638b892246b7db21d"},
+    {file = "pydantic-1.10.10-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c62376890b819bebe3c717a9ac841a532988372b7e600e76f75c9f7c128219d5"},
+    {file = "pydantic-1.10.10-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4870f13a4fafd5bc3e93cff3169222534fad867918b188e83ee0496452978437"},
+    {file = "pydantic-1.10.10-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:990027e77cda6072a566e433b6962ca3b96b4f3ae8bd54748e9d62a58284d9d7"},
+    {file = "pydantic-1.10.10-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8c40964596809eb616d94f9c7944511f620a1103d63d5510440ed2908fc410af"},
+    {file = "pydantic-1.10.10-cp311-cp311-win_amd64.whl", hash = "sha256:ea9eebc2ebcba3717e77cdeee3f6203ffc0e78db5f7482c68b1293e8cc156e5e"},
+    {file = "pydantic-1.10.10-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:762aa598f79b4cac2f275d13336b2dd8662febee2a9c450a49a2ab3bec4b385f"},
+    {file = "pydantic-1.10.10-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6dab5219659f95e357d98d70577b361383057fb4414cfdb587014a5f5c595f7b"},
+    {file = "pydantic-1.10.10-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f3d4ee957a727ccb5a36f1b0a6dbd9fad5dedd2a41eada99a8df55c12896e18d"},
+    {file = "pydantic-1.10.10-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:b69f9138dec566962ec65623c9d57bee44412d2fc71065a5f3ebb3820bdeee96"},
+    {file = "pydantic-1.10.10-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:7aa75d1bd9cc275cf9782f50f60cddaf74cbaae19b6ada2a28e737edac420312"},
+    {file = "pydantic-1.10.10-cp37-cp37m-win_amd64.whl", hash = "sha256:9f62a727f5c590c78c2d12fda302d1895141b767c6488fe623098f8792255fe5"},
+    {file = "pydantic-1.10.10-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:aac218feb4af73db8417ca7518fb3bade4534fcca6e3fb00f84966811dd94450"},
+    {file = "pydantic-1.10.10-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:88546dc10a40b5b52cae87d64666787aeb2878f9a9b37825aedc2f362e7ae1da"},
+    {file = "pydantic-1.10.10-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c41bbaae89e32fc582448e71974de738c055aef5ab474fb25692981a08df808a"},
+    {file = "pydantic-1.10.10-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2b71bd504d1573b0b722ae536e8ffb796bedeef978979d076bf206e77dcc55a5"},
+    {file = "pydantic-1.10.10-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:e088e3865a2270ecbc369924cd7d9fbc565667d9158e7f304e4097ebb9cf98dd"},
+    {file = "pydantic-1.10.10-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:3403a090db45d4027d2344859d86eb797484dfda0706cf87af79ace6a35274ef"},
+    {file = "pydantic-1.10.10-cp38-cp38-win_amd64.whl", hash = "sha256:e0014e29637125f4997c174dd6167407162d7af0da73414a9340461ea8573252"},
+    {file = "pydantic-1.10.10-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:9965e49c6905840e526e5429b09e4c154355b6ecc0a2f05492eda2928190311d"},
+    {file = "pydantic-1.10.10-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:748d10ab6089c5d196e1c8be9de48274f71457b01e59736f7a09c9dc34f51887"},
+    {file = "pydantic-1.10.10-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:86936c383f7c38fd26d35107eb669c85d8f46dfceae873264d9bab46fe1c7dde"},
+    {file = "pydantic-1.10.10-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7a26841be620309a9697f5b1ffc47dce74909e350c5315ccdac7a853484d468a"},
+    {file = "pydantic-1.10.10-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:409b810f387610cc7405ab2fa6f62bdf7ea485311845a242ebc0bd0496e7e5ac"},
+    {file = "pydantic-1.10.10-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:ce937a2a2c020bcad1c9fde02892392a1123de6dda906ddba62bfe8f3e5989a2"},
+    {file = "pydantic-1.10.10-cp39-cp39-win_amd64.whl", hash = "sha256:37ebddef68370e6f26243acc94de56d291e01227a67b2ace26ea3543cf53dd5f"},
+    {file = "pydantic-1.10.10-py3-none-any.whl", hash = "sha256:a5939ec826f7faec434e2d406ff5e4eaf1716eb1f247d68cd3d0b3612f7b4c8a"},
+    {file = "pydantic-1.10.10.tar.gz", hash = "sha256:3b8d5bd97886f9eb59260594207c9f57dce14a6f869c6ceea90188715d29921a"},
 ]
 
 [package.dependencies]
 typing-extensions = ">=4.2.0"
 
 [package.extras]
 dotenv = ["python-dotenv (>=0.10.4)"]
@@ -2133,14 +2184,35 @@
     {file = "pyobjc_framework_Cocoa-9.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:b236bb965e41aeb2e215d4e98a5a230d4b63252c6d26e00924ea2e69540a59d6"},
 ]
 
 [package.dependencies]
 pyobjc-core = ">=9.2"
 
 [[package]]
+name = "pyobjc-framework-security"
+version = "9.2"
+description = "Wrappers for the framework Security on macOS"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "pyobjc-framework-Security-9.2.tar.gz", hash = "sha256:8d4f7a22db2fe666c7bff4a5825b49d2345e9a8d96ea085f1a614ad9a559b4e5"},
+    {file = "pyobjc_framework_Security-9.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:06137e1dd28af61f9966e1dfddba4ff7dc25d3d77f49f9af47bb4791492e58ce"},
+    {file = "pyobjc_framework_Security-9.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:ca272397da447897d73e1b72ae0acddadfefbb575e452b85028b2d7ae13b0fc7"},
+    {file = "pyobjc_framework_Security-9.2-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:f9cfb6c44cefe7d6456ddfdda569867254a271d8fef10500e86456a105e255b9"},
+    {file = "pyobjc_framework_Security-9.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:3d627e92688dfb31a0399f12283256717e5a1bd05b2abfd8b470621f955995a3"},
+    {file = "pyobjc_framework_Security-9.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0f9435986f7cf74d22a2920a5d85d922e24caa3b5b2911fb6d07c3b89f9973f9"},
+    {file = "pyobjc_framework_Security-9.2-cp38-cp38-macosx_11_0_universal2.whl", hash = "sha256:aa18fbb458edf04b0c34d13443a4665aeff4ae90ee644f008cd58146740f166d"},
+    {file = "pyobjc_framework_Security-9.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:8be7f51fc483532100853a570d62570f553fce5d7e101a572ad70198acfc9a8e"},
+]
+
+[package.dependencies]
+pyobjc-core = ">=9.2"
+pyobjc-framework-Cocoa = ">=9.2"
+
+[[package]]
 name = "pyobjc-framework-webkit"
 version = "9.2"
 description = "Wrappers for the framework WebKit on macOS"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pyobjc-framework-WebKit-9.2.tar.gz", hash = "sha256:86761cba8c18c3d2ecbd3ca7ab8b92c8b2eae8514741ec63527b536b671ab296"},
@@ -2184,21 +2256,21 @@
 ]
 
 [package.dependencies]
 pywin32 = {version = "*", markers = "platform_system == \"Windows\""}
 
 [[package]]
 name = "pytest"
-version = "7.3.2"
+version = "7.4.0"
 description = "pytest: simple powerful testing with Python"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pytest-7.3.2-py3-none-any.whl", hash = "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295"},
-    {file = "pytest-7.3.2.tar.gz", hash = "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"},
+    {file = "pytest-7.4.0-py3-none-any.whl", hash = "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32"},
+    {file = "pytest-7.4.0.tar.gz", hash = "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "sys_platform == \"win32\""}
 exceptiongroup = {version = ">=1.0.0rc8", markers = "python_version < \"3.11\""}
 iniconfig = "*"
 packaging = "*"
@@ -2409,35 +2481,37 @@
 files = [
     {file = "pytz-2023.3-py2.py3-none-any.whl", hash = "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"},
     {file = "pytz-2023.3.tar.gz", hash = "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588"},
 ]
 
 [[package]]
 name = "pywebview"
-version = "4.1"
-description = "Build GUI for your Python program with JavaScript, HTML, and CSS."
+version = "4.2.2"
+description = "Build GUI for your Python program with JavaScript, HTML, and CSS"
 optional = false
-python-versions = "*"
+python-versions = ">=3.7"
 files = [
-    {file = "pywebview-4.1-py3-none-any.whl", hash = "sha256:d4945c3be285b1046f812032fff882cf640547b63be132016730ad5a11153304"},
-    {file = "pywebview-4.1.tar.gz", hash = "sha256:62efa24fff0b35fb8028556b6d44fc1c698a1deefa8df2c5557909af54679450"},
+    {file = "pywebview-4.2.2-py3-none-any.whl", hash = "sha256:1db26c0fcf9e856195467464b2a3e00189d231457189a102747d4a8694c974e4"},
+    {file = "pywebview-4.2.2.tar.gz", hash = "sha256:85be4215cd65ceacca5c7faef9d271e10bfe3ca25d2498c1c6d2e59a4d56e86c"},
 ]
 
 [package.dependencies]
 bottle = "*"
 proxy-tools = "*"
 pyobjc-core = {version = "*", markers = "sys_platform == \"darwin\""}
 pyobjc-framework-Cocoa = {version = "*", markers = "sys_platform == \"darwin\""}
+pyobjc-framework-security = {version = "*", markers = "sys_platform == \"darwin\""}
 pyobjc-framework-WebKit = {version = "*", markers = "sys_platform == \"darwin\""}
 pythonnet = {version = "*", markers = "sys_platform == \"win32\""}
 QtPy = {version = "*", markers = "sys_platform == \"openbsd6\""}
+typing-extensions = "*"
 
 [package.extras]
 cef = ["cefpython3"]
-gtk = ["PyGObject"]
+gtk = ["PyGObject", "PyGObject-stubs"]
 pyside2 = ["PySide2", "QtPy"]
 pyside6 = ["PySide6", "QtPy"]
 qt = ["PyQt5", "QtPy", "pyqtwebengine"]
 
 [[package]]
 name = "pywin32"
 version = "306"
@@ -2459,21 +2533,21 @@
     {file = "pywin32-306-cp38-cp38-win_amd64.whl", hash = "sha256:e8ac1ae3601bee6ca9f7cb4b5363bf1c0badb935ef243c4733ff9a393b1690c0"},
     {file = "pywin32-306-cp39-cp39-win32.whl", hash = "sha256:e25fd5b485b55ac9c057f67d94bc203f3f6595078d1fb3b458c9c28b7153a802"},
     {file = "pywin32-306-cp39-cp39-win_amd64.whl", hash = "sha256:39b61c15272833b5c329a2989999dcae836b1eed650252ab1b7bfbe1d59f30f4"},
 ]
 
 [[package]]
 name = "pywin32-ctypes"
-version = "0.2.1"
+version = "0.2.2"
 description = "A (partial) reimplementation of pywin32 using ctypes/cffi"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "pywin32-ctypes-0.2.1.tar.gz", hash = "sha256:934a2def1e5cbc472b2b6bf80680c0f03cd87df65dfd58bfd1846969de095b03"},
-    {file = "pywin32_ctypes-0.2.1-py3-none-any.whl", hash = "sha256:b9a53ef754c894a525469933ab2a447c74ec1ea6b9d2ef446f40ec50d3dcec9f"},
+    {file = "pywin32-ctypes-0.2.2.tar.gz", hash = "sha256:3426e063bdd5fd4df74a14fa3cf80a0b42845a87e1d1e81f6549f9daec593a60"},
+    {file = "pywin32_ctypes-0.2.2-py3-none-any.whl", hash = "sha256:bf490a1a709baf35d688fe0ecf980ed4de11d2b3e37b51e5442587a75d9957e7"},
 ]
 
 [[package]]
 name = "pyyaml"
 version = "6.0"
 description = "YAML parser and emitter for Python"
 optional = false
@@ -2536,21 +2610,21 @@
 packaging = "*"
 
 [package.extras]
 test = ["pytest (>=6,!=7.0.0,!=7.0.1)", "pytest-cov (>=3.0.0)", "pytest-qt"]
 
 [[package]]
 name = "readme-renderer"
-version = "37.3"
+version = "40.0"
 description = "readme_renderer is a library for rendering \"readme\" descriptions for Warehouse"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "readme_renderer-37.3-py3-none-any.whl", hash = "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"},
-    {file = "readme_renderer-37.3.tar.gz", hash = "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273"},
+    {file = "readme_renderer-40.0-py3-none-any.whl", hash = "sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a"},
+    {file = "readme_renderer-40.0.tar.gz", hash = "sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4"},
 ]
 
 [package.dependencies]
 bleach = ">=2.1.0"
 docutils = ">=0.13.1"
 Pygments = ">=2.5.1"
 
@@ -2589,14 +2663,28 @@
     {file = "requests_toolbelt-1.0.0-py2.py3-none-any.whl", hash = "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"},
 ]
 
 [package.dependencies]
 requests = ">=2.0.1,<3.0.0"
 
 [[package]]
+name = "retrying"
+version = "1.3.4"
+description = "Retrying"
+optional = false
+python-versions = "*"
+files = [
+    {file = "retrying-1.3.4-py3-none-any.whl", hash = "sha256:8cc4d43cb8e1125e0ff3344e9de678fefd85db3b750b81b2240dc0183af37b35"},
+    {file = "retrying-1.3.4.tar.gz", hash = "sha256:345da8c5765bd982b1d1915deb9102fd3d1f7ad16bd84a9700b85f64d24e8f3e"},
+]
+
+[package.dependencies]
+six = ">=1.7.0"
+
+[[package]]
 name = "rfc3986"
 version = "1.5.0"
 description = "Validating URI References per RFC 3986"
 optional = false
 python-versions = "*"
 files = [
     {file = "rfc3986-1.5.0-py2.py3-none-any.whl", hash = "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"},
@@ -2933,60 +3021,60 @@
 
 [package.extras]
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sqlalchemy"
-version = "2.0.16"
+version = "2.0.17"
 description = "Database Abstraction Library"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:7641f6ed2682de84d77c4894cf2e43700f3cf7a729361d7f9cac98febf3d8614"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8d3cbdb2f07fb0e4b897dc1df39166735e194fb946f28f26f4c9f9801c8b24f7"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a08a791c75d6154d46914d1e23bd81d9455f2950ec1de81f2723848c593d2c8b"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:91eb8f89fcce8f709f8a4d65d265bc48a80264ee14c7c9e955f3222f19b4b39c"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:fc1dae11bd5167f9eb53b3ccad24a79813004612141e76de21cf4c028dc30b34"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b2801f85c5c0293aa710f8aa5262c707a83c1c203962ae5a22b4d9095e71aa9d"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-win32.whl", hash = "sha256:c5e333b81fe10d14efebd4e9429b7bb865ed9463ca8bef07a7136dfa1fd4a37b"},
-    {file = "SQLAlchemy-2.0.16-cp310-cp310-win_amd64.whl", hash = "sha256:f387b496a4c9474d8580195bb2660264a3f295a04d3a9d00f4fa15e9e597427e"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:7be04dbe3470fe8dd332fdb48c979887c381ef6c635eddf2dec43d2766111be4"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f2938edc512dd1fa48653e14c1655ab46144d4450f0e6b33da7acd8ba77fbfd7"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a5a2856e12cf5f54301ddf043bcbf0552561d61555e1bcf348b63f42b8e1eec2"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:90d320fde566b864adbc19abb40ecb80f4e25d6f084639969bb972d5cca16858"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:6e85e315725807c127ad8ba3d628fdb861cf9ebfb0e10c39a97c01e257cdd71b"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:63ea36c08792a7a8a08958bc806ecff6b491386feeaf14607c3d9d2d9325e67f"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-win32.whl", hash = "sha256:bdaf89dd82f4a0e1b8b5ffc9cdc0c9551be6175f7eee5af6a838e92ba2e57100"},
-    {file = "SQLAlchemy-2.0.16-cp311-cp311-win_amd64.whl", hash = "sha256:5a934eff1a2882137be3384826f997db8441d43b61fda3094923e69fffe474be"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:fbcc51fdbc89fafe4f4fe66f59372a8be88ded04de34ef438ab04f980beb12d4"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ff6496ad5e9dc8baeb93a151cc2f599d01e5f8928a2aaf0b09a06428fdbaf553"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8d6ef848e5afcd1bda3e9a843751f845c0ca888b61e669237680e913d84ec206"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:3ef876615ff4b53e2033022195830ec4941a6e21068611f8d77de60203b90a98"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:8544c6e62eacb77d5106e2055ef10f2407fc0dbd547e879f8745b2032eefd2bc"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-win32.whl", hash = "sha256:2f3b6c31b915159b96b68372212fa77f69230b0a32acab40cf539d2823954f5a"},
-    {file = "SQLAlchemy-2.0.16-cp37-cp37m-win_amd64.whl", hash = "sha256:d0c96592f54edd571e00ba6b1ed5df8263328ca1da9e78088c0ebc93c2e6562c"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:a2e9f50a906d0b81292576a9fb458f8cace904c81a67088f4a2ca9ff2856f55d"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:dc97238fa44be86971270943a0c21c19ce18b8d1596919048e57912e8abc02cc"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0db6734cb5644c55d0262a813b764c6e2cda1e66e939a488b3d6298cdc7344c2"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:131f0c894c6572cb1bdcf97c92d999d3128c4ff1ca13061296057072f61afe13"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:f662cf69484c59f8a3435902c40dfc34d86050bdb15e23d437074ce9f153306b"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:b72f4e4def50414164a1d899f2ce4e782a029fad0ed5585981d1611e8ae29a74"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-win32.whl", hash = "sha256:0e4645b260cfe375a0603aa117f0a47680864cf37833129da870919e88b08d8f"},
-    {file = "SQLAlchemy-2.0.16-cp38-cp38-win_amd64.whl", hash = "sha256:f409f35a0330ab0cb18ece736b86d8b8233c64f4461fcb10993f67afc0ac7e5a"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:e19546924f0cf2ec930d1faf318b7365e5827276410a513340f31a2b423e96a4"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:ce1fc3f64fd42d5f763d6b83651471f32920338a1ba107a3186211474861af57"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8e2569dac4e3cb85365b91ab569d06a221e0e17e65ce59949d00c3958946282b"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:61f2035dea56ff1a429077e481496f813378beb02b823d2e3e7eb05bc1a7a8ca"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:81d867c1be5abd49f7e547c108391f371a9d980ba7ec34666c50d683f782b754"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:2de1477af7f48c633b8ecb88245aedd811dca88e88aee9e9d787b388abe74c44"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-win32.whl", hash = "sha256:5e8522b49e0e640287308b68f71cc338446bbe1c226c8f81743baa91b0246e92"},
-    {file = "SQLAlchemy-2.0.16-cp39-cp39-win_amd64.whl", hash = "sha256:43e69c8c1cea0188b7094e22fb93ae1a1890aac748628b7e925024a206f75368"},
-    {file = "SQLAlchemy-2.0.16-py3-none-any.whl", hash = "sha256:53081c6fce0d49bb36d05f12dc87e008c9b0df58a163b792c5fc4ac638925f98"},
-    {file = "SQLAlchemy-2.0.16.tar.gz", hash = "sha256:1e2caba78e7d1f5003e88817b7a1754d4e58f4a8f956dc423bf8e304c568ab09"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:04383f1e3452f6739084184e427e9d5cb4e68ddc765d52157bf5ef30d5eca14f"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:724355973297bbe547f3eb98b46ade65a67a3d5a6303f17ab59a2dc6fb938943"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cf07ff9920cb3ca9d73525dfd4f36ddf9e1a83734ea8b4f724edfd9a2c6e82d9"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f2f389f77c68dc22cb51f026619291c4a38aeb4b7ecb5f998fd145b2d81ca513"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ba03518e64d86f000dc24ab3d3a1aa876bcbaa8aa15662ac2df5e81537fa3394"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:218fb20c01e95004f50a3062bf4c447dcb360cab8274232f31947e254f118298"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-win32.whl", hash = "sha256:b47be4c6281a86670ea5cfbbbe6c3a65366a8742f5bc8b986f790533c60b5ddb"},
+    {file = "SQLAlchemy-2.0.17-cp310-cp310-win_amd64.whl", hash = "sha256:74ddcafb6488f382854a7da851c404c394be3729bb3d91b02ad86c5458140eff"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:51736cfb607cf4e8fafb693906f9bc4e5ee55be0b096d44bd7f20cd8489b8571"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8741d3d401383e54b2aada37cbd10f55c5d444b360eae3a82f74a2be568a7710"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ead58cae2a089eee1b0569060999cb5f2b2462109498a0937cc230a7556945a1"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5f40e3a7d0a464f1c8593f2991e5520b2f5b26da24e88000bbd4423f86103d4f"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:21583808d37f126a647652c90332ac1d3a102edf3c94bcc3319edcc0ea2300cc"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:f593170fc09c5abb1205a738290b39532f7380094dc151805009a07ae0e85330"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-win32.whl", hash = "sha256:b0eaf82cc844f6b46defe15ad243ea00d1e39ed3859df61130c263dc7204da6e"},
+    {file = "SQLAlchemy-2.0.17-cp311-cp311-win_amd64.whl", hash = "sha256:1822620c89779b85f7c23d535c8e04b79c517739ae07aaed48c81e591ed5498e"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:2269b1f9b8be47e52b70936069a25a3771eff53367aa5cc59bb94f28a6412e13"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:48111d56afea5699bab72c38ec95561796b81befff9e13d1dd5ce251ab25f51d"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:28da17059ecde53e2d10ba813d38db942b9f6344360b2958b25872d5cb729d35"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:48b40dc2895841ea89d89df9eb3ac69e2950a659db20a369acf4259f68e6dc1f"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:7f31d4e7ca1dd8ca5a27fd5eaa0f9e2732fe769ff7dd35bf7bba179597e4df07"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-win32.whl", hash = "sha256:7830e01b02d440c27f2a5be68296e74ccb55e6a5b5962ffafd360b98930b2e5e"},
+    {file = "SQLAlchemy-2.0.17-cp37-cp37m-win_amd64.whl", hash = "sha256:234678ed6576531b8e4be255b980f20368bf07241a2e67b84e6b0fe679edb9c4"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2c6ff5767d954f6091113fedcaaf49cdec2197ae4c5301fe83d5ae4393c82f33"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:aa995b21f853864996e4056d9fde479bcecf8b7bff4beb3555eebbbba815f35d"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:125f9f7e62ddf8b590c069729080ffe18b68a20d9882eb0947f72e06274601d7"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b114a16bc03dfe20b625062e456affd7b9938286e05a3f904a025b9aacc29dd4"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:cf175d26f6787cce30fe6c04303ca0aeeb0ad40eeb22e3391f24b32ec432a1e1"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:e2d5c3596254cf1a96474b98e7ce20041c74c008b0f101c1cb4f8261cb77c6d3"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-win32.whl", hash = "sha256:513411d73503a6fc5804f01fae3b3d44f267c1b3a06cfeac02e9286a7330e857"},
+    {file = "SQLAlchemy-2.0.17-cp38-cp38-win_amd64.whl", hash = "sha256:40a3dc52b2b16f08b5c16b9ee7646329e4b3411e9280e5e8d57b19eaa51cbef4"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:e3189432db2f5753b4fde1aa90a61c69976f4e7e31d1cf4611bfe3514ed07478"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:6150560fcffc6aee5ec9a97419ac768c7a9f56baf7a7eb59cb4b1b6a4d463ad9"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:910d45bf3673f0e4ef13858674bd23cfdafdc8368b45b948bf511797dbbb401d"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d0aeb3afaa19f187a70fa592fbe3c20a056b57662691fd3abf60f016aa5c1848"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:36a87e26fe8fa8c466fae461a8fcb780d0a1cbf8206900759fc6fe874475a3ce"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:e3a6b2788f193756076061626679c5c5a6d600ddf8324f986bc72004c3e9d92e"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-win32.whl", hash = "sha256:af7e2ba75bf84b64adb331918188dda634689a2abb151bc1a583e488363fd2f8"},
+    {file = "SQLAlchemy-2.0.17-cp39-cp39-win_amd64.whl", hash = "sha256:394ac3adf3676fad76d4b8fcecddf747627f17f0738dc94bac15f303d05b03d4"},
+    {file = "SQLAlchemy-2.0.17-py3-none-any.whl", hash = "sha256:cc9c2630c423ac4973492821b2969f5fe99d9736f3025da670095668fbfcd4d5"},
+    {file = "SQLAlchemy-2.0.17.tar.gz", hash = "sha256:e186e9e95fb5d993b075c33fe4f38a22105f7ce11cecb5c17b5618181e356702"},
 ]
 
 [package.dependencies]
 greenlet = {version = "!=0.4.17", markers = "platform_machine == \"win32\" or platform_machine == \"WIN32\" or platform_machine == \"AMD64\" or platform_machine == \"amd64\" or platform_machine == \"x86_64\" or platform_machine == \"ppc64le\" or platform_machine == \"aarch64\""}
 typing-extensions = ">=4.2.0"
 
 [package.extras]
@@ -3065,21 +3153,21 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tox"
-version = "4.6.2"
+version = "4.6.3"
 description = "tox is a generic virtualenv management and test command line tool"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "tox-4.6.2-py3-none-any.whl", hash = "sha256:52241851a7b0cd7de07d6ef067a13b092d2a4f82fe9048efb2444aed1708d713"},
-    {file = "tox-4.6.2.tar.gz", hash = "sha256:58c7c2acce2f3d44cd1b359349557162336288ecf19ef53ccda89c9cee0ad9c4"},
+    {file = "tox-4.6.3-py3-none-any.whl", hash = "sha256:2946a0bb38924c3a9f9575c7fb4ca1f4c11a7c69c61592f176778892155cb50c"},
+    {file = "tox-4.6.3.tar.gz", hash = "sha256:9e2c5091a117d03b583c57c4c40aecd068099c17d40520e7b165e85c19334534"},
 ]
 
 [package.dependencies]
 cachetools = ">=5.3.1"
 chardet = ">=5.1"
 colorama = ">=0.4.6"
 filelock = ">=3.12.2"
@@ -3114,21 +3202,21 @@
 requests-toolbelt = ">=0.8.0,<0.9.0 || >0.9.0"
 rfc3986 = ">=1.4.0"
 rich = ">=12.0.0"
 urllib3 = ">=1.26.0"
 
 [[package]]
 name = "typing-extensions"
-version = "4.6.3"
+version = "4.7.1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "typing_extensions-4.6.3-py3-none-any.whl", hash = "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26"},
-    {file = "typing_extensions-4.6.3.tar.gz", hash = "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"},
+    {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
+    {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 
 [[package]]
 name = "urllib3"
 version = "2.0.3"
 description = "HTTP library with thread-safe connection pooling, file post, and more."
 optional = false
@@ -3322,8 +3410,8 @@
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = ">=3.8, <3.11"
-content-hash = "37bcd1b8ebc4798b7c93e760a6dc1e837d6c458ceb86b75275aeba7c98ba4563"
+content-hash = "876ce19b6752cb197a31e95094df26a76c09fe9f3ecd2cefffea5de5c4f94bae"
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,113 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
-# CAPTURED v0.4.0 on 6/6/23 from:
+# CAPTURED v0.5.1 on 7/4/23 from:
 # https://github.com/Solution-Applications/common-files/blob/v0.4.0/setup-environment/setup_environment.py
 
 """
-A Python script to automate the setup of the ecosystem of a Python project.
+A Python script to automate the setup of the Python ecosystem of a project.
 
-Usage
------
+Prerequisites
+-------------
 
-This script needs to be executed at project's root.
+1. The following packages are required:
+    * packaging
+    * toml
 
-To create a virtual environment and install the dependency management system of the project (if any):
-    ``python setup_environment.py``
+2. This script needs to be executed at project's root.
 
-To override an existing install use the ``-f`` option to force the workspace clean-up:
-    ``python setup_environment.py -f``
+3. Currently, this code only supports:
+    * ``windows`` as operating system
+    * ``poetry`` as dependency management system
+    * projects without dependency management systems
+    * ``poetry`` 1.2 to latest.
 
-To select a particular version of the dependency management system use the ``-s`` option:
-    ``python setup_environment.py -s 1.3``
+4. The following project structure is expected for projects without a dependency management system:
+    project-name
+    ├──requirements/                    # Folder containing the optional group of dependencies.
+    │  ├── requirements_doc.txt         # Requirements file associated to the documentation group.
+    │  ├── requirements_tests.txt       # Requirements file associated to the tests group.
+    │  ├── requirements_style.txt       # Requirements file associated to the style group.
+    │  └── requirements_build.txt       # Requirements file associated to the build group.
+
+5. The following project structure is expected for projects with a dependency management system:
+    project-name
+    └── pyproject.toml                  # Configuration of the build system.
 
-To install the production dependencies as well as all the optional dependency groups of the project use the ``-d``
-option with the keyword ``all``:
-    ``python setup_environment.py -d all``
+The following packages are needed on top of the standard Python configuration: ``toml`` and ``packaging``.
+
+Usage
+-----
 
-To install only a particular dependency group use ``run`` for production, ``doc`` for documentation, ``tests`` for
-testing, ``style`` for code linting, and ``build`` for build. For example:
+To create a virtual environment and install the dependency management system of the project (if any):
+    ``python setup_environment.py``
+
+To install a particular dependency group use the ``-d`` option:
     ``python setup_environment.py -d run`` installs production dependencies
     ``python setup_environment.py -d doc`` installs doc dependencies
     ``python setup_environment.py -d tests`` installs tests dependencies
     ``python setup_environment.py -d style`` installs style dependencies
     ``python setup_environment.py -d build`` installs build dependencies
 
-It is also possible to combine several groups:
+It is possible to combine several groups:
     ``python setup_environment.py -d run doc tests``
 
+To install all available dependencies (production and optional) use the ``all`` option:
+    ``python setup_environment.py -d all``
+
 Extra dependency groups refer to any group declared in the configuration file of the dependency management system which
 are not part of doc, tests, style and build. To install these groups use the ``x`` option:
     ``python setup_environment.py -x <name-of-the-group>``
 
-Currently, this code only supports:
-    * ``windows`` as operating system
-    * ``poetry`` and ``flit`` as dependency management systems
-    * projects without dependency management systems
-
 There are two locations where the script will search for optional dependencies:
     * First it checks the ``pyproject.toml`` configuration file and search for optional dependency groups
     * Alternatively, it looks for a ``requirements`` folder at project root containing requirements files with the
       name of the dependency group. For instance: requirements/requirements_doc.txt for the documentation group.
 
-The following project structure is expected for projects without a dependency management system:
-project-name
-├──requirements/                    # Folder containing the optional group of dependencies.
-│  ├── requirements_doc.txt         # Requirements file associated to the documentation group.
-│  ├── requirements_tests.txt       # Requirements file associated to the tests group.
-│  ├── requirements_style.txt       # Requirements file associated to the style group.
-│  └── requirements_build.txt       # Requirements file associated to the build group.
-
-The following project structure is expected for projects with a dependency management system:
-project-name
-└── pyproject.toml                  # Configuration of the build system.
-
-The following lines should be present in the ``pyproject.toml`` file for managing the version of the dependency management system:
-Example for using poetry 1.4.0:
-[build-system-requirements]
-build-system-version = "1.4.0"
+To enforce the version of the dependency manager two options are possible:
+
+    1. ``setup_environment.py`` reads the ``pyproject.toml`` and looks for a ``build-system-version`` key within
+    the ``build-system-requirements`` section. The example below illustrates this. Note that,
+    ``build-system-requirements` and ``build-system-version`` are not part of the ``PEP518`` standard. These syntax is
+    purely internal.
+    ```
+    [build-system-requirements]
+    build-system-version = "1.4.2"
+    ```
+
+    2. If the ``pyproject.toml`` does not contain a ``build-system-version``, the ``setup_environment.py`` checks the
+    ``-s`` option which can be provided in the command line when executing the script. In the example below, version
+    1.4.2 is enforced:
+    ``python setup_environment.py -s 1.4.2``
+
+Note that ``-s`` takes precedence over ``build-system-version``. If none of the two options listed above are used, the
+script simply takes the latest version of the dependency manager.
+
+To reinstall all dependencies by deleting both venvs and local poetry cache:
+    ``python setup_environment.py -f``
+
+To reinstall all dependencies by deleting venvs, local poetry cache and lock file. This option must be
+used only if REALLY necessary as the installation time for the whole process will be quite long.
+    ``python setup_environment.py -F``
+
+What this script is doing?
+--------------------------
+
+The aim of this script is to automate the project installation. It creates a virtual environment, installs a
+dependency manager if a configuration file is detected at project's root, configures the dependency manager to
+enable package collection from private sources, installs the dependency groups following user desire.
+
+In case ``poetry`` is detected as the project's dependency manager, two virtual environment are created. The first one
+is named ``.venv`` and is located in a ``.poetry`` directory created at project's root. It is use to install
+``poetry``. The second one, also named ``.venv`` is created at project's root and is controlled by ``poetry`` to
+install the dependencies. This configuration is required by ``poetry``.
+
+Future development
+------------------
+
+Given its size and its scope, this script will be refactored and transformed into a package.
 """
 
 # ==================================================== [Imports] ==================================================== #
 
 import argparse
 import os
 from pathlib import Path
@@ -75,263 +115,302 @@
 import re
 import shutil
 import subprocess
 import sys
 import textwrap
 import time
 
-from packaging.markers import Marker
-import toml
+try:
+    from packaging.markers import Marker
+except:
+    sys.exit("Process stopped. The `packaging` library is missing. Install with: `pip install packaging`.")
+try:
+    import toml
+except:
+    sys.exit("Process stopped. The `toml` library is missing. Install with: `pip install toml`.")
 
 # =================================================== [Variables] =================================================== #
 
-supported_dependency_management_systems = {
-    "poetry": {
+DEPENDENCY_MANAGER_PATHS = {
+    "win32": {
+        "poetry_python_executable": Path(".poetry").absolute() / ".venv" / "Scripts" / "python.exe",
+        "build_sys_exec": Path(".poetry").absolute() / ".venv" / "Scripts" / "poetry.exe",
+        "dep_bin_venv_path": Path(".venv").absolute() / "Scripts" / "poetry.exe",
+        "python_executable": Path(".venv").absolute() / "Scripts" / "python.exe",
+        "shell": True,
+    },
+    "linux": {
+        "poetry_python_executable": Path(".poetry").absolute() / ".venv" / "bin" / "python",
+        "build_sys_exec": Path(".poetry").absolute() / ".venv" / "bin" / "poetry",
+        "dep_bin_venv_path": Path(".venv").absolute() / "bin" / "poetry",
+        "python_executable": Path(".venv").absolute() / "bin" / "python",
+        "shell": False,
+    },
+    "common": {
         "configuration_file": "pyproject.toml",
         "build_backend": "poetry.core.masonry.api",
         "required_venv_name": ".venv",
         "lock_file": "poetry.lock",
-        "cache_folder": ".poetry\.cache",
-        "build_system_venv": ".poetry\.venv",
-    },
-    "flit": {
-        "configuration_file": "pyproject.toml",
-        "build_backend": "flit_core.buildapi",
-        "required_venv_name": None,
-        "lock_file": None,
-        "cache_folder": ".flit/.cache",
-        "build_system_venv": ".flit/.venv",
+        "build_system_venv": Path(".poetry") / ".venv",
+        "cache_folder": Path(".poetry").absolute() / ".cache",
     },
 }
 
-standard_optional_dependency_groups = ["doc", "tests", "build", "style", "external"]
+configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
+STANDARD_OPTIONAL_DEPENDENCY_GROUPS = [group for group in configuration["tool"]["poetry"]["group"].keys()]
 
 # =================================================== [Functions] =================================================== #
 
 # Console prints ----------------------------------------------------------------------------------------------------
 
 
-def print_main_header(text, max_length=100):
+def print_main_header(text: str, max_length: int = 100) -> None:
     """Display main header."""
 
     for i in range(max_length):
         print("=", end="")
     print()
     print(text)
     for i in range(max_length):
         print("=", end="")
     print()
     print()
 
 
-def print_section_header(text, max_length=100):
+def print_section_header(text: str, max_length: int = 100) -> None:
     """Display a section header in the console."""
+
     section_header = ""
     if len(text) < max_length:
         section_header = text + " "
         for i in range(len(text), max_length):
             section_header += "-"
     else:
         section_header = text
     print(section_header)
     print()
 
 
-def print_input_value(input, value, separator=":", separator_position=60):
+def print_input_value(input: str, value: str, separator: str = ":", separator_position: int = 60) -> None:
     """Print input value in console."""
+
     if len(input) < separator_position:
         text = input
         for i in range(len(text), separator_position):
             text += " "
         text += separator + " " + value
     else:
         text = input + " " + separator + " " + value
     print(text)
 
 
-def print_inputs_summary(args):
+def print_inputs_summary(args: object) -> None:
     """Display a summary of the inputs."""
 
     print(f"OS                                   : {platform.system()}")
     print(f"Python version                       : {get_python_version()}")
     print(f"Virtual environment name             : {args.venv_name}")
     print(f"run dependencies                     : {'yes' if 'run' in args.dependencies else 'no'}")
-    for dependency_group in standard_optional_dependency_groups:
+    for dependency_group in STANDARD_OPTIONAL_DEPENDENCY_GROUPS:
         print_input_value(
             f"{dependency_group} dependencies",
             "yes" if dependency_group in args.dependencies else "no",
             separator=":",
             separator_position=37,
         )
-    if args.build_system and args.extra_dependencies:
+    if args.extra_dependencies:
         for dependency_group in args.extra_dependencies:
             print_input_value(
                 f"{dependency_group} dependencies",
                 "yes",
                 separator=":",
                 separator_position=37,
             )
-    print(f"Dependency management system         : {args.build_system}")
+    print(f"Dependency management system         : poetry")
     print(f"Dependency management system version : {args.build_system_version}")
     print(f"Credentials management               : {args.credentials_management_method}")
     print()
 
 
 # Checks ------------------------------------------------------------------------------------------------------------
 
 
-def check_dependency_management_system():
-    """Check if a dependency management system is available at project root."""
-    for dms_name in supported_dependency_management_systems.keys():
-        if os.path.exists(supported_dependency_management_systems[dms_name]["configuration_file"]):
-            dms_configuration = toml.load(supported_dependency_management_systems[dms_name]["configuration_file"])
-            if (
-                dms_configuration["build-system"]["build-backend"]
-                == supported_dependency_management_systems[dms_name]["build_backend"]
-            ):
-                return dms_name
-
-
-def check_virtual_environment_name(args):
+def check_virtual_environment_name(args: object) -> None:
     """Check if the virtual environment name is consistent with the build system expectations."""
-    if args.build_system:
-        if supported_dependency_management_systems[args.build_system]["required_venv_name"]:
-            if supported_dependency_management_systems[args.build_system]["required_venv_name"] != args.venv_name:
-                old_name = args.venv_name
-                args.venv_name = supported_dependency_management_systems[args.build_system]["required_venv_name"]
-                print(
-                    f"Warning: {args.build_system} expects the name of the virtual environment name to be {args.venv_name}."
-                    f"{old_name} is replaced by {args.venv_name}."
-                )
+
+    if DEPENDENCY_MANAGER_PATHS["common"]["required_venv_name"] != args.venv_name:
+        old_name = args.venv_name
+        args.venv_name = DEPENDENCY_MANAGER_PATHS["common"]["required_venv_name"]
+        print(
+            f"Warning: poetry expects the name of the virtual environment name to be"
+            f" {args.venv_name}. {old_name} is replaced by {args.venv_name}."
+        )
 
 
-def check_python_version(args):
+def check_python_version(args: object) -> None:
     """
     Check if the version of the current Python interpreter is consistent with the python version specifications
     from the build system.
     """
-    if args.build_system:
-        # Initialize lower/upper versions
-        lower_version, upper_version, lower_bound_symbol, upper_bound_symbol = None, None, None, None
-        lower_specification, upper_specification, single_specification = None, None, None
-        # Read TOML
-        configuration = toml.load(supported_dependency_management_systems[args.build_system]["configuration_file"])
-        # Read Python version constraint
-        python_compatibility = ""
-        if args.build_system == "poetry":
-            python_compatibility = configuration["tool"][args.build_system]["dependencies"]["python"].replace(" ", "")
-        elif args.build_system == "flit":
-            python_compatibility = configuration["project"]["requires-python"].replace(" ", "")
-        # Split lower/upper version constraint
-        if "," in python_compatibility:
-            lower_specification, upper_specification = (
-                python_compatibility.split(",")[0],
-                python_compatibility.split(",")[1],
-            )
+
+    # Initialize lower/upper versions
+    lower_version, upper_version, lower_bound_symbol, upper_bound_symbol = None, None, None, None
+    lower_specification, upper_specification, single_specification = None, None, None
+    # Read TOML
+    configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
+    # Read Python version constraint
+    python_compatibility = configuration["tool"]["poetry"]["dependencies"]["python"].replace(" ", "")
+    # Split lower/upper version constraint
+    if "," in python_compatibility:
+        lower_specification, upper_specification = (
+            python_compatibility.split(",")[0],
+            python_compatibility.split(",")[1],
+        )
+    else:
+        if python_compatibility.startswith(">"):
+            lower_specification, upper_specification = python_compatibility, None
+        elif python_compatibility.startswith("<"):
+            lower_specification, upper_specification = None, python_compatibility
         else:
-            if python_compatibility.startswith(">"):
-                lower_specification, upper_specification = python_compatibility, None
-            elif python_compatibility.startswith("<"):
-                lower_specification, upper_specification = None, python_compatibility
-            else:
-                single_specification = python_compatibility
-        # Process lower constraint
-        if lower_specification:
-            lower_version = get_version_from_python_specification(lower_specification)
-            lower_bound_symbol = get_sign_from_python_specification(lower_specification)
-            marker = Marker(f"python_full_version {lower_bound_symbol} '{lower_version}'")
-            if not marker.evaluate():
-                raise Exception(f"Python version must be {lower_bound_symbol} {lower_version}.")
-        # Process upper constraint
-        if upper_specification:
-            upper_version = get_version_from_python_specification(upper_specification)
-            upper_bound_symbol = get_sign_from_python_specification(upper_specification)
-            marker = Marker(f"python_full_version {upper_bound_symbol} '{upper_version}'")
-            if not marker.evaluate():
-                raise Exception(f"Python version must be {upper_bound_symbol} {upper_version}.")
-        # Process single
-        if single_specification:
-            version = get_version_from_python_specification(single_specification)
-            sign = get_sign_from_python_specification(single_specification)
-            if sign != "==":
-                raise Exception("Unable to interpret python version specification.")
-            marker = Marker(f"python_full_version {sign} '{version}'")
-            if not marker.evaluate():
-                raise Exception(f"Python version must be equal to {version}.")
+            single_specification = python_compatibility
+    # Process lower constraint
+    if lower_specification:
+        lower_version = get_version_from_python_specification(lower_specification)
+        lower_bound_symbol = get_sign_from_python_specification(lower_specification)
+        marker = Marker(f"python_full_version {lower_bound_symbol} '{lower_version}'")
+        if not marker.evaluate():
+            raise Exception(f"Python version must be {lower_bound_symbol} {lower_version}.")
+    # Process upper constraint
+    if upper_specification:
+        upper_version = get_version_from_python_specification(upper_specification)
+        upper_bound_symbol = get_sign_from_python_specification(upper_specification)
+        marker = Marker(f"python_full_version {upper_bound_symbol} '{upper_version}'")
+        if not marker.evaluate():
+            raise Exception(f"Python version must be {upper_bound_symbol} {upper_version}.")
+    # Process single
+    if single_specification:
+        version = get_version_from_python_specification(single_specification)
+        sign = get_sign_from_python_specification(single_specification)
+        if sign != "==":
+            raise Exception("Unable to interpret python version specification.")
+        marker = Marker(f"python_full_version {sign} '{version}'")
+        if not marker.evaluate():
+            raise Exception(f"Python version must be equal to {version}.")
 
 
-def check_existing_install(args):
+def check_existing_install(args: object) -> str:
     """Check if an install exists already."""
+
     return os.path.isdir(args.venv_name)
 
 
-def check_inputs(args):
+def check_inputs(args: object) -> None:
     """Check inputs consistency."""
-    # Check platform
-    if sys.platform != "win32":
-        raise Exception("Only Windows operating systems are supported.")
     # Rework dependencies argument if all option is selected
     if "all" in args.dependencies:
         args.install_all = True
-        args.dependencies = standard_optional_dependency_groups + ["run"]
+        args.dependencies = STANDARD_OPTIONAL_DEPENDENCY_GROUPS + ["run"]
     else:
         args.install_all = False
-    # Check if a dependency management system is declared
-    args.build_system = check_dependency_management_system()
     # Check virtual environment name
     check_virtual_environment_name(args)
     # Check python version
     check_python_version(args)
     # Check if an install already exists
     args.has_install = check_existing_install(args)
 
 
 # General-purpose ---------------------------------------------------------------------------------------------------
 
 
-def read_integers_from_string(string):
-    """
-    Scan a string and extract integers.
+def extract_substring_between_markers(string: str, marker_1: str, marker_2: str) -> str:
+    """Extract substring between two markers using find() and slice()."""
+
+    # find() method will search the given marker and stores its index
+    mk1 = string.find(marker_1) + len(marker_1)
+    # find() method will search the given marker and sotres its index
+    mk2 = string.find(marker_2, mk1)
+    # using slicing substring will be fetched in between markers.
+    return string[mk1:mk2]
+
 
-    The regex matches any digit character (0-9).
+def read_integers_from_string(string: str) -> list:
     """
+    Scan a string and extract integers. The regex matches any digit character (0-9).
+    """
+
     return re.findall(r"\d+", string)
 
 
-def remove_scheme_from_url(url):
+def remove_scheme_from_url(url: str) -> tuple:
     """Remove the scheme part of a URL."""
+
     items = url.split("://")
     if len(items) == 2:
         return items[0], items[1]
     else:
         raise Exception(f"Fail to return the URL without the scheme part for {url}.")
 
 
-def get_python_version():
+def get_python_version() -> None:
     """Get Python version."""
+
     return f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
 
 
+def set_pip_command(
+    package_version: str = "*",
+    method: str = "install",
+    pypi_url: str = "https://pypi.org/simple",
+    private_pypi_token_name: str = "",
+    no_deps: bool = False,
+    python_executable: str = sys.executable,
+) -> str:
+    """Make pip command."""
+
+    package_name = "poetry"
+
+    # Add package version if specified
+    if package_version != "*":
+        package_name += f"=={package_version}"
+    # Set command
+    command = [python_executable, "-m", "pip", method, package_name]
+    # Add part related to private PyPI source
+    if pypi_url != "https://pypi.org/simple":
+        # Check if token is available
+        if private_pypi_token_name is None:
+            raise Exception(f"No token specified for private PyPI server {pypi_url}.")
+        # Check if the environment variable associated to the private PyPI token exists
+        private_pypi_token = os.getenv(private_pypi_token_name)
+        if private_pypi_token is None:
+            raise Exception(f"Environment variable {private_pypi_token_name} does not exist.")
+        # Split absolute URL
+        url_scheme, relative_url = remove_scheme_from_url(pypi_url)
+        # Update command line
+        command += f" -i {url_scheme}://PAT:{private_pypi_token}@{relative_url}"
+    # Add no-deps option
+    if no_deps:
+        command += " --no-deps"
+
+    return command
+
+
 def get_python_package(
-    package_name: str,
     package_version: str = "*",
     method: str = "install",
     pypi_url: str = "https://pypi.org/simple",
     private_pypi_token_name: str = "",
     no_deps: bool = False,
     python_executable: str = sys.executable,
-    verbose: bool = True,
 ) -> None:
     """
     Install or download a python package using PIP.
 
     Parameters
     ----------
-    package_name : str
-        Name of the package.
     package_version : str
         Version of the package.
     method : str
         Get method: ``download`` or ``install``
     pypi_url : str
         URL of the PyPI server.
     private_pypi_token_name : str
@@ -340,275 +419,264 @@
         Path to the Python executable.
 
     Returns
     -------
     None
     """
 
-    # Set command
-    command = f"{python_executable} -m pip {method} {package_name}"
-    # Add package version if specified
-    if package_version != "*":
-        command += f"=={package_version}"
-    # Add part related to private PyPI source
-    if pypi_url != "https://pypi.org/simple":
-        # Check if token is available
-        if private_pypi_token_name is None:
-            raise Exception(f"No token specified for private PyPI server {pypi_url}.")
-        # Check if the environment variable associated to the private PyPI token exists
-        private_pypi_token = os.getenv(private_pypi_token_name)
-        if private_pypi_token is None:
-            raise Exception(f"Environment variable {private_pypi_token_name} does not exist.")
-        # Split absolute URL
-        url_scheme, relative_url = remove_scheme_from_url(pypi_url)
-        # Update command line
-        command += f" -i {url_scheme}://PAT:{private_pypi_token}@{relative_url}"
-    # Add no-deps option
-    if no_deps:
-        command += " --no-deps"
-    # Run command with dummy version to force PIP to return the list of released versions
-    returncode, stdout, stderr = run_command(command, display_output=verbose)
-    if returncode != 0:
-        print(stdout)
+    # Set pip command
+    command = set_pip_command(
+        package_version=package_version,
+        method=method,
+        pypi_url=pypi_url,
+        private_pypi_token_name=private_pypi_token_name,
+        no_deps=no_deps,
+        python_executable=python_executable,
+    )
+    # Run pip command
+    process = subprocess.run(
+        command, check=False, shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"], capture_output=True, text=True
+    )
+    if process.returncode != 0:
+        print(process.stdout)
+        print(process.stderr)
         raise Exception("Command failed with error.")
 
 
-def run_command(cmd, display_output=True):
-    """
-    Run command.
-    """
-    process = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-    if display_output:
-        stdout, stderr = b"", b""
-        if process.stdout is not None:
-            for line in process.stdout:
-                sys.stdout.buffer.write(line)
-                sys.stdout.buffer.flush()
-                stdout += line
-        process.wait()
-    else:
-        stdout, stderr = process.communicate()
-
-    if isinstance(stdout, bytes):
-        try:
-            stdout = stdout.decode().splitlines()
-        except:
-            raise Exception("Unable to decode stdout.")
-
-    if isinstance(stderr, bytes):
-        try:
-            stderr = stderr.decode().splitlines()
-        except:
-            raise Exception("Unable to decode stderr.")
+def get_python_package_versions(
+    pypi_url: str = "https://pypi.org/simple",
+    private_pypi_token_name: str = "",
+    python_executable: str = sys.executable,
+) -> None:
+    """Get available versions of a package."""
 
-    return process.returncode, stdout, stderr
+    # Set pip command
+    command = set_pip_command(
+        package_version="x",
+        pypi_url=pypi_url,
+        private_pypi_token_name=private_pypi_token_name,
+        python_executable=python_executable,
+    )
+    # Run pip command
+    process = subprocess.run(
+        command, check=False, shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"], capture_output=True, text=True
+    )
+    if process.returncode == 0:
+        print(command)
+        raise Exception("This command should have failed. There is something wrong.")
+    else:
+        return extract_substring_between_markers(process.stderr, "(from versions:", ")").replace(" ", "").split(",")
 
 
 def upgrade_pip(python_executable: str = sys.executable) -> None:
-    """Upgrade to latest PIP version in the virtual environment"""
+    """Upgrade to latest PIP version in the virtual environment."""
+
     print("Upgrade to latest pip version")
     subprocess.run(
         [python_executable, "-m", "pip", "install", "--upgrade", "pip"],
         check=True,
-        shell=True,
+        shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
     )
     print()
 
 
-def create_virtual_environment(args, venv: str = ".venv"):
+def create_virtual_environment(args: object, venv: str = ".venv") -> None:
     """Create a virtual environment."""
 
     print("Create virtual environment")
     if not args.has_install or args.force_clear or args.force_clear_all:
-        subprocess.run([sys.executable, "-m", "venv", venv], check=True, shell=True)
+        if sys.platform == "linux":
+            subprocess.run(["sudo", "apt-get", "install", "-y", "python3-venv"], check=True)
+        subprocess.run(
+            [sys.executable, "-m", "venv", venv], check=True, shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"]
+        )
     else:
         print("Skipped")
     print()
 
 
 # Dependency Management System (Build System) -----------------------------------------------------------------------
 
 
-def get_private_sources(configuration_file):
+def get_private_sources(configuration_file: str) -> list:
     """Get list of private sources from configuration file."""
+
     configuration = toml.load(configuration_file)
     try:
         private_sources = configuration["tool"]["poetry"]["source"]
     except:
         private_sources = []
     return private_sources
 
 
-def get_version_from_python_specification(specification):
+def get_version_from_python_specification(specification: str) -> str:
     """Read the version."""
+
     return ".".join(read_integers_from_string(specification))
 
 
-def get_sign_from_python_specification(specification):
+def get_sign_from_python_specification(specification: str) -> str:
     """Read the mathematical symbol expressing a constraint on the version."""
+
     first_part = specification.split(".")[0]
     sign = "".join([i for i in first_part if not i.isdigit()])
     if sign == "":
         sign = "=="
     return sign
 
 
-def install_build_system(args):
-    """Install build system."""
-    print("Install dependency management system.")
-    if args.build_system:
-        if not args.has_install or args.force_clear or args.force_clear_all:
-            configuration = toml.load(supported_dependency_management_systems[args.build_system]["configuration_file"])
+def get_build_system_version(args: object) -> str:
+    """Assign build system version."""
+
+    if not args.has_install or args.force_clear or args.force_clear_all:
+        configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
+        if "build-system-requirements" in configuration.keys():
             if (
                 args.build_system_version == "*"
                 and "build-system-version" in configuration["build-system-requirements"]
             ):
                 args.build_system_version = configuration["build-system-requirements"]["build-system-version"]
-            if args.build_system == "poetry":
-                create_virtual_environment(
-                    args, venv=supported_dependency_management_systems[args.build_system]["build_system_venv"]
-                )
-                upgrade_pip(
-                    python_executable=rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\python"
-                )
-                get_python_package(
-                    args.build_system,
-                    args.build_system_version,
-                    method="install",
-                    python_executable=rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\python",
-                    verbose=args.verbose,
-                )
-            else:
-                get_python_package(
-                    args.build_system,
-                    args.build_system_version,
-                    method="install",
-                    python_executable=rf".\{args.venv_name}\Scripts\python",
-                    verbose=args.verbose,
-                )
-            print()
-            # Create a file symbolic link from the virtual environment (.venv) that the build system (poetry) manages
-            # to the build system executable (poetry.exe) in the poetry virtual environment (.poetry/.venv).  This
-            # ensures that the correct poetry is accessible when the managed virtual environment is activated
-            build_system_executable = rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\{args.build_system}.exe"
-            if os.path.exists(build_system_executable):
+        else:
+            args.build_system_version = get_python_package_versions()[-1]
+
+
+def install_build_system(args: object) -> None:
+    """Install build system."""
+
+    print("Install dependency management system.")
+    if not args.has_install or args.force_clear or args.force_clear_all:
+        configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
+        if args.build_system_version == "*" and "build-system-version" in configuration["build-system-requirements"]:
+            args.build_system_version = configuration["build-system-requirements"]["build-system-version"]
+
+        create_virtual_environment(args, venv=DEPENDENCY_MANAGER_PATHS["common"]["build_system_venv"])
+        upgrade_pip(python_executable=DEPENDENCY_MANAGER_PATHS[sys.platform]["poetry_python_executable"])
+        get_python_package(
+            args.build_system_version,
+            method="install",
+            python_executable=DEPENDENCY_MANAGER_PATHS[sys.platform]["poetry_python_executable"],
+        )
+        print()
+        # Create a file symbolic link from the virtual environment (.venv) that the build system (poetry) manages
+        # to the build system executable (poetry.exe) in the poetry virtual environment (.poetry/.venv).  This
+        # ensures that the correct poetry is accessible when the managed virtual environment is activated
+        build_system_executable = DEPENDENCY_MANAGER_PATHS[sys.platform]["build_sys_exec"]
+        if os.path.exists(build_system_executable):
+            if sys.platform == "win32":
                 subprocess.run(
                     [
                         "powershell",
                         "-Command",
                         "New-Item",
                         "-ItemType",
                         "SymbolicLink",
                         "-Path",
-                        rf".\{args.venv_name}\Scripts\{args.build_system}.exe",
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["dep_bin_venv_path"],
                         "-Target",
                         build_system_executable,
                     ]
                 )
-            return
+            elif sys.platform == "linux":
+                subprocess.run(
+                    [
+                        "ln",
+                        "-sf",
+                        build_system_executable,
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["dep_bin_venv_path"],
+                    ]
+                )
+        return
     print("Skipped")
     print()
 
 
-def configure_build_system(args):
+def configure_build_system(args: object) -> None:
     """Configure the build system to enable connection to private sources."""
+
     print("Configure dependency management system.")
-    if args.build_system:
-        if not args.has_install or args.force_clear or args.force_clear_all:
-            if args.build_system == "poetry":
-                configure_poetry(
-                    supported_dependency_management_systems[args.build_system]["build_system_venv"],
-                    args.credentials_management_method,
-                )
-                print()
-            return
+    if not args.has_install or args.force_clear or args.force_clear_all:
+        configure_poetry(
+            DEPENDENCY_MANAGER_PATHS["common"]["build_system_venv"],
+            args.credentials_management_method,
+        )
+        print()
+        return
     print("Skipped")
     print()
 
 
-def configure_poetry(venv_name, credentials_management_method):
+def configure_poetry(venv_name: str, credentials_management_method: str) -> None:
     """Configure Poetry."""
+    poetry_executable = DEPENDENCY_MANAGER_PATHS[sys.platform]["dep_bin_venv_path"]
     # Get list of private sources
     private_sources = get_private_sources("pyproject.toml")
-    # Delete existing configuration
-    print("Clean-up existing poetry configurations")
-    if sys.platform == "win32":
-        username = os.getlogin()
-        path_poetry_config = rf"C:\Users\{username}\AppData\Roaming\pypoetry"
-        if os.path.isfile(os.path.join(path_poetry_config, "config.toml")):
-            os.remove(os.path.join(path_poetry_config, "config.toml"))
-        if os.path.isfile(os.path.join(path_poetry_config, "auth.toml")):
-            os.remove(os.path.join(path_poetry_config, "auth.toml"))
     # Turn-on in-project
-    subprocess.run([rf".\{venv_name}\Scripts\poetry", "config", "virtualenvs.in-project", "true"], check=True)
+    subprocess.run([poetry_executable, "config", "virtualenvs.create", "false", "--local"], check=True)
+    # Turn-off virtual environment creation
+    subprocess.run([poetry_executable, "config", "virtualenvs.in-project", "true", "--local"], check=True)
     # Turn-on poetry cache
     subprocess.run(
         [
-            rf".\{venv_name}\Scripts\poetry",
+            poetry_executable,
             "config",
             "cache-dir",
-            supported_dependency_management_systems["poetry"]["cache_folder"],
+            DEPENDENCY_MANAGER_PATHS["common"]["cache_folder"],
+            "--local",
         ],
         check=True,
     )
+    # Turn-on in-project
+    subprocess.run([poetry_executable, "config", "virtualenvs.create", "false", "--local"], check=True)
     # Declare credentials for private sources
     for source in private_sources:
         print(f"Declare credentials for {source['name']}")
-        # Get source PAT
         if source["name"].lower() == "pypi":
             continue
         elif source["url"] == "https://pkgs.dev.azure.com/pyansys/_packaging/pyansys/pypi/simple/":
             token = os.environ["PYANSYS_PRIVATE_PYPI_PAT"]
         elif source["url"] == "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple/":
             token = os.environ["SOLUTIONS_PRIVATE_PYPI_PAT"]
         else:
             raise Exception(f"Unknown private source {source['name']} with url {source['url']}.")
         # Store credentials
         if credentials_management_method == "keyring":
             # Declare source URL
-            command_line = f"{venv_name}/Scripts/poetry config repositories.{source['name']} {source['url']}"
+            command_line = [poetry_executable, "config", f"repositories.{source['name']}", source["url"], "--local"]
             subprocess.run(command_line, check=True)
             # Declare source credentials
-            command_line = f"{venv_name}/Scripts/poetry config http-basic.{source['name']} PAT {token}"
+            command_line = [poetry_executable, "config", f"http-basic.{source['name']}", "PAT", token, "--local"]
             subprocess.run(command_line, check=True)
         elif credentials_management_method == "environment-variables":
             # Format source name to comply with Poetry environment variable syntax
             source_name = source["name"].upper().replace("-", "_")
             # Create Poetry environment variable
             os.environ[f"POETRY_HTTP_BASIC_{source_name}_USERNAME"] = "PAT"
             os.environ[f"POETRY_HTTP_BASIC_{source_name}_PASSWORD"] = token
 
 
-def check_dependency_group(dependency_group, configuration):
+def check_dependency_group(dependency_group: str, configuration: str) -> bool:
     """Return True if the dependency group is available in the configuration file."""
+
     try:
         configuration["tool"]["poetry"]["group"][dependency_group]
         return True
     except:
         return False
 
-def configure_portal_database(venv_name):
-    subprocess.run(
-        [
-            rf".\{venv_name}\Scripts\poetry",
-            "run",
-            "configure-portal-database",
-        ],
-        check=True,
-    )
 
 # Specifics ---------------------------------------------------------------------------------------------------------
 
 
-def parser():
+def parser() -> None:
     """Parse command line arguments."""
+
     # Code Name
-    program_name = "Setup Environment"
+    program_name = "Setup Environment Utility"
     # Code description
-    program_description = "A Python script to setup the Python ecosystem of a solution or framework."
+    program_description = "A Python script to automate the setup of the Python ecosystem of a project."
     # Create top-level parser
     parser = argparse.ArgumentParser(
         prog=program_name,
         usage=None,
         prefix_chars="-",
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=textwrap.dedent(program_description),
@@ -620,15 +688,15 @@
     optional_inputs.add_argument(
         "-d",
         "--dependencies",
         type=str,
         nargs="+",
         help="List of dependency groups to be installed separated by space. Example: run tests doc style build",
         default=[],
-        choices=standard_optional_dependency_groups + ["run", "all"],
+        choices=STANDARD_OPTIONAL_DEPENDENCY_GROUPS + ["run", "all"],
         required=False,
     )
     optional_inputs.add_argument(
         "-x",
         "--extra-dependencies",
         type=str,
         nargs="+",
@@ -637,15 +705,15 @@
         required=False,
     )
     optional_inputs.add_argument(
         "-s",
         "--build-system-version",
         type=str,
         help="Build system version",
-        default="1.5.1",
+        default="*",
         required=False,
     )
     optional_inputs.add_argument(
         "-c",
         "--credentials-management-method",
         type=str,
         help="Method to store private sources credentials.",
@@ -682,140 +750,154 @@
         action="store_true",
         required=False,
     )
 
     return parser.parse_args()
 
 
-def clear_workspace(args):
+def clear_workspace(args: object) -> None:
     """Remove residual items form previous installation (like venv directory, lock file ...)."""
+
     print("Clear workspace")
     if args.force_clear or args.force_clear_all:
         # Remove virtual environment
         if os.path.isdir(args.venv_name):
             print(f"Delete existing virtual environment {args.venv_name}.")
             shutil.rmtree(args.venv_name)
         # Remove poetry virtual environment
-        if os.path.isdir(supported_dependency_management_systems[args.build_system]["build_system_venv"]):
+        if os.path.isdir(DEPENDENCY_MANAGER_PATHS["common"]["build_system_venv"]):
             print("Delete existing poetry virtual environment")
-            shutil.rmtree(supported_dependency_management_systems[args.build_system]["build_system_venv"])
+            shutil.rmtree(DEPENDENCY_MANAGER_PATHS["common"]["build_system_venv"])
         # Remove poetry cache
-        if os.path.isdir(supported_dependency_management_systems[args.build_system]["cache_folder"]):
+        if os.path.isdir(DEPENDENCY_MANAGER_PATHS["common"]["cache_folder"]):
             print("Delete existing poetry cache")
-            shutil.rmtree(supported_dependency_management_systems[args.build_system]["cache_folder"])
+            shutil.rmtree(DEPENDENCY_MANAGER_PATHS["common"]["cache_folder"])
         if args.force_clear_all:
             # Remove lock file
-            if args.build_system:
-                if supported_dependency_management_systems[args.build_system]["lock_file"]:
-                    if os.path.isfile(supported_dependency_management_systems[args.build_system]["lock_file"]):
-                        print("Delete existing poetry lock file")
-                        os.remove(supported_dependency_management_systems[args.build_system]["lock_file"])
+            if DEPENDENCY_MANAGER_PATHS["common"]["lock_file"]:
+                if os.path.isfile(DEPENDENCY_MANAGER_PATHS["common"]["lock_file"]):
+                    print("Delete existing poetry lock file")
+                    os.remove(DEPENDENCY_MANAGER_PATHS["common"]["lock_file"])
     else:
         print("Skipped")
     print()
 
 
-def install_production_dependencies(args):
+def install_production_dependencies(args: object) -> None:
     """Install the package (mandatory requirements only)."""
+
     print("Install production dependencies")
-    if args.build_system and "run" in args.dependencies:
-        if args.build_system == "poetry":
-            subprocess.run(
-                [
-                    rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\poetry",
-                    "install",
-                    "-vv",
-                ],
-                check=True,
-                shell=True,
-            )
-        elif args.build_system == "flit":
-            subprocess.run([rf".\{args.venv_name}\Scripts\flit", "install"], check=True, shell=True)
+    if "run" in args.dependencies:
+        subprocess.run(
+            [
+                DEPENDENCY_MANAGER_PATHS[sys.platform]["build_sys_exec"],
+                "install",
+                "-vv",
+            ],
+            check=True,
+            shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
+        )
         print()
         return
     print("Skipped")
     print()
 
 
-def install_optional_dependencies(args):
+def install_optional_dependencies(args: object) -> None:
     """Install optional requirements (doc, tests, build or style)."""
-    # Load configuration file if a dependency management system is available
-    if args.build_system:
-        configuration = toml.load(supported_dependency_management_systems[args.build_system]["configuration_file"])
-    else:
-        configuration = {}
+
+    # Load configuration file
+    configuration = toml.load(DEPENDENCY_MANAGER_PATHS["common"]["configuration_file"])
     # Install standard optional dependency groups
-    for dependency_group in standard_optional_dependency_groups:
+    for dependency_group in STANDARD_OPTIONAL_DEPENDENCY_GROUPS:
         print(f"Install {dependency_group} dependencies")
         if dependency_group in args.dependencies:
             # Install dependency group in the configuration file of the build system
-            if args.build_system:
-                has_dependency_group = check_dependency_group(dependency_group, configuration)
-                if has_dependency_group:
-                    print("Installing from build system configuration file.")
-                    subprocess.run(
-                        [
-                            rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\poetry",
-                            "install",
-                            "--only",
-                            dependency_group,
-                            "-vv",
-                        ],
-                        check=True,
-                        shell=True,
-                    )
-                    print()
-                    continue
+            has_dependency_group = check_dependency_group(dependency_group, configuration)
+            if has_dependency_group:
+                print("Installing from build system configuration file.")
+                subprocess.run(
+                    [
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["build_sys_exec"],
+                        "install",
+                        "--only",
+                        dependency_group,
+                        "-vv",
+                    ],
+                    check=True,
+                    shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
+                )
+                print()
+                continue
             # Alternatively search dependency group in the requirements folder
             requirements_file = os.path.join("requirements", f"requirements_{dependency_group}.txt")
             if os.path.exists(requirements_file):
                 print("Installing from requirements file.")
                 subprocess.run(
                     [
-                        rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\python",
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["poetry_python_executable"],
                         "-m",
                         "poetry",
                         "run",
                         "pip",
                         "install",
                         "-r",
                         requirements_file,
                         "--no-warn-conflicts",
                     ],
                     check=True,
-                    shell=True,
+                    shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
                 )
                 print()
                 continue
         print("Skipped")
         print()
     # Install extra optional dependency groups
-    if args.build_system and args.extra_dependencies:
+    if args.extra_dependencies:
         for dependency_group in args.extra_dependencies:
             print(f"Install {dependency_group} dependencies")
             has_dependency_group = check_dependency_group(dependency_group, configuration)
             if has_dependency_group:
                 subprocess.run(
                     [
-                        rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\poetry",
+                        DEPENDENCY_MANAGER_PATHS[sys.platform]["build_sys_exec"],
                         "install",
                         "--only",
                         dependency_group,
                         "-vv",
                     ],
                     check=True,
-                    shell=True,
+                    shell=DEPENDENCY_MANAGER_PATHS[sys.platform]["shell"],
                 )
             else:
                 print(f"No dependency group named {dependency_group}.")
                 print("Skipped")
             print()
 
 
-def main():
+def install_dotnet_linux_dependencies():
+    print("Install dotnet dependencies")
+    if sys.platform == "linux":
+        subprocess.run(
+            'set -xe \
+            && wget https://dot.net/v1/dotnet-install.sh \
+            && chmod +x dotnet-install.sh \
+            && ./dotnet-install.sh --install-dir /home/$USER/.dotnet --version 3.1.0 --runtime aspnetcore \
+            && grep -qxF "DOTNET_ROOT=/home/$USER/.dotnet" /home/$USER/.bash_profile \
+            || echo DOTNET_ROOT=/home/$USER/.dotnet >> /home/$USER/.bash_profile \
+            && grep -qxF "PATH=\$PATH:/home/$USER/.dotnet" /home/$USER/.bash_profile \
+            || echo "PATH=\$PATH:/home/$USER/.dotnet" >> /home/$USER/.bash_profile \
+            && echo "\nsource /home/$USER/.bash_profile" >> ./.venv/bin/activate \
+            && rm dotnet-install.sh',
+            check=True,
+            shell=True,
+        )
+
+
+def main() -> None:
     """Sequence of operations leading to the complete Python ecosystem."""
 
     # Start timer
     time_on = time.time()
     # Get current working directory
     working_directory = os.getcwd()
     # Get installation directory
@@ -827,14 +909,17 @@
 
     # Read command line inputs
     args = parser()
 
     # Check inputs consistency
     check_inputs(args)
 
+    # Update build system version
+    get_build_system_version(args)
+
     # Display header
     print_main_header("Setup Environment")
 
     # Display inputs summary
     print_inputs_summary(args)
 
     # Clear workspace -------------------------------------------------------------------------------------------------
@@ -845,15 +930,15 @@
 
     # Setup virtual environment ---------------------------------------------------------------------------------------
 
     print_section_header("Setup virtual environment", max_length=100)
 
     create_virtual_environment(args)
 
-    upgrade_pip(python_executable=rf".\{args.venv_name}\Scripts\python")
+    upgrade_pip(python_executable=DEPENDENCY_MANAGER_PATHS[sys.platform]["python_executable"])
 
     # Setup dependency management system ------------------------------------------------------------------------------
 
     print_section_header("Setup dependency management system", max_length=100)
 
     install_build_system(args)
 
@@ -863,28 +948,27 @@
 
     print_section_header("Install dependencies", max_length=100)
 
     install_production_dependencies(args)
 
     install_optional_dependencies(args)
 
+    install_dotnet_linux_dependencies()
+
     # Back to current working directory
     os.chdir(working_directory)
 
-    # Configure database
-    if 'run' in args.dependencies:
-        configure_portal_database(args.venv_name)
-
     # Compute execution time
     elapsed_time = (time.time() - time_on) / 60  # in minutes
 
     print("You are all set!")
     print("Navigate to project root and activate your environment with one these commands:")
     print(rf"   - For Windows CMD       : {args.venv_name}\Scripts\activate.bat")
     print(rf"   - For Windows Powershell: {args.venv_name}\Scripts\Activate.ps1")
+    print(rf"   - For Ubuntu            : source {args.venv_name}/bin/activate")
     print("Enjoy!")
     print()
     print("Execution time: %.1f minutes." % (elapsed_time))
     print()
 
 
 # =================================================== [Execution] =================================================== #
```

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.0.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/testing.py` & `ansys_templates-1.0.0/src/ansys/templates/testing.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/src/ansys/templates/utils.py` & `ansys_templates-1.0.0/src/ansys/templates/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.9.0/PKG-INFO` & `ansys_templates-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-templates
-Version: 0.9.0
+Version: 1.0.0
 Summary: Creates Python projects according to PyAnsys guidelines
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -12,23 +12,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata >=4.0
-Requires-Dist: click>=7.0,<8.0.0
+Requires-Dist: click>=7.0,<9.0.0
 Requires-Dist: cookiecutter>=2.1.0
 Requires-Dist: isort>=5.10.1
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: pytest==7.3.2 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
+Requires-Dist: pytest==7.4.0 ; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Project-URL: Documentation, https://templates.ansys.com/
 Project-URL: Homepage, https://templates.ansys.com/
 Project-URL: Source, https://github.com/ansys/ansys-templates
 Project-URL: Tracker, https://github.com/ansys/ansys-templates/issues
 Provides-Extra: doc
 Provides-Extra: tests
```

