# Comparing `tmp/amazon_codeguru_jupyterlab_extension-1.0.0.tar.gz` & `tmp/amazon_codeguru_jupyterlab_extension-1.1.0.tar.gz`

## Comparing `amazon_codeguru_jupyterlab_extension-1.0.0.tar` & `amazon_codeguru_jupyterlab_extension-1.1.0.tar`

### file list

```diff
@@ -1,75 +1,82 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.eslintrc.js
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.stylelintrc
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/SECURITY.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/babel.config.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/jest.config.js
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/package.json
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/setup.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tsconfig.json
--rw-r--r--   0        0        0   456516 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/yarn.lock
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/cfg.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/codeguru.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/constants.py
--rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/diagnostics.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/plugin.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json
--rw-r--r--   0        0        0    12496 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/606.839cc39e93f88938c736.js
--rw-r--r--   0        0        0  1808896 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/67.c97baf8a498fda49350d.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/67.c97baf8a498fda49350d.js.LICENSE.txt
--rw-r--r--   0        0        0   125329 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/703.60e17cd520b0c3ad0f9c.js
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/703.60e17cd520b0c3ad0f9c.js.LICENSE.txt
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/747.ecd0ef12675f88068557.js
--rw-r--r--   0        0        0   225367 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/860.5abb378d41ad4395b0af.js
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/910.1ab01fa00a55e966d7e8.js
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.60903ee90e17dc8ffe5d.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0   128918 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    24553 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/configuration/boto/codeguru-security/2018-05-10/service-2.json
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/schema/plugin.json
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/index.ts
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/svg.d.ts
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/components/About.tsx
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanButton.tsx
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanErrorPopup.tsx
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanStatus.tsx
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/icons.ts
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/index.ts
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/interface.ts
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/policy.ts
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/region.ts
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/utils/index.ts
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/style/index.css
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/style/index.js
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/style/icons/cg-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0    10760 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/test_diagnostics.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/test_plugin.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/converted.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/finding.json
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/simple.ipynb
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/simple.py
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   125819 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/NOTICE
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/README.md
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.eslintrc.js
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.stylelintrc
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/SECURITY.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/babel.config.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/jest.config.js
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/package.json
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/setup.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tsconfig.json
+-rw-r--r--   0        0        0   456516 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/yarn.lock
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/cfg.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/codeguru.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/constants.py
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/diagnostics.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/plugin.py
+-rw-r--r--   0        0        0    22393 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/build_log.json
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/install.json
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json
+-rw-r--r--   0        0        0    42849 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js
+-rw-r--r--   0        0        0    37569 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/lib_index_js-webpack_sharing_consume_default_jupyterlab_coreutils.c4c5385e7a8c0c90533a.js.map
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/node_modules_cloudscape-design_global-styles_dist_index_js.49bd81ccb2dba12e6001.js.map
+-rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.b23847fa632c515c4b3e.js
+-rw-r--r--   0        0        0    33982 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.b23847fa632c515c4b3e.js.map
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/style_index_js.cc72af7097c34762d4b6.js.map
+-rw-r--r--   0        0        0   593989 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js
+-rw-r--r--   0        0        0   632582 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_box_index_js-node_modules_cloudscape-design-140555.b6fe59bfb98ab1ea02c7.js.map
+-rw-r--r--   0        0        0  6116687 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js
+-rw-r--r--   0        0        0  6281464 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_cloudscape-design_components_index_js.6c9ca9a4c8f822138168.js.map
+-rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js
+-rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e6996744cc53a2504dda.js.map
+-rw-r--r--   0        0        0   848306 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js
+-rw-r--r--   0        0        0   836060 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/static/vendors-node_modules_jupyter-lsp_jupyterlab-lsp_lib_editor_integration_codemirror_js-node_mod-1ae516.faab484a03b81bb9ac8b.js.map
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/schema/plugin.json
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/index.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/svg.d.ts
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/components/About.tsx
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanButton.tsx
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanErrorPopup.tsx
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanStatus.tsx
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/icons.ts
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/index.ts
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/interface.ts
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/policy.ts
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/constants/region.ts
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/src/utils/index.ts
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/style/index.css
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/style/index.js
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/style/icons/cg-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0    11122 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/test_diagnostics.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/converted.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/finding.json
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/simple.ipynb
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/simple.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   125819 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/NOTICE
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/README.md
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.1.0/PKG-INFO
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/.eslintrc.js` & `amazon_codeguru_jupyterlab_extension-1.1.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/CONTRIBUTING.md` & `amazon_codeguru_jupyterlab_extension-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/jest.config.js` & `amazon_codeguru_jupyterlab_extension-1.1.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/package.json` & `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/tsconfig.json` & `amazon_codeguru_jupyterlab_extension-1.1.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/yarn.lock` & `amazon_codeguru_jupyterlab_extension-1.1.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/codeguru.py` & `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/codeguru.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 import os
 import boto3
-import sys
 
 CODEGURU_REGIONS = [
     'eu-north-1',
     'ap-southeast-2',
     'us-east-1',
     'us-east-2',
     'us-west-2',
     'ap-northeast-1',
     'ap-southeast-1',
     'eu-central-1',
     'eu-west-1',
     'eu-west-2'
 ]
 DEFAULT_AWS_REGION = 'us-east-1'
-session = boto3.Session()
-session._loader.search_paths.extend([os.path.join(sys.prefix, "boto")])
 
 
 def get_codeguru_security_client(overridden_region):
     aws_region = get_codeguru_supported_region(overridden_region)
-    return session.client('codeguru-security',
-                          endpoint_url="https://codeguru-security.{}.amazonaws.com".format(aws_region),
-                          region_name=aws_region)
+    return boto3.client('codeguru-security',
+                        region_name=aws_region)
 
 
 def get_codeguru_supported_region(overridden_region):
     aws_region = os.getenv("AWS_REGION")
     if is_codeguru_supported(aws_region) and overridden_region == DEFAULT_AWS_REGION:
         return aws_region
     return overridden_region or DEFAULT_AWS_REGION
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/diagnostics.py` & `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         zipf.write(py_filepath, arcname=os.path.basename(py_filepath))
     return zip_filepath
 
 
 def upload_file(zip_filepath: str, scan_name: str, codeguru_security, send_notification):
     try:
         create_upload_url_response = codeguru_security.create_upload_url(
-            fileName=os.path.basename(zip_filepath), scanName=scan_name)
+            scanName=scan_name)
     except ClientError as e:
         logger.error(e)
         send_notification({"status": CommandStatus.ERROR, "message": str(e)})
         return
     s3_url = create_upload_url_response['s3Url']
     request_headers = create_upload_url_response['requestHeaders']
     code_artifact_id = create_upload_url_response['codeArtifactId']
@@ -89,15 +89,16 @@
             send_notification(
                 {"status": CommandStatus.ERROR, "message": str(e)})
             return
         if get_scan_response['scanState'] == 'Successful':
             break
         elif get_scan_response['scanState'] == 'Failed':
             logger.error("Express scan failed")
-            send_notification({"status": CommandStatus.ERROR, "message": "Scan failed"})
+            send_notification(
+                {"status": CommandStatus.ERROR, "message": "Scan failed"})
             return
 
 
 def get_scan_findings(scan_name: str, codeguru_security, send_notification):
     try:
         get_findings_response = codeguru_security.get_findings(
             scanName=scan_name)
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py` & `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/plugin.py` & `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/plugin.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/package.json` & `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996345029239767%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b23847fa632c515c4b3e.js'}}"}*

```diff
@@ -54,15 +54,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/aws/amazon-codeguru-jupyterlab-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.60903ee90e17dc8ffe5d.js",
+            "load": "static/remoteEntry.b23847fa632c515c4b3e.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "amazon-codeguru-jupyterlab-extension"
                 },
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig` & `amazon_codeguru_jupyterlab_extension-1.1.0/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'1.1.0'"}*

