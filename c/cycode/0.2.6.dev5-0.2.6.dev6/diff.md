# Comparing `tmp/cycode-0.2.6.dev5.tar.gz` & `tmp/cycode-0.2.6.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.6.dev5.tar", max compression
+gzip compressed data, was "cycode-0.2.6.dev6.tar", max compression
```

## Comparing `cycode-0.2.6.dev5.tar` & `cycode-0.2.6.dev6.tar`

### file list

```diff
@@ -1,62 +1,65 @@
--rw-r--r--   0        0        0    32549 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/README.md
--rw-r--r--   0        0        0      115 2023-06-28 11:24:43.689310 cycode-0.2.6.dev5/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     2813 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4761 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1652 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    47480 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      453 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5245 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1698 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2196 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      992 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2993 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5835 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     7243 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/main.py
--rw-r--r--   0        0        0     1332 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      626 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0     1483 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/base_table_printer.py
--rw-r--r--   0        0        0     1891 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1537 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     5624 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/sca_table_printer.py
--rw-r--r--   0        0        0     2277 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/table.py
--rw-r--r--   0        0        0      477 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/table_models.py
--rw-r--r--   0        0        0     4701 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     8955 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4821 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     6925 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1908 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6853 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0      195 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      941 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     1989 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2700 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      815 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      929 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       57 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1708 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2458 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      119 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3617 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      543 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1705 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     9102 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6222 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1090 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1021 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      197 2023-06-28 11:24:14.585321 cycode-0.2.6.dev5/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     2032 2023-06-28 11:24:43.689310 cycode-0.2.6.dev5/pyproject.toml
--rw-r--r--   0        0        0    34073 1970-01-01 00:00:00.000000 cycode-0.2.6.dev5/PKG-INFO
+-rw-r--r--   0        0        0    32549 2023-07-05 09:56:16.667783 cycode-0.2.6.dev6/README.md
+-rw-r--r--   0        0        0      115 2023-07-05 09:56:52.720173 cycode-0.2.6.dev6/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:56:16.667783 cycode-0.2.6.dev6/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:56:16.667783 cycode-0.2.6.dev6/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2793 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4761 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    53872 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5510 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1698 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2196 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      992 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2993 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5835 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     8226 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/main.py
+-rw-r--r--   0        0        0     1562 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      700 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0     1378 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/base_table_printer.py
+-rw-r--r--   0        0        0     1910 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1672 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     5832 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/sca_table_printer.py
+-rw-r--r--   0        0        0     2277 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/table.py
+-rw-r--r--   0        0        0      477 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/table_models.py
+-rw-r--r--   0        0        0     5416 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     9336 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4821 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6925 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1908 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6853 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     2195 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     7687 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2768 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      941 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1989 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2700 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      929 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2458 2023-07-05 09:56:16.671783 cycode-0.2.6.dev6/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      119 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3927 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      543 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1751 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     9102 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6301 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1090 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1179 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      197 2023-07-05 09:56:16.675783 cycode-0.2.6.dev6/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     2014 2023-07-05 09:56:52.716173 cycode-0.2.6.dev6/pyproject.toml
+-rw-r--r--   0        0        0    34042 1970-01-01 00:00:00.000000 cycode-0.2.6.dev6/PKG-INFO
```

### Comparing `cycode-0.2.6.dev5/README.md` & `cycode-0.2.6.dev6/README.md`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/auth/auth_command.py` & `cycode-0.2.6.dev6/cycode/cli/auth/auth_command.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,22 +44,22 @@
         return printer.print_result(failed_auth_check_res)
 
     try:
         if CycodeTokenBasedClient(client_id, client_secret).api_token:
             return printer.print_result(passed_auth_check_res)
     except (NetworkError, HttpUnauthorizedError):
         if context.obj['verbose']:
-            click.secho(f'Error: {traceback.format_exc()}', fg='red', nl=False)
+            click.secho(f'Error: {traceback.format_exc()}', fg='red')
 
         return printer.print_result(failed_auth_check_res)
 
 
 def _handle_exception(context: click.Context, e: Exception):
     if context.obj['verbose']:
-        click.secho(f'Error: {traceback.format_exc()}', fg='red', nl=False)
+        click.secho(f'Error: {traceback.format_exc()}', fg='red')
 
     errors: CliErrors = {
         AuthProcessError: CliError(
             code='auth_error',
             message='Authentication failed. Please try again later using the command `cycode auth`'
         ),
         NetworkError: CliError(
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/auth/auth_manager.py` & `cycode-0.2.6.dev6/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/ci_integrations.py` & `cycode-0.2.6.dev6/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/code_scanner.py` & `cycode-0.2.6.dev6/cycode/cli/code_scanner.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,67 +3,90 @@
 import logging
 import os
 import sys
 import time
 import traceback
 from platform import platform
 from uuid import uuid4, UUID
+from typing import TYPE_CHECKING, Callable, List, Optional, Dict, Tuple
+
 from git import Repo, NULL_TREE, InvalidGitRepositoryError
 from sys import getsizeof
 
-from halo import Halo
-
 from cycode.cli.printers import ConsolePrinter
-from cycode.cli.models import Document, DocumentDetections, Severity, CliError, CliErrors
+from cycode.cli.models import Document, DocumentDetections, Severity, CliError, CliErrors, LocalScanResult
 from cycode.cli.ci_integrations import get_commit_range
-from cycode.cli.consts import *
+from cycode.cli import consts
 from cycode.cli.config import configuration_manager
+from cycode.cli.utils.progress_bar import ProgressBarSection
+from cycode.cli.utils.scan_utils import set_issue_detected
 from cycode.cli.utils.path_utils import is_sub_path, is_binary_file, get_file_size, get_relevant_files_in_path, \
     get_path_by_os, get_file_content
+from cycode.cli.utils.scan_batch import run_parallel_batched_scan
 from cycode.cli.utils.string_utils import get_content_size, is_binary_content
 from cycode.cli.utils.task_timer import TimeoutAfter
 from cycode.cli.utils import scan_utils
 from cycode.cli.user_settings.config_file_manager import ConfigFileManager
 from cycode.cli.zip_file import InMemoryZip
-from cycode.cli.exceptions.custom_exceptions import *
+from cycode.cli.exceptions import custom_exceptions
 from cycode.cli.helpers import sca_code_scanner
 from cycode.cyclient import logger
-from cycode.cyclient.models import *
+from cycode.cli.utils.progress_bar import logger as progress_bar_logger
+from cycode.cyclient.models import ZippedFileScanResult, Detection, DetectionsPerFile, DetectionSchema
+
+if TYPE_CHECKING:
+    from cycode.cyclient.scan_client import ScanClient
+    from cycode.cyclient.models import ScanDetailsResponse
+    from cycode.cli.utils.progress_bar import BaseProgressBar
 
 start_scan_time = time.time()
 
 
 @click.command()
 @click.argument("path", nargs=1, type=click.STRING, required=True)
 @click.option('--branch', '-b',
               default=None,
               help='Branch to scan, if not set scanning the default branch',
               type=str,
               required=False)
 @click.pass_context
-def scan_repository(context: click.Context, path, branch):
+def scan_repository(context: click.Context, path: str, branch: str):
     """ Scan git repository including its history """
     try:
         logger.debug('Starting repository scan process, %s', {'path': path, 'branch': branch})
-        context.obj["path"] = path
-        monitor = context.obj.get("monitor")
-        scan_type = context.obj["scan_type"]
-        if monitor and scan_type != SCA_SCAN_TYPE:
-            raise click.ClickException(f"Monitor flag is currently supported for SCA scan type only")
-
-        documents_to_scan = [
-            Document(obj.path if monitor else get_path_by_os(os.path.join(path, obj.path)),
-                     obj.data_stream.read().decode('utf-8', errors='replace'))
-            for obj
-            in get_git_repository_tree_file_entries(path, branch)]
+
+        scan_type = context.obj['scan_type']
+        monitor = context.obj.get('monitor')
+        if monitor and scan_type != consts.SCA_SCAN_TYPE:
+            raise click.ClickException(f'Monitor flag is currently supported for SCA scan type only')
+
+        progress_bar = context.obj['progress_bar']
+
+        file_entries = list(get_git_repository_tree_file_entries(path, branch))
+        progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, len(file_entries))
+
+        documents_to_scan = []
+        for file in file_entries:
+            progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
+
+            if monitor:
+                path = file.path
+            else:
+                path = get_path_by_os(os.path.join(path, file.path))
+
+            documents_to_scan.append(Document(path, file.data_stream.read().decode('UTF-8', errors='replace')))
+
         documents_to_scan = exclude_irrelevant_documents_to_scan(context, documents_to_scan)
-        perform_pre_scan_documents_actions(context, scan_type, documents_to_scan, False)
+
+        perform_pre_scan_documents_actions(context, scan_type, documents_to_scan, is_git_diff=False)
+
         logger.debug('Found all relevant files for scanning %s', {'path': path, 'branch': branch})
-        return scan_documents(context, documents_to_scan, is_git_diff=False,
-                              scan_parameters=get_scan_parameters(context))
+        return scan_documents(
+            context, documents_to_scan, is_git_diff=False, scan_parameters=get_scan_parameters(context, path)
+        )
     except Exception as e:
         _handle_exception(context, e)
 
 
 @click.command()
 @click.argument("path",
                 nargs=1,
@@ -82,54 +105,70 @@
         logger.debug('Starting commit history scan process, %s', {'path': path, 'commit_range': commit_range})
         return scan_commit_range(context, path=path, commit_range=commit_range)
     except Exception as e:
         _handle_exception(context, e)
 
 
 def scan_commit_range(context: click.Context, path: str, commit_range: str, max_commits_count: Optional[int] = None):
-    scan_type = context.obj["scan_type"]
-    if scan_type not in COMMIT_RANGE_SCAN_SUPPORTED_SCAN_TYPES:
-        raise click.ClickException(f"Commit range scanning for {str.upper(scan_type)} is not supported")
+    scan_type = context.obj['scan_type']
+    progress_bar = context.obj['progress_bar']
 
-    if scan_type == SCA_SCAN_TYPE:
+    if scan_type not in consts.COMMIT_RANGE_SCAN_SUPPORTED_SCAN_TYPES:
+        raise click.ClickException(f'Commit range scanning for {str.upper(scan_type)} is not supported')
+
+    if scan_type == consts.SCA_SCAN_TYPE:
         return scan_sca_commit_range(context, path, commit_range)
 
     documents_to_scan = []
     commit_ids_to_scan = []
 
     repo = Repo(path)
-    total_commits_count = repo.git.rev_list('--count', commit_range)
+    total_commits_count = int(repo.git.rev_list('--count', commit_range))
+    logger.debug(f'Calculating diffs for {total_commits_count} commits in the commit range {commit_range}')
+
+    progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, total_commits_count)
+
     scanned_commits_count = 0
-    logger.info(f'Calculating diffs for {total_commits_count} commits in the commit range {commit_range}')
     for commit in repo.iter_commits(rev=commit_range):
         if _does_reach_to_max_commits_to_scan_limit(commit_ids_to_scan, max_commits_count):
-            logger.info(f'Reached to max commits to scan count. Going to scan only {max_commits_count} last commits')
+            logger.debug(f'Reached to max commits to scan count. Going to scan only {max_commits_count} last commits')
+            progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES, total_commits_count - scanned_commits_count)
             break
 
-        if _should_update_progress(scanned_commits_count):
-            logger.info(f'Calculated diffs for {scanned_commits_count} out of {total_commits_count} commits')
+        progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
 
         commit_id = commit.hexsha
         commit_ids_to_scan.append(commit_id)
         parent = commit.parents[0] if commit.parents else NULL_TREE
         diff = commit.diff(parent, create_patch=True, R=True)
         commit_documents_to_scan = []
         for blob in diff:
-            doc = Document(get_path_by_os(os.path.join(path, get_diff_file_path(blob))),
-                           blob.diff.decode('utf-8', errors='replace'), True, unique_id=commit_id)
-            commit_documents_to_scan.append(doc)
-
-        logger.debug('Found all relevant files in commit %s',
-                     {'path': path, 'commit_range': commit_range, 'commit_id': commit_id})
-        commit_documents_to_scan = exclude_irrelevant_documents_to_scan(context, commit_documents_to_scan)
-        documents_to_scan.extend(commit_documents_to_scan)
+            blob_path = get_path_by_os(os.path.join(path, get_diff_file_path(blob)))
+            commit_documents_to_scan.append(Document(
+                path=blob_path,
+                content=blob.diff.decode('UTF-8', errors='replace'),
+                is_git_diff_format=True,
+                unique_id=commit_id
+            ))
+
+        logger.debug(
+            'Found all relevant files in commit %s',
+            {
+                'path': path,
+                'commit_range': commit_range,
+                'commit_id': commit_id
+            }
+        )
+
+        documents_to_scan.extend(exclude_irrelevant_documents_to_scan(context, commit_documents_to_scan))
         scanned_commits_count += 1
 
     logger.debug('List of commit ids to scan, %s', {'commit_ids': commit_ids_to_scan})
-    logger.info('Starting to scan commit range (It may take a few minutes)')
+    logger.debug('Starting to scan commit range (It may take a few minutes)')
+
     return scan_documents(context, documents_to_scan, is_git_diff=True, is_commit_range=True)
 
 
 @click.command()
 @click.pass_context
 def scan_ci(context: click.Context):
     """ Execute scan in a CI environment which relies on the
@@ -139,346 +178,509 @@
 
 @click.command()
 @click.argument("path", nargs=1, type=click.STRING, required=True)
 @click.pass_context
 def scan_path(context: click.Context, path):
     """	Scan the files in the path supplied in the command """
     logger.debug('Starting path scan process, %s', {'path': path})
-    context.obj["path"] = path
     files_to_scan = get_relevant_files_in_path(path=path, exclude_patterns=["**/.git/**", "**/.cycode/**"])
     files_to_scan = exclude_irrelevant_files(context, files_to_scan)
     logger.debug('Found all relevant files for scanning %s', {'path': path, 'file_to_scan_count': len(files_to_scan)})
-    return scan_disk_files(context, files_to_scan)
+    return scan_disk_files(context, path, files_to_scan)
 
 
 @click.command()
-@click.argument("ignored_args", nargs=-1, type=click.UNPROCESSED)
+@click.argument('ignored_args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
 def pre_commit_scan(context: click.Context, ignored_args: List[str]):
     """ Use this command to scan the content that was not committed yet """
     scan_type = context.obj['scan_type']
-    if scan_type == SCA_SCAN_TYPE:
+    progress_bar = context.obj['progress_bar']
+
+    if scan_type == consts.SCA_SCAN_TYPE:
         return scan_sca_pre_commit(context)
 
-    diff_files = Repo(os.getcwd()).index.diff("HEAD", create_patch=True, R=True)
-    documents_to_scan = [Document(get_path_by_os(get_diff_file_path(file)), get_diff_file_content(file))
-                         for file in diff_files]
+    diff_files = Repo(os.getcwd()).index.diff('HEAD', create_patch=True, R=True)
+
+    progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, len(diff_files))
+
+    documents_to_scan = []
+    for file in diff_files:
+        progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
+        documents_to_scan.append(Document(get_path_by_os(get_diff_file_path(file)), get_diff_file_content(file)))
+
     documents_to_scan = exclude_irrelevant_documents_to_scan(context, documents_to_scan)
     return scan_documents(context, documents_to_scan, is_git_diff=True)
 
 
 @click.command()
 @click.argument("ignored_args", nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
 def pre_receive_scan(context: click.Context, ignored_args: List[str]):
-    """ Use this command to scan commits on server side before pushing them to the repository """
+    """ Use this command to scan commits on the server side before pushing them to the repository """
     try:
         scan_type = context.obj['scan_type']
-        if scan_type != SECRET_SCAN_TYPE:
-            raise click.ClickException(f"Commit range scanning for {str.upper(scan_type)} is not supported")
+        if scan_type != consts.SECRET_SCAN_TYPE:
+            raise click.ClickException(f'Commit range scanning for {scan_type.upper()} is not supported')
 
         if should_skip_pre_receive_scan():
             logger.info(
                 "A scan has been skipped as per your request."
                 " Please note that this may leave your system vulnerable to secrets that have not been detected")
             return
 
         if is_verbose_mode_requested_in_pre_receive_scan():
             enable_verbose_mode(context)
             logger.debug('Verbose mode enabled, all log levels will be displayed')
 
         command_scan_type = context.info_name
         timeout = configuration_manager.get_pre_receive_command_timeout(command_scan_type)
         with TimeoutAfter(timeout):
-            if scan_type not in COMMIT_RANGE_SCAN_SUPPORTED_SCAN_TYPES:
-                raise click.ClickException(f"Commit range scanning for {str.upper(scan_type)} is not supported")
+            if scan_type not in consts.COMMIT_RANGE_SCAN_SUPPORTED_SCAN_TYPES:
+                raise click.ClickException(f'Commit range scanning for {scan_type.upper()} is not supported')
 
             branch_update_details = parse_pre_receive_input()
             commit_range = calculate_pre_receive_commit_range(branch_update_details)
             if not commit_range:
-                logger.info('No new commits found for pushed branch, %s',
-                            {'branch_update_details': branch_update_details})
+                logger.info(
+                    'No new commits found for pushed branch, %s',
+                    {'branch_update_details': branch_update_details}
+                )
                 return
 
             max_commits_to_scan = configuration_manager.get_pre_receive_max_commits_to_scan_count(command_scan_type)
             scan_commit_range(context, os.getcwd(), commit_range, max_commits_count=max_commits_to_scan)
             perform_post_pre_receive_scan_actions(context)
     except Exception as e:
         _handle_exception(context, e)
 
 
 def scan_sca_pre_commit(context: click.Context):
     scan_parameters = get_default_scan_parameters(context)
-    git_head_documents, pre_committed_documents = get_pre_commit_modified_documents()
+    git_head_documents, pre_committed_documents = get_pre_commit_modified_documents(context.obj['progress_bar'])
     git_head_documents = exclude_irrelevant_documents_to_scan(context, git_head_documents)
     pre_committed_documents = exclude_irrelevant_documents_to_scan(context, pre_committed_documents)
     sca_code_scanner.perform_pre_hook_range_scan_actions(git_head_documents, pre_committed_documents)
     return scan_commit_range_documents(context, git_head_documents, pre_committed_documents,
                                        scan_parameters,
                                        configuration_manager.get_sca_pre_commit_timeout_in_seconds())
 
 
 def scan_sca_commit_range(context: click.Context, path: str, commit_range: str):
-    context.obj["path"] = path
-    scan_parameters = get_scan_parameters(context)
+    progress_bar = context.obj['progress_bar']
+
+    scan_parameters = get_scan_parameters(context, path)
     from_commit_rev, to_commit_rev = parse_commit_range(commit_range, path)
-    from_commit_documents, to_commit_documents = \
-        get_commit_range_modified_documents(path, from_commit_rev, to_commit_rev)
+    from_commit_documents, to_commit_documents = get_commit_range_modified_documents(
+        progress_bar, path, from_commit_rev, to_commit_rev
+    )
     from_commit_documents = exclude_irrelevant_documents_to_scan(context, from_commit_documents)
     to_commit_documents = exclude_irrelevant_documents_to_scan(context, to_commit_documents)
     sca_code_scanner.perform_pre_commit_range_scan_actions(path, from_commit_documents, from_commit_rev,
                                                            to_commit_documents, to_commit_rev)
 
     return scan_commit_range_documents(context, from_commit_documents, to_commit_documents,
                                        scan_parameters=scan_parameters)
 
 
-def scan_disk_files(context: click.Context, paths: List[str]):
-    scan_parameters = get_scan_parameters(context)
+def scan_disk_files(context: click.Context, path: str, files_to_scan: List[str]):
+    scan_parameters = get_scan_parameters(context, path)
     scan_type = context.obj['scan_type']
+    progress_bar = context.obj['progress_bar']
+
     is_git_diff = False
+
+    progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, len(files_to_scan))
+
     documents: List[Document] = []
-    for path in paths:
-        with open(path, "r", encoding="utf-8") as f:
-            content = f.read()
-            documents.append(Document(path, content, is_git_diff))
+    for file in files_to_scan:
+        progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
+
+        with open(file, 'r', encoding='UTF-8') as f:
+            try:
+                documents.append(Document(file, f.read(), is_git_diff))
+            except UnicodeDecodeError:
+                continue
 
     perform_pre_scan_documents_actions(context, scan_type, documents, is_git_diff)
     return scan_documents(context, documents, is_git_diff=is_git_diff, scan_parameters=scan_parameters)
 
 
-def scan_documents(context: click.Context, documents_to_scan: List[Document], is_git_diff: bool = False,
-                   is_commit_range: bool = False, scan_parameters: dict = None):
-    cycode_client = context.obj["client"]
-    scan_type = context.obj["scan_type"]
-    severity_threshold = context.obj["severity_threshold"]
+def set_issue_detected_by_scan_results(context: click.Context, scan_results: List[LocalScanResult]) -> None:
+    set_issue_detected(context, any(scan_result.issue_detected for scan_result in scan_results))
+
+
+def _get_scan_documents_thread_func(
+        context: click.Context, is_git_diff: bool, is_commit_range: bool, scan_parameters: dict
+) -> Callable[[List[Document]], Tuple[str, CliError, LocalScanResult]]:
+    cycode_client = context.obj['client']
+    scan_type = context.obj['scan_type']
+    severity_threshold = context.obj['severity_threshold']
     command_scan_type = context.info_name
-    error_message = None
-    all_detections_count = 0
-    output_detections_count = 0
-    scan_id = _get_scan_id(context)
-    zipped_documents = InMemoryZip()
 
-    try:
-        logger.debug("Preparing local files")
-        zipped_documents = zip_documents_to_scan(scan_type, zipped_documents, documents_to_scan)
+    def _scan_batch_thread_func(batch: List[Document]) -> Tuple[str, CliError, LocalScanResult]:
+        local_scan_result = error = error_message = None
+        detections_count = relevant_detections_count = zip_file_size = 0
 
-        scan_result = perform_scan(context, cycode_client, zipped_documents, scan_type, scan_id, is_git_diff,
-                                   is_commit_range,
-                                   scan_parameters)
-
-        all_detections_count, output_detections_count = \
-            handle_scan_result(context, scan_result, command_scan_type, scan_type, severity_threshold,
-                               documents_to_scan)
-        scan_completed = True
-    except Exception as e:
-        _handle_exception(context, e)
-        error_message = str(e)
+        scan_id = str(_get_scan_id())
         scan_completed = False
 
-    zip_file_size = getsizeof(zipped_documents.in_memory_zip)
-    logger.debug('Finished scan process, %s',
-                 {'all_violations_count': all_detections_count, 'relevant_violations_count': output_detections_count,
-                  'scan_id': str(scan_id), 'zip_file_size': zip_file_size})
-    _report_scan_status(context, scan_type, str(scan_id), scan_completed, output_detections_count,
-                        all_detections_count, len(documents_to_scan), zip_file_size, command_scan_type, error_message)
+        try:
+            logger.debug('Preparing local files, %s', {'batch_size': len(batch)})
+            zipped_documents = zip_documents_to_scan(scan_type, InMemoryZip(), batch)
+            zip_file_size = getsizeof(zipped_documents.in_memory_zip)
+
+            scan_result = perform_scan(
+                cycode_client, zipped_documents, scan_type, scan_id, is_git_diff, is_commit_range, scan_parameters
+            )
+
+            local_scan_result = create_local_scan_result(
+                scan_result, batch, command_scan_type, scan_type, severity_threshold
+            )
+
+            scan_completed = True
+        except Exception as e:
+            error = _handle_exception(context, e, return_exception=True)
+            error_message = str(e)
+
+        if local_scan_result:
+            detections_count = local_scan_result.detections_count
+            relevant_detections_count = local_scan_result.relevant_detections_count
+            scan_id = local_scan_result.scan_id
+
+        logger.debug(
+            'Finished scan process, %s',
+            {
+                'all_violations_count': detections_count,
+                'relevant_violations_count': relevant_detections_count,
+                'scan_id': scan_id,
+                'zip_file_size': zip_file_size
+            }
+        )
+        _report_scan_status(
+            cycode_client, scan_type, scan_id, scan_completed, relevant_detections_count,
+            detections_count, len(batch), zip_file_size, command_scan_type, error_message
+        )
+
+        return scan_id, error, local_scan_result
+
+    return _scan_batch_thread_func
+
+
+def scan_documents(
+        context: click.Context,
+        documents_to_scan: List[Document],
+        is_git_diff: bool = False,
+        is_commit_range: bool = False,
+        scan_parameters: Optional[dict] = None,
+) -> None:
+    progress_bar = context.obj['progress_bar']
+
+    scan_batch_thread_func = _get_scan_documents_thread_func(context, is_git_diff, is_commit_range, scan_parameters)
+    errors, local_scan_results = run_parallel_batched_scan(
+        scan_batch_thread_func, documents_to_scan, progress_bar=progress_bar
+    )
+
+    progress_bar.set_section_length(ProgressBarSection.GENERATE_REPORT, 1)
+    progress_bar.update(ProgressBarSection.GENERATE_REPORT)
+    progress_bar.stop()
 
+    set_issue_detected_by_scan_results(context, local_scan_results)
+    print_results(context, local_scan_results)
+
+    if not errors:
+        return
+
+    if context.obj['output'] == 'json':
+        # TODO(MarshalX): we can't just print JSON formatted errors here
+        #  because we should return only one root json structure per scan
+        #  could be added later to "print_results" function if we wish to display detailed errors in UI
+        return
 
-def scan_commit_range_documents(context: click.Context, from_documents_to_scan: List[Document],
-                                to_documents_to_scan: List[Document], scan_parameters: dict = None,
-                                timeout: int = None):
-    cycode_client = context.obj["client"]
-    scan_type = context.obj["scan_type"]
-    severity_threshold = context.obj["severity_threshold"]
+    click.secho(
+        'Unfortunately, Cycode was unable to complete the full scan. '
+        'Please note that not all results may be available:',
+        fg='red'
+    )
+    for scan_id, error in errors.items():
+        click.echo(f'- {scan_id}: ', nl=False)
+        ConsolePrinter(context).print_error(error)
+
+
+def scan_commit_range_documents(
+        context: click.Context,
+        from_documents_to_scan: List[Document],
+        to_documents_to_scan: List[Document],
+        scan_parameters: Optional[dict] = None,
+        timeout: Optional[int] = None
+) -> None:
+    cycode_client = context.obj['client']
+    scan_type = context.obj['scan_type']
+    severity_threshold = context.obj['severity_threshold']
     scan_command_type = context.info_name
-    error_message = None
-    all_detections_count = 0
-    output_detections_count = 0
-    scan_id = _get_scan_id(context)
+    progress_bar = context.obj['progress_bar']
+
+    local_scan_result = error_message = None
+    scan_completed = False
+    scan_id = str(_get_scan_id())
+
     from_commit_zipped_documents = InMemoryZip()
     to_commit_zipped_documents = InMemoryZip()
 
     try:
-        scan_result = init_default_scan_result(str(scan_id))
+        progress_bar.set_section_length(ProgressBarSection.SCAN, 1)
+
+        scan_result = init_default_scan_result(scan_id)
         if should_scan_documents(from_documents_to_scan, to_documents_to_scan):
-            logger.debug("Preparing from-commit zip")
-            from_commit_zipped_documents = zip_documents_to_scan(scan_type, from_commit_zipped_documents,
-                                                                 from_documents_to_scan)
-            logger.debug("Preparing to-commit zip")
-            to_commit_zipped_documents = zip_documents_to_scan(scan_type, to_commit_zipped_documents,
-                                                               to_documents_to_scan)
-            scan_result = perform_commit_range_scan_async(context, cycode_client, from_commit_zipped_documents,
-                                                          to_commit_zipped_documents, scan_type, scan_parameters,
-                                                          timeout)
-        all_detections_count, output_detections_count = \
-            handle_scan_result(context, scan_result, scan_command_type, scan_type, severity_threshold,
-                               to_documents_to_scan)
+            logger.debug('Preparing from-commit zip')
+            from_commit_zipped_documents = zip_documents_to_scan(
+                scan_type, from_commit_zipped_documents, from_documents_to_scan
+            )
+
+            logger.debug('Preparing to-commit zip')
+            to_commit_zipped_documents = zip_documents_to_scan(
+                scan_type, to_commit_zipped_documents, to_documents_to_scan
+            )
+
+            scan_result = perform_commit_range_scan_async(
+                cycode_client, from_commit_zipped_documents, to_commit_zipped_documents,
+                scan_type, scan_parameters, timeout
+            )
+
+        progress_bar.update(ProgressBarSection.SCAN)
+        progress_bar.set_section_length(ProgressBarSection.GENERATE_REPORT, 1)
+
+        local_scan_result = create_local_scan_result(
+            scan_result, to_documents_to_scan, scan_command_type, scan_type, severity_threshold
+        )
+        set_issue_detected_by_scan_results(context, [local_scan_result])
+
+        progress_bar.update(ProgressBarSection.GENERATE_REPORT)
+        progress_bar.stop()
+
+        print_results(context, [local_scan_result])
+
         scan_completed = True
     except Exception as e:
         _handle_exception(context, e)
         error_message = str(e)
-        scan_completed = False
 
-    zip_file_size = getsizeof(from_commit_zipped_documents.in_memory_zip) + getsizeof(
-        to_commit_zipped_documents.in_memory_zip)
-    logger.debug('Finished scan process, %s',
-                 {'all_violations_count': all_detections_count, 'relevant_violations_count': output_detections_count,
-                  'scan_id': str(scan_id), 'zip_file_size': zip_file_size})
-    _report_scan_status(context, scan_type, str(scan_id), scan_completed, output_detections_count,
-                        all_detections_count, len(to_documents_to_scan), zip_file_size, scan_command_type,
-                        error_message)
+    zip_file_size = getsizeof(from_commit_zipped_documents.in_memory_zip) + \
+        getsizeof(to_commit_zipped_documents.in_memory_zip)
+
+    detections_count = relevant_detections_count = 0
+    if local_scan_result:
+        detections_count = local_scan_result.detections_count
+        relevant_detections_count = local_scan_result.relevant_detections_count
+        scan_id = local_scan_result.scan_id
+
+    logger.debug(
+        'Finished scan process, %s',
+        {
+            'all_violations_count': detections_count,
+            'relevant_violations_count': relevant_detections_count,
+            'scan_id': scan_id,
+            'zip_file_size': zip_file_size
+        }
+    )
+    _report_scan_status(
+        cycode_client, scan_type, local_scan_result.scan_id, scan_completed,
+        local_scan_result.relevant_detections_count, local_scan_result.detections_count, len(to_documents_to_scan),
+        zip_file_size, scan_command_type, error_message
+    )
 
 
 def should_scan_documents(from_documents_to_scan: List[Document], to_documents_to_scan: List[Document]) -> bool:
     return len(from_documents_to_scan) > 0 or len(to_documents_to_scan) > 0
 
 
-def handle_scan_result(context, scan_result, command_scan_type, scan_type, severity_threshold, to_documents_to_scan):
-    document_detections_list = enrich_scan_result(scan_result, to_documents_to_scan)
-    relevant_document_detections_list = exclude_irrelevant_scan_results(document_detections_list, scan_type,
-                                                                        command_scan_type, severity_threshold)
-    context.obj['report_url'] = scan_result.report_url
-    print_results(context, relevant_document_detections_list)
-    context.obj['issue_detected'] = len(relevant_document_detections_list) > 0
-    all_detections_count = sum(
-        [len(document_detections.detections) for document_detections in document_detections_list])
-    output_detections_count = sum(
-        [len(document_detections.detections) for document_detections in relevant_document_detections_list])
-    return all_detections_count, output_detections_count
-
-
-def perform_pre_scan_documents_actions(context: click.Context, scan_type: str, documents_to_scan: List[Document],
-                                       is_git_diff: bool = False):
-    if scan_type == SCA_SCAN_TYPE:
-        logger.debug(
-            f"Perform pre scan document actions")
+def create_local_scan_result(
+        scan_result: ZippedFileScanResult,
+        documents_to_scan: List[Document],
+        command_scan_type: str,
+        scan_type: str,
+        severity_threshold: str,
+) -> LocalScanResult:
+    document_detections = get_document_detections(scan_result, documents_to_scan)
+    relevant_document_detections_list = exclude_irrelevant_document_detections(
+        document_detections, scan_type, command_scan_type, severity_threshold
+    )
+
+    detections_count = sum([len(document_detection.detections) for document_detection in document_detections])
+    relevant_detections_count = sum(
+        [len(document_detections.detections) for document_detections in relevant_document_detections_list]
+    )
+
+    return LocalScanResult(
+        scan_id=scan_result.scan_id,
+        report_url=scan_result.report_url,
+        document_detections=relevant_document_detections_list,
+        issue_detected=len(relevant_document_detections_list) > 0,
+        detections_count=detections_count,
+        relevant_detections_count=relevant_detections_count
+    )
+
+
+def perform_pre_scan_documents_actions(
+        context: click.Context, scan_type: str, documents_to_scan: List[Document], is_git_diff: bool = False
+) -> None:
+    if scan_type == consts.SCA_SCAN_TYPE:
+        logger.debug(f'Perform pre scan document actions')
         sca_code_scanner.add_dependencies_tree_document(context, documents_to_scan, is_git_diff)
 
 
-def zip_documents_to_scan(scan_type: str, zip: InMemoryZip, documents: List[Document]):
+def zip_documents_to_scan(scan_type: str, zip_file: InMemoryZip, documents: List[Document]) -> InMemoryZip:
     start_zip_creation_time = time.time()
 
     for index, document in enumerate(documents):
-        zip_file_size = getsizeof(zip.in_memory_zip)
+        zip_file_size = getsizeof(zip_file.in_memory_zip)
         validate_zip_file_size(scan_type, zip_file_size)
 
         logger.debug('adding file to zip, %s',
                      {'index': index, 'filename': document.path, 'unique_id': document.unique_id})
-        zip.append(document.path, document.unique_id, document.content)
-    zip.close()
+        zip_file.append(document.path, document.unique_id, document.content)
+    zip_file.close()
 
     end_zip_creation_time = time.time()
     zip_creation_time = int(end_zip_creation_time - start_zip_creation_time)
     logger.debug('finished to create zip file, %s', {'zip_creation_time': zip_creation_time})
-    return zip
+    return zip_file
 
 
-def validate_zip_file_size(scan_type, zip_file_size):
-    if scan_type == SCA_SCAN_TYPE:
-        if zip_file_size > SCA_ZIP_MAX_SIZE_LIMIT_IN_BYTES:
-            raise ZipTooLargeError(SCA_ZIP_MAX_SIZE_LIMIT_IN_BYTES)
+def validate_zip_file_size(scan_type: str, zip_file_size: int) -> None:
+    if scan_type == consts.SCA_SCAN_TYPE:
+        if zip_file_size > consts.SCA_ZIP_MAX_SIZE_LIMIT_IN_BYTES:
+            raise custom_exceptions.ZipTooLargeError(consts.SCA_ZIP_MAX_SIZE_LIMIT_IN_BYTES)
     else:
-        if zip_file_size > ZIP_MAX_SIZE_LIMIT_IN_BYTES:
-            raise ZipTooLargeError(ZIP_MAX_SIZE_LIMIT_IN_BYTES)
-
-
-def perform_scan(context, cycode_client, zipped_documents: InMemoryZip, scan_type: str, scan_id: UUID,
-                 is_git_diff: bool,
-                 is_commit_range: bool, scan_parameters: dict):
-    if scan_type == SCA_SCAN_TYPE or scan_type == SAST_SCAN_TYPE:
-        return perform_scan_async(context, cycode_client, zipped_documents, scan_type, scan_parameters)
-
-    scan_result = cycode_client.commit_range_zipped_file_scan(scan_type, zipped_documents, scan_id) \
-        if is_commit_range else cycode_client.zipped_file_scan(scan_type, zipped_documents, scan_id,
-                                                               scan_parameters, is_git_diff)
-
-    return scan_result
+        if zip_file_size > consts.ZIP_MAX_SIZE_LIMIT_IN_BYTES:
+            raise custom_exceptions.ZipTooLargeError(consts.ZIP_MAX_SIZE_LIMIT_IN_BYTES)
 
 
-def perform_scan_async(context: click.Context, cycode_client, zipped_documents: InMemoryZip, scan_type: str,
-                       scan_parameters: dict) -> ZippedFileScanResult:
+def perform_scan(
+        cycode_client: 'ScanClient',
+        zipped_documents: InMemoryZip,
+        scan_type: str,
+        scan_id: str,
+        is_git_diff: bool,
+        is_commit_range: bool,
+        scan_parameters: dict
+) -> ZippedFileScanResult:
+    if scan_type in (consts.SCA_SCAN_TYPE, consts.SAST_SCAN_TYPE):
+        return perform_scan_async(cycode_client, zipped_documents, scan_type, scan_parameters)
+
+    if is_commit_range:
+        return cycode_client.commit_range_zipped_file_scan(scan_type, zipped_documents, scan_id)
+
+    return cycode_client.zipped_file_scan(scan_type, zipped_documents, scan_id, scan_parameters, is_git_diff)
+
+
+def perform_scan_async(
+        cycode_client: 'ScanClient',
+        zipped_documents: InMemoryZip,
+        scan_type: str,
+        scan_parameters: dict
+) -> ZippedFileScanResult:
     scan_async_result = cycode_client.zipped_file_scan_async(zipped_documents, scan_type, scan_parameters)
     logger.debug("scan request has been triggered successfully, scan id: %s", scan_async_result.scan_id)
 
-    return poll_scan_results(context, cycode_client, scan_async_result.scan_id)
+    return poll_scan_results(cycode_client, scan_async_result.scan_id)
 
 
-def perform_commit_range_scan_async(context: click.Context, cycode_client, from_commit_zipped_documents: InMemoryZip,
-                                    to_commit_zipped_documents: InMemoryZip, scan_type: str,
-                                    scan_parameters: dict, timeout: int = None) -> ZippedFileScanResult:
-    scan_async_result = \
-        cycode_client.multiple_zipped_file_scan_async(from_commit_zipped_documents, to_commit_zipped_documents,
-                                                      scan_type, scan_parameters)
+def perform_commit_range_scan_async(
+        cycode_client: 'ScanClient',
+        from_commit_zipped_documents: InMemoryZip,
+        to_commit_zipped_documents: InMemoryZip,
+        scan_type: str,
+        scan_parameters: dict,
+        timeout: int = None
+) -> ZippedFileScanResult:
+    scan_async_result = cycode_client.multiple_zipped_file_scan_async(
+        from_commit_zipped_documents, to_commit_zipped_documents, scan_type, scan_parameters
+    )
+
     logger.debug("scan request has been triggered successfully, scan id: %s", scan_async_result.scan_id)
-    return poll_scan_results(context, cycode_client, scan_async_result.scan_id, timeout)
+    return poll_scan_results(cycode_client, scan_async_result.scan_id, timeout)
 
 
-def poll_scan_results(context: click.Context, cycode_client, scan_id: str, polling_timeout: int = None):
+def poll_scan_results(
+        cycode_client: 'ScanClient', scan_id: str, polling_timeout: Optional[int] = None
+) -> ZippedFileScanResult:
     if polling_timeout is None:
         polling_timeout = configuration_manager.get_scan_polling_timeout_in_seconds()
 
     last_scan_update_at = None
     end_polling_time = time.time() + polling_timeout
-    spinner = Halo(spinner='dots')
-    spinner.start("Scan in progress")
+
     while time.time() < end_polling_time:
         scan_details = cycode_client.get_scan_details(scan_id)
+
         if scan_details.scan_update_at is not None and scan_details.scan_update_at != last_scan_update_at:
-            click.echo()
             last_scan_update_at = scan_details.scan_update_at
-            print_scan_details(scan_details)
-        if scan_details.scan_status == SCAN_STATUS_COMPLETED:
-            spinner.succeed()
+            print_debug_scan_details(scan_details)
+
+        if scan_details.scan_status == consts.SCAN_STATUS_COMPLETED:
             return _get_scan_result(cycode_client, scan_id, scan_details)
-        if scan_details.scan_status == SCAN_STATUS_ERROR:
-            spinner.fail()
-            raise ScanAsyncError(f'error occurred while trying to scan zip file. {scan_details.message}')
-        time.sleep(SCAN_POLLING_WAIT_INTERVAL_IN_SECONDS)
+        elif scan_details.scan_status == consts.SCAN_STATUS_ERROR:
+            raise custom_exceptions.ScanAsyncError(
+                f'Error occurred while trying to scan zip file. {scan_details.message}'
+            )
 
-    spinner.stop_and_persist(symbol="⏰".encode('utf-8'), text='Timeout')
-    raise ScanAsyncError(f'Failed to complete scan after {polling_timeout} seconds')
+        time.sleep(consts.SCAN_POLLING_WAIT_INTERVAL_IN_SECONDS)
 
+    raise custom_exceptions.ScanAsyncError(f'Failed to complete scan after {polling_timeout} seconds')
 
-def print_scan_details(scan_details_response: ScanDetailsResponse):
-    logger.info(f"Scan update: (scan_id: {scan_details_response.id})")
-    logger.info(f"Scan status: {scan_details_response.scan_status}")
-    if scan_details_response.message is not None:
-        logger.info(f"Scan message: {scan_details_response.message}")
 
+def print_debug_scan_details(scan_details_response: 'ScanDetailsResponse') -> None:
+    logger.debug(f'Scan update: (scan_id: {scan_details_response.id})')
+    logger.debug(f'Scan status: {scan_details_response.scan_status}')
 
-def print_results(context: click.Context, document_detections_list: List[DocumentDetections]) -> None:
+    if scan_details_response.message:
+        logger.debug(f'Scan message: {scan_details_response.message}')
+
+
+def print_results(context: click.Context, local_scan_results: List[LocalScanResult]) -> None:
     printer = ConsolePrinter(context)
-    printer.print_scan_results(document_detections_list)
+    printer.print_scan_results(local_scan_results)
 
 
-def enrich_scan_result(
+def get_document_detections(
         scan_result: ZippedFileScanResult, documents_to_scan: List[Document]
 ) -> List[DocumentDetections]:
-    logger.debug('enriching scan result')
-    document_detections_list = []
+    logger.debug('Get document detections')
+
+    document_detections = []
     for detections_per_file in scan_result.detections_per_file:
         file_name = get_path_by_os(detections_per_file.file_name)
         commit_id = detections_per_file.commit_id
-        logger.debug("going to find document of violated file, %s", {'file_name': file_name, 'commit_id': commit_id})
-        document = _get_document_by_file_name(documents_to_scan, file_name, commit_id)
-        document_detections_list.append(
-            DocumentDetections(document=document, detections=detections_per_file.detections))
 
-    return document_detections_list
+        logger.debug('Going to find document of violated file, %s', {'file_name': file_name, 'commit_id': commit_id})
+
+        document = _get_document_by_file_name(documents_to_scan, file_name, commit_id)
+        document_detections.append(
+            DocumentDetections(document=document, detections=detections_per_file.detections)
+        )
+
+    return document_detections
 
 
-def exclude_irrelevant_scan_results(document_detections_list: List[DocumentDetections], scan_type: str,
-                                    command_scan_type: str, severity_threshold: str) -> List[DocumentDetections]:
+def exclude_irrelevant_document_detections(
+        document_detections_list: List[DocumentDetections],
+        scan_type: str,
+        command_scan_type: str,
+        severity_threshold: str
+) -> List[DocumentDetections]:
     relevant_document_detections_list = []
     for document_detections in document_detections_list:
-        relevant_detections = exclude_irrelevant_detections(scan_type, command_scan_type, severity_threshold,
-                                                            document_detections.detections)
+        relevant_detections = exclude_irrelevant_detections(
+            document_detections.detections, scan_type, command_scan_type, severity_threshold
+        )
         if relevant_detections:
-            relevant_document_detections_list.append(DocumentDetections(document=document_detections.document,
-                                                                        detections=relevant_detections))
+            relevant_document_detections_list.append(
+                DocumentDetections(document=document_detections.document, detections=relevant_detections)
+            )
 
     return relevant_document_detections_list
 
 
 def parse_pre_receive_input() -> str:
     """
     Parsing input to pushed branch update details
@@ -488,30 +690,31 @@
     -----------------------------------------------
     0000000000000000000000000000000000000000 9cf90954ef26e7c58284f8ebf7dcd0fcf711152a refs/heads/main
     973a96d3e925b65941f7c47fa16129f1577d499f 0000000000000000000000000000000000000000 refs/heads/feature-branch
     59564ef68745bca38c42fc57a7822efd519a6bd9 3378e52dcfa47fb11ce3a4a520bea5f85d5d0bf3 refs/heads/develop
 
     :return: first branch update details (input's first line)
     """
+    # FIXME(MarshalX): this blocks main thread forever if called outside of pre-receive hook
     pre_receive_input = sys.stdin.read().strip()
     if not pre_receive_input:
         raise ValueError(
             "Pre receive input was not found. Make sure that you are using this command only in pre-receive hook")
 
     # each line represents a branch update request, handle the first one only
-    # TODO support case of multiple update branch requests
+    # TODO(MichalBor): support case of multiple update branch requests
     branch_update_details = pre_receive_input.splitlines()[0]
     return branch_update_details
 
 
 def calculate_pre_receive_commit_range(branch_update_details: str) -> Optional[str]:
     end_commit = get_end_commit_from_branch_update_details(branch_update_details)
 
     # branch is deleted, no need to perform scan
-    if end_commit == EMPTY_COMMIT_SHA:
+    if end_commit == consts.EMPTY_COMMIT_SHA:
         return
 
     start_commit = get_oldest_unupdated_commit_for_branch(end_commit)
 
     # no new commit to update found
     if not start_commit:
         return
@@ -539,15 +742,15 @@
     return file.b_path if file.b_path else file.a_path
 
 
 def get_diff_file_content(file):
     return file.diff.decode('utf-8', errors='replace')
 
 
-def should_process_git_object(obj, depth):
+def should_process_git_object(obj, _: int) -> bool:
     return obj.type == 'blob' and obj.size > 0
 
 
 def get_git_repository_tree_file_entries(path: str, branch: str):
     return Repo(path).tree(branch).traverse(predicate=should_process_git_object)
 
 
@@ -556,20 +759,20 @@
         "monitor": context.obj.get("monitor"),
         "report": context.obj.get("report"),
         "package_vulnerabilities": context.obj.get("package-vulnerabilities"),
         "license_compliance": context.obj.get("license-compliance")
     }
 
 
-def get_scan_parameters(context: click.Context) -> dict:
-    path = context.obj["path"]
+def get_scan_parameters(context: click.Context, path: str) -> dict:
     scan_parameters = get_default_scan_parameters(context)
     remote_url = try_get_git_remote_url(path)
     if remote_url:
-        context.obj["remote_url"] = remote_url
+        # TODO(MarshalX): remove hardcode
+        context.obj['remote_url'] = remote_url
         scan_parameters.update(remote_url)
     return scan_parameters
 
 
 def try_get_git_remote_url(path: str) -> Optional[dict]:
     try:
         git_remote_url = Repo(path).remotes[0].config_reader.get('url')
@@ -577,128 +780,164 @@
             'remote_url': git_remote_url,
         }
     except Exception as e:
         logger.debug('Failed to get git remote URL. %s', {'exception_message': str(e)})
         return None
 
 
-def exclude_irrelevant_documents_to_scan(context: click.Context, documents_to_scan: List[Document]) -> \
-        List[Document]:
+def exclude_irrelevant_documents_to_scan(
+        context: click.Context, documents_to_scan: List[Document]
+) -> List[Document]:
+    logger.debug('Excluding irrelevant documents to scan')
+
     scan_type = context.obj['scan_type']
-    logger.debug("excluding irrelevant documents to scan")
-    return [document for document in documents_to_scan if
-            _is_relevant_document_to_scan(scan_type, document.path, document.content)]
+
+    relevant_documents = []
+    for document in documents_to_scan:
+        if _is_relevant_document_to_scan(scan_type, document.path, document.content):
+            relevant_documents.append(document)
+
+    return relevant_documents
 
 
 def exclude_irrelevant_files(context: click.Context, filenames: List[str]) -> List[str]:
     scan_type = context.obj['scan_type']
-    return [filename for filename in filenames if _is_relevant_file_to_scan(scan_type, filename)]
+
+    relevant_files = []
+    for filename in filenames:
+        if _is_relevant_file_to_scan(scan_type, filename):
+            relevant_files.append(filename)
+
+    return relevant_files
 
 
-def exclude_irrelevant_detections(scan_type: str, command_scan_type: str, severity_threshold: str, detections) -> List:
-    relevant_detections = exclude_detections_by_exclusions_configuration(scan_type, detections)
-    relevant_detections = exclude_detections_by_scan_type(scan_type, command_scan_type, relevant_detections)
-    relevant_detections = exclude_detections_by_severity(scan_type, severity_threshold, relevant_detections)
+def exclude_irrelevant_detections(
+        detections: List[Detection], scan_type: str, command_scan_type: str, severity_threshold: str
+) -> List[Detection]:
+    relevant_detections = _exclude_detections_by_exclusions_configuration(detections, scan_type)
+    relevant_detections = _exclude_detections_by_scan_type(relevant_detections, scan_type, command_scan_type)
+    relevant_detections = _exclude_detections_by_severity(relevant_detections, scan_type, severity_threshold)
 
     return relevant_detections
 
 
-def exclude_detections_by_severity(scan_type: str, severity_threshold: str, detections) -> List:
-    if scan_type != SCA_SCAN_TYPE or severity_threshold is None:
+def _exclude_detections_by_severity(
+        detections: List[Detection], scan_type: str, severity_threshold: str
+) -> List[Detection]:
+    if scan_type != consts.SCA_SCAN_TYPE or severity_threshold is None:
         return detections
 
-    return [detection for detection in detections if
-            _does_severity_match_severity_threshold(detection.detection_details.get('advisory_severity'),
-                                                    severity_threshold)]
+    relevant_detections = []
+    for detection in detections:
+        severity = detection.detection_details.get('advisory_severity')
+        if _does_severity_match_severity_threshold(severity, severity_threshold):
+            relevant_detections.append(detection)
+
+    return relevant_detections
 
 
-def exclude_detections_by_scan_type(scan_type: str, command_scan_type: str, detections) -> List:
-    if command_scan_type == PRE_COMMIT_COMMAND_SCAN_TYPE:
+def _exclude_detections_by_scan_type(
+        detections: List[Detection], scan_type: str, command_scan_type: str
+) -> List[Detection]:
+    if command_scan_type == consts.PRE_COMMIT_COMMAND_SCAN_TYPE:
         return exclude_detections_in_deleted_lines(detections)
 
-    if command_scan_type in COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES \
-            and scan_type == SECRET_SCAN_TYPE \
-            and configuration_manager.get_should_exclude_detections_in_deleted_lines(command_scan_type):
-        return exclude_detections_in_deleted_lines(detections)
+    exclude_in_deleted_lines = configuration_manager.get_should_exclude_detections_in_deleted_lines(command_scan_type)
+    if command_scan_type in consts.COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES:
+        if scan_type == consts.SECRET_SCAN_TYPE and exclude_in_deleted_lines:
+            return exclude_detections_in_deleted_lines(detections)
+
     return detections
 
 
 def exclude_detections_in_deleted_lines(detections) -> List:
     return [detection for detection in detections if detection.detection_details.get('line_type') != 'Removed']
 
 
-def exclude_detections_by_exclusions_configuration(scan_type: str, detections) -> List:
+def _exclude_detections_by_exclusions_configuration(detections: List[Detection], scan_type: str) -> List[Detection]:
     exclusions = configuration_manager.get_exclusions_by_scan_type(scan_type)
     return [detection for detection in detections if not _should_exclude_detection(detection, exclusions)]
 
 
-def get_pre_commit_modified_documents():
-    repo = Repo(os.getcwd())
-    diff_files = repo.index.diff(GIT_HEAD_COMMIT_REV, create_patch=True, R=True)
+def get_pre_commit_modified_documents(progress_bar: 'BaseProgressBar') -> Tuple[List[Document], List[Document]]:
     git_head_documents = []
     pre_committed_documents = []
+
+    repo = Repo(os.getcwd())
+    diff_files = repo.index.diff(consts.GIT_HEAD_COMMIT_REV, create_patch=True, R=True)
+    progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, len(diff_files))
     for file in diff_files:
+        progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
+
         diff_file_path = get_diff_file_path(file)
         file_path = get_path_by_os(diff_file_path)
 
-        file_content = sca_code_scanner.get_file_content_from_commit(repo, GIT_HEAD_COMMIT_REV, diff_file_path)
+        file_content = sca_code_scanner.get_file_content_from_commit(repo, consts.GIT_HEAD_COMMIT_REV, diff_file_path)
         if file_content is not None:
             git_head_documents.append(Document(file_path, file_content))
 
         if os.path.exists(file_path):
             file_content = get_file_content(file_path)
             pre_committed_documents.append(Document(file_path, file_content))
 
     return git_head_documents, pre_committed_documents
 
 
-def get_commit_range_modified_documents(path: str, from_commit_rev: str, to_commit_rev: str) -> (
-        List[Document], List[Document]):
+def get_commit_range_modified_documents(
+        progress_bar: 'BaseProgressBar',  path: str, from_commit_rev: str, to_commit_rev: str
+) -> Tuple[List[Document], List[Document]]:
     from_commit_documents = []
     to_commit_documents = []
+
     repo = Repo(path)
     diff = repo.commit(from_commit_rev).diff(to_commit_rev)
-    modified_files_diff = [change for change in diff if change.change_type != COMMIT_DIFF_DELETED_FILE_CHANGE_TYPE]
+
+    modified_files_diff = [
+        change for change in diff if change.change_type != consts.COMMIT_DIFF_DELETED_FILE_CHANGE_TYPE
+    ]
+    progress_bar.set_section_length(ProgressBarSection.PREPARE_LOCAL_FILES, len(modified_files_diff))
     for blob in modified_files_diff:
+        progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
+
         diff_file_path = get_diff_file_path(blob)
         file_path = get_path_by_os(diff_file_path)
 
         file_content = sca_code_scanner.get_file_content_from_commit(repo, from_commit_rev, diff_file_path)
         if file_content is not None:
             from_commit_documents.append(Document(file_path, file_content))
 
         file_content = sca_code_scanner.get_file_content_from_commit(repo, to_commit_rev, diff_file_path)
         if file_content is not None:
             to_commit_documents.append(Document(file_path, file_content))
 
     return from_commit_documents, to_commit_documents
 
 
-def _should_exclude_detection(detection, exclusions: Dict) -> bool:
-    exclusions_by_value = exclusions.get(EXCLUSIONS_BY_VALUE_SECTION_NAME, [])
+def _should_exclude_detection(detection: Detection, exclusions: Dict) -> bool:
+    exclusions_by_value = exclusions.get(consts.EXCLUSIONS_BY_VALUE_SECTION_NAME, [])
     if _is_detection_sha_configured_in_exclusions(detection, exclusions_by_value):
         logger.debug('Going to ignore violations because is in the values to ignore list, %s',
                      {'sha': detection.detection_details.get('sha512', '')})
         return True
 
-    exclusions_by_sha = exclusions.get(EXCLUSIONS_BY_SHA_SECTION_NAME, [])
+    exclusions_by_sha = exclusions.get(consts.EXCLUSIONS_BY_SHA_SECTION_NAME, [])
     if _is_detection_sha_configured_in_exclusions(detection, exclusions_by_sha):
         logger.debug('Going to ignore violations because is in the shas to ignore list, %s',
                      {'sha': detection.detection_details.get('sha512', '')})
         return True
 
-    exclusions_by_rule = exclusions.get(EXCLUSIONS_BY_RULE_SECTION_NAME, [])
+    exclusions_by_rule = exclusions.get(consts.EXCLUSIONS_BY_RULE_SECTION_NAME, [])
     if exclusions_by_rule:
         detection_rule = detection.detection_rule_id
         if detection_rule in exclusions_by_rule:
             logger.debug('Going to ignore violations because is in the shas to ignore list, %s',
                          {'detection_rule': detection_rule})
             return True
 
-    exclusions_by_package = exclusions.get(EXCLUSIONS_BY_PACKAGE_SECTION_NAME, [])
+    exclusions_by_package = exclusions.get(consts.EXCLUSIONS_BY_PACKAGE_SECTION_NAME, [])
     if exclusions_by_package:
         package = _get_package_name(detection)
         if package in exclusions_by_package:
             logger.debug('Going to ignore violations because is in the packages to ignore list, %s',
                          {'package': package})
             return True
 
@@ -707,38 +946,41 @@
 
 def _is_detection_sha_configured_in_exclusions(detection, exclusions: List[str]) -> bool:
     detection_sha = detection.detection_details.get('sha512', '')
     return detection_sha in exclusions
 
 
 def _is_path_configured_in_exclusions(scan_type: str, file_path: str) -> bool:
-    exclusions_by_path = configuration_manager.get_exclusions_by_scan_type(scan_type).get(
-        EXCLUSIONS_BY_PATH_SECTION_NAME, [])
+    exclusions_by_path = \
+        configuration_manager.get_exclusions_by_scan_type(scan_type).get(consts.EXCLUSIONS_BY_PATH_SECTION_NAME, [])
     for exclusion_path in exclusions_by_path:
         if is_sub_path(exclusion_path, file_path):
             return True
     return False
 
 
-def _get_package_name(detection) -> str:
+def _get_package_name(detection: Detection) -> str:
     package_name = detection.detection_details.get('vulnerable_component', '')
     package_version = detection.detection_details.get('vulnerable_component_version', '')
 
     if package_name == '':
         package_name = detection.detection_details.get('package_name', '')
         package_version = detection.detection_details.get('package_version', '')
 
     return f'{package_name}@{package_version}'
 
 
 def _is_file_relevant_for_sca_scan(filename: str) -> bool:
-    if any([sca_excluded_path in filename for sca_excluded_path in SCA_EXCLUDED_PATHS]):
-        logger.debug("file is irrelevant because it is from node_modules's inner path, %s",
-                     {'filename': filename})
+    if any([sca_excluded_path in filename for sca_excluded_path in consts.SCA_EXCLUDED_PATHS]):
+        logger.debug(
+            "file is irrelevant because it is from node_modules's inner path, %s",
+            {'filename': filename}
+        )
         return False
+
     return True
 
 
 def _is_relevant_file_to_scan(scan_type: str, filename: str) -> bool:
     if _is_subpath_of_cycode_configuration_folder(filename):
         logger.debug("file is irrelevant because it is in cycode configuration directory, %s",
                      {'filename': filename})
@@ -755,20 +997,20 @@
         return False
 
     if is_binary_file(filename):
         logger.debug("file is irrelevant because it is binary file, %s",
                      {'filename': filename})
         return False
 
-    if scan_type != SCA_SCAN_TYPE and _does_file_exceed_max_size_limit(filename):
+    if scan_type != consts.SCA_SCAN_TYPE and _does_file_exceed_max_size_limit(filename):
         logger.debug("file is irrelevant because its exceeded max size limit, %s",
                      {'filename': filename})
         return False
 
-    if scan_type == SCA_SCAN_TYPE and not _is_file_relevant_for_sca_scan(filename):
+    if scan_type == consts.SCA_SCAN_TYPE and not _is_file_relevant_for_sca_scan(filename):
         return False
 
     return True
 
 
 def _is_relevant_document_to_scan(scan_type: str, filename: str, content: str) -> bool:
     if _is_subpath_of_cycode_configuration_folder(filename):
@@ -787,79 +1029,85 @@
         return False
 
     if is_binary_content(content):
         logger.debug("document is irrelevant because it is binary, %s",
                      {'filename': filename})
         return False
 
-    if scan_type != SCA_SCAN_TYPE and _does_document_exceed_max_size_limit(content):
+    if scan_type != consts.SCA_SCAN_TYPE and _does_document_exceed_max_size_limit(content):
         logger.debug("document is irrelevant because its exceeded max size limit, %s",
                      {'filename': filename})
         return False
     return True
 
 
 def _is_file_extension_supported(scan_type: str, filename: str) -> bool:
-    if scan_type == INFRA_CONFIGURATION_SCAN_TYPE:
-        return any(filename.lower().endswith(supported_file_extension) for supported_file_extension in
-                   INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES)
-    if scan_type == SCA_SCAN_TYPE:
-        return any(filename.lower().endswith(supported_file) for supported_file in
-                   SCA_CONFIGURATION_SCAN_SUPPORTED_FILES)
-    return all(not filename.lower().endswith(file_extension_to_ignore) for file_extension_to_ignore in
-               SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE)
+    filename = filename.lower()
 
+    if scan_type == consts.INFRA_CONFIGURATION_SCAN_TYPE:
+        return any(filename.endswith(supported_file_extension)
+                   for supported_file_extension in consts.INFRA_CONFIGURATION_SCAN_SUPPORTED_FILES)
+    elif scan_type == consts.SCA_SCAN_TYPE:
+        return any(filename.endswith(supported_file)
+                   for supported_file in consts.SCA_CONFIGURATION_SCAN_SUPPORTED_FILES)
 
-def _does_file_exceed_max_size_limit(filename: str) -> bool:
-    return FILE_MAX_SIZE_LIMIT_IN_BYTES < get_file_size(filename)
+    return all(not filename.endswith(file_extension_to_ignore)
+               for file_extension_to_ignore in consts.SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE)
 
 
-def _get_document_by_file_name(documents: List[Document], file_name: str, unique_id: Optional[str] = None) \
-        -> Optional[Document]:
-    return next(
-        (document for document in documents if _normalize_file_path(document.path) == _normalize_file_path(file_name)
-         and document.unique_id == unique_id), None)
+def _does_file_exceed_max_size_limit(filename: str) -> bool:
+    return consts.FILE_MAX_SIZE_LIMIT_IN_BYTES < get_file_size(filename)
 
 
 def _does_document_exceed_max_size_limit(content: str) -> bool:
-    return FILE_MAX_SIZE_LIMIT_IN_BYTES < get_content_size(content)
+    return consts.FILE_MAX_SIZE_LIMIT_IN_BYTES < get_content_size(content)
+
+
+def _get_document_by_file_name(
+        documents: List[Document], file_name: str, unique_id: Optional[str] = None
+) -> Optional[Document]:
+    for document in documents:
+        if _normalize_file_path(document.path) == _normalize_file_path(file_name) and document.unique_id == unique_id:
+            return document
+
+    return None
 
 
 def _is_subpath_of_cycode_configuration_folder(filename: str) -> bool:
     return is_sub_path(configuration_manager.global_config_file_manager.get_config_directory_path(), filename) \
         or is_sub_path(configuration_manager.local_config_file_manager.get_config_directory_path(), filename) \
         or filename.endswith(ConfigFileManager.get_config_file_route())
 
 
-def _handle_exception(context: click.Context, e: Exception):
+def _handle_exception(context: click.Context, e: Exception, *, return_exception: bool = False) -> Optional[CliError]:
     context.obj['did_fail'] = True
 
     if context.obj['verbose']:
-        click.secho(f'Error: {traceback.format_exc()}', fg='red', nl=False)
+        click.secho(f'Error: {traceback.format_exc()}', fg='red')
 
     errors: CliErrors = {
-        NetworkError: CliError(
+        custom_exceptions.NetworkError: CliError(
             soft_fail=True,
             code='cycode_error',
             message='Cycode was unable to complete this scan. '
                     'Please try again by executing the `cycode scan` command'
         ),
-        ScanAsyncError: CliError(
+        custom_exceptions.ScanAsyncError: CliError(
             soft_fail=True,
             code='scan_error',
             message='Cycode was unable to complete this scan. '
                     'Please try again by executing the `cycode scan` command'
         ),
-        HttpUnauthorizedError: CliError(
+        custom_exceptions.HttpUnauthorizedError: CliError(
             soft_fail=True,
             code='auth_error',
             message='Unable to authenticate to Cycode, your token is either invalid or has expired. '
                     'Please re-generate your token and reconfigure it by running the `cycode configure` command'
         ),
-        ZipTooLargeError: CliError(
+        custom_exceptions.ZipTooLargeError: CliError(
             soft_fail=True,
             code='zip_too_large_error',
             message='The path you attempted to scan exceeds the current maximum scanning size cap (10MB). '
                     'Please try ignoring irrelevant paths using the ‘cycode ignore --by-path’ command '
                     'and execute the scan again'
         ),
         InvalidGitRepositoryError: CliError(
@@ -872,27 +1120,33 @@
 
     if type(e) in errors:
         error = errors[type(e)]
 
         if error.soft_fail is True:
             context.obj['soft_fail'] = True
 
-        return ConsolePrinter(context).print_error(error)
+        if return_exception:
+            return error
+
+        ConsolePrinter(context).print_error(error)
+        return
+
+    if return_exception:
+        return CliError(code='unknown_error', message=str(e))
 
     if isinstance(e, click.ClickException):
         raise e
 
     raise click.ClickException(str(e))
 
 
-def _report_scan_status(context: click.Context, scan_type: str, scan_id: str, scan_completed: bool,
+def _report_scan_status(cycode_client: 'ScanClient', scan_type: str, scan_id: str, scan_completed: bool,
                         output_detections_count: int, all_detections_count: int, files_to_scan_count: int,
-                        zip_size: int, command_scan_type: str, error_message: Optional[str]):
+                        zip_size: int, command_scan_type: str, error_message: Optional[str]) -> None:
     try:
-        cycode_client = context.obj["client"]
         end_scan_time = time.time()
         scan_status = {
             'zip_size': zip_size,
             'execution_time': int(end_scan_time - start_scan_time),
             'output_detections_count': output_detections_count,
             'all_detections_count': all_detections_count,
             'scannable_files_count': files_to_scan_count,
@@ -902,76 +1156,91 @@
             'error_message': error_message,
             'scan_type': scan_type
         }
 
         cycode_client.report_scan_status(scan_type, scan_id, scan_status)
     except Exception as e:
         logger.debug('Failed to report scan status, %s', {'exception_message': str(e)})
-        pass
 
 
-def _get_scan_id(context: click.Context):
-    scan_id = uuid4()
-    context.obj['scan_id'] = scan_id
-    return scan_id
+def _get_scan_id() -> UUID:
+    return uuid4()
 
 
 def _does_severity_match_severity_threshold(severity: str, severity_threshold: str) -> bool:
     detection_severity_value = Severity.try_get_value(severity)
     if detection_severity_value is None:
         return True
 
     return detection_severity_value >= Severity.try_get_value(severity_threshold)
 
 
-def _get_scan_result(cycode_client, scan_id: str, scan_details: ScanDetailsResponse) -> ZippedFileScanResult:
-    scan_result = init_default_scan_result(scan_id, scan_details.metadata)
+def _get_scan_result(
+        cycode_client: 'ScanClient', scan_id: str, scan_details: 'ScanDetailsResponse'
+) -> ZippedFileScanResult:
     if not scan_details.detections_count:
-        return scan_result
+        return init_default_scan_result(scan_id, scan_details.metadata)
 
     wait_for_detections_creation(cycode_client, scan_id, scan_details.detections_count)
-    scan_detections = cycode_client.get_scan_detections(scan_id)
-    scan_result.detections_per_file = _map_detections_per_file(scan_detections)
-    scan_result.did_detect = True
-    return scan_result
 
-
-def init_default_scan_result(scan_id: str, scan_metadata: str = None) -> ZippedFileScanResult:
-    return ZippedFileScanResult(did_detect=False, detections_per_file=[],
-                                scan_id=scan_id,
-                                report_url=_try_get_report_url(scan_metadata))
+    scan_detections = cycode_client.get_scan_detections(scan_id)
+    return ZippedFileScanResult(
+        did_detect=True,
+        detections_per_file=_map_detections_per_file(scan_detections),
+        scan_id=scan_id,
+        report_url=_try_get_report_url(scan_details.metadata)
+    )
+
+
+def init_default_scan_result(scan_id: str, scan_metadata: Optional[str] = None) -> ZippedFileScanResult:
+    return ZippedFileScanResult(
+        did_detect=False,
+        detections_per_file=[],
+        scan_id=scan_id,
+        report_url=_try_get_report_url(scan_metadata)
+    )
 
 
-def _try_get_report_url(metadata: str) -> Optional[str]:
-    if metadata is None:
+def _try_get_report_url(metadata_json: Optional[str]) -> Optional[str]:
+    if metadata_json is None:
         return None
+
     try:
-        metadata = json.loads(metadata)
-        return metadata.get('report_url')
-    except ValueError:
+        metadata_json = json.loads(metadata_json)
+        return metadata_json.get('report_url')
+    except json.JSONDecodeError:
         return None
 
 
-def wait_for_detections_creation(cycode_client, scan_id: str, expected_detections_count: int):
-    logger.debug("waiting for detections to be created")
+def wait_for_detections_creation(cycode_client: 'ScanClient', scan_id: str, expected_detections_count: int) -> None:
+    logger.debug('Waiting for detections to be created')
+
     scan_persisted_detections_count = 0
-    end_polling_time = time.time() + DETECTIONS_COUNT_VERIFICATION_TIMEOUT_IN_SECONDS
-    spinner = Halo(spinner='dots')
-    spinner.start("Please wait until printing scan result...")
+    polling_timeout = consts.DETECTIONS_COUNT_VERIFICATION_TIMEOUT_IN_SECONDS
+    end_polling_time = time.time() + polling_timeout
+
     while time.time() < end_polling_time:
         scan_persisted_detections_count = cycode_client.get_scan_detections_count(scan_id)
+        logger.debug(
+            f'Excepted {expected_detections_count} detections, got {scan_persisted_detections_count} detections '
+            f'({expected_detections_count - scan_persisted_detections_count} more; '
+            f'{round(end_polling_time - time.time())} seconds left)'
+        )
         if scan_persisted_detections_count == expected_detections_count:
-            spinner.succeed()
             return
-        time.sleep(DETECTIONS_COUNT_VERIFICATION_WAIT_INTERVAL_IN_SECONDS)
-    spinner.stop_and_persist(symbol="⏰".encode('utf-8'), text='Timeout')
-    logger.debug("%i detections has been created", scan_persisted_detections_count)
+
+        time.sleep(consts.DETECTIONS_COUNT_VERIFICATION_WAIT_INTERVAL_IN_SECONDS)
+
+    logger.debug(f'{scan_persisted_detections_count} detections has been created')
+    raise custom_exceptions.ScanAsyncError(
+        f'Failed to wait for detections to be created after {polling_timeout} seconds'
+    )
 
 
-def _map_detections_per_file(detections) -> List[DetectionsPerFile]:
+def _map_detections_per_file(detections: List[dict]) -> List[DetectionsPerFile]:
     detections_per_files = {}
     for detection in detections:
         try:
             detection['message'] = detection['correlation_message']
             file_name = _get_file_name_from_detection(detection)
             if file_name is None:
                 logger.debug("file name is missing from detection with id %s", detection.get('id'))
@@ -984,63 +1253,65 @@
             logger.debug("Failed to parse detection: %s", str(e))
             continue
 
     return [DetectionsPerFile(file_name=file_name, detections=file_detections)
             for file_name, file_detections in detections_per_files.items()]
 
 
-def _get_file_name_from_detection(detection):
-    if detection['category'] == "SAST":
+def _get_file_name_from_detection(detection: dict) -> str:
+    if detection['category'] == 'SAST':
         return detection['detection_details']['file_path']
 
     return detection['detection_details']['file_name']
 
 
-def _does_reach_to_max_commits_to_scan_limit(commit_ids: List, max_commits_count: Optional[int]) -> bool:
-    return max_commits_count is not None and len(commit_ids) >= max_commits_count
-
+def _does_reach_to_max_commits_to_scan_limit(commit_ids: List[str], max_commits_count: Optional[int]) -> bool:
+    if max_commits_count is None:
+        return False
 
-def _should_update_progress(scanned_commits_count: int) -> bool:
-    return scanned_commits_count and scanned_commits_count % PROGRESS_UPDATE_COMMITS_INTERVAL == 0
+    return len(commit_ids) >= max_commits_count
 
 
-def parse_commit_range(commit_range: str, path: str) -> (str, str):
+def parse_commit_range(commit_range: str, path: str) -> Tuple[str, str]:
     from_commit_rev = None
     to_commit_rev = None
+
     for commit in Repo(path).iter_commits(rev=commit_range):
         if not to_commit_rev:
             to_commit_rev = commit.hexsha
         from_commit_rev = commit.hexsha
 
     return from_commit_rev, to_commit_rev
 
 
-def _normalize_file_path(path: str):
-    if path.startswith("/"):
+def _normalize_file_path(path: str) -> str:
+    if path.startswith('/'):
         return path[1:]
-    if path.startswith("./"):
+    if path.startswith('./'):
         return path[2:]
     return path
 
 
-def perform_post_pre_receive_scan_actions(context: click.Context):
+def perform_post_pre_receive_scan_actions(context: click.Context) -> None:
     if scan_utils.is_scan_failed(context):
-        click.echo(PRE_RECEIVE_REMEDIATION_MESSAGE)
+        click.echo(consts.PRE_RECEIVE_REMEDIATION_MESSAGE)
 
 
-def enable_verbose_mode(context: click.Context):
-    context.obj["verbose"] = True
+def enable_verbose_mode(context: click.Context) -> None:
+    context.obj['verbose'] = True
+    # TODO(MarshalX): rework setting the log level for loggers
     logger.setLevel(logging.DEBUG)
+    progress_bar_logger.setLevel(logging.DEBUG)
 
 
 def is_verbose_mode_requested_in_pre_receive_scan() -> bool:
-    return does_git_push_option_have_value(VERBOSE_SCAN_FLAG)
+    return does_git_push_option_have_value(consts.VERBOSE_SCAN_FLAG)
 
 
 def should_skip_pre_receive_scan() -> bool:
-    return does_git_push_option_have_value(SKIP_SCAN_FLAG)
+    return does_git_push_option_have_value(consts.SKIP_SCAN_FLAG)
 
 
 def does_git_push_option_have_value(value: str) -> bool:
-    option_count_env_value = os.getenv(GIT_PUSH_OPTION_COUNT_ENV_VAR_NAME, '')
+    option_count_env_value = os.getenv(consts.GIT_PUSH_OPTION_COUNT_ENV_VAR_NAME, '')
     option_count = int(option_count_env_value) if option_count_env_value.isdigit() else 0
-    return any(os.getenv(f'{GIT_PUSH_OPTION_ENV_VAR_PREFIX}{i}') == value for i in range(option_count))
+    return any(os.getenv(f'{consts.GIT_PUSH_OPTION_ENV_VAR_PREFIX}{i}') == value for i in range(option_count))
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/consts.py` & `cycode-0.2.6.dev6/cycode/cli/consts.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,25 +80,30 @@
 FILE_MAX_SIZE_LIMIT_IN_BYTES = 1000000
 
 # 20MB in bytes (in binary)
 ZIP_MAX_SIZE_LIMIT_IN_BYTES = 20971520
 # 200MB in bytes (in binary)
 SCA_ZIP_MAX_SIZE_LIMIT_IN_BYTES = 209715200
 
+# scan in batches
+SCAN_BATCH_MAX_SIZE_IN_BYTES = 9 * 1024 * 1024
+SCAN_BATCH_MAX_FILES_COUNT = 1000
+# if we increase this values, the server doesn't allow connecting (ConnectionError)
+SCAN_BATCH_MAX_PARALLEL_SCANS = 5
+SCAN_BATCH_SCANS_PER_CPU = 1
+
 # scan with polling
 SCAN_POLLING_WAIT_INTERVAL_IN_SECONDS = 5
 DEFAULT_SCAN_POLLING_TIMEOUT_IN_SECONDS = 3600
 SCAN_POLLING_TIMEOUT_IN_SECONDS_ENV_VAR_NAME = 'SCAN_POLLING_TIMEOUT_IN_SECONDS'
 DETECTIONS_COUNT_VERIFICATION_TIMEOUT_IN_SECONDS = 600
 DETECTIONS_COUNT_VERIFICATION_WAIT_INTERVAL_IN_SECONDS = 10
 DEFAULT_SCA_PRE_COMMIT_TIMEOUT_IN_SECONDS = 600
 SCA_PRE_COMMIT_TIMEOUT_IN_SECONDS_ENV_VAR_NAME = 'SCA_PRE_COMMIT_TIMEOUT_IN_SECONDS'
 
-PROGRESS_UPDATE_COMMITS_INTERVAL = 100
-
 # pre receive scan
 PRE_RECEIVE_MAX_COMMITS_TO_SCAN_COUNT_ENV_VAR_NAME = 'PRE_RECEIVE_MAX_COMMITS_TO_SCAN_COUNT'
 DEFAULT_PRE_RECEIVE_MAX_COMMITS_TO_SCAN_COUNT = 50
 PRE_RECEIVE_COMMAND_TIMEOUT_ENV_VAR_NAME = 'PRE_RECEIVE_COMMAND_TIMEOUT'
 DEFAULT_PRE_RECEIVE_COMMAND_TIMEOUT_IN_SECONDS = 60
 PRE_RECEIVE_REMEDIATION_MESSAGE = """
 Cycode Secrets Push Protection
@@ -120,14 +125,17 @@
 EMPTY_COMMIT_SHA = '0000000000000000000000000000000000000000'
 GIT_PUSH_OPTION_COUNT_ENV_VAR_NAME = 'GIT_PUSH_OPTION_COUNT'
 GIT_PUSH_OPTION_ENV_VAR_PREFIX = 'GIT_PUSH_OPTION_'
 
 SKIP_SCAN_FLAG = 'skip-cycode-scan'
 VERBOSE_SCAN_FLAG = 'verbose'
 
+ISSUE_DETECTED_STATUS_CODE = 1
+NO_ISSUES_STATUS_CODE = 0
+
 LICENSE_COMPLIANCE_POLICY_ID = '8f681450-49e1-4f7e-85b7-0c8fe84b3a35'
 PACKAGE_VULNERABILITY_POLICY_ID = '9369d10a-9ac0-48d3-9921-5de7fe9a37a7'
 
 # Shortcut dependency paths by remove all middle depndencies between direct dependency and influence/vulnerable dependency.
 # Example: A -> B -> C
 # Result: A -> ... -> C
 SCA_SHORTCUT_DEPENDENCY_PATHS = 2
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.6.dev6/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.6.dev6/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.6.dev6/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.6.dev6/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.6.dev6/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/main.py` & `cycode-0.2.6.dev6/cycode/cli/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import logging
 
 import click
 import sys
 
-from typing import List, Optional
+from typing import List, Optional, TYPE_CHECKING
 
 from cycode import __version__
+from cycode.cli.consts import NO_ISSUES_STATUS_CODE, ISSUE_DETECTED_STATUS_CODE
 from cycode.cli.models import Severity
 from cycode.cli.config import config
 from cycode.cli import code_scanner
 from cycode.cli.user_settings.credentials_manager import CredentialsManager
 from cycode.cli.user_settings.configuration_manager import ConfigurationManager
 from cycode.cli.user_settings.user_settings_commands import set_credentials, add_exclusions
 from cycode.cli.auth.auth_command import authenticate
 from cycode.cli.utils import scan_utils
+from cycode.cli.utils.progress_bar import get_progress_bar
 from cycode.cyclient import logger
+from cycode.cli.utils.progress_bar import logger as progress_bar_logger
 from cycode.cyclient.cycode_client_base import CycodeClientBase
 from cycode.cyclient.models import UserAgentOptionScheme
 from cycode.cyclient.scan_config.scan_config_creator import create_scan_client
 
+if TYPE_CHECKING:
+    from cycode.cyclient.scan_client import ScanClient
+
 CONTEXT = dict()
-ISSUE_DETECTED_STATUS_CODE = 1
-NO_ISSUES_STATUS_CODE = 0
 
 
 @click.group(
     commands={
         "repository": code_scanner.scan_repository,
         "commit_history": code_scanner.scan_repository_commit_history,
         "path": code_scanner.scan_path,
@@ -102,33 +106,49 @@
 
     if soft_fail:
         context.obj["soft_fail"] = soft_fail
     else:
         context.obj["soft_fail"] = config["soft_fail"]
 
     context.obj["scan_type"] = scan_type
+
+    # save backward compatability with old style command
     if output is not None:
-        # save backward compatability with old style command
         context.obj["output"] = output
+        if output == "json":
+            context.obj["no_progress_meter"] = True
+
     context.obj["client"] = get_cycode_client(client_id, secret)
     context.obj["severity_threshold"] = severity_threshold
     context.obj["monitor"] = monitor
     context.obj["report"] = report
+
     _sca_scan_to_context(context, sca_scan)
 
+    context.obj["progress_bar"] = get_progress_bar(hidden=context.obj["no_progress_meter"])
+    context.obj["progress_bar"].start()
+
     return 1
 
 
 @code_scan.result_callback()
 @click.pass_context
-def finalize(context: click.Context, *args, **kwargs):
-    if context.obj["soft_fail"]:
+def finalize(context: click.Context, *_, **__):
+    progress_bar = context.obj.get('progress_bar')
+    if progress_bar:
+        progress_bar.stop()
+
+    if context.obj['soft_fail']:
         sys.exit(0)
 
-    sys.exit(ISSUE_DETECTED_STATUS_CODE if _should_fail_scan(context) else NO_ISSUES_STATUS_CODE)
+    exit_code = NO_ISSUES_STATUS_CODE
+    if _should_fail_scan(context):
+        exit_code = ISSUE_DETECTED_STATUS_CODE
+
+    sys.exit(exit_code)
 
 
 @click.group(
     commands={
         "scan": code_scan,
         "configure": set_credentials,
         "ignore": add_exclusions,
@@ -136,44 +156,53 @@
     },
     context_settings=CONTEXT
 )
 @click.option(
     "--verbose", "-v", is_flag=True, default=False, help="Show detailed logs",
 )
 @click.option(
+    '--no-progress-meter', is_flag=True, default=False, help='Do not show the progress meter',
+)
+@click.option(
     '--output',
     default='text',
     help='Specify the output (text/json/table), the default is text',
     type=click.Choice(['text', 'json', 'table'])
 )
 @click.option(
     '--user-agent',
     default=None,
     help='Characteristic JSON object that lets servers identify the application',
     type=str,
 )
 @click.version_option(__version__, prog_name="cycode")
 @click.pass_context
-def main_cli(context: click.Context, verbose: bool, output: str, user_agent: Optional[str]):
+def main_cli(context: click.Context, verbose: bool, no_progress_meter: bool, output: str, user_agent: Optional[str]):
     context.ensure_object(dict)
     configuration_manager = ConfigurationManager()
 
     verbose = verbose or configuration_manager.get_verbose_flag()
     context.obj['verbose'] = verbose
+    # TODO(MarshalX): rework setting the log level for loggers
     log_level = logging.DEBUG if verbose else logging.INFO
     logger.setLevel(log_level)
+    progress_bar_logger.setLevel(log_level)
 
     context.obj['output'] = output
+    if output == 'json':
+        no_progress_meter = True
+
+    context.obj['no_progress_meter'] = no_progress_meter
 
     if user_agent:
         user_agent_option = UserAgentOptionScheme().loads(user_agent)
         CycodeClientBase.enrich_user_agent(user_agent_option.user_agent_suffix)
 
 
-def get_cycode_client(client_id, client_secret):
+def get_cycode_client(client_id: str, client_secret: str) -> 'ScanClient':
     if not client_id or not client_secret:
         client_id, client_secret = _get_configured_credentials()
         if not client_id:
             raise click.ClickException("Cycode client id needed.")
         if not client_secret:
             raise click.ClickException("Cycode client secret is needed.")
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/models.py` & `cycode-0.2.6.dev6/cycode/cli/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import List, NamedTuple, Dict, Type
+from typing import List, NamedTuple, Dict, Type, Optional
 
 from cycode.cyclient.models import Detection
 
 
 class Document:
     def __init__(self, path: str, content: str, is_git_diff_format: bool = False, unique_id: str = None):
         self.path = path
@@ -54,7 +54,16 @@
 
 CliErrors = Dict[Type[Exception], CliError]
 
 
 class CliResult(NamedTuple):
     success: bool
     message: str
+
+
+class LocalScanResult(NamedTuple):
+    scan_id: str
+    report_url: Optional[str]
+    document_detections: List[DocumentDetections]
+    issue_detected: bool
+    detections_count: int
+    relevant_detections_count: int
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/printers/base_table_printer.py` & `cycode-0.2.6.dev6/cycode/cli/printers/base_table_printer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 import abc
-from typing import List
+from typing import List, TYPE_CHECKING
 
 import click
 
 from cycode.cli.printers.text_printer import TextPrinter
-from cycode.cli.models import DocumentDetections, CliError, CliResult
+from cycode.cli.models import CliError, CliResult
 from cycode.cli.printers.base_printer import BasePrinter
 
+if TYPE_CHECKING:
+    from cycode.cli.models import LocalScanResult
+
 
 class BaseTablePrinter(BasePrinter, abc.ABC):
     def __init__(self, context: click.Context):
         super().__init__(context)
         self.context = context
-        self.scan_id: str = context.obj.get('scan_id')
         self.scan_type: str = context.obj.get('scan_type')
         self.show_secret: bool = context.obj.get('show_secret', False)
 
     def print_result(self, result: CliResult) -> None:
         TextPrinter(self.context).print_result(result)
 
     def print_error(self, error: CliError) -> None:
         TextPrinter(self.context).print_error(error)
 
-    def print_scan_results(self, results: List[DocumentDetections]):
-        click.secho(f'Scan Results: (scan_id: {self.scan_id})')
-
-        if not results:
+    def print_scan_results(self, local_scan_results: List['LocalScanResult']):
+        if all(result.issue_detected == 0 for result in local_scan_results):
             click.secho('Good job! No issues were found!!! 👏👏👏', fg=self.GREEN_COLOR_NAME)
             return
 
-        self._print_results(results)
-
-        report_url = self.context.obj.get('report_url')
-        if report_url:
-            click.secho(f'Report URL: {report_url}')
+        self._print_results(local_scan_results)
 
     def _is_git_repository(self) -> bool:
         return self.context.obj.get('remote_url') is not None
 
     @abc.abstractmethod
-    def _print_results(self, results: List[DocumentDetections]) -> None:
+    def _print_results(self, local_scan_results: List['LocalScanResult']) -> None:
         raise NotImplementedError
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/printers/console_printer.py` & `cycode-0.2.6.dev6/cycode/cli/printers/console_printer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import click
 from typing import List, TYPE_CHECKING
 
 from cycode.cli.exceptions.custom_exceptions import CycodeError
-from cycode.cli.models import DocumentDetections, CliResult, CliError
+from cycode.cli.models import CliResult, CliError
 from cycode.cli.printers.table_printer import TablePrinter
 from cycode.cli.printers.sca_table_printer import SCATablePrinter
 from cycode.cli.printers.json_printer import JsonPrinter
 from cycode.cli.printers.text_printer import TextPrinter
 
 if TYPE_CHECKING:
+    from cycode.cli.models import LocalScanResult
     from cycode.cli.printers.base_printer import BasePrinter
 
 
 class ConsolePrinter:
     _AVAILABLE_PRINTERS = {
         'text': TextPrinter,
         'json': JsonPrinter,
@@ -27,17 +28,17 @@
         self.scan_type = self.context.obj.get('scan_type')
         self.output_type = self.context.obj.get('output')
 
         self._printer_class = self._AVAILABLE_PRINTERS.get(self.output_type)
         if self._printer_class is None:
             raise CycodeError(f'"{self.output_type}" output type is not supported.')
 
-    def print_scan_results(self, detections_results_list: List[DocumentDetections]) -> None:
+    def print_scan_results(self, local_scan_results: List['LocalScanResult']) -> None:
         printer = self._get_scan_printer()
-        printer.print_scan_results(detections_results_list)
+        printer.print_scan_results(local_scan_results)
 
     def _get_scan_printer(self) -> 'BasePrinter':
         printer_class = self._printer_class
 
         composite_printer = self._AVAILABLE_PRINTERS.get(f'{self.output_type}_{self.scan_type}')
         if composite_printer:
             printer_class = composite_printer
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/printers/json_printer.py` & `cycode-0.2.6.dev6/cycode/cli/printers/json_printer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import json
-from typing import List
+from typing import List, TYPE_CHECKING
 
 import click
 
-from cycode.cli.models import DocumentDetections, CliResult, CliError
+from cycode.cli.models import CliResult, CliError
 from cycode.cli.printers.base_printer import BasePrinter
 from cycode.cyclient.models import DetectionSchema
 
+if TYPE_CHECKING:
+    from cycode.cli.models import LocalScanResult
 
-class JsonPrinter(BasePrinter):
-    def __init__(self, context: click.Context):
-        super().__init__(context)
-        self.scan_id = context.obj.get('scan_id')
 
+class JsonPrinter(BasePrinter):
     def print_result(self, result: CliResult) -> None:
         result = {
             'result': result.success,
             'message': result.message
         }
 
         click.secho(self.get_data_json(result))
@@ -25,26 +24,27 @@
         result = {
             'error': error.code,
             'message': error.message
         }
 
         click.secho(self.get_data_json(result))
 
-    def print_scan_results(self, results: List[DocumentDetections]) -> None:
+    def print_scan_results(self, local_scan_results: List['LocalScanResult']) -> None:
         detections = []
-        for result in results:
-            detections.extend(result.detections)
+        for local_scan_result in local_scan_results:
+            for document_detections in local_scan_result.document_detections:
+                detections.extend(document_detections.detections)
 
         detections_dict = DetectionSchema(many=True).dump(detections)
 
         click.secho(self._get_json_scan_result(detections_dict))
 
     def _get_json_scan_result(self, detections: dict) -> str:
         result = {
-            'scan_id': str(self.scan_id),
+            'scan_id': 'DEPRECATED',    # FIXME(MarshalX): we need change JSON struct to support multiple scan results
             'detections': detections
         }
 
         return self.get_data_json(result)
 
     @staticmethod
     def get_data_json(data: dict) -> str:
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/printers/sca_table_printer.py` & `cycode-0.2.6.dev6/cycode/cli/printers/sca_table_printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from collections import defaultdict
-from typing import List, Dict
+from typing import List, Dict, TYPE_CHECKING
 
 import click
 from texttable import Texttable
 
 from cycode.cli.consts import LICENSE_COMPLIANCE_POLICY_ID, PACKAGE_VULNERABILITY_POLICY_ID
-from cycode.cli.models import DocumentDetections, Detection
+from cycode.cli.models import Detection
 from cycode.cli.printers.base_table_printer import BaseTablePrinter
 from cycode.cli.utils.string_utils import shortcut_dependency_paths
 
+if TYPE_CHECKING:
+    from cycode.cli.models import LocalScanResult
+
 SEVERITY_COLUMN = 'Severity'
 LICENSE_COLUMN = 'License'
 UPGRADE_COLUMN = 'Upgrade'
 REPOSITORY_COLUMN = 'Repository'
 CVE_COLUMN = 'CVE'
 
 PREVIEW_DETECTIONS_COMMON_HEADERS = [
@@ -22,50 +25,53 @@
     'Direct Dependency',
     'Development Dependency',
     'Dependency Paths',
 ]
 
 
 class SCATablePrinter(BaseTablePrinter):
-    def _print_results(self, results: List[DocumentDetections]) -> None:
-        detections_per_detection_type_id = self._extract_detections_per_detection_type_id(results)
+    def _print_results(self, local_scan_results: List['LocalScanResult']) -> None:
+        detections_per_detection_type_id = self._extract_detections_per_detection_type_id(local_scan_results)
         self._print_detection_per_detection_type_id(detections_per_detection_type_id)
 
     @staticmethod
-    def _extract_detections_per_detection_type_id(results: List[DocumentDetections]) -> Dict[str, List[Detection]]:
+    def _extract_detections_per_detection_type_id(
+            local_scan_results: List['LocalScanResult']
+    ) -> Dict[str, List[Detection]]:
         detections_per_detection_type_id = defaultdict(list)
 
-        for document_detection in results:
-            for detection in document_detection.detections:
-                detections_per_detection_type_id[detection.detection_type_id].append(detection)
+        for local_scan_result in local_scan_results:
+            for document_detection in local_scan_result.document_detections:
+                for detection in document_detection.detections:
+                    detections_per_detection_type_id[detection.detection_type_id].append(detection)
 
         return detections_per_detection_type_id
 
     def _print_detection_per_detection_type_id(
             self, detections_per_detection_type_id: Dict[str, List[Detection]]
     ) -> None:
         for detection_type_id in detections_per_detection_type_id:
             detections = detections_per_detection_type_id[detection_type_id]
             headers = self._get_table_headers()
 
             title = None
             rows = []
 
             if detection_type_id == PACKAGE_VULNERABILITY_POLICY_ID:
-                title = "Dependencies Vulnerabilities"
+                title = 'Dependencies Vulnerabilities'
 
                 headers = [SEVERITY_COLUMN] + headers
                 headers.extend(PREVIEW_DETECTIONS_COMMON_HEADERS)
                 headers.append(CVE_COLUMN)
                 headers.append(UPGRADE_COLUMN)
 
                 for detection in detections:
                     rows.append(self._get_upgrade_package_vulnerability(detection))
             elif detection_type_id == LICENSE_COMPLIANCE_POLICY_ID:
-                title = "License Compliance"
+                title = 'License Compliance'
 
                 headers.extend(PREVIEW_DETECTIONS_COMMON_HEADERS)
                 headers.append(LICENSE_COLUMN)
 
                 for detection in detections:
                     rows.append(self._get_license(detection))
 
@@ -134,15 +140,15 @@
         row = [
             detection.detection_details.get('advisory_severity'),
             *self._get_common_detection_fields(detection),
             detection.detection_details.get('vulnerability_id')
         ]
 
         upgrade = ''
-        if alert.get("first_patched_version"):
+        if alert.get('first_patched_version'):
             upgrade = f'{alert.get("vulnerable_requirements")} -> {alert.get("first_patched_version")}'
         row.append(upgrade)
 
         return row
 
     def _get_license(self, detection: Detection) -> List[str]:
         row = self._get_common_detection_fields(detection)
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/printers/table.py` & `cycode-0.2.6.dev6/cycode/cli/printers/table.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/printers/table_printer.py` & `cycode-0.2.6.dev6/cycode/cli/printers/table_printer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,84 @@
-from typing import List
+from typing import List, TYPE_CHECKING
 
 import click
 
 from cycode.cli.printers.base_table_printer import BaseTablePrinter
 from cycode.cli.printers.table_models import ColumnInfoBuilder, ColumnWidthsConfig
 from cycode.cli.printers.table import Table
 from cycode.cli.utils.string_utils import obfuscate_text, get_position_in_line
 from cycode.cli.consts import SECRET_SCAN_TYPE, INFRA_CONFIGURATION_SCAN_TYPE, SAST_SCAN_TYPE
-from cycode.cli.models import DocumentDetections, Detection, Document
+from cycode.cli.models import Detection, Document
+
+if TYPE_CHECKING:
+    from cycode.cli.models import LocalScanResult
 
 # Creation must have strict order. Represents the order of the columns in the table (from left to right)
 ISSUE_TYPE_COLUMN = ColumnInfoBuilder.build(name='Issue Type')
 RULE_ID_COLUMN = ColumnInfoBuilder.build(name='Rule ID')
 FILE_PATH_COLUMN = ColumnInfoBuilder.build(name='File Path')
 SECRET_SHA_COLUMN = ColumnInfoBuilder.build(name='Secret SHA')
 COMMIT_SHA_COLUMN = ColumnInfoBuilder.build(name='Commit SHA')
 LINE_NUMBER_COLUMN = ColumnInfoBuilder.build(name='Line Number')
 COLUMN_NUMBER_COLUMN = ColumnInfoBuilder.build(name='Column Number')
 VIOLATION_LENGTH_COLUMN = ColumnInfoBuilder.build(name='Violation Length')
 VIOLATION_COLUMN = ColumnInfoBuilder.build(name='Violation')
+SCAN_ID_COLUMN = ColumnInfoBuilder.build(name='Scan ID')
+REPORT_URL_COLUMN = ColumnInfoBuilder.build(name='Report URL')
 
 COLUMN_WIDTHS_CONFIG: ColumnWidthsConfig = {
     SECRET_SCAN_TYPE: {
         ISSUE_TYPE_COLUMN: 2,
         RULE_ID_COLUMN: 2,
         FILE_PATH_COLUMN: 2,
         SECRET_SHA_COLUMN: 2,
         VIOLATION_COLUMN: 2,
+        SCAN_ID_COLUMN: 2,
     },
     INFRA_CONFIGURATION_SCAN_TYPE: {
         ISSUE_TYPE_COLUMN: 4,
         RULE_ID_COLUMN: 3,
         FILE_PATH_COLUMN: 3,
+        SCAN_ID_COLUMN: 2,
     },
     SAST_SCAN_TYPE: {
         ISSUE_TYPE_COLUMN: 7,
         RULE_ID_COLUMN: 2,
         FILE_PATH_COLUMN: 3,
+        SCAN_ID_COLUMN: 2,
     },
 }
 
 
 class TablePrinter(BaseTablePrinter):
-    def _print_results(self, results: List[DocumentDetections]) -> None:
+    def _print_results(self, local_scan_results: List['LocalScanResult']) -> None:
         table = self._get_table()
         if self.scan_type in COLUMN_WIDTHS_CONFIG:
             table.set_cols_width(COLUMN_WIDTHS_CONFIG[self.scan_type])
 
-        for result in results:
-            for detection in result.detections:
-                self._enrich_table_with_values(table, detection, result.document)
+        for local_scan_result in local_scan_results:
+            for document_detections in local_scan_result.document_detections:
+                report_url = local_scan_result.report_url if local_scan_result.report_url else 'N/A'
+                for detection in document_detections.detections:
+                    table.set(REPORT_URL_COLUMN, report_url)
+                    table.set(SCAN_ID_COLUMN, local_scan_result.scan_id)
+                    self._enrich_table_with_values(table, detection, document_detections.document)
 
         click.echo(table.get_table().draw())
 
     def _get_table(self) -> Table:
         table = Table()
 
         table.add(ISSUE_TYPE_COLUMN)
         table.add(RULE_ID_COLUMN)
         table.add(FILE_PATH_COLUMN)
         table.add(LINE_NUMBER_COLUMN)
         table.add(COLUMN_NUMBER_COLUMN)
+        table.add(SCAN_ID_COLUMN)
+        table.add(REPORT_URL_COLUMN)
 
         if self._is_git_repository():
             table.add(COMMIT_SHA_COLUMN)
 
         if self.scan_type == SECRET_SCAN_TYPE:
             table.add(SECRET_SHA_COLUMN)
             table.add(VIOLATION_LENGTH_COLUMN)
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/printers/text_printer.py` & `cycode-0.2.6.dev6/cycode/cli/printers/text_printer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,77 @@
 import math
-from typing import List, Optional
+from typing import List, Optional, TYPE_CHECKING
 
 import click
 
 from cycode.cli.printers.base_printer import BasePrinter
 from cycode.cli.models import DocumentDetections, Detection, Document, CliResult, CliError
 from cycode.cli.config import config
 from cycode.cli.consts import SECRET_SCAN_TYPE, COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES
 from cycode.cli.utils.string_utils import obfuscate_text, get_position_in_line
 
+if TYPE_CHECKING:
+    from cycode.cli.models import LocalScanResult
+
 
 class TextPrinter(BasePrinter):
     def __init__(self, context: click.Context):
         super().__init__(context)
-        self.scan_id: str = context.obj.get('scan_id')
         self.scan_type: str = context.obj.get('scan_type')
         self.command_scan_type: str = context.info_name
         self.show_secret: bool = context.obj.get('show_secret', False)
 
     def print_result(self, result: CliResult) -> None:
         color = None
         if not result.success:
             color = self.RED_COLOR_NAME
 
         click.secho(result.message, fg=color)
 
     def print_error(self, error: CliError) -> None:
-        click.secho(error.message, fg=self.RED_COLOR_NAME, nl=False)
-
-    def print_scan_results(self, results: List[DocumentDetections]):
-        click.secho(f"Scan Results: (scan_id: {self.scan_id})")
+        click.secho(error.message, fg=self.RED_COLOR_NAME)
 
-        if not results:
-            click.secho("Good job! No issues were found!!! 👏👏👏", fg=self.GREEN_COLOR_NAME)
+    def print_scan_results(self, local_scan_results: List['LocalScanResult']):
+        if all(result.issue_detected == 0 for result in local_scan_results):
+            click.secho('Good job! No issues were found!!! 👏👏👏', fg=self.GREEN_COLOR_NAME)
             return
 
-        for document_detections in results:
-            self._print_document_detections(document_detections)
-
-        report_url = self.context.obj.get('report_url')
-        if report_url:
-            click.secho(f'Report URL: {report_url}')
-
-    def _print_document_detections(self, document_detections: DocumentDetections):
+        for local_scan_result in local_scan_results:
+            for document_detections in local_scan_result.document_detections:
+                self._print_document_detections(
+                    document_detections, local_scan_result.scan_id, local_scan_result.report_url
+                )
+
+    def _print_document_detections(
+            self, document_detections: DocumentDetections, scan_id: str, report_url: Optional[str]
+    ):
         document = document_detections.document
         lines_to_display = self._get_lines_to_display_count()
         for detection in document_detections.detections:
-            self._print_detection_summary(detection, document.path)
+            self._print_detection_summary(detection, document.path, scan_id, report_url)
             self._print_detection_code_segment(detection, document, lines_to_display)
 
-    def _print_detection_summary(self, detection: Detection, document_path: str):
+    def _print_detection_summary(
+            self, detection: Detection, document_path: str, scan_id: str, report_url: Optional[str]
+    ):
         detection_name = detection.type if self.scan_type == SECRET_SCAN_TYPE else detection.message
+
         detection_sha = detection.detection_details.get('sha512')
         detection_sha_message = f'\nSecret SHA: {detection_sha}' if detection_sha else ''
+
+        scan_id_message = f'\nScan ID: {scan_id}'
+        report_url_message = f'\nReport URL: {report_url}' if report_url else ''
+
         detection_commit_id = detection.detection_details.get('commit_id')
         detection_commit_id_message = f'\nCommit SHA: {detection_commit_id}' if detection_commit_id else ''
+
         click.echo(
             f'⛔  Found issue of type: {click.style(detection_name, fg="bright_red", bold=True)} '
             f'(rule ID: {detection.detection_rule_id}) in file: {click.format_filename(document_path)} '
-            f'{detection_sha_message}{detection_commit_id_message}  ⛔'
+            f'{detection_sha_message}{scan_id_message}{report_url_message}{detection_commit_id_message}  ⛔'
         )
 
     def _print_detection_code_segment(self, detection: Detection, document: Document, code_segment_size: int):
         if self._is_git_diff_based_scan():
             self._print_detection_from_git_diff(detection, document)
             return
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.6.dev6/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.6.dev6/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.6.dev6/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.6.dev6/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.6.dev6/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/utils/path_utils.py` & `cycode-0.2.6.dev6/cycode/cli/utils/path_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterable, List, Optional
+from typing import Iterable, List, Optional, AnyStr
 import pathspec
 import os
 from pathlib import Path
 from binaryornot.check import is_binary
 
 
 def get_relevant_files_in_path(path: str, exclude_patterns: Iterable[str]) -> List[str]:
@@ -61,14 +61,14 @@
     return os.path.dirname(path)
 
 
 def join_paths(path: str, filename: str) -> str:
     return os.path.join(path, filename)
 
 
-def get_file_content(file_path: str) -> Optional[str]:
+def get_file_content(file_path: str) -> Optional[AnyStr]:
     try:
-        with open(file_path, "r", encoding="utf-8") as f:
+        with open(file_path, 'r', encoding='UTF-8') as f:
             content = f.read()
         return content
-    except FileNotFoundError:
+    except (FileNotFoundError, UnicodeDecodeError):
         return None
```

