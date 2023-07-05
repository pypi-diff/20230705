# Comparing `tmp/cycode-0.2.6.dev6.tar.gz` & `tmp/cycode-0.2.6.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.6.dev6.tar", max compression
+gzip compressed data, was "cycode-0.2.6.dev7.tar", max compression
```

## Comparing `cycode-0.2.6.dev6.tar` & `cycode-0.2.6.dev7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    32549 2023-07-05 09:56:16.667783 cycode-0.2.6.dev6/README.md
--rw-r--r--   0        0        0      115 2023-07-05 09:56:52.720173 cycode-0.2.6.dev6/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:56:16.667783 cycode-0.2.6.dev6/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:56:16.667783 cycode-0.2.6.dev6/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     2793 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4761 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1652 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    53872 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      453 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5510 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1698 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2196 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      992 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2993 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5835 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     8226 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/main.py
--rw-r--r--   0        0        0     1562 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      700 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0     1378 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/base_table_printer.py
--rw-r--r--   0        0        0     1910 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1672 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     5832 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/sca_table_printer.py
--rw-r--r--   0        0        0     2277 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/table.py
--rw-r--r--   0        0        0      477 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/table_models.py
--rw-r--r--   0        0        0     5416 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     9336 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4821 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     6925 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1908 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6853 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0      154 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/enum_utils.py
--rw-r--r--   0        0        0     2195 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0     7687 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/progress_bar.py
--rw-r--r--   0        0        0     2768 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/scan_batch.py
--rw-r--r--   0        0        0      334 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      941 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     1989 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2700 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      815 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      929 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       57 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1708 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2458 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      119 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3927 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      543 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1751 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     9102 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6301 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1090 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1179 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      197 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     2014 2023-07-05 09:56:52.716173 cycode-0.2.6.dev6/pyproject.toml
--rw-r--r--   0        0        0    34042 1970-01-01 00:00:00.000000 cycode-0.2.6.dev6/PKG-INFO
+-rw-r--r--   0        0        0    32549 2023-07-05 11:43:18.016185 cycode-0.2.6.dev7/README.md
+-rw-r--r--   0        0        0      114 2023-07-05 11:43:52.182712 cycode-0.2.6.dev7/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:43:18.016185 cycode-0.2.6.dev7/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:43:18.016185 cycode-0.2.6.dev7/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2765 2023-07-05 11:43:18.016185 cycode-0.2.6.dev7/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4741 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    53478 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5689 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1717 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2139 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      975 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2888 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5607 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     7911 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/main.py
+-rw-r--r--   0        0        0     1490 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      700 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0     1378 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/base_table_printer.py
+-rw-r--r--   0        0        0     1910 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1603 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     5809 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/sca_table_printer.py
+-rw-r--r--   0        0        0     2277 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/table.py
+-rw-r--r--   0        0        0      477 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/table_models.py
+-rw-r--r--   0        0        0     5409 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     9514 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4581 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6929 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1873 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6598 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     2195 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     7657 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2751 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      937 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1989 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2664 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      930 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2461 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      120 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3647 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      542 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1751 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     9228 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6296 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1087 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1157 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      199 2023-07-05 11:43:18.020185 cycode-0.2.6.dev7/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     2333 2023-07-05 11:43:52.182712 cycode-0.2.6.dev7/pyproject.toml
+-rw-r--r--   0        0        0    34044 1970-01-01 00:00:00.000000 cycode-0.2.6.dev7/PKG-INFO
```

### Comparing `cycode-0.2.6.dev6/README.md` & `cycode-0.2.6.dev7/README.md`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cli/auth/auth_command.py` & `cycode-0.2.6.dev7/cycode/cli/auth/auth_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cycode.cyclient import logger
 from cycode.cyclient.cycode_token_based_client import CycodeTokenBasedClient
 
 
 @click.group(invoke_without_command=True)
 @click.pass_context
 def authenticate(context: click.Context):
-    """ Authenticates your machine to associate CLI with your cycode account """
+    """Authenticates your machine to associate CLI with your cycode account"""
     if context.invoked_subcommand is not None:
         # if it is a subcommand do nothing
         return
 
     try:
         logger.debug('Starting authentication process')
 
@@ -29,15 +29,15 @@
     except Exception as e:
         _handle_exception(context, e)
 
 
 @authenticate.command(name='check')
 @click.pass_context
 def authorization_check(context: click.Context):
-    """ Check your machine associating CLI with your cycode account """
+    """Check your machine associating CLI with your cycode account"""
     printer = ConsolePrinter(context)
 
     passed_auth_check_res = CliResult(success=True, message='You are authorized')
     failed_auth_check_res = CliResult(success=False, message='You are not authorized')
 
     client_id, client_secret = CredentialsManager().get_credentials()
     if not client_id or not client_secret:
@@ -55,20 +55,18 @@
 
 def _handle_exception(context: click.Context, e: Exception):
     if context.obj['verbose']:
         click.secho(f'Error: {traceback.format_exc()}', fg='red')
 
     errors: CliErrors = {
         AuthProcessError: CliError(
-            code='auth_error',
-            message='Authentication failed. Please try again later using the command `cycode auth`'
+            code='auth_error', message='Authentication failed. Please try again later using the command `cycode auth`'
         ),
         NetworkError: CliError(
-            code='cycode_error',
-            message='Authentication failed. Please try again later using the command `cycode auth`'
+            code='cycode_error', message='Authentication failed. Please try again later using the command `cycode auth`'
         ),
     }
 
     error = errors.get(type(e))
     if error:
         return ConsolePrinter(context).print_error(error)
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/auth/auth_manager.py` & `cycode-0.2.6.dev7/cycode/cli/auth/auth_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,28 +76,27 @@
 
     def save_api_token(self, api_token: ApiToken):
         self.credentials_manager.update_credentials_file(api_token.client_id, api_token.secret)
 
     def _build_login_url(self, code_challenge: str, session_id: str):
         app_url = self.configuration_manager.get_cycode_app_url()
         login_url = f'{app_url}/account/sign-in'
-        query_params = {
-            'source': 'cycode_cli',
-            'code_challenge': code_challenge,
-            'session_id': session_id
-        }
+        query_params = {'source': 'cycode_cli', 'code_challenge': code_challenge, 'session_id': session_id}
         # TODO(MarshalX). Use auth_client instead and don't depend on "requests" lib here
         request = Request(url=login_url, params=query_params)
         return request.prepare().url
 
     def _generate_pkce_code_pair(self) -> (str, str):
         code_verifier = generate_random_string(self.CODE_VERIFIER_LENGTH)
         code_challenge = hash_string_to_sha256(code_verifier)
         return code_challenge, code_verifier
 
     def _is_api_token_process_completed(self, api_token_polling_response: ApiTokenGenerationPollingResponse) -> bool:
-        return api_token_polling_response is not None \
-               and api_token_polling_response.status == self.COMPLETED_POLLING_STATUS
+        return (
+            api_token_polling_response is not None
+            and api_token_polling_response.status == self.COMPLETED_POLLING_STATUS
+        )
 
     def _is_api_token_process_failed(self, api_token_polling_response: ApiTokenGenerationPollingResponse) -> bool:
-        return api_token_polling_response is not None \
-               and api_token_polling_response.status == self.FAILED_POLLING_STATUS
+        return (
+            api_token_polling_response is not None and api_token_polling_response.status == self.FAILED_POLLING_STATUS
+        )
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/ci_integrations.py` & `cycode-0.2.6.dev7/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cli/code_scanner.py` & `cycode-0.2.6.dev7/cycode/cli/code_scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,22 @@
 from cycode.cli.printers import ConsolePrinter
 from cycode.cli.models import Document, DocumentDetections, Severity, CliError, CliErrors, LocalScanResult
 from cycode.cli.ci_integrations import get_commit_range
 from cycode.cli import consts
 from cycode.cli.config import configuration_manager
 from cycode.cli.utils.progress_bar import ProgressBarSection
 from cycode.cli.utils.scan_utils import set_issue_detected
-from cycode.cli.utils.path_utils import is_sub_path, is_binary_file, get_file_size, get_relevant_files_in_path, \
-    get_path_by_os, get_file_content
+from cycode.cli.utils.path_utils import (
+    is_sub_path,
+    is_binary_file,
+    get_file_size,
+    get_relevant_files_in_path,
+    get_path_by_os,
+    get_file_content,
+)
 from cycode.cli.utils.scan_batch import run_parallel_batched_scan
 from cycode.cli.utils.string_utils import get_content_size, is_binary_content
 from cycode.cli.utils.task_timer import TimeoutAfter
 from cycode.cli.utils import scan_utils
 from cycode.cli.user_settings.config_file_manager import ConfigFileManager
 from cycode.cli.zip_file import InMemoryZip
 from cycode.cli.exceptions import custom_exceptions
@@ -39,22 +45,25 @@
     from cycode.cli.utils.progress_bar import BaseProgressBar
 
 start_scan_time = time.time()
 
 
 @click.command()
 @click.argument("path", nargs=1, type=click.STRING, required=True)
-@click.option('--branch', '-b',
-              default=None,
-              help='Branch to scan, if not set scanning the default branch',
-              type=str,
-              required=False)
+@click.option(
+    '--branch',
+    '-b',
+    default=None,
+    help='Branch to scan, if not set scanning the default branch',
+    type=str,
+    required=False,
+)
 @click.pass_context
 def scan_repository(context: click.Context, path: str, branch: str):
-    """ Scan git repository including its history """
+    """Scan git repository including its history"""
     try:
         logger.debug('Starting repository scan process, %s', {'path': path, 'branch': branch})
 
         scan_type = context.obj['scan_type']
         monitor = context.obj.get('monitor')
         if monitor and scan_type != consts.SCA_SCAN_TYPE:
             raise click.ClickException(f'Monitor flag is currently supported for SCA scan type only')
@@ -84,27 +93,26 @@
             context, documents_to_scan, is_git_diff=False, scan_parameters=get_scan_parameters(context, path)
         )
     except Exception as e:
         _handle_exception(context, e)
 
 
 @click.command()
-@click.argument("path",
-                nargs=1,
-                type=click.STRING,
-                required=True)
-@click.option("--commit_range", "-r",
-              help='Scan a commit range in this git repository, by default cycode scans all '
-                   'commit history (example: HEAD~1)',
-              type=click.STRING,
-              default="--all",
-              required=False)
+@click.argument("path", nargs=1, type=click.STRING, required=True)
+@click.option(
+    "--commit_range",
+    "-r",
+    help='Scan a commit range in this git repository, by default cycode scans all ' 'commit history (example: HEAD~1)',
+    type=click.STRING,
+    default="--all",
+    required=False,
+)
 @click.pass_context
 def scan_repository_commit_history(context: click.Context, path: str, commit_range: str):
-    """	Scan all the commits history in this git repository """
+    """Scan all the commits history in this git repository"""
     try:
         logger.debug('Starting commit history scan process, %s', {'path': path, 'commit_range': commit_range})
         return scan_commit_range(context, path=path, commit_range=commit_range)
     except Exception as e:
         _handle_exception(context, e)
 
 
@@ -139,64 +147,62 @@
         commit_id = commit.hexsha
         commit_ids_to_scan.append(commit_id)
         parent = commit.parents[0] if commit.parents else NULL_TREE
         diff = commit.diff(parent, create_patch=True, R=True)
         commit_documents_to_scan = []
         for blob in diff:
             blob_path = get_path_by_os(os.path.join(path, get_diff_file_path(blob)))
-            commit_documents_to_scan.append(Document(
-                path=blob_path,
-                content=blob.diff.decode('UTF-8', errors='replace'),
-                is_git_diff_format=True,
-                unique_id=commit_id
-            ))
+            commit_documents_to_scan.append(
+                Document(
+                    path=blob_path,
+                    content=blob.diff.decode('UTF-8', errors='replace'),
+                    is_git_diff_format=True,
+                    unique_id=commit_id,
+                )
+            )
 
         logger.debug(
             'Found all relevant files in commit %s',
-            {
-                'path': path,
-                'commit_range': commit_range,
-                'commit_id': commit_id
-            }
+            {'path': path, 'commit_range': commit_range, 'commit_id': commit_id},
         )
 
         documents_to_scan.extend(exclude_irrelevant_documents_to_scan(context, commit_documents_to_scan))
         scanned_commits_count += 1
 
     logger.debug('List of commit ids to scan, %s', {'commit_ids': commit_ids_to_scan})
     logger.debug('Starting to scan commit range (It may take a few minutes)')
 
     return scan_documents(context, documents_to_scan, is_git_diff=True, is_commit_range=True)
 
 
 @click.command()
 @click.pass_context
 def scan_ci(context: click.Context):
-    """ Execute scan in a CI environment which relies on the
-    CYCODE_TOKEN and CYCODE_REPO_LOCATION environment variables """
+    """Execute scan in a CI environment which relies on the
+    CYCODE_TOKEN and CYCODE_REPO_LOCATION environment variables"""
     return scan_commit_range(context, path=os.getcwd(), commit_range=get_commit_range())
 
 
 @click.command()
 @click.argument("path", nargs=1, type=click.STRING, required=True)
 @click.pass_context
 def scan_path(context: click.Context, path):
-    """	Scan the files in the path supplied in the command """
+    """Scan the files in the path supplied in the command"""
     logger.debug('Starting path scan process, %s', {'path': path})
     files_to_scan = get_relevant_files_in_path(path=path, exclude_patterns=["**/.git/**", "**/.cycode/**"])
     files_to_scan = exclude_irrelevant_files(context, files_to_scan)
     logger.debug('Found all relevant files for scanning %s', {'path': path, 'file_to_scan_count': len(files_to_scan)})
     return scan_disk_files(context, path, files_to_scan)
 
 
 @click.command()
 @click.argument('ignored_args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
 def pre_commit_scan(context: click.Context, ignored_args: List[str]):
-    """ Use this command to scan the content that was not committed yet """
+    """Use this command to scan the content that was not committed yet"""
     scan_type = context.obj['scan_type']
     progress_bar = context.obj['progress_bar']
 
     if scan_type == consts.SCA_SCAN_TYPE:
         return scan_sca_pre_commit(context)
 
     diff_files = Repo(os.getcwd()).index.diff('HEAD', create_patch=True, R=True)
@@ -212,24 +218,25 @@
     return scan_documents(context, documents_to_scan, is_git_diff=True)
 
 
 @click.command()
 @click.argument("ignored_args", nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
 def pre_receive_scan(context: click.Context, ignored_args: List[str]):
-    """ Use this command to scan commits on the server side before pushing them to the repository """
+    """Use this command to scan commits on the server side before pushing them to the repository"""
     try:
         scan_type = context.obj['scan_type']
         if scan_type != consts.SECRET_SCAN_TYPE:
             raise click.ClickException(f'Commit range scanning for {scan_type.upper()} is not supported')
 
         if should_skip_pre_receive_scan():
             logger.info(
                 "A scan has been skipped as per your request."
-                " Please note that this may leave your system vulnerable to secrets that have not been detected")
+                " Please note that this may leave your system vulnerable to secrets that have not been detected"
+            )
             return
 
         if is_verbose_mode_requested_in_pre_receive_scan():
             enable_verbose_mode(context)
             logger.debug('Verbose mode enabled, all log levels will be displayed')
 
         command_scan_type = context.info_name
@@ -238,16 +245,15 @@
             if scan_type not in consts.COMMIT_RANGE_SCAN_SUPPORTED_SCAN_TYPES:
                 raise click.ClickException(f'Commit range scanning for {scan_type.upper()} is not supported')
 
             branch_update_details = parse_pre_receive_input()
             commit_range = calculate_pre_receive_commit_range(branch_update_details)
             if not commit_range:
                 logger.info(
-                    'No new commits found for pushed branch, %s',
-                    {'branch_update_details': branch_update_details}
+                    'No new commits found for pushed branch, %s', {'branch_update_details': branch_update_details}
                 )
                 return
 
             max_commits_to_scan = configuration_manager.get_pre_receive_max_commits_to_scan_count(command_scan_type)
             scan_commit_range(context, os.getcwd(), commit_range, max_commits_count=max_commits_to_scan)
             perform_post_pre_receive_scan_actions(context)
     except Exception as e:
@@ -256,34 +262,40 @@
 
 def scan_sca_pre_commit(context: click.Context):
     scan_parameters = get_default_scan_parameters(context)
     git_head_documents, pre_committed_documents = get_pre_commit_modified_documents(context.obj['progress_bar'])
     git_head_documents = exclude_irrelevant_documents_to_scan(context, git_head_documents)
     pre_committed_documents = exclude_irrelevant_documents_to_scan(context, pre_committed_documents)
     sca_code_scanner.perform_pre_hook_range_scan_actions(git_head_documents, pre_committed_documents)
-    return scan_commit_range_documents(context, git_head_documents, pre_committed_documents,
-                                       scan_parameters,
-                                       configuration_manager.get_sca_pre_commit_timeout_in_seconds())
+    return scan_commit_range_documents(
+        context,
+        git_head_documents,
+        pre_committed_documents,
+        scan_parameters,
+        configuration_manager.get_sca_pre_commit_timeout_in_seconds(),
+    )
 
 
 def scan_sca_commit_range(context: click.Context, path: str, commit_range: str):
     progress_bar = context.obj['progress_bar']
 
     scan_parameters = get_scan_parameters(context, path)
     from_commit_rev, to_commit_rev = parse_commit_range(commit_range, path)
     from_commit_documents, to_commit_documents = get_commit_range_modified_documents(
         progress_bar, path, from_commit_rev, to_commit_rev
     )
     from_commit_documents = exclude_irrelevant_documents_to_scan(context, from_commit_documents)
     to_commit_documents = exclude_irrelevant_documents_to_scan(context, to_commit_documents)
-    sca_code_scanner.perform_pre_commit_range_scan_actions(path, from_commit_documents, from_commit_rev,
-                                                           to_commit_documents, to_commit_rev)
+    sca_code_scanner.perform_pre_commit_range_scan_actions(
+        path, from_commit_documents, from_commit_rev, to_commit_documents, to_commit_rev
+    )
 
-    return scan_commit_range_documents(context, from_commit_documents, to_commit_documents,
-                                       scan_parameters=scan_parameters)
+    return scan_commit_range_documents(
+        context, from_commit_documents, to_commit_documents, scan_parameters=scan_parameters
+    )
 
 
 def scan_disk_files(context: click.Context, path: str, files_to_scan: List[str]):
     scan_parameters = get_scan_parameters(context, path)
     scan_type = context.obj['scan_type']
     progress_bar = context.obj['progress_bar']
 
@@ -306,15 +318,15 @@
 
 
 def set_issue_detected_by_scan_results(context: click.Context, scan_results: List[LocalScanResult]) -> None:
     set_issue_detected(context, any(scan_result.issue_detected for scan_result in scan_results))
 
 
 def _get_scan_documents_thread_func(
-        context: click.Context, is_git_diff: bool, is_commit_range: bool, scan_parameters: dict
+    context: click.Context, is_git_diff: bool, is_commit_range: bool, scan_parameters: dict
 ) -> Callable[[List[Document]], Tuple[str, CliError, LocalScanResult]]:
     cycode_client = context.obj['client']
     scan_type = context.obj['scan_type']
     severity_threshold = context.obj['severity_threshold']
     command_scan_type = context.info_name
 
     def _scan_batch_thread_func(batch: List[Document]) -> Tuple[str, CliError, LocalScanResult]:
@@ -349,33 +361,41 @@
 
         logger.debug(
             'Finished scan process, %s',
             {
                 'all_violations_count': detections_count,
                 'relevant_violations_count': relevant_detections_count,
                 'scan_id': scan_id,
-                'zip_file_size': zip_file_size
-            }
+                'zip_file_size': zip_file_size,
+            },
         )
         _report_scan_status(
-            cycode_client, scan_type, scan_id, scan_completed, relevant_detections_count,
-            detections_count, len(batch), zip_file_size, command_scan_type, error_message
+            cycode_client,
+            scan_type,
+            scan_id,
+            scan_completed,
+            relevant_detections_count,
+            detections_count,
+            len(batch),
+            zip_file_size,
+            command_scan_type,
+            error_message,
         )
 
         return scan_id, error, local_scan_result
 
     return _scan_batch_thread_func
 
 
 def scan_documents(
-        context: click.Context,
-        documents_to_scan: List[Document],
-        is_git_diff: bool = False,
-        is_commit_range: bool = False,
-        scan_parameters: Optional[dict] = None,
+    context: click.Context,
+    documents_to_scan: List[Document],
+    is_git_diff: bool = False,
+    is_commit_range: bool = False,
+    scan_parameters: Optional[dict] = None,
 ) -> None:
     progress_bar = context.obj['progress_bar']
 
     scan_batch_thread_func = _get_scan_documents_thread_func(context, is_git_diff, is_commit_range, scan_parameters)
     errors, local_scan_results = run_parallel_batched_scan(
         scan_batch_thread_func, documents_to_scan, progress_bar=progress_bar
     )
@@ -395,27 +415,27 @@
         #  because we should return only one root json structure per scan
         #  could be added later to "print_results" function if we wish to display detailed errors in UI
         return
 
     click.secho(
         'Unfortunately, Cycode was unable to complete the full scan. '
         'Please note that not all results may be available:',
-        fg='red'
+        fg='red',
     )
     for scan_id, error in errors.items():
         click.echo(f'- {scan_id}: ', nl=False)
         ConsolePrinter(context).print_error(error)
 
 
 def scan_commit_range_documents(
-        context: click.Context,
-        from_documents_to_scan: List[Document],
-        to_documents_to_scan: List[Document],
-        scan_parameters: Optional[dict] = None,
-        timeout: Optional[int] = None
+    context: click.Context,
+    from_documents_to_scan: List[Document],
+    to_documents_to_scan: List[Document],
+    scan_parameters: Optional[dict] = None,
+    timeout: Optional[int] = None,
 ) -> None:
     cycode_client = context.obj['client']
     scan_type = context.obj['scan_type']
     severity_threshold = context.obj['severity_threshold']
     scan_command_type = context.info_name
     progress_bar = context.obj['progress_bar']
 
@@ -438,16 +458,20 @@
 
             logger.debug('Preparing to-commit zip')
             to_commit_zipped_documents = zip_documents_to_scan(
                 scan_type, to_commit_zipped_documents, to_documents_to_scan
             )
 
             scan_result = perform_commit_range_scan_async(
-                cycode_client, from_commit_zipped_documents, to_commit_zipped_documents,
-                scan_type, scan_parameters, timeout
+                cycode_client,
+                from_commit_zipped_documents,
+                to_commit_zipped_documents,
+                scan_type,
+                scan_parameters,
+                timeout,
             )
 
         progress_bar.update(ProgressBarSection.SCAN)
         progress_bar.set_section_length(ProgressBarSection.GENERATE_REPORT, 1)
 
         local_scan_result = create_local_scan_result(
             scan_result, to_documents_to_scan, scan_command_type, scan_type, severity_threshold
@@ -460,49 +484,57 @@
         print_results(context, [local_scan_result])
 
         scan_completed = True
     except Exception as e:
         _handle_exception(context, e)
         error_message = str(e)
 
-    zip_file_size = getsizeof(from_commit_zipped_documents.in_memory_zip) + \
-        getsizeof(to_commit_zipped_documents.in_memory_zip)
+    zip_file_size = getsizeof(from_commit_zipped_documents.in_memory_zip) + getsizeof(
+        to_commit_zipped_documents.in_memory_zip
+    )
 
     detections_count = relevant_detections_count = 0
     if local_scan_result:
         detections_count = local_scan_result.detections_count
         relevant_detections_count = local_scan_result.relevant_detections_count
         scan_id = local_scan_result.scan_id
 
     logger.debug(
         'Finished scan process, %s',
         {
             'all_violations_count': detections_count,
             'relevant_violations_count': relevant_detections_count,
             'scan_id': scan_id,
-            'zip_file_size': zip_file_size
-        }
+            'zip_file_size': zip_file_size,
+        },
     )
     _report_scan_status(
-        cycode_client, scan_type, local_scan_result.scan_id, scan_completed,
-        local_scan_result.relevant_detections_count, local_scan_result.detections_count, len(to_documents_to_scan),
-        zip_file_size, scan_command_type, error_message
+        cycode_client,
+        scan_type,
+        local_scan_result.scan_id,
+        scan_completed,
+        local_scan_result.relevant_detections_count,
+        local_scan_result.detections_count,
+        len(to_documents_to_scan),
+        zip_file_size,
+        scan_command_type,
+        error_message,
     )
 
 
 def should_scan_documents(from_documents_to_scan: List[Document], to_documents_to_scan: List[Document]) -> bool:
     return len(from_documents_to_scan) > 0 or len(to_documents_to_scan) > 0
 
 
 def create_local_scan_result(
-        scan_result: ZippedFileScanResult,
-        documents_to_scan: List[Document],
-        command_scan_type: str,
-        scan_type: str,
-        severity_threshold: str,
+    scan_result: ZippedFileScanResult,
+    documents_to_scan: List[Document],
+    command_scan_type: str,
+    scan_type: str,
+    severity_threshold: str,
 ) -> LocalScanResult:
     document_detections = get_document_detections(scan_result, documents_to_scan)
     relevant_document_detections_list = exclude_irrelevant_document_detections(
         document_detections, scan_type, command_scan_type, severity_threshold
     )
 
     detections_count = sum([len(document_detection.detections) for document_detection in document_detections])
@@ -512,35 +544,36 @@
 
     return LocalScanResult(
         scan_id=scan_result.scan_id,
         report_url=scan_result.report_url,
         document_detections=relevant_document_detections_list,
         issue_detected=len(relevant_document_detections_list) > 0,
         detections_count=detections_count,
-        relevant_detections_count=relevant_detections_count
+        relevant_detections_count=relevant_detections_count,
     )
 
 
 def perform_pre_scan_documents_actions(
-        context: click.Context, scan_type: str, documents_to_scan: List[Document], is_git_diff: bool = False
+    context: click.Context, scan_type: str, documents_to_scan: List[Document], is_git_diff: bool = False
 ) -> None:
     if scan_type == consts.SCA_SCAN_TYPE:
         logger.debug(f'Perform pre scan document actions')
         sca_code_scanner.add_dependencies_tree_document(context, documents_to_scan, is_git_diff)
 
 
 def zip_documents_to_scan(scan_type: str, zip_file: InMemoryZip, documents: List[Document]) -> InMemoryZip:
     start_zip_creation_time = time.time()
 
     for index, document in enumerate(documents):
         zip_file_size = getsizeof(zip_file.in_memory_zip)
         validate_zip_file_size(scan_type, zip_file_size)
 
-        logger.debug('adding file to zip, %s',
-                     {'index': index, 'filename': document.path, 'unique_id': document.unique_id})
+        logger.debug(
+            'adding file to zip, %s', {'index': index, 'filename': document.path, 'unique_id': document.unique_id}
+        )
         zip_file.append(document.path, document.unique_id, document.content)
     zip_file.close()
 
     end_zip_creation_time = time.time()
     zip_creation_time = int(end_zip_creation_time - start_zip_creation_time)
     logger.debug('finished to create zip file, %s', {'zip_creation_time': zip_creation_time})
     return zip_file
@@ -552,61 +585,58 @@
             raise custom_exceptions.ZipTooLargeError(consts.SCA_ZIP_MAX_SIZE_LIMIT_IN_BYTES)
     else:
         if zip_file_size > consts.ZIP_MAX_SIZE_LIMIT_IN_BYTES:
             raise custom_exceptions.ZipTooLargeError(consts.ZIP_MAX_SIZE_LIMIT_IN_BYTES)
 
 
 def perform_scan(
-        cycode_client: 'ScanClient',
-        zipped_documents: InMemoryZip,
-        scan_type: str,
-        scan_id: str,
-        is_git_diff: bool,
-        is_commit_range: bool,
-        scan_parameters: dict
+    cycode_client: 'ScanClient',
+    zipped_documents: InMemoryZip,
+    scan_type: str,
+    scan_id: str,
+    is_git_diff: bool,
+    is_commit_range: bool,
+    scan_parameters: dict,
 ) -> ZippedFileScanResult:
     if scan_type in (consts.SCA_SCAN_TYPE, consts.SAST_SCAN_TYPE):
         return perform_scan_async(cycode_client, zipped_documents, scan_type, scan_parameters)
 
     if is_commit_range:
         return cycode_client.commit_range_zipped_file_scan(scan_type, zipped_documents, scan_id)
 
     return cycode_client.zipped_file_scan(scan_type, zipped_documents, scan_id, scan_parameters, is_git_diff)
 
 
 def perform_scan_async(
-        cycode_client: 'ScanClient',
-        zipped_documents: InMemoryZip,
-        scan_type: str,
-        scan_parameters: dict
+    cycode_client: 'ScanClient', zipped_documents: InMemoryZip, scan_type: str, scan_parameters: dict
 ) -> ZippedFileScanResult:
     scan_async_result = cycode_client.zipped_file_scan_async(zipped_documents, scan_type, scan_parameters)
     logger.debug("scan request has been triggered successfully, scan id: %s", scan_async_result.scan_id)
 
     return poll_scan_results(cycode_client, scan_async_result.scan_id)
 
 
 def perform_commit_range_scan_async(
-        cycode_client: 'ScanClient',
-        from_commit_zipped_documents: InMemoryZip,
-        to_commit_zipped_documents: InMemoryZip,
-        scan_type: str,
-        scan_parameters: dict,
-        timeout: int = None
+    cycode_client: 'ScanClient',
+    from_commit_zipped_documents: InMemoryZip,
+    to_commit_zipped_documents: InMemoryZip,
+    scan_type: str,
+    scan_parameters: dict,
+    timeout: int = None,
 ) -> ZippedFileScanResult:
     scan_async_result = cycode_client.multiple_zipped_file_scan_async(
         from_commit_zipped_documents, to_commit_zipped_documents, scan_type, scan_parameters
     )
 
     logger.debug("scan request has been triggered successfully, scan id: %s", scan_async_result.scan_id)
     return poll_scan_results(cycode_client, scan_async_result.scan_id, timeout)
 
 
 def poll_scan_results(
-        cycode_client: 'ScanClient', scan_id: str, polling_timeout: Optional[int] = None
+    cycode_client: 'ScanClient', scan_id: str, polling_timeout: Optional[int] = None
 ) -> ZippedFileScanResult:
     if polling_timeout is None:
         polling_timeout = configuration_manager.get_scan_polling_timeout_in_seconds()
 
     last_scan_update_at = None
     end_polling_time = time.time() + polling_timeout
 
@@ -639,38 +669,33 @@
 
 def print_results(context: click.Context, local_scan_results: List[LocalScanResult]) -> None:
     printer = ConsolePrinter(context)
     printer.print_scan_results(local_scan_results)
 
 
 def get_document_detections(
-        scan_result: ZippedFileScanResult, documents_to_scan: List[Document]
+    scan_result: ZippedFileScanResult, documents_to_scan: List[Document]
 ) -> List[DocumentDetections]:
     logger.debug('Get document detections')
 
     document_detections = []
     for detections_per_file in scan_result.detections_per_file:
         file_name = get_path_by_os(detections_per_file.file_name)
         commit_id = detections_per_file.commit_id
 
         logger.debug('Going to find document of violated file, %s', {'file_name': file_name, 'commit_id': commit_id})
 
         document = _get_document_by_file_name(documents_to_scan, file_name, commit_id)
-        document_detections.append(
-            DocumentDetections(document=document, detections=detections_per_file.detections)
-        )
+        document_detections.append(DocumentDetections(document=document, detections=detections_per_file.detections))
 
     return document_detections
 
 
 def exclude_irrelevant_document_detections(
-        document_detections_list: List[DocumentDetections],
-        scan_type: str,
-        command_scan_type: str,
-        severity_threshold: str
+    document_detections_list: List[DocumentDetections], scan_type: str, command_scan_type: str, severity_threshold: str
 ) -> List[DocumentDetections]:
     relevant_document_detections_list = []
     for document_detections in document_detections_list:
         relevant_detections = exclude_irrelevant_detections(
             document_detections.detections, scan_type, command_scan_type, severity_threshold
         )
         if relevant_detections:
@@ -694,15 +719,16 @@
 
     :return: first branch update details (input's first line)
     """
     # FIXME(MarshalX): this blocks main thread forever if called outside of pre-receive hook
     pre_receive_input = sys.stdin.read().strip()
     if not pre_receive_input:
         raise ValueError(
-            "Pre receive input was not found. Make sure that you are using this command only in pre-receive hook")
+            "Pre receive input was not found. Make sure that you are using this command only in pre-receive hook"
+        )
 
     # each line represents a branch update request, handle the first one only
     # TODO(MichalBor): support case of multiple update branch requests
     branch_update_details = pre_receive_input.splitlines()[0]
     return branch_update_details
 
 
@@ -755,15 +781,15 @@
 
 
 def get_default_scan_parameters(context: click.Context) -> dict:
     return {
         "monitor": context.obj.get("monitor"),
         "report": context.obj.get("report"),
         "package_vulnerabilities": context.obj.get("package-vulnerabilities"),
-        "license_compliance": context.obj.get("license-compliance")
+        "license_compliance": context.obj.get("license-compliance"),
     }
 
 
 def get_scan_parameters(context: click.Context, path: str) -> dict:
     scan_parameters = get_default_scan_parameters(context)
     remote_url = try_get_git_remote_url(path)
     if remote_url:
@@ -780,17 +806,15 @@
             'remote_url': git_remote_url,
         }
     except Exception as e:
         logger.debug('Failed to get git remote URL. %s', {'exception_message': str(e)})
         return None
 
 
-def exclude_irrelevant_documents_to_scan(
-        context: click.Context, documents_to_scan: List[Document]
-) -> List[Document]:
+def exclude_irrelevant_documents_to_scan(context: click.Context, documents_to_scan: List[Document]) -> List[Document]:
     logger.debug('Excluding irrelevant documents to scan')
 
     scan_type = context.obj['scan_type']
 
     relevant_documents = []
     for document in documents_to_scan:
         if _is_relevant_document_to_scan(scan_type, document.path, document.content):
@@ -807,40 +831,40 @@
         if _is_relevant_file_to_scan(scan_type, filename):
             relevant_files.append(filename)
 
     return relevant_files
 
 
 def exclude_irrelevant_detections(
-        detections: List[Detection], scan_type: str, command_scan_type: str, severity_threshold: str
+    detections: List[Detection], scan_type: str, command_scan_type: str, severity_threshold: str
 ) -> List[Detection]:
     relevant_detections = _exclude_detections_by_exclusions_configuration(detections, scan_type)
     relevant_detections = _exclude_detections_by_scan_type(relevant_detections, scan_type, command_scan_type)
     relevant_detections = _exclude_detections_by_severity(relevant_detections, scan_type, severity_threshold)
 
     return relevant_detections
 
 
 def _exclude_detections_by_severity(
-        detections: List[Detection], scan_type: str, severity_threshold: str
+    detections: List[Detection], scan_type: str, severity_threshold: str
 ) -> List[Detection]:
     if scan_type != consts.SCA_SCAN_TYPE or severity_threshold is None:
         return detections
 
     relevant_detections = []
     for detection in detections:
         severity = detection.detection_details.get('advisory_severity')
         if _does_severity_match_severity_threshold(severity, severity_threshold):
             relevant_detections.append(detection)
 
     return relevant_detections
 
 
 def _exclude_detections_by_scan_type(
-        detections: List[Detection], scan_type: str, command_scan_type: str
+    detections: List[Detection], scan_type: str, command_scan_type: str
 ) -> List[Detection]:
     if command_scan_type == consts.PRE_COMMIT_COMMAND_SCAN_TYPE:
         return exclude_detections_in_deleted_lines(detections)
 
     exclude_in_deleted_lines = configuration_manager.get_should_exclude_detections_in_deleted_lines(command_scan_type)
     if command_scan_type in consts.COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES:
         if scan_type == consts.SECRET_SCAN_TYPE and exclude_in_deleted_lines:
@@ -879,15 +903,15 @@
             file_content = get_file_content(file_path)
             pre_committed_documents.append(Document(file_path, file_content))
 
     return git_head_documents, pre_committed_documents
 
 
 def get_commit_range_modified_documents(
-        progress_bar: 'BaseProgressBar',  path: str, from_commit_rev: str, to_commit_rev: str
+    progress_bar: 'BaseProgressBar', path: str, from_commit_rev: str, to_commit_rev: str
 ) -> Tuple[List[Document], List[Document]]:
     from_commit_documents = []
     to_commit_documents = []
 
     repo = Repo(path)
     diff = repo.commit(from_commit_rev).diff(to_commit_rev)
 
@@ -911,51 +935,59 @@
 
     return from_commit_documents, to_commit_documents
 
 
 def _should_exclude_detection(detection: Detection, exclusions: Dict) -> bool:
     exclusions_by_value = exclusions.get(consts.EXCLUSIONS_BY_VALUE_SECTION_NAME, [])
     if _is_detection_sha_configured_in_exclusions(detection, exclusions_by_value):
-        logger.debug('Going to ignore violations because is in the values to ignore list, %s',
-                     {'sha': detection.detection_details.get('sha512', '')})
+        logger.debug(
+            'Going to ignore violations because is in the values to ignore list, %s',
+            {'sha': detection.detection_details.get('sha512', '')},
+        )
         return True
 
     exclusions_by_sha = exclusions.get(consts.EXCLUSIONS_BY_SHA_SECTION_NAME, [])
     if _is_detection_sha_configured_in_exclusions(detection, exclusions_by_sha):
-        logger.debug('Going to ignore violations because is in the shas to ignore list, %s',
-                     {'sha': detection.detection_details.get('sha512', '')})
+        logger.debug(
+            'Going to ignore violations because is in the shas to ignore list, %s',
+            {'sha': detection.detection_details.get('sha512', '')},
+        )
         return True
 
     exclusions_by_rule = exclusions.get(consts.EXCLUSIONS_BY_RULE_SECTION_NAME, [])
     if exclusions_by_rule:
         detection_rule = detection.detection_rule_id
         if detection_rule in exclusions_by_rule:
-            logger.debug('Going to ignore violations because is in the shas to ignore list, %s',
-                         {'detection_rule': detection_rule})
+            logger.debug(
+                'Going to ignore violations because is in the shas to ignore list, %s',
+                {'detection_rule': detection_rule},
+            )
             return True
 
     exclusions_by_package = exclusions.get(consts.EXCLUSIONS_BY_PACKAGE_SECTION_NAME, [])
     if exclusions_by_package:
         package = _get_package_name(detection)
         if package in exclusions_by_package:
-            logger.debug('Going to ignore violations because is in the packages to ignore list, %s',
-                         {'package': package})
+            logger.debug(
+                'Going to ignore violations because is in the packages to ignore list, %s', {'package': package}
+            )
             return True
 
     return False
 
 
 def _is_detection_sha_configured_in_exclusions(detection, exclusions: List[str]) -> bool:
     detection_sha = detection.detection_details.get('sha512', '')
     return detection_sha in exclusions
 
 
 def _is_path_configured_in_exclusions(scan_type: str, file_path: str) -> bool:
-    exclusions_by_path = \
-        configuration_manager.get_exclusions_by_scan_type(scan_type).get(consts.EXCLUSIONS_BY_PATH_SECTION_NAME, [])
+    exclusions_by_path = configuration_manager.get_exclusions_by_scan_type(scan_type).get(
+        consts.EXCLUSIONS_BY_PATH_SECTION_NAME, []
+    )
     for exclusion_path in exclusions_by_path:
         if is_sub_path(exclusion_path, file_path):
             return True
     return False
 
 
 def _get_package_name(detection: Detection) -> str:
@@ -967,158 +999,156 @@
         package_version = detection.detection_details.get('package_version', '')
 
     return f'{package_name}@{package_version}'
 
 
 def _is_file_relevant_for_sca_scan(filename: str) -> bool:
     if any([sca_excluded_path in filename for sca_excluded_path in consts.SCA_EXCLUDED_PATHS]):
-        logger.debug(
-            "file is irrelevant because it is from node_modules's inner path, %s",
-            {'filename': filename}
-        )
+        logger.debug("file is irrelevant because it is from node_modules's inner path, %s", {'filename': filename})
         return False
 
     return True
 
 
 def _is_relevant_file_to_scan(scan_type: str, filename: str) -> bool:
     if _is_subpath_of_cycode_configuration_folder(filename):
-        logger.debug("file is irrelevant because it is in cycode configuration directory, %s",
-                     {'filename': filename})
+        logger.debug("file is irrelevant because it is in cycode configuration directory, %s", {'filename': filename})
         return False
 
     if _is_path_configured_in_exclusions(scan_type, filename):
-        logger.debug("file is irrelevant because the file path is in the ignore paths list, %s",
-                     {'filename': filename})
+        logger.debug("file is irrelevant because the file path is in the ignore paths list, %s", {'filename': filename})
         return False
 
     if not _is_file_extension_supported(scan_type, filename):
-        logger.debug("file is irrelevant because the file extension is not supported, %s",
-                     {'filename': filename})
+        logger.debug("file is irrelevant because the file extension is not supported, %s", {'filename': filename})
         return False
 
     if is_binary_file(filename):
-        logger.debug("file is irrelevant because it is binary file, %s",
-                     {'filename': filename})
+        logger.debug("file is irrelevant because it is binary file, %s", {'filename': filename})
         return False
 
     if scan_type != consts.SCA_SCAN_TYPE and _does_file_exceed_max_size_limit(filename):
-        logger.debug("file is irrelevant because its exceeded max size limit, %s",
-                     {'filename': filename})
+        logger.debug("file is irrelevant because its exceeded max size limit, %s", {'filename': filename})
         return False
 
     if scan_type == consts.SCA_SCAN_TYPE and not _is_file_relevant_for_sca_scan(filename):
         return False
 
     return True
 
 
 def _is_relevant_document_to_scan(scan_type: str, filename: str, content: str) -> bool:
     if _is_subpath_of_cycode_configuration_folder(filename):
-        logger.debug("document is irrelevant because it is in cycode configuration directory, %s",
-                     {'filename': filename})
+        logger.debug(
+            "document is irrelevant because it is in cycode configuration directory, %s", {'filename': filename}
+        )
         return False
 
     if _is_path_configured_in_exclusions(scan_type, filename):
-        logger.debug("document is irrelevant because the document path is in the ignore paths list, %s",
-                     {'filename': filename})
+        logger.debug(
+            "document is irrelevant because the document path is in the ignore paths list, %s", {'filename': filename}
+        )
         return False
 
     if not _is_file_extension_supported(scan_type, filename):
-        logger.debug("document is irrelevant because the file extension is not supported, %s",
-                     {'filename': filename})
+        logger.debug("document is irrelevant because the file extension is not supported, %s", {'filename': filename})
         return False
 
     if is_binary_content(content):
-        logger.debug("document is irrelevant because it is binary, %s",
-                     {'filename': filename})
+        logger.debug("document is irrelevant because it is binary, %s", {'filename': filename})
         return False
 
     if scan_type != consts.SCA_SCAN_TYPE and _does_document_exceed_max_size_limit(content):
-        logger.debug("document is irrelevant because its exceeded max size limit, %s",
-                     {'filename': filename})
+        logger.debug("document is irrelevant because its exceeded max size limit, %s", {'filename': filename})
         return False
     return True
 
 
 def _is_file_extension_supported(scan_type: str, filename: str) -> bool:
     filename = filename.lower()
 
     if scan_type == consts.INFRA_CONFIGURATION_SCAN_TYPE:
-        return any(filename.endswith(supported_file_extension)
-                   for supported_file_extension in consts.INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES)
+        return any(
+            filename.endswith(supported_file_extension)
+            for supported_file_extension in consts.INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES
+        )
     elif scan_type == consts.SCA_SCAN_TYPE:
-        return any(filename.endswith(supported_file)
-                   for supported_file in consts.SCA_CONFIGURATION_SCAN_SUPPORTED_FILES)
+        return any(
+            filename.endswith(supported_file) for supported_file in consts.SCA_CONFIGURATION_SCAN_SUPPORTED_FILES
+        )
 
-    return all(not filename.endswith(file_extension_to_ignore)
-               for file_extension_to_ignore in consts.SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE)
+    return all(
+        not filename.endswith(file_extension_to_ignore)
+        for file_extension_to_ignore in consts.SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE
+    )
 
 
 def _does_file_exceed_max_size_limit(filename: str) -> bool:
     return consts.FILE_MAX_SIZE_LIMIT_IN_BYTES < get_file_size(filename)
 
 
 def _does_document_exceed_max_size_limit(content: str) -> bool:
     return consts.FILE_MAX_SIZE_LIMIT_IN_BYTES < get_content_size(content)
 
 
 def _get_document_by_file_name(
-        documents: List[Document], file_name: str, unique_id: Optional[str] = None
+    documents: List[Document], file_name: str, unique_id: Optional[str] = None
 ) -> Optional[Document]:
     for document in documents:
         if _normalize_file_path(document.path) == _normalize_file_path(file_name) and document.unique_id == unique_id:
             return document
 
     return None
 
 
 def _is_subpath_of_cycode_configuration_folder(filename: str) -> bool:
-    return is_sub_path(configuration_manager.global_config_file_manager.get_config_directory_path(), filename) \
-        or is_sub_path(configuration_manager.local_config_file_manager.get_config_directory_path(), filename) \
+    return (
+        is_sub_path(configuration_manager.global_config_file_manager.get_config_directory_path(), filename)
+        or is_sub_path(configuration_manager.local_config_file_manager.get_config_directory_path(), filename)
         or filename.endswith(ConfigFileManager.get_config_file_route())
+    )
 
 
 def _handle_exception(context: click.Context, e: Exception, *, return_exception: bool = False) -> Optional[CliError]:
     context.obj['did_fail'] = True
 
     if context.obj['verbose']:
         click.secho(f'Error: {traceback.format_exc()}', fg='red')
 
     errors: CliErrors = {
         custom_exceptions.NetworkError: CliError(
             soft_fail=True,
             code='cycode_error',
             message='Cycode was unable to complete this scan. '
-                    'Please try again by executing the `cycode scan` command'
+            'Please try again by executing the `cycode scan` command',
         ),
         custom_exceptions.ScanAsyncError: CliError(
             soft_fail=True,
             code='scan_error',
             message='Cycode was unable to complete this scan. '
-                    'Please try again by executing the `cycode scan` command'
+            'Please try again by executing the `cycode scan` command',
         ),
         custom_exceptions.HttpUnauthorizedError: CliError(
             soft_fail=True,
             code='auth_error',
             message='Unable to authenticate to Cycode, your token is either invalid or has expired. '
-                    'Please re-generate your token and reconfigure it by running the `cycode configure` command'
+            'Please re-generate your token and reconfigure it by running the `cycode configure` command',
         ),
         custom_exceptions.ZipTooLargeError: CliError(
             soft_fail=True,
             code='zip_too_large_error',
             message='The path you attempted to scan exceeds the current maximum scanning size cap (10MB). '
-                    'Please try ignoring irrelevant paths using the ‘cycode ignore --by-path’ command '
-                    'and execute the scan again'
+            'Please try ignoring irrelevant paths using the ‘cycode ignore --by-path’ command '
+            'and execute the scan again',
         ),
         InvalidGitRepositoryError: CliError(
             soft_fail=False,
             code='invalid_git_error',
             message='The path you supplied does not correlate to a git repository. '
-                    'Should you still wish to scan this path, use: ‘cycode scan path <path>’'
+            'Should you still wish to scan this path, use: ‘cycode scan path <path>’',
         ),
     }
 
     if type(e) in errors:
         error = errors[type(e)]
 
         if error.soft_fail is True:
@@ -1135,30 +1165,39 @@
 
     if isinstance(e, click.ClickException):
         raise e
 
     raise click.ClickException(str(e))
 
 
-def _report_scan_status(cycode_client: 'ScanClient', scan_type: str, scan_id: str, scan_completed: bool,
-                        output_detections_count: int, all_detections_count: int, files_to_scan_count: int,
-                        zip_size: int, command_scan_type: str, error_message: Optional[str]) -> None:
+def _report_scan_status(
+    cycode_client: 'ScanClient',
+    scan_type: str,
+    scan_id: str,
+    scan_completed: bool,
+    output_detections_count: int,
+    all_detections_count: int,
+    files_to_scan_count: int,
+    zip_size: int,
+    command_scan_type: str,
+    error_message: Optional[str],
+) -> None:
     try:
         end_scan_time = time.time()
         scan_status = {
             'zip_size': zip_size,
             'execution_time': int(end_scan_time - start_scan_time),
             'output_detections_count': output_detections_count,
             'all_detections_count': all_detections_count,
             'scannable_files_count': files_to_scan_count,
             'status': 'Completed' if scan_completed else 'Error',
             'scan_command_type': command_scan_type,
             'operation_system': platform(),
             'error_message': error_message,
-            'scan_type': scan_type
+            'scan_type': scan_type,
         }
 
         cycode_client.report_scan_status(scan_type, scan_id, scan_status)
     except Exception as e:
         logger.debug('Failed to report scan status, %s', {'exception_message': str(e)})
 
 
@@ -1171,36 +1210,33 @@
     if detection_severity_value is None:
         return True
 
     return detection_severity_value >= Severity.try_get_value(severity_threshold)
 
 
 def _get_scan_result(
-        cycode_client: 'ScanClient', scan_id: str, scan_details: 'ScanDetailsResponse'
+    cycode_client: 'ScanClient', scan_id: str, scan_details: 'ScanDetailsResponse'
 ) -> ZippedFileScanResult:
     if not scan_details.detections_count:
         return init_default_scan_result(scan_id, scan_details.metadata)
 
     wait_for_detections_creation(cycode_client, scan_id, scan_details.detections_count)
 
     scan_detections = cycode_client.get_scan_detections(scan_id)
     return ZippedFileScanResult(
         did_detect=True,
         detections_per_file=_map_detections_per_file(scan_detections),
         scan_id=scan_id,
-        report_url=_try_get_report_url(scan_details.metadata)
+        report_url=_try_get_report_url(scan_details.metadata),
     )
 
 
 def init_default_scan_result(scan_id: str, scan_metadata: Optional[str] = None) -> ZippedFileScanResult:
     return ZippedFileScanResult(
-        did_detect=False,
-        detections_per_file=[],
-        scan_id=scan_id,
-        report_url=_try_get_report_url(scan_metadata)
+        did_detect=False, detections_per_file=[], scan_id=scan_id, report_url=_try_get_report_url(scan_metadata)
     )
 
 
 def _try_get_report_url(metadata_json: Optional[str]) -> Optional[str]:
     if metadata_json is None:
         return None
 
@@ -1249,16 +1285,18 @@
                 detections_per_files[file_name] = [DetectionSchema().load(detection)]
             else:
                 detections_per_files[file_name].append(DetectionSchema().load(detection))
         except Exception as e:
             logger.debug("Failed to parse detection: %s", str(e))
             continue
 
-    return [DetectionsPerFile(file_name=file_name, detections=file_detections)
-            for file_name, file_detections in detections_per_files.items()]
+    return [
+        DetectionsPerFile(file_name=file_name, detections=file_detections)
+        for file_name, file_detections in detections_per_files.items()
+    ]
 
 
 def _get_file_name_from_detection(detection: dict) -> str:
     if detection['category'] == 'SAST':
         return detection['detection_details']['file_path']
 
     return detection['detection_details']['file_name']
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/consts.py` & `cycode-0.2.6.dev7/cycode/cli/consts.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,55 +3,98 @@
 COMMIT_HISTORY_COMMAND_SCAN_TYPE = 'commit_history'
 
 SECRET_SCAN_TYPE = 'secret'
 INFRA_CONFIGURATION_SCAN_TYPE = 'iac'
 SCA_SCAN_TYPE = "sca"
 SAST_SCAN_TYPE = "sast"
 
-INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES = [
-    '.tf', '.tf.json', '.json', '.yaml', '.yml', 'dockerfile'
-]
+INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES = ['.tf', '.tf.json', '.json', '.yaml', '.yml', 'dockerfile']
 
 SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE = [
-    '.7z', '.bmp', '.bz2', '.dmg', '.exe', '.gif', '.gz', '.ico', '.jar', '.jpg', '.jpeg', '.png', '.rar',
-    '.realm', '.s7z', '.svg', '.tar', '.tif', '.tiff', '.webp', '.zi', '.lock', '.css', '.less', '.dll',
-    '.enc', '.deb', '.obj', '.model'
+    '.7z',
+    '.bmp',
+    '.bz2',
+    '.dmg',
+    '.exe',
+    '.gif',
+    '.gz',
+    '.ico',
+    '.jar',
+    '.jpg',
+    '.jpeg',
+    '.png',
+    '.rar',
+    '.realm',
+    '.s7z',
+    '.svg',
+    '.tar',
+    '.tif',
+    '.tiff',
+    '.webp',
+    '.zi',
+    '.lock',
+    '.css',
+    '.less',
+    '.dll',
+    '.enc',
+    '.deb',
+    '.obj',
+    '.model',
 ]
 
 SCA_CONFIGURATION_SCAN_SUPPORTED_FILES = [
-    'cargo.lock', 'cargo.toml',
-    'composer.json', 'composer.lock',
-    'go.sum', 'go.mod', 'gopkg.lock',
-    'pom.xml', 'build.gradle', 'gradle.lockfile', 'build.gradle.kts',
-    'package.json', 'package-lock.json', 'yarn.lock', 'npm-shrinkwrap.json',
-    'packages.config', 'project.assets.json', 'packages.lock.json', 'nuget.config', '.csproj',
-    'gemfile', 'gemfile.lock',
-    'build.sbt', 'build.scala', 'build.sbt.lock',
-    'pyproject.toml', 'poetry.lock',
-    'pipfile', 'pipfile.lock', 'requirements.txt', 'setup.py'
+    'cargo.lock',
+    'cargo.toml',
+    'composer.json',
+    'composer.lock',
+    'go.sum',
+    'go.mod',
+    'gopkg.lock',
+    'pom.xml',
+    'build.gradle',
+    'gradle.lockfile',
+    'build.gradle.kts',
+    'package.json',
+    'package-lock.json',
+    'yarn.lock',
+    'npm-shrinkwrap.json',
+    'packages.config',
+    'project.assets.json',
+    'packages.lock.json',
+    'nuget.config',
+    '.csproj',
+    'gemfile',
+    'gemfile.lock',
+    'build.sbt',
+    'build.scala',
+    'build.sbt.lock',
+    'pyproject.toml',
+    'poetry.lock',
+    'pipfile',
+    'pipfile.lock',
+    'requirements.txt',
+    'setup.py',
 ]
 
-SCA_EXCLUDED_PATHS = [
-    'node_modules'
-]
+SCA_EXCLUDED_PATHS = ['node_modules']
 
 PROJECT_FILES_BY_ECOSYSTEM_MAP = {
     "crates": ["Cargo.lock", "Cargo.toml"],
     "composer": ["composer.json", "composer.lock"],
     "go": ["go.sum", "go.mod", "Gopkg.lock"],
     "maven_pom": ["pom.xml"],
     "maven_gradle": ["build.gradle", "build.gradle.kts", "gradle.lockfile"],
     "npm": ["package.json", "package-lock.json", "yarn.lock", "npm-shrinkwrap.json", ".npmrc"],
     "nuget": ["packages.config", "project.assets.json", "packages.lock.json", "nuget.config"],
     "ruby_gems": ["Gemfile", "Gemfile.lock"],
     "sbt": ["build.sbt", "build.scala", "build.sbt.lock"],
     "pypi_poetry": ["pyproject.toml", "poetry.lock"],
     "pypi_pipenv": ["Pipfile", "Pipfile.lock"],
     "pypi_requirements": ["requirements.txt"],
-    "pypi_setup": ["setup.py"]
+    "pypi_setup": ["setup.py"],
 }
 
 COMMIT_RANGE_SCAN_SUPPORTED_SCAN_TYPES = [SECRET_SCAN_TYPE, SCA_SCAN_TYPE]
 
 COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES = [PRE_RECEIVE_COMMAND_SCAN_TYPE, COMMIT_HISTORY_COMMAND_SCAN_TYPE]
 
 DEFAULT_CYCODE_API_URL = "https://api.cycode.com"
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.6.dev7/cycode/cli/exceptions/custom_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,18 @@
     def __init__(self, status_code: int, error_message: str, response: Response):
         self.status_code = status_code
         self.error_message = error_message
         self.response = response
         super().__init__(self.error_message)
 
     def __str__(self):
-        return f'error occurred during the request. status code: {self.status_code}, error message: ' \
-               f'{self.error_message}'
+        return (
+            f'error occurred during the request. status code: {self.status_code}, error message: '
+            f'{self.error_message}'
+        )
 
 
 class ScanAsyncError(CycodeError):
     def __init__(self, error_message: str):
         self.error_message = error_message
         super().__init__(self.error_message)
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.6.dev7/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,36 +13,36 @@
     return join_paths(get_file_dir(path), generated_file_name)
 
 
 def execute_command(command: List[str], file_name: str, command_timeout: int) -> Optional[Dict]:
     try:
         dependencies = shell(command, command_timeout)
     except Exception as e:
-        logger.debug('Failed to restore dependencies shell comment. %s',
-                     {'filename': file_name, 'exception': str(e)})
+        logger.debug('Failed to restore dependencies shell comment. %s', {'filename': file_name, 'exception': str(e)})
         return None
 
     return dependencies
 
 
 class BaseRestoreMavenDependencies(ABC):
-
-    def __init__(self, context: click.Context, is_git_diff: bool,
-                 command_timeout: int):
+    def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int):
         self.context = context
         self.is_git_diff = is_git_diff
         self.command_timeout = command_timeout
 
     def restore(self, document: Document) -> Optional[Document]:
         restore_dependencies_document = self.try_restore_dependencies(document)
         return restore_dependencies_document
 
     def get_manifest_file_path(self, document: Document) -> str:
-        return join_paths(self.context.params.get('path'), document.path) if self.context.obj.get(
-            'monitor') else document.path
+        return (
+            join_paths(self.context.params.get('path'), document.path)
+            if self.context.obj.get('monitor')
+            else document.path
+        )
 
     @abstractmethod
     def is_project(self, document: Document) -> bool:
         pass
 
     @abstractmethod
     def get_command(self, manifest_file_path: str) -> List[str]:
@@ -50,12 +50,13 @@
 
     @abstractmethod
     def get_lock_file_name(self) -> str:
         pass
 
     def try_restore_dependencies(self, document: Document) -> Optional[Document]:
         manifest_file_path = self.get_manifest_file_path(document)
-        document = Document(build_dep_tree_path(document.path, self.get_lock_file_name()),
-                            execute_command(self.get_command(manifest_file_path), manifest_file_path,
-                                            self.command_timeout),
-                            self.is_git_diff)
+        document = Document(
+            build_dep_tree_path(document.path, self.get_lock_file_name()),
+            execute_command(self.get_command(manifest_file_path), manifest_file_path, self.command_timeout),
+            self.is_git_diff,
+        )
         return document
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.6.dev7/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 BUILD_GRADLE_FILE_NAME = 'build.gradle'
 BUILD_GRADLE_KTS_FILE_NAME = 'build.gradle.kts'
 BUILD_GRADLE_DEP_TREE_FILE_NAME = 'gradle-dependencies-generated.txt'
 
 
 class RestoreGradleDependencies(BaseRestoreMavenDependencies):
-    def __init__(self, context: click.Context, is_git_diff: bool,
-                 command_timeout: int):
+    def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int):
         super().__init__(context, is_git_diff, command_timeout)
 
     def is_project(self, document: Document) -> bool:
         return document.path.endswith(BUILD_GRADLE_FILE_NAME) or document.path.endswith(BUILD_GRADLE_KTS_FILE_NAME)
 
     def get_command(self, manifest_file_path: str) -> List[str]:
         return ['gradle', 'dependencies', '-b', manifest_file_path, '-q', '--console', 'plain']
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.6.dev7/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from os import path
 from typing import List, Optional
 
 import click
 
-from cycode.cli.helpers.maven.base_restore_maven_dependencies import BaseRestoreMavenDependencies, build_dep_tree_path, \
-    execute_command
+from cycode.cli.helpers.maven.base_restore_maven_dependencies import (
+    BaseRestoreMavenDependencies,
+    build_dep_tree_path,
+    execute_command,
+)
 from cycode.cli.models import Document
 from cycode.cli.utils.path_utils import get_file_dir, get_file_content, join_paths
 
 BUILD_MAVEN_FILE_NAME = 'pom.xml'
 MAVEN_CYCLONE_DEP_TREE_FILE_NAME = 'bom.json'
 MAVEN_DEP_TREE_FILE_NAME = 'bcde.mvndeps'
 
 
 class RestoreMavenDependencies(BaseRestoreMavenDependencies):
-    def __init__(self, context: click.Context, is_git_diff: bool,
-                 command_timeout: int):
+    def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int):
         super().__init__(context, is_git_diff, command_timeout)
 
     def is_project(self, document: Document) -> bool:
         return path.basename(document.path).split('/')[-1] == BUILD_MAVEN_FILE_NAME
 
     def get_command(self, manifest_file_path: str) -> List[str]:
         return ['mvn', 'org.cyclonedx:cyclonedx-maven-plugin:2.7.4:makeAggregateBom', '-f', manifest_file_path]
@@ -27,36 +29,42 @@
     def get_lock_file_name(self) -> str:
         return join_paths('target', MAVEN_CYCLONE_DEP_TREE_FILE_NAME)
 
     def try_restore_dependencies(self, document: Document) -> Optional[Document]:
         restore_dependencies_document = super().try_restore_dependencies(document)
         manifest_file_path = self.get_manifest_file_path(document)
         if document.content is None:
-            restore_dependencies_document = self.restore_from_secondary_command(document, manifest_file_path,
-                                                                                restore_dependencies_document)
+            restore_dependencies_document = self.restore_from_secondary_command(
+                document, manifest_file_path, restore_dependencies_document
+            )
         else:
             restore_dependencies_document.content = get_file_content(
-                join_paths(get_file_dir(manifest_file_path), self.get_lock_file_name()))
+                join_paths(get_file_dir(manifest_file_path), self.get_lock_file_name())
+            )
 
         return restore_dependencies_document
 
     def restore_from_secondary_command(self, document, manifest_file_path, restore_dependencies_document):
         # TODO(MarshalX): does it even work? Missing argument
         secondary_restore_command = create_secondary_restore_command(manifest_file_path)
-        backup_restore_content = execute_command(
-            secondary_restore_command,
-            manifest_file_path,
-            self.command_timeout)
-        restore_dependencies_document = Document(build_dep_tree_path(document.path, MAVEN_DEP_TREE_FILE_NAME),
-                                                 backup_restore_content,
-                                                 self.is_git_diff)
+        backup_restore_content = execute_command(secondary_restore_command, manifest_file_path, self.command_timeout)
+        restore_dependencies_document = Document(
+            build_dep_tree_path(document.path, MAVEN_DEP_TREE_FILE_NAME), backup_restore_content, self.is_git_diff
+        )
         restore_dependencies = None
         if restore_dependencies_document.content is not None:
             restore_dependencies = restore_dependencies_document
             restore_dependencies.content = get_file_content(MAVEN_DEP_TREE_FILE_NAME)
 
         return restore_dependencies
 
 
 def create_secondary_restore_command(self, manifest_file_path):
-    return ['mvn', 'dependency:tree', '-B', '-DoutputType=text', '-f', manifest_file_path,
-            f'-DoutputFile={MAVEN_DEP_TREE_FILE_NAME}']
+    return [
+        'mvn',
+        'dependency:tree',
+        '-B',
+        '-DoutputType=text',
+        '-f',
+        manifest_file_path,
+        f'-DoutputFile={MAVEN_DEP_TREE_FILE_NAME}',
+    ]
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.6.dev7/cycode/cli/helpers/sca_code_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,48 +13,58 @@
 
 BUILD_GRADLE_FILE_NAME = 'build.gradle'
 BUILD_GRADLE_KTS_FILE_NAME = 'build.gradle.kts'
 BUILD_GRADLE_DEP_TREE_FILE_NAME = 'gradle-dependencies-generated.txt'
 BUILD_GRADLE_DEP_TREE_TIMEOUT = 180
 
 
-def perform_pre_commit_range_scan_actions(path: str, from_commit_documents: List[Document],
-                                          from_commit_rev: str, to_commit_documents: List[Document],
-                                          to_commit_rev: str) -> None:
+def perform_pre_commit_range_scan_actions(
+    path: str,
+    from_commit_documents: List[Document],
+    from_commit_rev: str,
+    to_commit_documents: List[Document],
+    to_commit_rev: str,
+) -> None:
     repo = Repo(path)
     add_ecosystem_related_files_if_exists(from_commit_documents, repo, from_commit_rev)
     add_ecosystem_related_files_if_exists(to_commit_documents, repo, to_commit_rev)
 
 
-def perform_pre_hook_range_scan_actions(git_head_documents: List[Document],
-                                        pre_committed_documents: List[Document]) -> None:
+def perform_pre_hook_range_scan_actions(
+    git_head_documents: List[Document], pre_committed_documents: List[Document]
+) -> None:
     repo = Repo(os.getcwd())
     add_ecosystem_related_files_if_exists(git_head_documents, repo, GIT_HEAD_COMMIT_REV)
     add_ecosystem_related_files_if_exists(pre_committed_documents)
 
 
-def add_ecosystem_related_files_if_exists(documents: List[Document], repo: Optional[Repo] = None,
-                                          commit_rev: Optional[str] = None):
+def add_ecosystem_related_files_if_exists(
+    documents: List[Document], repo: Optional[Repo] = None, commit_rev: Optional[str] = None
+):
     for doc in documents:
         ecosystem = get_project_file_ecosystem(doc)
         if ecosystem is None:
             logger.debug("failed to resolve project file ecosystem: %s", doc.path)
             continue
         documents_to_add = get_doc_ecosystem_related_project_files(doc, documents, ecosystem, commit_rev, repo)
         documents.extend(documents_to_add)
 
 
-def get_doc_ecosystem_related_project_files(doc: Document, documents: List[Document], ecosystem: str,
-                                            commit_rev: Optional[str], repo: Optional[Repo]) -> List[Document]:
+def get_doc_ecosystem_related_project_files(
+    doc: Document, documents: List[Document], ecosystem: str, commit_rev: Optional[str], repo: Optional[Repo]
+) -> List[Document]:
     documents_to_add: List[Document] = []
     for ecosystem_project_file in PROJECT_FILES_BY_ECOSYSTEM_MAP.get(ecosystem):
         file_to_search = join_paths(get_file_dir(doc.path), ecosystem_project_file)
         if not is_project_file_exists_in_documents(documents, file_to_search):
-            file_content = get_file_content_from_commit(repo, commit_rev, file_to_search) if repo \
+            file_content = (
+                get_file_content_from_commit(repo, commit_rev, file_to_search)
+                if repo
                 else get_file_content(file_to_search)
+            )
 
             if file_content is not None:
                 documents_to_add.append(Document(file_to_search, file_content))
 
     return documents_to_add
 
 
@@ -66,55 +76,55 @@
     for ecosystem, project_files in PROJECT_FILES_BY_ECOSYSTEM_MAP.items():
         for project_file in project_files:
             if document.path.endswith(project_file):
                 return ecosystem
     return None
 
 
-def try_restore_dependencies(context: click.Context, documents_to_add: List[Document], restore_dependencies,
-                             document: Document):
+def try_restore_dependencies(
+    context: click.Context, documents_to_add: List[Document], restore_dependencies, document: Document
+):
     if restore_dependencies.is_project(document):
         restore_dependencies_document = restore_dependencies.restore(document)
         if restore_dependencies_document is None:
-            logger.warning('Error occurred while trying to generate dependencies tree. %s',
-                           {'filename': document.path})
+            logger.warning('Error occurred while trying to generate dependencies tree. %s', {'filename': document.path})
             return
 
         if restore_dependencies_document.content is None:
-            logger.warning('Error occurred while trying to generate dependencies tree. %s',
-                           {'filename': document.path})
+            logger.warning('Error occurred while trying to generate dependencies tree. %s', {'filename': document.path})
             restore_dependencies_document.content = ''
         else:
             is_monitor_action = context.obj.get('monitor')
             project_path = context.params.get('path')
             manifest_file_path = get_manifest_file_path(document, is_monitor_action, project_path)
             logger.debug(f"Succeeded to generate dependencies tree on path: {manifest_file_path}")
 
         if restore_dependencies_document.path in documents_to_add:
             logger.debug(f"Duplicate document on restore for path: {restore_dependencies_document.path}")
         else:
             documents_to_add[restore_dependencies_document.path] = restore_dependencies_document
 
 
-def add_dependencies_tree_document(context: click.Context, documents_to_scan: List[Document],
-                                   is_git_diff: bool = False) -> None:
+def add_dependencies_tree_document(
+    context: click.Context, documents_to_scan: List[Document], is_git_diff: bool = False
+) -> None:
     documents_to_add: Dict[str, Document] = {}
     restore_dependencies_list = restore_handlers(context, is_git_diff)
 
     for restore_dependencies in restore_dependencies_list:
         for document in documents_to_scan:
             try_restore_dependencies(context, documents_to_add, restore_dependencies, document)
 
     documents_to_scan.extend(list(documents_to_add.values()))
 
 
 def restore_handlers(context, is_git_diff):
     return [
         RestoreGradleDependencies(context, is_git_diff, BUILD_GRADLE_DEP_TREE_TIMEOUT),
-        RestoreMavenDependencies(context, is_git_diff, BUILD_GRADLE_DEP_TREE_TIMEOUT)
+        RestoreMavenDependencies(context, is_git_diff, BUILD_GRADLE_DEP_TREE_TIMEOUT),
     ]
 
 
 def get_manifest_file_path(document: Document, is_monitor_action: bool, project_path: str) -> str:
     return join_paths(project_path, document.path) if is_monitor_action else document.path
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/main.py` & `cycode-0.2.6.dev7/cycode/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,79 +30,108 @@
 
 @click.group(
     commands={
         "repository": code_scanner.scan_repository,
         "commit_history": code_scanner.scan_repository_commit_history,
         "path": code_scanner.scan_path,
         "pre_commit": code_scanner.pre_commit_scan,
-        "pre_receive": code_scanner.pre_receive_scan
+        "pre_receive": code_scanner.pre_receive_scan,
     },
 )
-@click.option('--scan-type', '-t', default="secret",
-              help="""
+@click.option(
+    '--scan-type',
+    '-t',
+    default="secret",
+    help="""
               \b
               Specify the scan you wish to execute (secret/iac/sca), 
               the default is secret
               """,
-              type=click.Choice(config['scans']['supported_scans']))
-@click.option('--secret',
-              default=None,
-              help='Specify a Cycode client secret for this specific scan execution',
-              type=str,
-              required=False)
-@click.option('--client-id',
-              default=None,
-              help='Specify a Cycode client ID for this specific scan execution',
-              type=str,
-              required=False)
-@click.option('--show-secret',
-              is_flag=True,
-              default=False,
-              help='Show secrets in plain text',
-              type=bool,
-              required=False)
-@click.option('--soft-fail',
-              is_flag=True,
-              default=False,
-              help='Run scan without failing, always return a non-error status code',
-              type=bool,
-              required=False)
-@click.option('--output', default=None,
-              help="""
+    type=click.Choice(config['scans']['supported_scans']),
+)
+@click.option(
+    '--secret',
+    default=None,
+    help='Specify a Cycode client secret for this specific scan execution',
+    type=str,
+    required=False,
+)
+@click.option(
+    '--client-id',
+    default=None,
+    help='Specify a Cycode client ID for this specific scan execution',
+    type=str,
+    required=False,
+)
+@click.option(
+    '--show-secret', is_flag=True, default=False, help='Show secrets in plain text', type=bool, required=False
+)
+@click.option(
+    '--soft-fail',
+    is_flag=True,
+    default=False,
+    help='Run scan without failing, always return a non-error status code',
+    type=bool,
+    required=False,
+)
+@click.option(
+    '--output',
+    default=None,
+    help="""
               \b
               Specify the results output (text/json/table), 
               the default is text
               """,
-              type=click.Choice(['text', 'json', 'table']))
-@click.option('--severity-threshold',
-              default=None,
-              help='Show only violations at the specified level or higher (supported for SCA scan type only).',
-              type=click.Choice([e.name for e in Severity]),
-              required=False)
-@click.option('--sca-scan',
-              default=None,
-              help="Specify the sca scan you wish to execute (package-vulnerabilities/license-compliance), the default is both",
-              multiple=True,
-              type=click.Choice(config['scans']['supported_sca_scans']))
-@click.option('--monitor',
-              is_flag=True,
-              default=False,
-              help="When specified, the scan results will be recorded in the knowledge graph. Please note that when working in 'monitor' mode, the knowledge graph will not be updated as a result of SCM events (Push, Repo creation).(supported for SCA scan type only).",
-              type=bool,
-              required=False)
-@click.option('--report',
-              is_flag=True,
-              default=False,
-              help="When specified, a violations report will be generated. A URL link to the report will be printed as an output to the command execution",
-              type=bool,
-              required=False)
+    type=click.Choice(['text', 'json', 'table']),
+)
+@click.option(
+    '--severity-threshold',
+    default=None,
+    help='Show only violations at the specified level or higher (supported for SCA scan type only).',
+    type=click.Choice([e.name for e in Severity]),
+    required=False,
+)
+@click.option(
+    '--sca-scan',
+    default=None,
+    help="Specify the sca scan you wish to execute (package-vulnerabilities/license-compliance), the default is both",
+    multiple=True,
+    type=click.Choice(config['scans']['supported_sca_scans']),
+)
+@click.option(
+    '--monitor',
+    is_flag=True,
+    default=False,
+    help="When specified, the scan results will be recorded in the knowledge graph. Please note that when working in 'monitor' mode, the knowledge graph will not be updated as a result of SCM events (Push, Repo creation).(supported for SCA scan type only).",
+    type=bool,
+    required=False,
+)
+@click.option(
+    '--report',
+    is_flag=True,
+    default=False,
+    help="When specified, a violations report will be generated. A URL link to the report will be printed as an output to the command execution",
+    type=bool,
+    required=False,
+)
 @click.pass_context
-def code_scan(context: click.Context, scan_type, client_id, secret, show_secret, soft_fail, output, severity_threshold,
-              sca_scan: List[str], monitor, report):
-    """ Scan content for secrets/IaC/sca/SAST violations, You need to specify which scan type: ci/commit_history/path/repository/etc """
+def code_scan(
+    context: click.Context,
+    scan_type,
+    client_id,
+    secret,
+    show_secret,
+    soft_fail,
+    output,
+    severity_threshold,
+    sca_scan: List[str],
+    monitor,
+    report,
+):
+    """Scan content for secrets/IaC/sca/SAST violations, You need to specify which scan type: ci/commit_history/path/repository/etc"""
     if show_secret:
         context.obj["show_secret"] = show_secret
     else:
         context.obj["show_secret"] = config["result_printer"]["default"]["show_secret"]
 
     if soft_fail:
         context.obj["soft_fail"] = soft_fail
@@ -144,33 +173,35 @@
     if _should_fail_scan(context):
         exit_code = ISSUE_DETECTED_STATUS_CODE
 
     sys.exit(exit_code)
 
 
 @click.group(
-    commands={
-        "scan": code_scan,
-        "configure": set_credentials,
-        "ignore": add_exclusions,
-        "auth": authenticate
-    },
-    context_settings=CONTEXT
+    commands={"scan": code_scan, "configure": set_credentials, "ignore": add_exclusions, "auth": authenticate},
+    context_settings=CONTEXT,
 )
 @click.option(
-    "--verbose", "-v", is_flag=True, default=False, help="Show detailed logs",
+    "--verbose",
+    "-v",
+    is_flag=True,
+    default=False,
+    help="Show detailed logs",
 )
 @click.option(
-    '--no-progress-meter', is_flag=True, default=False, help='Do not show the progress meter',
+    '--no-progress-meter',
+    is_flag=True,
+    default=False,
+    help='Do not show the progress meter',
 )
 @click.option(
     '--output',
     default='text',
     help='Specify the output (text/json/table), the default is text',
-    type=click.Choice(['text', 'json', 'table'])
+    type=click.Choice(['text', 'json', 'table']),
 )
 @click.option(
     '--user-agent',
     default=None,
     help='Characteristic JSON object that lets servers identify the application',
     type=str,
 )
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/models.py` & `cycode-0.2.6.dev7/cycode/cli/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,24 @@
     def __init__(self, path: str, content: str, is_git_diff_format: bool = False, unique_id: str = None):
         self.path = path
         self.content = content
         self.is_git_diff_format = is_git_diff_format
         self.unique_id = unique_id
 
     def __repr__(self) -> str:
-        return (
-            "path:{0}, "
-            "content:{1}".format(self.path, self.content)
-        )
+        return "path:{0}, " "content:{1}".format(self.path, self.content)
 
 
 class DocumentDetections:
     def __init__(self, document: Document, detections: List[Detection]):
         self.document = document
         self.detections = detections
 
     def __repr__(self) -> str:
-        return (
-            "document:{0}, "
-            "detections:{1}".format(self.document, self.detections)
-        )
+        return "document:{0}, " "detections:{1}".format(self.document, self.detections)
 
 
 class Severity(Enum):
     INFO = -1
     LOW = 0
     MEDIUM = 1
     MODERATE = 1
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/printers/base_printer.py` & `cycode-0.2.6.dev7/cycode/cli/printers/base_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cli/printers/base_table_printer.py` & `cycode-0.2.6.dev7/cycode/cli/printers/base_table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cli/printers/console_printer.py` & `cycode-0.2.6.dev7/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cli/printers/json_printer.py` & `cycode-0.2.6.dev7/cycode/cli/printers/json_printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,20 @@
 
 if TYPE_CHECKING:
     from cycode.cli.models import LocalScanResult
 
 
 class JsonPrinter(BasePrinter):
     def print_result(self, result: CliResult) -> None:
-        result = {
-            'result': result.success,
-            'message': result.message
-        }
+        result = {'result': result.success, 'message': result.message}
 
         click.secho(self.get_data_json(result))
 
     def print_error(self, error: CliError) -> None:
-        result = {
-            'error': error.code,
-            'message': error.message
-        }
+        result = {'error': error.code, 'message': error.message}
 
         click.secho(self.get_data_json(result))
 
     def print_scan_results(self, local_scan_results: List['LocalScanResult']) -> None:
         detections = []
         for local_scan_result in local_scan_results:
             for document_detections in local_scan_result.document_detections:
@@ -36,16 +30,16 @@
 
         detections_dict = DetectionSchema(many=True).dump(detections)
 
         click.secho(self._get_json_scan_result(detections_dict))
 
     def _get_json_scan_result(self, detections: dict) -> str:
         result = {
-            'scan_id': 'DEPRECATED',    # FIXME(MarshalX): we need change JSON struct to support multiple scan results
-            'detections': detections
+            'scan_id': 'DEPRECATED',  # FIXME(MarshalX): we need change JSON struct to support multiple scan results
+            'detections': detections,
         }
 
         return self.get_data_json(result)
 
     @staticmethod
     def get_data_json(data: dict) -> str:
         # ensure_ascii is disabled for symbols like "`". Eg: `cycode scan`
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/printers/sca_table_printer.py` & `cycode-0.2.6.dev7/cycode/cli/printers/sca_table_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 class SCATablePrinter(BaseTablePrinter):
     def _print_results(self, local_scan_results: List['LocalScanResult']) -> None:
         detections_per_detection_type_id = self._extract_detections_per_detection_type_id(local_scan_results)
         self._print_detection_per_detection_type_id(detections_per_detection_type_id)
 
     @staticmethod
     def _extract_detections_per_detection_type_id(
-            local_scan_results: List['LocalScanResult']
+        local_scan_results: List['LocalScanResult'],
     ) -> Dict[str, List[Detection]]:
         detections_per_detection_type_id = defaultdict(list)
 
         for local_scan_result in local_scan_results:
             for document_detection in local_scan_result.document_detections:
                 for detection in document_detection.detections:
                     detections_per_detection_type_id[detection.detection_type_id].append(detection)
 
         return detections_per_detection_type_id
 
     def _print_detection_per_detection_type_id(
-            self, detections_per_detection_type_id: Dict[str, List[Detection]]
+        self, detections_per_detection_type_id: Dict[str, List[Detection]]
     ) -> None:
         for detection_type_id in detections_per_detection_type_id:
             detections = detections_per_detection_type_id[detection_type_id]
             headers = self._get_table_headers()
 
             title = None
             rows = []
