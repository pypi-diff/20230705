# Comparing `tmp/scicookie-0.2.0.tar.gz` & `tmp/scicookie-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicookie-0.2.0.tar", max compression
+gzip compressed data, was "scicookie-0.3.0.tar", max compression
```

## Comparing `scicookie-0.2.0.tar` & `scicookie-0.3.0.tar`

### file list

```diff
@@ -1,61 +1,67 @@
--rw-r--r--   0        0        0     1551 2023-06-17 01:11:15.787381 scicookie-0.2.0/LICENSE
--rw-r--r--   0        0        0     2060 2023-06-17 01:16:30.327177 scicookie-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/__init__.py
--rw-r--r--   0        0        0      115 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/__main__.py
--rw-r--r--   0        0        0     3132 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/cli.py
--rw-r--r--   0        0        0     1704 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/cookiecutter.json
--rw-r--r--   0        0        0     5707 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/hooks/post_gen_project.py
--rw-r--r--   0        0        0      359 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      969 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/logs.py
--rw-r--r--   0        0        0     1385 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/profile.py
--rw-r--r--   0        0        0     3695 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/profiles/base.yaml
--rw-r--r--   0        0        0      739 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/profiles/osl.yaml
--rw-r--r--   0        0        0     2122 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/ui.py
--rw-r--r--   0        0        0      292 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
--rw-r--r--   0        0        0     4617 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      892 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1712 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
--rw-r--r--   0        0        0     2550 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      342 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1387 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      814 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1666 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1274 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0        0        0     2867 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2295 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
--rw-r--r--   0        0        0     5996 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0        0        0     2637 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0     3325 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0        0        0     6433 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
--rw-r--r--   0        0        0     6434 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5488 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
--rw-r--r--   0        0        0     5488 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
--rw-r--r--   0        0        0      255 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml
--rw-r--r--   0        0        0     1998 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
--rw-r--r--   0        0        0      300 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
--rw-r--r--   0        0        0       54 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
--rw-r--r--   0        0        0      182 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
--rw-r--r--   0        0        0       20 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
--rw-r--r--   0        0        0     5666 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
--rw-r--r--   0        0        0     1116 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
--rw-r--r--   0        0        0     3386 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
--rw-r--r--   0        0        0      996 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
--rw-r--r--   0        0        0      967 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
--rw-r--r--   0        0        0      151 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
--rw-r--r--   0        0        0     4249 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
--rwxr-xr-x   0        0        0     5275 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
--rw-r--r--   0        0        0      374 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
--rw-r--r--   0        0        0      829 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
--rw-r--r--   0        0        0       30 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
--rw-r--r--   0        0        0    16493 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
--rw-r--r--   0        0        0     6843 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
--rw-r--r--   0        0        0     4381 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0     1558 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
--rw-r--r--   0        0        0       61 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      317 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0        0        0      809 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
--rw-r--r--   0        0        0      631 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
--rw-r--r--   0        0        0       19 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 scicookie-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1551 2023-07-05 20:50:33.388224 scicookie-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2060 2023-07-05 20:54:30.191225 scicookie-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/__init__.py
+-rw-r--r--   0        0        0      115 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/__main__.py
+-rw-r--r--   0        0        0     3132 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/cli.py
+-rw-r--r--   0        0        0     1787 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/cookiecutter.json
+-rw-r--r--   0        0        0     7388 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      359 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      969 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/logs.py
+-rw-r--r--   0        0        0     1417 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/profile.py
+-rw-r--r--   0        0        0     3888 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/profiles/base.yaml
+-rw-r--r--   0        0        0      770 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/profiles/osl.yaml
+-rw-r--r--   0        0        0     2122 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/ui.py
+-rw-r--r--   0        0        0      292 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
+-rw-r--r--   0        0        0     4617 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      892 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1712 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
+-rw-r--r--   0        0        0     2550 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      342 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1387 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      814 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1666 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1274 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0        0        0     2867 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2295 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
+-rw-r--r--   0        0        0     5996 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0        0        0     3092 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0     3325 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0        0        0     1717 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml
+-rw-r--r--   0        0        0     3963 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit-pyproject.toml
+-rw-r--r--   0        0        0      400 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/meson.build
+-rw-r--r--   0        0        0     3886 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy-pyproject.toml
+-rw-r--r--   0        0        0     3880 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm-pyproject.toml
+-rw-r--r--   0        0        0     2567 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml
+-rw-r--r--   0        0        0     3745 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools-pyproject.toml
+-rw-r--r--   0        0        0     6433 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
+-rw-r--r--   0        0        0     6434 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5488 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
+-rw-r--r--   0        0        0     5488 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
+-rw-r--r--   0        0        0      575 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml
+-rw-r--r--   0        0        0     1998 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
+-rw-r--r--   0        0        0      300 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
+-rw-r--r--   0        0        0       54 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
+-rw-r--r--   0        0        0      182 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
+-rw-r--r--   0        0        0       20 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
+-rw-r--r--   0        0        0     8386 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
+-rw-r--r--   0        0        0     1116 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
+-rw-r--r--   0        0        0     3386 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
+-rw-r--r--   0        0        0      996 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
+-rw-r--r--   0        0        0      967 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
+-rw-r--r--   0        0        0      151 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
+-rw-r--r--   0        0        0     4398 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
+-rwxr-xr-x   0        0        0     5275 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      374 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
+-rw-r--r--   0        0        0      829 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
+-rw-r--r--   0        0        0       30 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
+-rw-r--r--   0        0        0    16493 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
+-rw-r--r--   0        0        0     6843 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
+-rw-r--r--   0        0        0     1558 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
+-rw-r--r--   0        0        0       61 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1266 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.package_slug}}.py
+-rw-r--r--   0        0        0      809 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
+-rw-r--r--   0        0        0      631 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
+-rw-r--r--   0        0        0       19 2023-07-05 20:50:33.392223 scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 scicookie-0.3.0/PKG-INFO
```

### Comparing `scicookie-0.2.0/LICENSE` & `scicookie-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/pyproject.toml` & `scicookie-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scicookie"
-version = "0.2.0"  # semantic-release
+version = "0.3.0"  # semantic-release
 description = "Cookiecutter template for a Python package"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD"
 include = [
     {path = "src/scicookie/cookiecutter.json"},
     {path = "src/scicookie/{{cookiecutter.project_slug}}"},
     {path = "src/scicookie/hooks"},
```

### Comparing `scicookie-0.2.0/src/scicookie/cli.py` & `scicookie-0.3.0/src/scicookie/cli.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/cookiecutter.json` & `scicookie-0.3.0/src/scicookie/cookiecutter.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9621621621621622%*

 * *Differences: {"'build_system'": "{insert: [(1, 'flit'), (2, 'mesonpy'), (3, 'setuptools'), (4, 'pdm')]}",*

 * * "'use_hypothesis'": "'yes'"}*

```diff
@@ -1,12 +1,16 @@
 {
     "author_email": "zoro@one.piece",
     "author_full_name": "Roronoa Zoro",
     "build_system": [
-        "poetry"
+        "poetry",
+        "flit",
+        "mesonpy",
+        "setuptools",
+        "pdm"
     ],
     "code_of_conduct": [
         "None",
         "contributor-covenant",
         "citizen-code-of-conduct"
     ],
     "command_line_interface": [
@@ -57,14 +61,15 @@
     "use_containers": [
         "None",
         "Docker",
         "Podman"
     ],
     "use_coverage": "yes",
     "use_flake8": "yes",
+    "use_hypothesis": "yes",
     "use_isort": "yes",
     "use_mccabe": "yes",
     "use_mypy": "yes",
     "use_pre_commit": "yes",
     "use_pydocstyle": "yes",
     "use_pytest": "yes",
     "use_ruff": "yes",
```

### Comparing `scicookie-0.2.0/src/scicookie/logs.py` & `scicookie-0.3.0/src/scicookie/logs.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/profile.py` & `scicookie-0.3.0/src/scicookie/profile.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 PROFILE_DIR_PATH = PACKAGE_PATH / "profiles"
 
 
 class Profile:
     """Profile class that handles profiles defined in the .yaml files."""
 
     profile_name: str = ""
-    config: dict = {}
-    profiles_available: list = []
+    config: dict = {}  # noqa: RUF012
+    profiles_available: list = []  # noqa: RUF012
 
     def __init__(self, profile_name: str):
         self._load_profiles_available()
 
         if profile_name not in self.profiles_available:
             SciCookieLogs.raise_error(
                 "The given profiles is not available.",
```

### Comparing `scicookie-0.2.0/src/scicookie/profiles/base.yaml` & `scicookie-0.3.0/src/scicookie/profiles/base.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,26 @@
   help: ""
   type: single-choice
   choices:
     - src
     - flat
   enabled: false
 
+build_system:
+  message: Select the build system
+  help: ""
+  type: single-choice
+  choices:
+    - poetry
+    - flit
+    - mesonpy
+    - setuptools
+    - pdm
+  enabled: false
+
 command_line_interface:
   message: Select the Command Line Interface (CLI)
   help: ""
   type: single-choice
   choices:
     - No command-line interface
     - Click
@@ -109,14 +121,15 @@
     - flake8
     - ruff
     - isort
     - mccabe
     - pre-commit
     - pydocstyle
     - pytest
+    - hypothesis
     - shellcheck
     - vulture
   enabled: false
 
 use_containers:
   message: Select the container technology for this project
   help: ""
```

### Comparing `scicookie-0.2.0/src/scicookie/profiles/osl.yaml` & `scicookie-0.3.0/src/scicookie/profiles/osl.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
 governance_document:
   enabled: true
 
 roadmap_document:
   enabled: true
 
+build_system:
+  enabled: true
+
 use_tools:
   enabled: true
 
 use_containers:
   enabled: true
 
 # use_git:
```

### Comparing `scicookie-0.2.0/src/scicookie/ui.py` & `scicookie-0.3.0/src/scicookie/ui.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -56,19 +56,23 @@
 	rm -fr htmlcov/
 	rm -fr .pytest_cache
 
 .PHONY:lint
 lint:
 	pre-commit run --all-files
 
-{% if cookiecutter.use_pytest %}
-.PHONY:test
+.PHONY: test
 test: ## run tests quickly with the default Python
+	{%- if cookiecutter.use_pytest == "yes" %}
 	pytest
-{% endif %}
+	{%- elif cookiecutter.use_hypothesis == "yes" %}
+	python -m unittest discover
+	{%- else %}
+	@echo "No test library selected."
+	{%- endif %}
 
 {% if cookiecutter.documentation_engine == 'mkdocs' -%}
 .PHONY:docs-build
 docs-build:
 	mkdocs build --config-file docs/mkdocs.yaml
 
 .PHONY: docs-preview
@@ -93,15 +97,25 @@
 .PHONY: docs-preview
 docs-preview: docs-build
 	cd docs/_build/html/ && python -m http.server
 {%- endif +%}
 
 .PHONY:build
 build:
+{%- if cookiecutter.build_system == "poetry" %}
 	poetry build
+{%- elif cookiecutter.build_system == "flit" %}
+	flit build
+{%- elif cookiecutter.build_system == "mesonpy" %}
+	meson build
+{%- elif cookiecutter.build_system == "setuptools" %}
+	python -m build
+{%- elif cookiecutter.build_system == "pdm" %}
+	pdm build
+{%- endif %}
 
 .PHONY:release-ci
 release-ci:
 	$(RELEASE_APP) --ci
 
 .PHONY:release-dry
 release-dry:
```

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/README.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,19 @@
   # - exclude:
   #     glob:
   #       - backends/template.md
   - mkdocstrings:
       enable_inventory: true
       handlers:
         python:
+          {% if cookiecutter.project_layout == "src" -%}
+          paths: [../src]
+          {% else %}
+          paths: [..]
+          {%- endif %}
           import:
             - https://docs.python.org/3/objects.inv
           options:
             docstring_style: numpy
             filters:
               - "!^Bounds"
               - "!^__class__"
```

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools-pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,182 +1,117 @@
-{% if cookiecutter.project_layout == "src" -%}
-{% set package_path = "src/" + cookiecutter.package_slug -%}
-{% else -%}
-{% set package_path = cookiecutter.package_slug -%}
-{% endif -%}
-[tool.poetry]
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+
+[project]
 name = "{{ cookiecutter.project_slug }}"
-version = "{{ cookiecutter.project_version }}"  # semantic-release
-description = "{{ cookiecutter.project_short_description }}"
-authors = ["{{ cookiecutter.author_full_name }} <{{ cookiecutter.author_email }}>"]
-license = "{{ cookiecutter.project_license }}"
-include = [
-  "*.cfg",
-  "*.ini",
-  "*.js",
-  "*.json",
-  "*.lock",
-  "*.md",
-  "*.py",
-  "*.sh",
-  "*.rst",
-  "*.txt",
-  "*.toml",
-  "*.yml",
-  "*.yaml",
-  ".github",
-  "conda",
-  "docker",
-  "docs",
-  ".dockerignore",
-  ".env.tpl",
-  ".makim.yaml",
-  ".containers-sugar.yaml",
-  ".gitignore",
-  "Makefile",
+authors = [
+  { name = "{{ cookiecutter.author_full_name }}", email = "{{ cookiecutter.author_email }}" },
 ]
-exclude = [
-  ".git/*",
-  ".env*",
+description = "{{ cookiecutter.project_short_description }}"
+readme = "README.md"
+classifiers = [
+{%- if cookiecutter.project_license == "MIT" %}
+  "License :: OSI Approved :: MIT License",
+{%- elif cookiecutter.project_license == "BSD 3 Clause" %}
+  "License :: OSI Approved :: BSD License",
+{%- elif cookiecutter.project_license == "Apache Software License 2.0" %}
+  "License :: OSI Approved :: Apache Software License",
+{%- elif cookiecutter.project_license == "GNU General Public License v3" %}
+  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+{%- endif %}
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
-
-[tool.poetry.dependencies]
-python = "^3.8.1"
-
-[tool.poetry.dev-dependencies]
-urllib3 = "<2"  # fix poetry issues
+dynamic = ["version"]
+requires-python = '>=3.8.1'
+dependencies = [
 {# keep this line here #}
 {%- if cookiecutter.use_pytest == "yes" -%}
-pytest = "^7.3.2"
+    "pytest >= 7.3.2",
 {% if cookiecutter.use_coverage == "yes" -%}
-pytest-cov = "^4.1.0"
+    "pytest-cov >= 4.1.0",
 {% endif %}
 {%- endif -%}{#- end of use_pytest -#}
+{%- if cookiecutter.use_hypothesis == "yes" -%}
+    "hypothesis >= 6.0",
+{% endif %}
 {%- if cookiecutter.use_coverage == "yes" -%}
-coverage = "^7.2.7"
+    "coverage >= 7.2.7",
 {% endif %}
 {%- if cookiecutter.use_blue == "yes" -%}
-blue = "^0.9.1"
+    "blue >= 0.9.1",
 {% endif %}
 {%- if cookiecutter.use_black == "yes" -%}
-black = "^23.3.0"
+    "black >= 23.3.0",
 {% endif %}
 {%- if cookiecutter.use_isort == "yes" -%}
-isort = "^5.12.0"
+    "isort >= 5.12.0",
 {% endif %}
 {%- if cookiecutter.use_pre_commit -%}
-pre-commit = "^3.3.2"
+    "pre-commit >= 3.3.2",
 {% endif %}
 {%- if cookiecutter.use_flake8 == "yes" -%}
-flake8 = ">=4.0.1, <7"
+    "flake8 >= 4.0.1, < 7",
 {% endif %}
 {%- if cookiecutter.use_ruff == "yes" -%}
-ruff = "^0.0.272"
+    "ruff >= 0.0.272",
 {% endif %}
 {%- if cookiecutter.use_mypy == "yes" -%}
-mypy = "^1.3.0"
+    "mypy >= 1.3.0",
 {% endif %}
 {%- if cookiecutter.use_bandit == "yes" -%}
-bandit = "^1.7.5"
+    "bandit >= 1.7.5",
 {% endif %}
 {%- if cookiecutter.use_pydocstyle == "yes" -%}
-pydocstyle = "^6.3.0"
+    "pydocstyle >= 6.3.0",
 {% endif %}
 {%- if cookiecutter.use_vulture == "yes" -%}
-vulture = "^2.7"
+    "vulture >= 2.7",
 {% endif %}
 {%- if cookiecutter.use_mccabe == "yes" -%}
-mccabe = "^0.6.1"
+    "mccabe >= 0.6.1",
 {% endif %}
-{%- if cookiecutter.use_containers in ['Docker', 'Podman'] -%}
+{%- if cookiecutter.use_containers in ["Docker", "Podman"] -%}
 # if you want to use docker-compose from your system, remove compose-go here
-compose-go = "^2.18.1"
+    "compose-go >= 2.18.1",
 {% endif %}
-{%- if cookiecutter.documentation_engine == 'mkdocs' -%}
-Jinja2 = "^3.1.2"
-mkdocs = "^1.4.3"
-mkdocs-exclude = "^1.0.2"
-mkdocs-jupyter = "^0.24.1"
-mkdocs-literate-nav = "^0.6.0"
-mkdocs-macros-plugin = ">=0.7.0,<1"
-mkdocs-material = "^9.1.15"
-mkdocstrings = "^0.21.2"
-mkdocstrings-python = "^1.1.2"
-{% elif cookiecutter.documentation_engine == 'sphinx' -%}
-Sphinx = "^6.2.1"
-sphinx-rtd-theme = "^1.2.2"
-importlib-metadata = "^6.5.1"
-myst-parser = "^0.19.2"
-nbsphinx = "^0.9.2"
-pandoc = "^2.3"
-{% elif cookiecutter.documentation_engine == 'jupyter-book' -%}
-jupyter-book = "^0.15.1"
-myst-parser = "^0.18.1"
-{% endif %}
-{%- if cookiecutter.use_pytest == "yes" %}
-[tool.pytest.ini_options]
-testpaths = [
-    "tests",
-]
+    "ipython <  8",
+    "ipykernel >= 6.0.0",
+{%- if cookiecutter.documentation_engine == "mkdocs" -%}
+    "Jinja2 >= 3.1.2",
+    "mkdocs >= 1.4.3",
+    "mkdocs-exclude >= 1.0.2",
+    "mkdocs-jupyter >= 0.24.1",
+    "mkdocs-literate-nav >= 0.6.0",
+    "mkdocs-macros-plugin >= 0.7.0, <1",
+    "mkdocs-material >= 9.1.15",
+    "mkdocstrings >= 0.21.2",
+    "mkdocstrings-python >= 1.1.2",
+{% elif cookiecutter.documentation_engine == "sphinx" -%}
+    "Sphinx >= 6.2.1",
+    "sphinx-rtd-theme >= 1.2.2",
+    "importlib-metadata >= 6.5.1",
+    "myst-parser >= 0.19.2",
+    "nbsphinx >= 0.9.2",
+    "pandoc >= 2.3",
+{% elif cookiecutter.documentation_engine == "jupyter-book" -%}
+    "jupyter-book >= 0.15.1",
+    "myst-parser >= 0.18.1",
 {% endif %}
-{%- if cookiecutter.use_blue == "yes" %}
-[tool.blue]
-line-length = 79
-target-version = ["py38"]
-force-exclude = '''(?x)(
-    docs/*
-  | .*\\.egg-info
-)'''  # TOML's single-quoted strings do not require escaping backslashes
-{% endif %}
-{%- if cookiecutter.use_black == "yes" %}
-[tool.black]
-line-length = 79
-target-version = ["py38"]
-force-exclude = '''(?x)(
-    docs/*
-  | .*\\.egg-info
-)'''  # TOML's single-quoted strings do not require escaping backslashes
-{% endif %}
-{%- if cookiecutter.use_isort == "yes" %}
-[tool.isort]
-ensure_newline_before_comments = true
-line_length = 79
-multi_line_output = 3
-include_trailing_comma = true
-skip_glob = ["docs/*", "*.egg-info"]
-{% endif %}
-{%- if cookiecutter.use_bandit == "yes" %}
-[tool.bandit]
-exclude_dirs = ["tests"]
-targets = "{{ package_path }}"
-{% endif %}
-{%- if cookiecutter.use_vulture == "yes" %}
-[tool.vulture]
-exclude = ["tests"]
-ignore_decorators = []
-ignore_names = []
-make_whitelist = true
-min_confidence = 80
-paths = ["{{ package_path }}"]
-sort_by_size = true
-verbose = false
-{% endif %}
-{%- if cookiecutter.use_ruff == "yes" %}
-[tool.ruff]
-line-length = 79
-force-exclude = true
-src = ["{{ package_path }}"]
-exclude = [
-  'docs',
-]
-select = [
-  "F",   # pyflakes
 ]
 
-[tool.ruff.pydocstyle]
-convention = "numpy"
-{% endif %}
-{%- if cookiecutter.use_mypy == "yes" %}
-[tool.mypy]
-no_strict_optional = false
-{% endif %}
+[project.urls]
+Homepage = "{{ cookiecutter.project_url }}"
+"Bug Tracker" = "{{ cookiecutter.project_url }}/issues"
+Discussions = "{{ cookiecutter.project_url }}/discussions"
+Changelog = "{{ cookiecutter.project_url }}/releases"
+
+{% include "build-system/base-pyproject.toml" %}
 {#- keep this line at the end of the file -#}
```

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py` & `scicookie-0.3.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.2.0/PKG-INFO` & `scicookie-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scicookie
-Version: 0.2.0
+Version: 0.3.0
 Summary: Cookiecutter template for a Python package
 License: BSD
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