### Comparing `cycode-0.2.6.dev5/cycode/cli/utils/shell_executor.py` & `cycode-0.2.6.dev6/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/utils/string_utils.py` & `cycode-0.2.6.dev6/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/utils/task_timer.py` & `cycode-0.2.6.dev6/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.6.dev6/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cli/zip_file.py` & `cycode-0.2.6.dev6/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cyclient/auth_client.py` & `cycode-0.2.6.dev6/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cyclient/config.py` & `cycode-0.2.6.dev6/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cyclient/cycode_client_base.py` & `cycode-0.2.6.dev6/cycode/cyclient/cycode_client_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import platform
 from typing import Dict
 
+from cycode.cyclient import logger
 from requests import Response, request, exceptions
 
 from cycode import __version__
 from . import config
 from ..cli.exceptions.custom_exceptions import NetworkError, HttpUnauthorizedError
 from ..cli.user_settings.configuration_manager import ConfigurationManager
 
@@ -68,29 +69,34 @@
         return self._execute(method='get', endpoint=url_path, headers=headers, **kwargs)
 
     def _execute(
             self,
             method: str,
             endpoint: str,
             headers: dict = None,
+            without_auth: bool = False,
             **kwargs
     ) -> Response:
         url = self.build_full_url(self.api_url, endpoint)