@@ -80,17 +80,15 @@
 
     def _get_table_headers(self) -> list:
         if self._is_git_repository():
             return [REPOSITORY_COLUMN]
 
         return []
 
-    def _print_table_detections(
-            self, detections: List[Detection], headers: List[str], rows, title: str
-    ) -> None:
+    def _print_table_detections(self, detections: List[Detection], headers: List[str], rows, title: str) -> None:
         self._print_summary_issues(detections, title)
         text_table = Texttable()
         text_table.header(headers)
 
         self.set_table_width(headers, text_table)
 
         for row in rows:
@@ -123,28 +121,28 @@
 
         row = [
             detection.detection_details.get('file_name'),
             detection.detection_details.get('ecosystem'),
             detection.detection_details.get('package_name'),
             detection.detection_details.get('is_direct_dependency_str'),
             detection.detection_details.get('is_dev_dependency_str'),
-            dependency_paths
+            dependency_paths,
         ]
 
         if self._is_git_repository():
             row = [detection.detection_details.get('repository_name')] + row
 
         return row
 
     def _get_upgrade_package_vulnerability(self, detection: Detection) -> List[str]:
         alert = detection.detection_details.get('alert')
         row = [
             detection.detection_details.get('advisory_severity'),
             *self._get_common_detection_fields(detection),
-            detection.detection_details.get('vulnerability_id')
+            detection.detection_details.get('vulnerability_id'),
         ]
 
         upgrade = ''
         if alert.get('first_patched_version'):
             upgrade = f'{alert.get("vulnerable_requirements")} -> {alert.get("first_patched_version")}'
         row.append(upgrade)
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/printers/table.py` & `cycode-0.2.6.dev7/cycode/cli/printers/table.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cli/printers/table_printer.py` & `cycode-0.2.6.dev7/cycode/cli/printers/table_printer.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,43 +87,43 @@
         return table
 
     def _enrich_table_with_values(self, table: Table, detection: Detection, document: Document) -> None:
         self._enrich_table_with_detection_summary_values(table, detection, document)
         self._enrich_table_with_detection_code_segment_values(table, detection, document)
 
     def _enrich_table_with_detection_summary_values(
-            self, table: Table, detection: Detection, document: Document
+        self, table: Table, detection: Detection, document: Document
     ) -> None:
         issue_type = detection.message
         if self.scan_type == SECRET_SCAN_TYPE:
             issue_type = detection.type
 
         table.set(ISSUE_TYPE_COLUMN, issue_type)
         table.set(RULE_ID_COLUMN, detection.detection_rule_id)
         table.set(FILE_PATH_COLUMN, click.format_filename(document.path))
         table.set(SECRET_SHA_COLUMN, detection.detection_details.get('sha512', ''))
         table.set(COMMIT_SHA_COLUMN, detection.detection_details.get('commit_id', ''))
 
     def _enrich_table_with_detection_code_segment_values(
-            self, table: Table, detection: Detection, document: Document
+        self, table: Table, detection: Detection, document: Document
     ) -> None:
         detection_details = detection.detection_details
 
         detection_line = detection_details.get('line_in_file', -1)
         if self.scan_type == SECRET_SCAN_TYPE:
             detection_line = detection_details.get('line', -1)
 
         detection_column = get_position_in_line(document.content, detection_details.get('start_position', -1))
         violation_length = detection_details.get('length', -1)
 
         violation = ''
         file_content_lines = document.content.splitlines()
         if detection_line < len(file_content_lines):
             line = file_content_lines[detection_line]