```diff
@@ -127,9 +127,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.1.0"
 }
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json` & `amazon_codeguru_jupyterlab_extension-1.1.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/schema/plugin.json` & `amazon_codeguru_jupyterlab_extension-1.1.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/src/index.ts` & `amazon_codeguru_jupyterlab_extension-1.1.0/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -19,33 +19,35 @@
   PLUGIN_ID,
   REGISTER_ID,
   RUN_CODEGURU_SCAN_ID
 } from './constants';
 import { codeGuruIcon } from './constants/icons';
 import { AutoScan, IProgressMessageResponse } from './constants/interface';
 import { DEFAULT_AWS_REGION, Region } from './constants/region';
+import { getPlatformAcronym } from './utils';
 
 class CodeGuruCM extends CodeMirrorIntegration {}
 
 let overriddenRegion = DEFAULT_AWS_REGION;
 
 const COMMANDS = (button: CreateCodeScanButtonExtension): IFeatureCommand[] => [
   {
     id: RUN_CODEGURU_SCAN_ID,
     label: CODEGURU_RUN_SCAN_LABEL,
     icon: codeGuruIcon,
     execute: ({ connection, document }) => {
+      const platform = getPlatformAcronym();
       let token: string;
       if (connection?.isConnected) {
         // eslint-disable-next-line @typescript-eslint/ban-ts-comment
         // @ts-ignore
         const wsConnection = connection.connection;
         void wsConnection.sendRequest('workspace/executeCommand', {
           command: 'cgs.runScan',
-          arguments: [document.document_info.uri, overriddenRegion]
+          arguments: [document.document_info.uri, overriddenRegion, platform]
         });
 
         wsConnection.onNotification(
           '$/progress',
           (response: IProgressMessageResponse) => {
             if (response.value.title === 'command: runScan') {
               token = response.token;
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/src/components/About.tsx` & `amazon_codeguru_jupyterlab_extension-1.1.0/src/components/About.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanButton.tsx` & `amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanButton.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanErrorPopup.tsx` & `amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanErrorPopup.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanStatus.tsx` & `amazon_codeguru_jupyterlab_extension-1.1.0/src/components/CodeScanStatus.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/style/base.css` & `amazon_codeguru_jupyterlab_extension-1.1.0/style/base.css`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/style/icons/cg-icon.svg` & `amazon_codeguru_jupyterlab_extension-1.1.0/style/icons/cg-icon.svg`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/tests/conftest.py` & `amazon_codeguru_jupyterlab_extension-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/tests/test_diagnostics.py` & `amazon_codeguru_jupyterlab_extension-1.1.0/tests/test_diagnostics.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,22 @@
         [2, 4, 19, 79, 66],
         [3, 89, 90, 80, -1]
     ]
     assert result == expected
 
 
 def test_get_message_for_finding_for_nb(finding):
-    result = diagnostics.get_message_for_finding(finding, fixtures_dir / "converted.py", True)
+    result = diagnostics.get_message_for_finding(
+        finding, fixtures_dir / "converted.py", True)
     expected = {
         "code": "python/improper-error-handling@v1.0",
         "message": "Issue: Improper error handling\n\nSuggested remediation: Try, Except, Pass detected. https://bandit.readthedocs.io/en/latest/plugins/b110_try_except_pass.html",
         "range": {
-            "end": { "character": 22, "line": 26 },
-            "start": { "character": 4, "line": 26 }
+            "end": {"character": 22, "line": 26},
+            "start": {"character": 4, "line": 26}
         },
         "severity": 2,
         "source": "codeguru-security"
     }
     assert result == expected
 
 
@@ -61,47 +62,53 @@
     expected_path = "/tmp/simple.zip"
     assert os.path.isfile(expected_path)
     assert result == expected_path
 
 
 def test_get_diagnostics_from_other_sources(config, workspace, document):
     mock_hook_handlers = Mock(return_value=[[{"message": "other"}]])
-    config.plugin_manager.subset_hook_caller = Mock(return_value=mock_hook_handlers)
-    result = diagnostics.get_diagnostics_from_other_sources(config, workspace, document)
+    config.plugin_manager.subset_hook_caller = Mock(
+        return_value=mock_hook_handlers)
+    result = diagnostics.get_diagnostics_from_other_sources(
+        config, workspace, document)
     expected = [{"message": "other"}]
     assert result == expected
 
 
 def test_create_scan():
     client = diagnostics.get_codeguru_security_client("us-west-2")
     create_scan_response = {
         "runId": "123",
-        "scanName": "scan-name",
+        "scanName": "jl-scan-name",
         "resourceId": {"codeArtifactId": "code-artifact-id"},
         "scanState": "Pending"
     }
     expected_params = {
         "resourceId": {"codeArtifactId": "code-artifact-id"},
-        "scanName": "scan-name",
+        "scanName": "jl-scan-name",
         "scanType": "Express",
         "analysisType": "All"
     }
     with Stubber(client) as stubber:
-        stubber.add_response("create_scan", create_scan_response, expected_params)
+        stubber.add_response(
+            "create_scan", create_scan_response, expected_params)
         send_notification = Mock()
-        result = diagnostics.create_scan("code-artifact-id", "scan-name", client, send_notification)
+        result = diagnostics.create_scan(
+            "code-artifact-id", "jl-scan-name", client, send_notification)
         assert result == "123"
 
 
 def test_create_scan_failed():
     client = diagnostics.get_codeguru_security_client("us-west-2")
     with Stubber(client) as stubber:
-        stubber.add_client_error("create_scan", service_error_code="foo", service_message="bar")
+        stubber.add_client_error(
+            "create_scan", service_error_code="foo", service_message="bar")
         send_notification = Mock()
-        diagnostics.create_scan("code-artifact-id", "scan-name", client, send_notification)
+        diagnostics.create_scan(
+            "code-artifact-id", "jl-scan-name", client, send_notification)
         send_notification.assert_called_once_with({
             "message": "An error occurred (foo) when calling the CreateScan operation: bar",
             "status": "error",
         })
 
 
 @mock.patch('requests.put')
@@ -109,31 +116,35 @@
     client = diagnostics.get_codeguru_security_client("us-west-2")
     create_upload_url_response = {
         "s3Url": "https://s3-url.com",
         "requestHeaders": {"a": "b", "c": "d"},
         "codeArtifactId": "code-artifact-id"
     }
     create_upload_url_expected_params = {
-        "fileName": "simple.zip",
-        "scanName": "scan-name"
+        "scanName": "jl-scan-name"
     }
     with Stubber(client) as stubber:
-        stubber.add_response("create_upload_url", create_upload_url_response, create_upload_url_expected_params)
+        stubber.add_response(
+            "create_upload_url", create_upload_url_response, create_upload_url_expected_params)
         send_notification = Mock()
-        result = diagnostics.upload_file("/tmp/simple.zip", "scan-name", client, send_notification)
-        mock_put.assert_called_once_with("https://s3-url.com", data=mock.ANY, headers={"a": "b", "c": "d"})
+        result = diagnostics.upload_file(
+            "/tmp/simple.zip", "jl-scan-name", client, send_notification)
+        mock_put.assert_called_once_with(
+            "https://s3-url.com", data=mock.ANY, headers={"a": "b", "c": "d"})
         assert result == "code-artifact-id"
 
 
 def test_upload_file_create_upload_url_failed():
     client = diagnostics.get_codeguru_security_client("us-west-2")
     with Stubber(client) as stubber:
-        stubber.add_client_error("create_upload_url", service_error_code="foo", service_message="bar")
+        stubber.add_client_error(
+            "create_upload_url", service_error_code="foo", service_message="bar")
         send_notification = Mock()
-        diagnostics.upload_file("/tmp/simple.zip", "scan-name", client, send_notification)
+        diagnostics.upload_file(
+            "/tmp/simple.zip", "jl-scan-name", client, send_notification)
         send_notification.assert_called_once_with({
             "message": "An error occurred (foo) when calling the CreateUploadUrl operation: bar",
             "status": "error",
         })
 
 
 @mock.patch('requests.put')
@@ -144,102 +155,114 @@
         "requestHeaders": {"a": "b", "c": "d"},
         "codeArtifactId": "code-artifact-id"
     }
     with Stubber(client) as stubber:
         stubber.add_response("create_upload_url", create_upload_url_response)
         send_notification = Mock()
         mock_put.return_value.ok = False
-        diagnostics.upload_file("/tmp/simple.zip", "scan-name", client, send_notification)
-        mock_put.assert_called_once_with("https://s3-url.com", data=mock.ANY, headers={"a": "b", "c": "d"})
+        diagnostics.upload_file(
+            "/tmp/simple.zip", "jl-scan-name", client, send_notification)
+        mock_put.assert_called_once_with(
+            "https://s3-url.com", data=mock.ANY, headers={"a": "b", "c": "d"})
         send_notification.assert_called_once_with({
             "message": "File upload failed",
             "status": "error",
         })
 
 
 def test_get_scan_findings(finding):
     client = diagnostics.get_codeguru_security_client("us-west-2")
     get_findings_response = {
         "findings": [finding]
     }
     get_findings_expected_params = {
-        "scanName": "scan-name"
+        "scanName": "jl-scan-name"
     }
     with Stubber(client) as stubber:
-        stubber.add_response("get_findings", get_findings_response, get_findings_expected_params)
+        stubber.add_response(
+            "get_findings", get_findings_response, get_findings_expected_params)
         send_notification = Mock()
-        result = diagnostics.get_scan_findings("scan-name", client, send_notification)
+        result = diagnostics.get_scan_findings(
+            "jl-scan-name", client, send_notification)
         send_notification.assert_called_once_with({
             "message": 1,
             "status": "completed"
         })
         assert result == [finding]
 
 
 def test_get_scan_findings_failed():
     client = diagnostics.get_codeguru_security_client("us-west-2")
     with Stubber(client) as stubber:
-        stubber.add_client_error("get_findings", service_error_code="foo", service_message="bar")
+        stubber.add_client_error(
+            "get_findings", service_error_code="foo", service_message="bar")
         send_notification = Mock()
-        diagnostics.get_scan_findings("scan-name", client, send_notification)
+        diagnostics.get_scan_findings(
+            "jl-scan-name", client, send_notification)
         send_notification.assert_called_once_with({
             "message": "An error occurred (foo) when calling the GetFindings operation: bar",
             "status": "error"
         })
 
 
 def test_poll_scan_status_succeeded():
     client = diagnostics.get_codeguru_security_client("us-west-2")
     get_scan_response = {
         "scanState": "Successful",
-        "scanName": "scan-name",
+        "scanName": "jl-scan-name",
         "runId": "run-id",
         "createdAt": 1,
         "analysisType": "All"
     }
     get_scan_expected_params = {
-        "scanName": "scan-name",
+        "scanName": "jl-scan-name",
         "runId": "run-id"
     }
     with Stubber(client) as stubber:
-        stubber.add_response("get_scan", get_scan_response, get_scan_expected_params)
+        stubber.add_response("get_scan", get_scan_response,
+                             get_scan_expected_params)
         send_notification = Mock()
-        diagnostics.poll_scan_status("scan-name", "run-id", client, send_notification)
+        diagnostics.poll_scan_status(
+            "jl-scan-name", "run-id", client, send_notification)
         send_notification.assert_not_called()
 
 
 def test_poll_scan_status_failed():
     client = diagnostics.get_codeguru_security_client("us-west-2")
     get_scan_response = {
         "scanState": "Failed",
-        "scanName": "scan-name",
+        "scanName": "jl-scan-name",
         "runId": "run-id",
         "createdAt": 1,
         "analysisType": "All"
     }
     get_scan_expected_params = {
-        "scanName": "scan-name",
+        "scanName": "jl-scan-name",
         "runId": "run-id"
     }
     with Stubber(client) as stubber:
-        stubber.add_response("get_scan", get_scan_response, get_scan_expected_params)
+        stubber.add_response("get_scan", get_scan_response,
+                             get_scan_expected_params)
         send_notification = Mock()
-        diagnostics.poll_scan_status("scan-name", "run-id", client, send_notification)
+        diagnostics.poll_scan_status(
+            "jl-scan-name", "run-id", client, send_notification)
         send_notification.assert_called_once_with({
             "message": "Scan failed",
             "status": "error"
         })
 
 
 def test_poll_scan_status_get_scan_failed():
     client = diagnostics.get_codeguru_security_client("us-west-2")
     with Stubber(client) as stubber:
-        stubber.add_client_error("get_scan", service_error_code="foo", service_message="bar")
+        stubber.add_client_error(
+            "get_scan", service_error_code="foo", service_message="bar")
         send_notification = Mock()
-        diagnostics.poll_scan_status("scan_name", "run-id", client, send_notification)
+        diagnostics.poll_scan_status(
+            "scan_name", "run-id", client, send_notification)
         send_notification.assert_called_once_with({
             "message": "An error occurred (foo) when calling the GetScan operation: bar",
             "status": "error"
         })
 
 
 def test_get_message_for_finding_nb():
@@ -255,15 +278,16 @@
         "vulnerability": {
             "filePath": {
                 "startLine": 4,
                 "endLine": 4
             }
         }
     }
-    result = diagnostics.get_message_for_finding(finding, "/tmp/simple.py", True)
+    result = diagnostics.get_message_for_finding(
+        finding, "/tmp/simple.py", True)
     assert result == {
         "source": "codeguru-security",
         "code": "python/foo@v1.0",
         "message": "Issue: Foo\n\nSuggested remediation: Bar",
         "range": {
             "start": {"line": 0, "character": 0},
             "end": {"line": 0, "character": 11}
@@ -285,19 +309,19 @@
         "vulnerability": {
             "filePath": {
                 "startLine": 4,
                 "endLine": 4
             }
         }
     }
-    result = diagnostics.get_message_for_finding(finding, "/tmp/simple.py", False)
+    result = diagnostics.get_message_for_finding(
+        finding, "/tmp/simple.py", False)
     assert result == {
         "source": "codeguru-security",
         "code": "python/foo@v1.0",
         "message": "Issue: Foo\n\nSuggested remediation: Bar",
         "range": {
             "start": {"line": 3, "character": 0},
             "end": {"line": 3, "character": 11}
         },
         "severity": 2
     }
-
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/tests/test_plugin.py` & `amazon_codeguru_jupyterlab_extension-1.1.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/converted.py` & `amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/converted.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/finding.json` & `amazon_codeguru_jupyterlab_extension-1.1.0/tests/fixtures/finding.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/README.md` & `amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/jupyter_server_test_config.py` & `amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/yarn.lock` & `amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts` & `amazon_codeguru_jupyterlab_extension-1.1.0/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/.gitignore` & `amazon_codeguru_jupyterlab_extension-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/LICENSE` & `amazon_codeguru_jupyterlab_extension-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/README.md` & `amazon_codeguru_jupyterlab_extension-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/pyproject.toml` & `amazon_codeguru_jupyterlab_extension-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "jupyterlab_lsp >= 4.0.0",
     "python-lsp-server <= 1.7.1",
-    "boto3"
+    "boto3 >= 1.26.162"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.entry-points.pylsp]
 amazon_codeguru_jupyterlab_extension = "amazon_codeguru_jupyterlab_extension.plugin"
 
 [project.optional-dependencies]
@@ -44,15 +44,14 @@
 [tool.hatch.build.targets.sdist]
 artifacts = ["amazon_codeguru_jupyterlab_extension/labextension"]
 exclude = [".github", "binder"]
 
 [tool.hatch.build.targets.wheel.shared-data]
 "amazon_codeguru_jupyterlab_extension/labextension" = "share/jupyter/labextensions/@aws/amazon-codeguru-extension"
 "install.json" = "share/jupyter/labextensions/@aws/amazon-codeguru-extension/install.json"
-"configuration/boto" = "boto"
 
 [tool.hatch.build.hooks.version]
 path = "amazon_codeguru_jupyterlab_extension/_version.py"
 
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder>=0.5"]
 build-function = "hatch_jupyter_builder.npm_builder"
```

### Comparing `amazon_codeguru_jupyterlab_extension-1.0.0/PKG-INFO` & `amazon_codeguru_jupyterlab_extension-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_codeguru_jupyterlab_extension
-Version: 1.0.0
+Version: 1.1.0
 Summary: Security, code quality, and ML recommendations
 Project-URL: Homepage, https://github.com/aws/amazon-codeguru-jupyterlab-extension
 Project-URL: Bug Tracker, https://github.com/aws/amazon-codeguru-jupyterlab-extension/issues
 Project-URL: Repository, https://github.com/aws/amazon-codeguru-jupyterlab-extension.git
 License-File: LICENSE
 License-File: NOTICE
 Classifier: Framework :: Jupyter
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: boto3
+Requires-Dist: boto3>=1.26.162
 Requires-Dist: jupyterlab-lsp>=4.0.0
 Requires-Dist: python-lsp-server<=1.7.1
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Provides-Extra: tests
```