+        logger.debug(f'Executing {method.upper()} request to {url}')
 
         try:
+            headers = self.get_request_headers(headers, without_auth=without_auth)
             response = request(
-                method=method, url=url, timeout=self.timeout, headers=self.get_request_headers(headers), **kwargs
+                method=method, url=url, timeout=self.timeout, headers=headers, **kwargs
             )
 
+            logger.debug(f'Response {response.status_code} from {url}. Content: {response.text}')
+
             response.raise_for_status()
             return response
         except Exception as e:
             self._handle_exception(e)
 
-    def get_request_headers(self, additional_headers: dict = None) -> dict:
+    def get_request_headers(self, additional_headers: dict = None, **kwargs) -> dict:
         if additional_headers is None:
             return self.MANDATORY_HEADERS.copy()
         return {**self.MANDATORY_HEADERS, **additional_headers}
 
     def build_full_url(self, url: str, endpoint: str) -> str:
         return f'{url}/{endpoint}'
```

### Comparing `cycode-0.2.6.dev5/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.6.dev6/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.6.dev6/cycode/cyclient/cycode_token_based_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,26 @@
     def refresh_api_token_if_needed(self) -> None:
         if self._api_token is None or self._expires_in is None or arrow.utcnow() >= self._expires_in:
             self.refresh_api_token()
 
     def refresh_api_token(self) -> None:
         auth_response = self.post(
             url_path=f'api/v1/auth/api-token',
-            body={'clientId': self.client_id, 'secret': self.client_secret}
+            body={'clientId': self.client_id, 'secret': self.client_secret},
+            without_auth=True,
         )
         auth_response_data = auth_response.json()
 
         self._api_token = auth_response_data['token']
         self._expires_in = arrow.utcnow().shift(seconds=auth_response_data['expires_in'] * 0.8)
 