-            violation = line[detection_column: detection_column + violation_length]
+            violation = line[detection_column : detection_column + violation_length]
 
             if not self.show_secret:
                 violation = obfuscate_text(violation)
 
         table.set(LINE_NUMBER_COLUMN, str(detection_line))
         table.set(COLUMN_NUMBER_COLUMN, str(detection_column))
         table.set(VIOLATION_LENGTH_COLUMN, f'{violation_length} chars')
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/printers/text_printer.py` & `cycode-0.2.6.dev7/cycode/cli/printers/text_printer.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,24 +38,24 @@
         for local_scan_result in local_scan_results:
             for document_detections in local_scan_result.document_detections:
                 self._print_document_detections(
                     document_detections, local_scan_result.scan_id, local_scan_result.report_url
                 )
 
     def _print_document_detections(
-            self, document_detections: DocumentDetections, scan_id: str, report_url: Optional[str]
+        self, document_detections: DocumentDetections, scan_id: str, report_url: Optional[str]
     ):
         document = document_detections.document
         lines_to_display = self._get_lines_to_display_count()
         for detection in document_detections.detections:
             self._print_detection_summary(detection, document.path, scan_id, report_url)
             self._print_detection_code_segment(detection, document, lines_to_display)
 
     def _print_detection_summary(
-            self, detection: Detection, document_path: str, scan_id: str, report_url: Optional[str]
+        self, detection: Detection, document_path: str, scan_id: str, report_url: Optional[str]
     ):
         detection_name = detection.type if self.scan_type == SECRET_SCAN_TYPE else detection.message
 
         detection_sha = detection.detection_details.get('sha512')
         detection_sha_message = f'\nSecret SHA: {detection_sha}' if detection_sha else ''
 
         scan_id_message = f'\nScan ID: {scan_id}'
@@ -77,23 +77,31 @@
 
         self._print_detection_from_file(detection, document, code_segment_size)
 
     def _get_code_segment_start_line(self, detection_line: int, code_segment_size: int):
         start_line = detection_line - math.ceil(code_segment_size / 2)
         return 0 if start_line < 0 else start_line
 
-    def _print_line_of_code_segment(self, document: Document, line: str, line_number: int,
-                                    detection_position_in_line: int, violation_length: int, is_detection_line: bool):
+    def _print_line_of_code_segment(
+        self,
+        document: Document,
+        line: str,
+        line_number: int,
+        detection_position_in_line: int,
+        violation_length: int,
+        is_detection_line: bool,
+    ):
         if is_detection_line:
             self._print_detection_line(document, line, line_number, detection_position_in_line, violation_length)
         else:
             self._print_line(document, line, line_number)
 
-    def _print_detection_line(self, document: Document, line: str, line_number: int, detection_position_in_line: int,
-                              violation_length: int) -> None:
+    def _print_detection_line(
+        self, document: Document, line: str, line_number: int, detection_position_in_line: int, violation_length: int
+    ) -> None:
         click.echo(
             f'{self._get_line_number_style(line_number)} '
             f'{self._get_detection_line_style(line, document.is_git_diff_format, detection_position_in_line, violation_length)}'
         )
 
     def _print_line(self, document: Document, line: str, line_number: int):
         line_no = self._get_line_number_style(line_number)