-    def get_request_headers(self, additional_headers: dict = None) -> dict:
+    def get_request_headers(self, additional_headers: dict = None, without_auth=False) -> dict:
         headers = super().get_request_headers(additional_headers=additional_headers)
 
-        if not self.lock.locked():
+        if not without_auth:
             headers = self._add_auth_header(headers)
 
         return headers
 
     def _add_auth_header(self, headers: dict) -> dict:
         headers['Authorization'] = f'Bearer {self.api_token}'
         return headers
```

### Comparing `cycode-0.2.6.dev5/cycode/cyclient/models.py` & `cycode-0.2.6.dev6/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/cycode/cyclient/scan_client.py` & `cycode-0.2.6.dev6/cycode/cyclient/scan_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         files = {'file': ('multiple_files_scan.zip', zip_file.read())}
 
         response = self.scan_cycode_client.post(
             url_path=url_path,
             data={'scan_id': scan_id, 'is_git_diff': is_git_diff, 'scan_parameters': json.dumps(scan_parameters)},
             files=files
         )
+
         return self.parse_zipped_file_scan_response(response)
 
     def zipped_file_scan_async(self, zip_file: InMemoryZip, scan_type: str, scan_parameters: dict,
                                is_git_diff: bool = False) -> models.ScanInitializationResponse:
         url_path = f'{self.scan_config.get_scans_prefix()}/{self.SCAN_CONTROLLER_PATH}/{scan_type}/repository'
         files = {'file': ('multiple_files_scan.zip', zip_file.read())}
         response = self.scan_cycode_client.post(
@@ -68,22 +69,28 @@
 
     def get_scan_details(self, scan_id: str) -> models.ScanDetailsResponse:
         url_path = f'{self.scan_config.get_scans_prefix()}/{self.SCAN_CONTROLLER_PATH}/{scan_id}'
         response = self.scan_cycode_client.get(url_path=url_path)
         return models.ScanDetailsResponseSchema().load(response.json())
 
     def get_scan_detections(self, scan_id: str) -> List[dict]:
+        url_path = f'{self.scan_config.get_detections_prefix()}/{self.DETECTIONS_SERVICE_CONTROLLER_PATH}'
+        params = {'scan_id': scan_id}
+
+        page_size = 200
+
         detections = []
+
         page_number = 0
-        page_size = 200
         last_response_size = 0
-
         while page_number == 0 or last_response_size == page_size:
-            url_path = f'{self.scan_config.get_detections_prefix()}/{self.DETECTIONS_SERVICE_CONTROLLER_PATH}?scan_id={scan_id}&page_size={page_size}&page_number={page_number}'
-            response = self.scan_cycode_client.get(url_path=url_path).json()
+            params['page_size'] = page_size
+            params['page_number'] = page_number
+
+            response = self.scan_cycode_client.get(url_path=url_path, params=params).json()
             detections.extend(response)
 
             page_number += 1
             last_response_size = len(response)
 
         return detections
```

### Comparing `cycode-0.2.6.dev5/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.6.dev6/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev5/pyproject.toml` & `cycode-0.2.6.dev6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.6.dev5" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.6.dev6" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
@@ -31,15 +31,14 @@
 colorama = ">=0.4.3,<0.5.0"
 pyyaml = ">=6.0,<7.0"
 marshmallow = ">=3.8.0,<3.9.0"
 pathspec = ">=0.8.0,<0.9.0"
 gitpython = ">=3.1.30,<3.2.0"
 arrow = ">=0.17.0,<0.18.0"
 binaryornot = ">=0.4.4,<0.5.0"
-halo = "==0.0.31"
 texttable = ">=1.6.7,<1.7.0"
 requests = ">=2.24,<3.0"
 
 [tool.poetry.group.test.dependencies]
 mock = ">=4.0.3,<4.1.0"
 pytest = ">=7.3.1,<7.4.0"
 pytest-mock = ">=3.10.0,<3.11.0"
```

### Comparing `cycode-0.2.6.dev5/PKG-INFO` & `cycode-0.2.6.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.6.dev5
+Version: 0.2.6.dev6
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
@@ -22,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: arrow (>=0.17.0,<0.18.0)
 Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
 Requires-Dist: click (>=8.1.0,<8.2.0)
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
 Requires-Dist: gitpython (>=3.1.30,<3.2.0)
-Requires-Dist: halo (==0.0.31)
 Requires-Dist: marshmallow (>=3.8.0,<3.9.0)
 Requires-Dist: pathspec (>=0.8.0,<0.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.24,<3.0)
 Requires-Dist: texttable (>=1.6.7,<1.7.0)
 Project-URL: Repository, https://github.com/cycodehq-public/cycode-cli
 Description-Content-Type: text/markdown
```