@@ -102,27 +110,29 @@
         click.echo(f'{line_no} {line}')
 
     def _get_detection_line_style(self, line: str, is_git_diff: bool, start_position: int, length: int) -> str:
         line_color = self._get_line_color(line, is_git_diff)
         if self.scan_type != SECRET_SCAN_TYPE or start_position < 0 or length < 0:
             return self._get_line_style(line, is_git_diff, line_color)
 
-        violation = line[start_position: start_position + length]
+        violation = line[start_position : start_position + length]
         if not self.show_secret:
             violation = obfuscate_text(violation)
 
-        line_to_violation = line[0: start_position]
-        line_from_violation = line[start_position + length:]
+        line_to_violation = line[0:start_position]
+        line_from_violation = line[start_position + length :]
 
-        return f'{self._get_line_style(line_to_violation, is_git_diff, line_color)}' \
-               f'{self._get_line_style(violation, is_git_diff, line_color, underline=True)}' \
-               f'{self._get_line_style(line_from_violation, is_git_diff, line_color)}'
+        return (
+            f'{self._get_line_style(line_to_violation, is_git_diff, line_color)}'
+            f'{self._get_line_style(violation, is_git_diff, line_color, underline=True)}'
+            f'{self._get_line_style(line_from_violation, is_git_diff, line_color)}'
+        )
 
     def _get_line_style(
-            self, line: str, is_git_diff: bool, color: Optional[str] = None, underline: bool = False
+        self, line: str, is_git_diff: bool, color: Optional[str] = None, underline: bool = False
     ) -> str:
         if color is None:
             color = self._get_line_color(line, is_git_diff)
 
         return click.style(line, fg=color, bold=False, underline=underline)
 
     def _get_line_color(self, line: str, is_git_diff: bool) -> str:
@@ -134,30 +144,36 @@
 
         if line.startswith('-'):
             return self.RED_COLOR_NAME
 
         return self.WHITE_COLOR_NAME
 
     def _get_line_number_style(self, line_number: int):
-        return f'{click.style(str(line_number), fg=self.WHITE_COLOR_NAME, bold=False)} ' \
-               f'{click.style("|", fg=self.RED_COLOR_NAME, bold=False)}'
+        return (
+            f'{click.style(str(line_number), fg=self.WHITE_COLOR_NAME, bold=False)} '
+            f'{click.style("|", fg=self.RED_COLOR_NAME, bold=False)}'
+        )
 
     def _get_lines_to_display_count(self) -> int:
         result_printer_configuration = config.get('result_printer')
-        lines_to_display_of_scan = result_printer_configuration.get(self.scan_type, {}) \
-            .get(self.command_scan_type, {}).get('lines_to_display')
+        lines_to_display_of_scan = (
+            result_printer_configuration.get(self.scan_type, {}).get(self.command_scan_type, {}).get('lines_to_display')
+        )
         if lines_to_display_of_scan:
             return lines_to_display_of_scan
 
         return result_printer_configuration.get('default').get('lines_to_display')
 
     def _print_detection_from_file(self, detection: Detection, document: Document, code_segment_size: int):
         detection_details = detection.detection_details
-        detection_line = detection_details.get('line', -1) if self.scan_type == SECRET_SCAN_TYPE else \
-            detection_details.get('line_in_file', -1)
+        detection_line = (
+            detection_details.get('line', -1)
+            if self.scan_type == SECRET_SCAN_TYPE
+            else detection_details.get('line_in_file', -1)
+        )
         detection_position = detection_details.get('start_position', -1)
         violation_length = detection_details.get('length', -1)
 
         file_content = document.content
         file_lines = file_content.splitlines()
         start_line = self._get_code_segment_start_line(detection_line, code_segment_size)
         detection_position_in_line = get_position_in_line(file_content, detection_position)
@@ -166,16 +182,22 @@
         for i in range(code_segment_size):
             current_line_index = start_line + i
             if current_line_index >= len(file_lines):
                 break
 
             current_line = file_lines[current_line_index]
             is_detection_line = current_line_index == detection_line
-            self._print_line_of_code_segment(document, current_line, current_line_index + 1, detection_position_in_line,
-                                             violation_length, is_detection_line)
+            self._print_line_of_code_segment(
+                document,
+                current_line,
+                current_line_index + 1,
+                detection_position_in_line,
+                violation_length,
+                is_detection_line,
+            )
         click.echo()
 
     def _print_detection_from_git_diff(self, detection: Detection, document: Document):
         detection_details = detection.detection_details
         detection_line_number = detection_details.get('line', -1)
         detection_line_number_in_original_file = detection_details.get('line_in_file', -1)
         detection_position = detection_details.get('start_position', -1)
@@ -183,13 +205,18 @@
 
         git_diff_content = document.content
         git_diff_lines = git_diff_content.splitlines()
         detection_line = git_diff_lines[detection_line_number]
         detection_position_in_line = get_position_in_line(git_diff_content, detection_position)
 
         click.echo()
-        self._print_detection_line(document, detection_line, detection_line_number_in_original_file,
-                                   detection_position_in_line, violation_length)
+        self._print_detection_line(
+            document,
+            detection_line,
+            detection_line_number_in_original_file,
+            detection_position_in_line,
+            violation_length,
+        )
         click.echo()
 
     def _is_git_diff_based_scan(self):
         return self.command_scan_type in COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES and self.scan_type == SECRET_SCAN_TYPE
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.6.dev7/cycode/cli/user_settings/base_file_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 from abc import ABC, abstractmethod
 from cycode.cli.utils.yaml_utils import update_file, read_file
 
 
 class BaseFileManager(ABC):
-
     @abstractmethod
     def get_filename(self):
         pass
 
     def read_file(self):
         try:
             return read_file(self.get_filename())
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.6.dev7/cycode/cli/user_settings/config_file_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,50 +42,37 @@
     def get_max_commits(self, command_scan_type) -> Optional[int]:
         return self._get_value_from_command_scan_type_configuration(command_scan_type, self.MAX_COMMITS_FIELD_NAME)
 
     def get_command_timeout(self, command_scan_type) -> Optional[int]:
         return self._get_value_from_command_scan_type_configuration(command_scan_type, self.COMMAND_TIMEOUT_FIELD_NAME)
 
     def get_exclude_detections_in_deleted_lines(self, command_scan_type) -> Optional[bool]:
-        return self._get_value_from_command_scan_type_configuration(command_scan_type,
-                                                                    self.EXCLUDE_DETECTIONS_IN_DELETED_LINES)
+        return self._get_value_from_command_scan_type_configuration(
+            command_scan_type, self.EXCLUDE_DETECTIONS_IN_DELETED_LINES
+        )
 
     def update_base_url(self, base_url: str):
-        update_data = {
-            self.ENVIRONMENT_SECTION_NAME: {
-                self.API_URL_FIELD_NAME: base_url
-            }
-        }
+        update_data = {self.ENVIRONMENT_SECTION_NAME: {self.API_URL_FIELD_NAME: base_url}}
         self.write_content_to_file(update_data)
 
     def get_installation_id(self) -> Optional[str]:
         return self._get_value_from_environment_section(self.INSTALLATION_ID_FIELD_NAME)
 
     def update_installation_id(self, installation_id: str) -> None:
-        update_data = {
-            self.ENVIRONMENT_SECTION_NAME: {
-                self.INSTALLATION_ID_FIELD_NAME: installation_id
-            }
-        }
+        update_data = {self.ENVIRONMENT_SECTION_NAME: {self.INSTALLATION_ID_FIELD_NAME: installation_id}}
         self.write_content_to_file(update_data)
 
     def add_exclusion(self, scan_type, exclusion_type, new_exclusion):
         exclusions = self._get_exclusions_by_exclusion_type(scan_type, exclusion_type)
         if new_exclusion in exclusions:
             return
 
         exclusions.append(new_exclusion)
 
-        update_data = {
-            self.EXCLUSIONS_SECTION_NAME: {
-                scan_type: {
-                    exclusion_type: exclusions
-                }
-            }
-        }
+        update_data = {self.EXCLUSIONS_SECTION_NAME: {scan_type: {exclusion_type: exclusions}}}
         self.write_content_to_file(update_data)
 
     def get_config_directory_path(self) -> str:
         return os.path.join(self.path, self.CYCODE_HIDDEN_DIRECTORY)
 
     def get_filename(self) -> str:
         return os.path.join(self.get_config_directory_path(), self.FILE_NAME)
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.6.dev7/cycode/cli/user_settings/configuration_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,20 +91,26 @@
     def get_config_file_manager(self, scope: Optional[str] = None) -> ConfigFileManager:
         if scope == 'local':
             return self.local_config_file_manager
 
         return self.global_config_file_manager
 
     def get_scan_polling_timeout_in_seconds(self) -> int:
-        return int(self._get_value_from_environment_variables(SCAN_POLLING_TIMEOUT_IN_SECONDS_ENV_VAR_NAME,
-                                                              DEFAULT_SCAN_POLLING_TIMEOUT_IN_SECONDS))
+        return int(
+            self._get_value_from_environment_variables(
+                SCAN_POLLING_TIMEOUT_IN_SECONDS_ENV_VAR_NAME, DEFAULT_SCAN_POLLING_TIMEOUT_IN_SECONDS
+            )
+        )
 
     def get_sca_pre_commit_timeout_in_seconds(self) -> int:
-        return int(self._get_value_from_environment_variables(SCA_PRE_COMMIT_TIMEOUT_IN_SECONDS_ENV_VAR_NAME,
-                                                              DEFAULT_SCA_PRE_COMMIT_TIMEOUT_IN_SECONDS))
+        return int(
+            self._get_value_from_environment_variables(
+                SCA_PRE_COMMIT_TIMEOUT_IN_SECONDS_ENV_VAR_NAME, DEFAULT_SCA_PRE_COMMIT_TIMEOUT_IN_SECONDS
+            )
+        )
 
     def get_pre_receive_max_commits_to_scan_count(self, command_scan_type: str) -> int:
         max_commits = self._get_value_from_environment_variables(PRE_RECEIVE_MAX_COMMITS_TO_SCAN_COUNT_ENV_VAR_NAME)
         if max_commits is not None:
             return int(max_commits)
 
         max_commits = self.local_config_file_manager.get_max_commits(command_scan_type)
@@ -130,25 +136,28 @@
         if command_timeout is not None:
             return command_timeout
 
         return DEFAULT_PRE_RECEIVE_COMMAND_TIMEOUT_IN_SECONDS
 
     def get_should_exclude_detections_in_deleted_lines(self, command_scan_type: str) -> bool:
         exclude_detections_in_deleted_lines = self._get_value_from_environment_variables(
-            EXCLUDE_DETECTIONS_IN_DELETED_LINES_ENV_VAR_NAME)
+            EXCLUDE_DETECTIONS_IN_DELETED_LINES_ENV_VAR_NAME
+        )
         if exclude_detections_in_deleted_lines is not None:
             return exclude_detections_in_deleted_lines.lower() in ('true', '1')
 
-        exclude_detections_in_deleted_lines = self.local_config_file_manager \
-            .get_exclude_detections_in_deleted_lines(command_scan_type)
+        exclude_detections_in_deleted_lines = self.local_config_file_manager.get_exclude_detections_in_deleted_lines(
+            command_scan_type
+        )
         if exclude_detections_in_deleted_lines is not None:
             return exclude_detections_in_deleted_lines
 
-        exclude_detections_in_deleted_lines = self.global_config_file_manager\
-            .get_exclude_detections_in_deleted_lines(command_scan_type)
+        exclude_detections_in_deleted_lines = self.global_config_file_manager.get_exclude_detections_in_deleted_lines(
+            command_scan_type
+        )
         if exclude_detections_in_deleted_lines is not None:
             return exclude_detections_in_deleted_lines
 
         return DEFAULT_EXCLUDE_DETECTIONS_IN_DELETED_LINES
 
     @staticmethod
     def _get_value_from_environment_variables(env_var_name, default=None):
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.6.dev7/cycode/cli/user_settings/credentials_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from cycode.cli.utils.yaml_utils import read_file
 from cycode.cli.config import CYCODE_CLIENT_ID_ENV_VAR_NAME, CYCODE_CLIENT_SECRET_ENV_VAR_NAME
 from cycode.cli.user_settings.base_file_manager import BaseFileManager
 
 
 class CredentialsManager(BaseFileManager):
-
     HOME_PATH: str = Path.home()
     CYCODE_HIDDEN_DIRECTORY: str = '.cycode'
     FILE_NAME: str = 'credentials.yaml'
     CLIENT_ID_FIELD_NAME: str = 'cycode_client_id'
     CLIENT_SECRET_FIELD_NAME: str = 'cycode_client_secret'
 
     def get_credentials(self) -> (str, str):
@@ -34,17 +33,14 @@
             return None, None
 
         client_id = file_content.get(self.CLIENT_ID_FIELD_NAME)
         client_secret = file_content.get(self.CLIENT_SECRET_FIELD_NAME)
         return client_id, client_secret
 
     def update_credentials_file(self, client_id: str, client_secret: str):
-        credentials = {
-            self.CLIENT_ID_FIELD_NAME: client_id,
-            self.CLIENT_SECRET_FIELD_NAME: client_secret
-        }
+        credentials = {self.CLIENT_ID_FIELD_NAME: client_id, self.CLIENT_SECRET_FIELD_NAME: client_secret}
 
         filename = self.get_filename()
         self.write_content_to_file(credentials)
 
     def get_filename(self) -> str:
         return os.path.join(self.HOME_PATH, self.CYCODE_HIDDEN_DIRECTORY, self.FILE_NAME)
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.6.dev7/cycode/cli/user_settings/user_settings_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,59 +8,88 @@
 from cycode.cli.utils.path_utils import get_absolute_path
 from cycode.cli.user_settings.credentials_manager import CredentialsManager
 from cycode.cli.config import configuration_manager, config
 from cycode.cli.consts import *
 from cycode.cyclient import logger
 
 CREDENTIALS_UPDATED_SUCCESSFULLY_MESSAGE = 'Successfully configured CLI credentials!'
-CREDENTIALS_ARE_SET_IN_ENVIRONMENT_VARIABLES_MESSAGE = 'Note that the credentials that already exist in environment' \
-                                                       ' variables (CYCODE_CLIENT_ID and CYCODE_CLIENT_SECRET) take' \
-                                                       ' precedent over these credentials; either update or remove ' \
-                                                       'the environment variables.'
+CREDENTIALS_ARE_SET_IN_ENVIRONMENT_VARIABLES_MESSAGE = (
+    'Note that the credentials that already exist in environment'
+    ' variables (CYCODE_CLIENT_ID and CYCODE_CLIENT_SECRET) take'
+    ' precedent over these credentials; either update or remove '
+    'the environment variables.'
+)
 credentials_manager = CredentialsManager()
 
 
 @click.command()
 def set_credentials():
-    """ Initial command to authenticate your CLI client with Cycode using client ID and client secret """
+    """Initial command to authenticate your CLI client with Cycode using client ID and client secret"""
     click.echo(f'Update credentials in file ({credentials_manager.get_filename()})')
     current_client_id, current_client_secret = credentials_manager.get_credentials_from_file()
     client_id = _get_client_id_input(current_client_id)
     client_secret = _get_client_secret_input(current_client_secret)
 
     if not _should_update_credentials(current_client_id, current_client_secret, client_id, client_secret):
         return
 
     credentials_manager.update_credentials_file(client_id, client_secret)
     click.echo(_get_credentials_update_result_message())
 
 
 @click.command()
-@click.option("--by-value", type=click.STRING, required=False,
-              help="Ignore a specific value while scanning for secrets")
-@click.option("--by-sha", type=click.STRING, required=False,
-              help='Ignore a specific SHA512 representation of a string while scanning for secrets')
-@click.option("--by-path", type=click.STRING, required=False,
-              help='Avoid scanning a specific path. Need to specify scan type ')
-@click.option("--by-rule", type=click.STRING, required=False,
-              help='Ignore scanning a specific secret rule ID/IaC rule ID. Need to specify scan type.')
-@click.option("--by-package", type=click.STRING, required=False,
-              help='Ignore scanning a specific package version while running SCA scan. expected pattern - name@version')
-@click.option('--scan-type', '-t', default='secret',
-              help="""
+@click.option(
+    "--by-value", type=click.STRING, required=False, help="Ignore a specific value while scanning for secrets"
+)
+@click.option(
+    "--by-sha",
+    type=click.STRING,
+    required=False,
+    help='Ignore a specific SHA512 representation of a string while scanning for secrets',
+)
+@click.option(
+    "--by-path", type=click.STRING, required=False, help='Avoid scanning a specific path. Need to specify scan type '
+)
+@click.option(
+    "--by-rule",
+    type=click.STRING,
+    required=False,
+    help='Ignore scanning a specific secret rule ID/IaC rule ID. Need to specify scan type.',
+)
+@click.option(
+    "--by-package",
+    type=click.STRING,
+    required=False,
+    help='Ignore scanning a specific package version while running SCA scan. expected pattern - name@version',
+)
+@click.option(
+    '--scan-type',
+    '-t',
+    default='secret',
+    help="""
               \b
               Specify the scan you wish to execute (secrets/iac), 
               the default is secrets
               """,
-              type=click.Choice(config['scans']['supported_scans']), required=False)
-@click.option('--global', '-g', 'is_global', is_flag=True, default=False, required=False,
-              help='Add an ignore rule and update it in the global .cycode config file')
-def add_exclusions(by_value: str, by_sha: str, by_path: str, by_rule: str, by_package: str, scan_type: str,
-                   is_global: bool):
-    """ Ignore a specific value, path or rule ID """
+    type=click.Choice(config['scans']['supported_scans']),
+    required=False,
+)
+@click.option(
+    '--global',
+    '-g',
+    'is_global',
+    is_flag=True,
+    default=False,
+    required=False,
+    help='Add an ignore rule and update it in the global .cycode config file',
+)
+def add_exclusions(
+    by_value: str, by_sha: str, by_path: str, by_rule: str, by_package: str, scan_type: str, is_global: bool
+):
+    """Ignore a specific value, path or rule ID"""
     if not by_value and not by_sha and not by_path and not by_rule and not by_package:
         raise click.ClickException("ignore by type is missing")
 
     if by_value is not None:
         if scan_type != SECRET_SCAN_TYPE:
             raise click.ClickException("exclude by value is supported only for secret scan type")
         exclusion_type = EXCLUSIONS_BY_VALUE_SECTION_NAME
@@ -84,32 +113,37 @@
         exclusion_type = EXCLUSIONS_BY_PACKAGE_SECTION_NAME
         exclusion_value = by_package
     else:
         exclusion_type = EXCLUSIONS_BY_RULE_SECTION_NAME
         exclusion_value = by_rule
 
     configuration_scope = 'global' if is_global else 'local'
-    logger.debug('Adding ignore rule, %s',
-                 {'configuration_scope': configuration_scope, 'exclusion_type': exclusion_type,
-                  'exclusion_value': exclusion_value})
+    logger.debug(
+        'Adding ignore rule, %s',
+        {
+            'configuration_scope': configuration_scope,
+            'exclusion_type': exclusion_type,
+            'exclusion_value': exclusion_value,
+        },
+    )
     configuration_manager.add_exclusion(configuration_scope, scan_type, exclusion_type, exclusion_value)
 
 
 def _get_client_id_input(current_client_id: str) -> str:
-    new_client_id = click.prompt(f'cycode client id [{_obfuscate_credential(current_client_id)}]',
-                                 default='',
-                                 show_default=False)
+    new_client_id = click.prompt(
+        f'cycode client id [{_obfuscate_credential(current_client_id)}]', default='', show_default=False
+    )
 
     return current_client_id if not new_client_id else new_client_id
 
 
 def _get_client_secret_input(current_client_secret: str) -> str:
-    new_client_secret = click.prompt(f'cycode client secret [{_obfuscate_credential(current_client_secret)}]',
-                                     default='',
-                                     show_default=False)
+    new_client_secret = click.prompt(
+        f'cycode client secret [{_obfuscate_credential(current_client_secret)}]', default='', show_default=False
+    )
     return current_client_secret if not new_client_secret else new_client_secret
 
 
 def _get_credentials_update_result_message():
     if not _are_credentials_exist_in_environment_variables():
         return CREDENTIALS_UPDATED_SUCCESSFULLY_MESSAGE
 
@@ -117,16 +151,17 @@
 
 
 def _are_credentials_exist_in_environment_variables():
     client_id, client_secret = credentials_manager.get_credentials_from_environment_variables()
     return client_id is not None or client_secret is not None
 
 
-def _should_update_credentials(current_client_id: str, current_client_secret: str, new_client_id: str,
-                               new_client_secret: str) -> bool:
+def _should_update_credentials(
+    current_client_id: str, current_client_secret: str, new_client_id: str, new_client_secret: str
+) -> bool:
     return current_client_id != new_client_id or current_client_secret != new_client_secret
 
 
 def _obfuscate_credential(credential: Optional[str]) -> str:
     return '' if not credential else obfuscate_text(credential)
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/utils/path_utils.py` & `cycode-0.2.6.dev7/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cli/utils/progress_bar.py` & `cycode-0.2.6.dev7/cycode/cli/utils/progress_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,17 +175,15 @@
         if not self._current_section.section.has_next():
             return
 
         max_val = self._section_lengths.get(self._current_section.section, 0)
         cur_val = self._section_values.get(self._current_section.section, 0)
         if cur_val >= max_val:
             next_section = _PROGRESS_BAR_SECTIONS[self._current_section.section.next()]
-            logger.debug(
-                f'_update_current_section: {self._current_section.section} -> {next_section.section}'
-            )
+            logger.debug(f'_update_current_section: {self._current_section.section} -> {next_section.section}')
 
             self._current_section = next_section
             self._current_section_value = 0
             self._rerender_progress_bar()
 
     def _get_increment_progress_value(self, section: 'ProgressBarSection') -> int:
         max_val = self._section_lengths[section]
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/utils/scan_batch.py` & `cycode-0.2.6.dev7/cycode/cli/utils/scan_batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import os
 from multiprocessing.pool import ThreadPool
 from typing import List, TYPE_CHECKING, Callable, Tuple, Dict
 
-from cycode.cli.consts import SCAN_BATCH_MAX_SIZE_IN_BYTES, SCAN_BATCH_MAX_FILES_COUNT, SCAN_BATCH_SCANS_PER_CPU, \
-    SCAN_BATCH_MAX_PARALLEL_SCANS
+from cycode.cli.consts import (
+    SCAN_BATCH_MAX_SIZE_IN_BYTES,
+    SCAN_BATCH_MAX_FILES_COUNT,
+    SCAN_BATCH_SCANS_PER_CPU,
+    SCAN_BATCH_MAX_PARALLEL_SCANS,
+)
 from cycode.cli.models import Document
 from cycode.cli.utils.progress_bar import ProgressBarSection
 
 if TYPE_CHECKING:
     from cycode.cli.models import LocalScanResult, CliError
     from cycode.cli.utils.progress_bar import BaseProgressBar
 
 
 def split_documents_into_batches(
-        documents: List[Document],
-        max_size_mb: int = SCAN_BATCH_MAX_SIZE_IN_BYTES,
-        max_files_count: int = SCAN_BATCH_MAX_FILES_COUNT,
+    documents: List[Document],
+    max_size_mb: int = SCAN_BATCH_MAX_SIZE_IN_BYTES,
+    max_files_count: int = SCAN_BATCH_MAX_FILES_COUNT,
 ) -> List[List[Document]]:
     batches = []
 
     current_size = 0
     current_batch = []
     for document in documents:
         document_size = len(document.content.encode('UTF-8'))
@@ -40,19 +44,19 @@
 
 
 def _get_threads_count() -> int:
     return min(os.cpu_count() * SCAN_BATCH_SCANS_PER_CPU, SCAN_BATCH_MAX_PARALLEL_SCANS)
 
 
 def run_parallel_batched_scan(
-        scan_function: Callable[[List[Document]], Tuple[str, 'CliError', 'LocalScanResult']],
-        documents: List[Document],
-        progress_bar: 'BaseProgressBar',
-        max_size_mb: int = SCAN_BATCH_MAX_SIZE_IN_BYTES,
-        max_files_count: int = SCAN_BATCH_MAX_FILES_COUNT,
+    scan_function: Callable[[List[Document]], Tuple[str, 'CliError', 'LocalScanResult']],
+    documents: List[Document],
+    progress_bar: 'BaseProgressBar',
+    max_size_mb: int = SCAN_BATCH_MAX_SIZE_IN_BYTES,
+    max_files_count: int = SCAN_BATCH_MAX_FILES_COUNT,
 ) -> Tuple[Dict[str, 'CliError'], List['LocalScanResult']]:
     batches = split_documents_into_batches(documents, max_size_mb, max_files_count)
     progress_bar.set_section_length(ProgressBarSection.SCAN, len(batches))  # * 3
     # TODO(MarshalX): we should multiply the count of batches in SCAN section because each batch has 3 steps:
     # 1. scan creation
     # 2. scan completion
     # 3. detection creation
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/utils/shell_executor.py` & `cycode-0.2.6.dev7/cycode/cli/utils/shell_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from cycode.cyclient import logger
 
 _SUBPROCESS_DEFAULT_TIMEOUT_SEC = 60
 
 
 def shell(
-        command: Union[str, List[str]], timeout: int = _SUBPROCESS_DEFAULT_TIMEOUT_SEC, execute_in_shell=False
+    command: Union[str, List[str]], timeout: int = _SUBPROCESS_DEFAULT_TIMEOUT_SEC, execute_in_shell=False
 ) -> Optional[str]:
     logger.debug(f'Executing shell command: {command}')
 
     try:
         result = subprocess.run(
             command,
             timeout=timeout,
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/utils/string_utils.py` & `cycode-0.2.6.dev7/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cli/utils/task_timer.py` & `cycode-0.2.6.dev7/cycode/cli/utils/task_timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from threading import Thread, Event
 from _thread import interrupt_main
 from typing import Optional, Callable, List, Dict, Type
 from types import TracebackType
 
 
 class FunctionContext:
-
     def __init__(self, function: Callable, args: List = None, kwargs: Dict = None):
         self.function = function
         self.args = args or []
         self.kwargs = kwargs or {}
 
 
 class TimerThread(Thread):
     """
     Custom thread class for executing timer in the background
 
     Members:
         timeout - the amount of time to count until timeout in seconds
         quit_function (Mandatory) - function to perform when reaching to timeout
     """
-    def __init__(self, timeout: int,
-                 quit_function: FunctionContext):
+
+    def __init__(self, timeout: int, quit_function: FunctionContext):
         Thread.__init__(self)
         self._timeout = timeout
         self._quit_function = quit_function
         self.event = Event()
 
     def run(self):
         self._run_quit_function_on_timeout()
@@ -52,26 +51,27 @@
             <task logic>
 
     Members:
         timeout - the amount of time to count until timeout in seconds
         quit_function (Optional) - function to perform when reaching to timeout,
                                    the default option is to interrupt main thread
     """
-    def __init__(self, timeout: int,
-                 quit_function: Optional[FunctionContext] = None):
+
+    def __init__(self, timeout: int, quit_function: Optional[FunctionContext] = None):
         self.timeout = timeout
         self._quit_function = quit_function or FunctionContext(function=self.timeout_function)
         self.timer = TimerThread(timeout, quit_function=self._quit_function)
 
     def __enter__(self) -> None:
         if self.timeout:
             self.timer.start()
 
-    def __exit__(self, exc_type: Optional[Type[BaseException]], exc_val: Optional[BaseException],
-                 exc_tb: Optional[TracebackType]) -> None:
+    def __exit__(
+        self, exc_type: Optional[Type[BaseException]], exc_val: Optional[BaseException], exc_tb: Optional[TracebackType]
+    ) -> None:
         if self.timeout:
             self.timer.stop()
 
         # catch the exception of interrupt_main before exiting
         # the with statement and throw timeout error instead
         if exc_type == KeyboardInterrupt:
             raise TimeoutError(f"Task timed out after {self.timeout} seconds")
```

### Comparing `cycode-0.2.6.dev6/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.6.dev7/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cli/zip_file.py` & `cycode-0.2.6.dev7/cycode/cli/zip_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,10 +24,10 @@
         self.in_memory_zip.seek(0)
         return self.in_memory_zip.read()
 
 
 def concat_unique_id(filename: str, unique_id: str) -> str:
     if filename.startswith(os.sep):
         # remove leading slash to join path correctly
-        filename = filename[len(os.sep):]
+        filename = filename[len(os.sep) :]
 
     return os.path.join(unique_id, filename)
```

### Comparing `cycode-0.2.6.dev6/cycode/cyclient/auth_client.py` & `cycode-0.2.6.dev7/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cyclient/config.py` & `cycode-0.2.6.dev7/cycode/cyclient/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 import os
 import sys
 from urllib.parse import urlparse
 
 from cycode.cli.consts import *
 from cycode.cli.user_settings.configuration_manager import ConfigurationManager
+
 # set io encoding (for windows)
 from .config_dev import DEV_MODE_ENV_VAR_NAME, DEV_TENANT_ID_ENV_VAR_NAME
 
 sys.stdout.reconfigure(encoding='utf-8')
 sys.stderr.reconfigure(encoding='utf-8')
 
 # logs
 logging.basicConfig(
     stream=sys.stdout,
     level=logging.DEBUG,
     format="%(asctime)s [%(name)s] %(levelname)s: %(message)s",
-    datefmt="%Y-%m-%d %H:%M:%S"
+    datefmt="%Y-%m-%d %H:%M:%S",
 )
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 logging.getLogger("werkzeug").setLevel(logging.WARNING)
 logging.getLogger("schedule").setLevel(logging.WARNING)
 logging.getLogger("kubernetes").setLevel(logging.WARNING)
 logging.getLogger("binaryornot").setLevel(logging.WARNING)
 logging.getLogger("chardet").setLevel(logging.WARNING)
@@ -28,15 +29,15 @@
 logging.getLogger("git.util").setLevel(logging.WARNING)
 
 # configs
 DEFAULT_CONFIGURATION = {
     TIMEOUT_ENV_VAR_NAME: 300,
     LOGGING_LEVEL_ENV_VAR_NAME: logging.INFO,
     DEV_MODE_ENV_VAR_NAME: 'False',
-    BATCH_SIZE_ENV_VAR_NAME: 20
+    BATCH_SIZE_ENV_VAR_NAME: 20,
 }
 
 configuration = dict(DEFAULT_CONFIGURATION, **os.environ)
 
 
 def get_logger(logger_name=None):
     logger = logging.getLogger(logger_name)
```

### Comparing `cycode-0.2.6.dev6/cycode/cyclient/cycode_client_base.py` & `cycode-0.2.6.dev7/cycode/cyclient/cycode_client_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,56 +38,32 @@
     def reset_user_agent() -> None:
         CycodeClientBase.MANDATORY_HEADERS['User-Agent'] = get_cli_user_agent()
 
     @staticmethod
     def enrich_user_agent(user_agent_suffix: str) -> None:
         CycodeClientBase.MANDATORY_HEADERS['User-Agent'] += f' {user_agent_suffix}'
 
-    def post(
-            self,
-            url_path: str,
-            body: dict = None,
-            headers: dict = None,
-            **kwargs
-    ) -> Response:
+    def post(self, url_path: str, body: dict = None, headers: dict = None, **kwargs) -> Response:
         return self._execute(method='post', endpoint=url_path, json=body, headers=headers, **kwargs)
 
-    def put(
-            self,
-            url_path: str,
-            body: dict = None,
-            headers: dict = None,
-            **kwargs
-    ) -> Response:
+    def put(self, url_path: str, body: dict = None, headers: dict = None, **kwargs) -> Response:
         return self._execute(method='put', endpoint=url_path, json=body, headers=headers, **kwargs)
 
-    def get(
-            self,
-            url_path: str,
-            headers: dict = None,
-            **kwargs
-    ) -> Response:
+    def get(self, url_path: str, headers: dict = None, **kwargs) -> Response:
         return self._execute(method='get', endpoint=url_path, headers=headers, **kwargs)
 
     def _execute(
-            self,
-            method: str,
-            endpoint: str,
-            headers: dict = None,
-            without_auth: bool = False,
-            **kwargs
+        self, method: str, endpoint: str, headers: dict = None, without_auth: bool = False, **kwargs
     ) -> Response:
         url = self.build_full_url(self.api_url, endpoint)
         logger.debug(f'Executing {method.upper()} request to {url}')
 
         try:
             headers = self.get_request_headers(headers, without_auth=without_auth)
-            response = request(
-                method=method, url=url, timeout=self.timeout, headers=headers, **kwargs
-            )
+            response = request(method=method, url=url, timeout=self.timeout, headers=headers, **kwargs)
 
             logger.debug(f'Response {response.status_code} from {url}. Content: {response.text}')
 
             response.raise_for_status()
             return response
         except Exception as e:
             self._handle_exception(e)
```

### Comparing `cycode-0.2.6.dev6/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.6.dev7/cycode/cyclient/cycode_dev_based_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 """
 Send requests with api token
 """
 
 
 class CycodeDevBasedClient(CycodeClientBase):
-
     def __init__(self, api_url):
         super().__init__(api_url)
 
     def get_request_headers(self, additional_headers: dict = None):
         headers = super().get_request_headers(additional_headers=additional_headers)
         headers['X-Tenant-Id'] = dev_tenant_id
```

### Comparing `cycode-0.2.6.dev6/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.6.dev7/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev6/cycode/cyclient/models.py` & `cycode-0.2.6.dev7/cycode/cyclient/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from dataclasses import dataclass
 from typing import List, Dict, Optional
 from marshmallow import Schema, fields, EXCLUDE, post_load
 
 
 class Detection(Schema):
-    def __init__(self, detection_type_id: str, type: str, message: str, detection_details: dict,
-                 detection_rule_id: str, severity: Optional[str] = None):
+    def __init__(
+        self,
+        detection_type_id: str,
+        type: str,
+        message: str,
+        detection_details: dict,
+        detection_rule_id: str,
+        severity: Optional[str] = None,
+    ):
         super().__init__()
         self.message = message
         self.type = type
         self.severity = severity
         self.detection_type_id = detection_type_id
         self.detection_details = detection_details
         self.detection_rule_id = detection_rule_id
 
     def __repr__(self) -> str:
-        return f'type:{self.type}, ' \
-               f'severity:{self.severity}, ' \
-               f'message:{self.message}, ' \
-               f'detection_details:{repr(self.detection_details)}, ' \
-               f'detection_rule_id:{self.detection_rule_id}'
+        return (
+            f'type:{self.type}, '
+            f'severity:{self.severity}, '
+            f'message:{self.message}, '
+            f'detection_details:{repr(self.detection_details)}, '
+            f'detection_rule_id:{self.detection_rule_id}'
+        )
 
 
 class DetectionSchema(Schema):
     class Meta:
         unknown = EXCLUDE
 
     message = fields.String()
@@ -57,16 +66,22 @@
 
     @post_load
     def build_dto(self, data, **kwargs):
         return DetectionsPerFile(**data)
 
 
 class ZippedFileScanResult(Schema):
-    def __init__(self, did_detect: bool, detections_per_file: List[DetectionsPerFile], report_url: Optional[str] = None,
-                 scan_id: str = None, err: str = None):
+    def __init__(
+        self,
+        did_detect: bool,
+        detections_per_file: List[DetectionsPerFile],
+        report_url: Optional[str] = None,
+        scan_id: str = None,
+        err: str = None,
+    ):
         super().__init__()
         self.did_detect = did_detect
         self.detections_per_file = detections_per_file
         self.scan_id = scan_id
         self.report_url = report_url
         self.err = err
 
@@ -74,16 +89,15 @@
 class ZippedFileScanResultSchema(Schema):
     class Meta:
         unknown = EXCLUDE
 
     did_detect = fields.Boolean()
     scan_id = fields.String()
     report_url = fields.String(allow_none=True)
-    detections_per_file = fields.List(
-        fields.Nested(DetectionsPerFileSchema))
+    detections_per_file = fields.List(fields.Nested(DetectionsPerFileSchema))
     err = fields.String()
 
     @post_load
     def build_dto(self, data, **kwargs):
         return ZippedFileScanResult(**data)
 
 
@@ -98,16 +112,15 @@
 
 class ScanResultSchema(Schema):
     class Meta:
         unknown = EXCLUDE
 
     did_detect = fields.Boolean()
     scan_id = fields.String()
-    detections = fields.List(
-        fields.Nested(DetectionSchema), required=False, allow_none=True)
+    detections = fields.List(fields.Nested(DetectionSchema), required=False, allow_none=True)
     err = fields.String()
 
     @post_load
     def build_dto(self, data, **kwargs):
         return ScanResult(**data)
 
 
@@ -127,16 +140,24 @@
 
     @post_load
     def build_dto(self, data, **kwargs):
         return ScanInitializationResponse(**data)
 
 
 class ScanDetailsResponse(Schema):
-    def __init__(self, id: str = None, scan_status: str = None, results_count: int = None, metadata: str = None, message: str = None,
-                 scan_update_at: str = None, err: str = None):
+    def __init__(
+        self,
+        id: str = None,
+        scan_status: str = None,
+        results_count: int = None,
+        metadata: str = None,
+        message: str = None,
+        scan_update_at: str = None,
+        err: str = None,
+    ):
         super().__init__()
         self.id = id
         self.scan_status = scan_status
         self.detections_count = results_count
         self.metadata = metadata
         self.message = message
         self.scan_update_at = scan_update_at
@@ -283,17 +304,17 @@
     @post_load
     def build_dto(self, data, **kwargs):
         return ApiTokenGenerationPollingResponse(**data)
 
 
 class UserAgentOptionScheme(Schema):
     app_name = fields.String(required=True)  # ex. vscode_extension
-    app_version = fields.String(required=True)   # ex. 0.2.3
+    app_version = fields.String(required=True)  # ex. 0.2.3
     env_name = fields.String(required=True)  # ex.: Visual Studio Code
-    env_version = fields.String(required=True)   # ex. 1.78.2
+    env_version = fields.String(required=True)  # ex. 1.78.2
 
     @post_load
     def build_dto(self, data: dict, **_) -> 'UserAgentOption':
         return UserAgentOption(**data)
 
 
 @dataclass
@@ -305,12 +326,14 @@
 
     @property
     def user_agent_suffix(self) -> str:
         """Returns suffix of User-Agent.
 
         Example: vscode_extension (AppVersion: 0.1.2; EnvName: vscode; EnvVersion: 1.78.2)
         """
-        return f'{self.app_name} ' \
-               f'(' \
-               f'AppVersion: {self.app_version}; ' \
-               f'EnvName: {self.env_name}; EnvVersion: {self.env_version}' \
-               f')'
+        return (
+            f'{self.app_name} '
+            f'('
+            f'AppVersion: {self.app_version}; '
+            f'EnvName: {self.env_name}; EnvVersion: {self.env_version}'
+            f')'
+        )
```

### Comparing `cycode-0.2.6.dev6/cycode/cyclient/scan_client.py` & `cycode-0.2.6.dev7/cycode/cyclient/scan_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,50 +24,59 @@
 
     def file_scan(self, scan_type: str, path: str) -> models.ScanResult:
         url_path = f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}'
         files = {'file': open(path, 'rb')}
         response = self.scan_cycode_client.post(url_path=url_path, files=files)
         return self.parse_scan_response(response)
 
-    def zipped_file_scan(self, scan_type: str, zip_file: InMemoryZip, scan_id: str, scan_parameters: dict,
-                         is_git_diff: bool = False) -> models.ZippedFileScanResult:
+    def zipped_file_scan(
+        self, scan_type: str, zip_file: InMemoryZip, scan_id: str, scan_parameters: dict, is_git_diff: bool = False
+    ) -> models.ZippedFileScanResult:
         url_path = f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}/zipped-file'
         files = {'file': ('multiple_files_scan.zip', zip_file.read())}
 
         response = self.scan_cycode_client.post(
             url_path=url_path,
             data={'scan_id': scan_id, 'is_git_diff': is_git_diff, 'scan_parameters': json.dumps(scan_parameters)},
-            files=files
+            files=files,
         )
 
         return self.parse_zipped_file_scan_response(response)
 
-    def zipped_file_scan_async(self, zip_file: InMemoryZip, scan_type: str, scan_parameters: dict,
-                               is_git_diff: bool = False) -> models.ScanInitializationResponse:
+    def zipped_file_scan_async(
+        self, zip_file: InMemoryZip, scan_type: str, scan_parameters: dict, is_git_diff: bool = False
+    ) -> models.ScanInitializationResponse:
         url_path = f'{self.scan_config.get_scans_prefix()}/{self.SCAN_CONTROLLER_PATH}/{scan_type}/repository'
         files = {'file': ('multiple_files_scan.zip', zip_file.read())}
         response = self.scan_cycode_client.post(
             url_path=url_path,
             data={'is_git_diff': is_git_diff, 'scan_parameters': json.dumps(scan_parameters)},
-            files=files
+            files=files,
         )
         return models.ScanInitializationResponseSchema().load(response.json())
 
-    def multiple_zipped_file_scan_async(self, from_commit_zip_file: InMemoryZip, to_commit_zip_file: InMemoryZip,
-                                        scan_type: str, scan_parameters: dict,
-                                        is_git_diff: bool = False) -> models.ScanInitializationResponse:
-        url_path = f'{self.scan_config.get_scans_prefix()}/{self.SCAN_CONTROLLER_PATH}/{scan_type}/repository/commit-range'
+    def multiple_zipped_file_scan_async(
+        self,
+        from_commit_zip_file: InMemoryZip,
+        to_commit_zip_file: InMemoryZip,
+        scan_type: str,
+        scan_parameters: dict,
+        is_git_diff: bool = False,
+    ) -> models.ScanInitializationResponse:
+        url_path = (
+            f'{self.scan_config.get_scans_prefix()}/{self.SCAN_CONTROLLER_PATH}/{scan_type}/repository/commit-range'
+        )
         files = {
             'file_from_commit': ('multiple_files_scan.zip', from_commit_zip_file.read()),
-            'file_to_commit': ('multiple_files_scan.zip', to_commit_zip_file.read())
+            'file_to_commit': ('multiple_files_scan.zip', to_commit_zip_file.read()),
         }
         response = self.scan_cycode_client.post(
             url_path=url_path,
             data={'is_git_diff': is_git_diff, 'scan_parameters': json.dumps(scan_parameters)},
-            files=files
+            files=files,
         )
         return models.ScanInitializationResponseSchema().load(response.json())
 
     def get_scan_details(self, scan_id: str) -> models.ScanDetailsResponse:
         url_path = f'{self.scan_config.get_scans_prefix()}/{self.SCAN_CONTROLLER_PATH}/{scan_id}'
         response = self.scan_cycode_client.get(url_path=url_path)
         return models.ScanDetailsResponseSchema().load(response.json())
@@ -96,17 +105,19 @@
 
     def get_scan_detections_count(self, scan_id: str) -> int:
         url_path = f'{self.scan_config.get_detections_prefix()}/{self.DETECTIONS_SERVICE_CONTROLLER_PATH}/count?scan_id={scan_id}'
         response = self.scan_cycode_client.get(url_path=url_path)
         return response.json().get('count', 0)
 
     def commit_range_zipped_file_scan(
-            self, scan_type: str, zip_file: InMemoryZip, scan_id: str
+        self, scan_type: str, zip_file: InMemoryZip, scan_id: str
     ) -> models.ZippedFileScanResult:
-        url_path = f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}/commit-range-zipped-file'
+        url_path = (
+            f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}/commit-range-zipped-file'
+        )
         files = {'file': ('multiple_files_scan.zip', zip_file.read())}
         response = self.scan_cycode_client.post(url_path=url_path, data={'scan_id': scan_id}, files=files)
         return self.parse_zipped_file_scan_response(response)
 
     def report_scan_status(self, scan_type: str, scan_id: str, scan_status: dict):
         url_path = f'{self.scan_config.get_service_name(scan_type)}/{self.SCAN_CONTROLLER_PATH}/{scan_id}/status'
         self.scan_cycode_client.post(url_path=url_path, body=scan_status)
```

### Comparing `cycode-0.2.6.dev6/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.6.dev7/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from abc import ABC, abstractmethod
 
 
 class ScanConfigBase(ABC):
-
     @abstractmethod
     def get_service_name(self, scan_type):
         pass
 
     @abstractmethod
     def get_scans_prefix(self):
         pass
 
     @abstractmethod
     def get_detections_prefix(self):
         pass
 
 
 class DevScanConfig(ScanConfigBase):
-
     def get_service_name(self, scan_type):
         if scan_type == 'secret':
             return '5025'
         elif scan_type == 'iac':
             return '5026'
         elif scan_type == 'sca' or scan_type == 'sast':
             return '5004'
@@ -30,15 +28,14 @@
         return '5004'
 
     def get_detections_prefix(self):
         return '5016'
 
 
 class DefaultScanConfig(ScanConfigBase):
-
     def get_service_name(self, scan_type):
         if scan_type == 'secret':
             return 'secret'
         elif scan_type == 'iac':
             return 'iac'
         elif scan_type == 'sca' or scan_type == 'sast':
             return 'scans'
```

### Comparing `cycode-0.2.6.dev6/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.6.dev7/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 def create_scan_client(client_id: str, client_secret: str) -> ScanClient:
     if dev_mode:
         scan_cycode_client, scan_config = create_scan_for_dev_env()
     else:
         scan_cycode_client, scan_config = create_scan(client_id, client_secret)
 
-    return ScanClient(scan_cycode_client=scan_cycode_client,
-                      scan_config=scan_config)
+    return ScanClient(scan_cycode_client=scan_cycode_client, scan_config=scan_config)
 
 
 def create_scan(client_id: str, client_secret: str) -> Tuple[CycodeTokenBasedClient, DefaultScanConfig]:
     scan_cycode_client = CycodeTokenBasedClient(client_id, client_secret)
     scan_config = DefaultScanConfig()
     return scan_cycode_client, scan_config
```

### Comparing `cycode-0.2.6.dev6/pyproject.toml` & `cycode-0.2.6.dev7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.6.dev6" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.6.dev7" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
@@ -27,15 +27,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 click = ">=8.1.0,<8.2.0"
 colorama = ">=0.4.3,<0.5.0"
 pyyaml = ">=6.0,<7.0"
 marshmallow = ">=3.8.0,<3.9.0"
-pathspec = ">=0.8.0,<0.9.0"
+pathspec = ">=0.11.1,<0.12.0"
 gitpython = ">=3.1.30,<3.2.0"
 arrow = ">=0.17.0,<0.18.0"
 binaryornot = ">=0.4.4,<0.5.0"
 texttable = ">=1.6.7,<1.7.0"
 requests = ">=2.24,<3.0"
 
 [tool.poetry.group.test.dependencies]
@@ -45,22 +45,45 @@
 coverage = ">=7.2.3,<7.3.0"
 responses = ">=0.23.1,<0.24.0"
 
 [tool.poetry.group.executable.dependencies]
 pyinstaller = ">=5.11.0,<5.12.0"
 dunamai = ">=1.16.1,<1.17.0"
 
+[tool.poetry.group.dev.dependencies]
+black = ">=23.3.0,<23.4.0"
+
 [tool.pytest.ini_options]
 log_cli = true
 
 [tool.poetry-dynamic-versioning]
 # poetry self add "poetry-dynamic-versioning[plugin]"
 enable = false
 strict = true
 bump = true
 metadata = false
 vcs = "git"
 style = "pep440"
 
+[tool.black]
+line-length = 120
+skip-string-normalization=true
+target-version = ['py37']
+include = '\.pyi?$'
+exclude = '''
+(
+  /(
+      \.git
+    | \.mypy_cache
+    | .idea
+    | .pytest_cache
+    | venv
+    | htmlcov
+    | build
+    | dist
+  )/
+)
+'''
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `cycode-0.2.6.dev6/PKG-INFO` & `cycode-0.2.6.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.6.dev6
+Version: 0.2.6.dev7
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: arrow (>=0.17.0,<0.18.0)
 Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
 Requires-Dist: click (>=8.1.0,<8.2.0)
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
 Requires-Dist: gitpython (>=3.1.30,<3.2.0)
 Requires-Dist: marshmallow (>=3.8.0,<3.9.0)
-Requires-Dist: pathspec (>=0.8.0,<0.9.0)
+Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.24,<3.0)
 Requires-Dist: texttable (>=1.6.7,<1.7.0)
 Project-URL: Repository, https://github.com/cycodehq-public/cycode-cli
 Description-Content-Type: text/markdown
 
 # Cycode CLI User Guide
```

