# Comparing `tmp/cycode-0.2.5.dev6.tar.gz` & `tmp/cycode-0.2.5.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.5.dev6.tar", max compression
+gzip compressed data, was "cycode-0.2.5.dev7.tar", max compression
```

## Comparing `cycode-0.2.5.dev6.tar` & `cycode-0.2.5.dev7.tar`

### file list

```diff
@@ -1,58 +1,62 @@
--rw-r--r--   0        0        0    32320 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/README.md
--rw-r--r--   0        0        0      115 2023-06-11 19:03:10.048696 cycode-0.2.5.dev6/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     2813 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4761 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1652 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    47480 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      453 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5039 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1698 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2196 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      992 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2993 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5835 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     7213 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/main.py
--rw-r--r--   0        0        0     1332 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      564 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0     1709 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1537 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     6108 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     9166 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4821 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     6925 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1908 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6853 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0      195 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      941 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     1229 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2700 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      815 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      929 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       57 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1708 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2458 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      119 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3617 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      543 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1705 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     9102 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6222 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1090 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1021 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      197 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     2032 2023-06-11 19:03:10.048696 cycode-0.2.5.dev6/pyproject.toml
--rw-r--r--   0        0        0    33844 1970-01-01 00:00:00.000000 cycode-0.2.5.dev6/PKG-INFO
+-rw-r--r--   0        0        0    32410 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/README.md
+-rw-r--r--   0        0        0      115 2023-06-13 10:32:01.488846 cycode-0.2.5.dev7/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2813 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4761 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    47480 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5039 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1698 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2196 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      992 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2993 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5835 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     7243 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/main.py
+-rw-r--r--   0        0        0     1332 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      626 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0     1483 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/base_table_printer.py
+-rw-r--r--   0        0        0     1891 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1537 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     5272 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/sca_table_printer.py
+-rw-r--r--   0        0        0     2277 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/table.py
+-rw-r--r--   0        0        0      477 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/table_models.py
+-rw-r--r--   0        0        0     4701 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     8955 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4821 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6925 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1908 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6853 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0      195 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      941 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1346 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2700 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      929 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2458 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      119 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3617 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      543 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1705 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     9102 2023-06-13 10:31:32.857023 cycode-0.2.5.dev7/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6222 2023-06-13 10:31:32.861023 cycode-0.2.5.dev7/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:31:32.861023 cycode-0.2.5.dev7/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1090 2023-06-13 10:31:32.861023 cycode-0.2.5.dev7/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1021 2023-06-13 10:31:32.861023 cycode-0.2.5.dev7/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      197 2023-06-13 10:31:32.861023 cycode-0.2.5.dev7/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     2032 2023-06-13 10:32:01.488846 cycode-0.2.5.dev7/pyproject.toml
+-rw-r--r--   0        0        0    33934 1970-01-01 00:00:00.000000 cycode-0.2.5.dev7/PKG-INFO
```

### Comparing `cycode-0.2.5.dev6/README.md` & `cycode-0.2.5.dev7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -207,20 +207,20 @@
 > Successful hook installation will result in the message:<br/>
 `Pre-commit installed at .git/hooks/pre-commit`
 
 # Cycode Command
 
 The following are the options and commands available with the Cycode CLI application:
 
-| Option                  | Description                                               |
-|-------------------------|-----------------------------------------------------------|
-| `--output [text\|json]` | Specify the output (`text`/`json`). The default is `text` |
-| `-v`, `--verbose`       | Show detailed logs                                        |
-| `--version`             | Show the version and exit.                                |
-| `--help`                | Show options for given command.                           |
+| Option                         | Description                                                       |
+|--------------------------------|-------------------------------------------------------------------|
+| `--output [text\|json\|table]` | Specify the output (`text`/`json`/`table`). The default is `text` |
+| `-v`, `--verbose`              | Show detailed logs                                                |
+| `--version`                    | Show the version and exit.                                        |
+| `--help`                       | Show options for given command.                                   |
 
 | Command                             | Description |
 |-------------------------------------|-------------|
 | [auth](#use-auth-command)           | Authenticates your machine to associate CLI with your Cycode account. |
 | [configure](#use-configure-command) | Initial command to authenticate your CLI client with Cycode using client ID and client secret. |
 | [ignore](#ingoring-scan-results)    | Ignore a specific value, path or rule ID |
 | [scan](#running-a-scan)             | Scan content for secrets/IaC/SCA/SAST violations. You need to specify which scan type: `ci`/`commit_history`/`path`/`repository`/etc |
```

### Comparing `cycode-0.2.5.dev6/cycode/cli/auth/auth_command.py` & `cycode-0.2.5.dev7/cycode/cli/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/auth/auth_manager.py` & `cycode-0.2.5.dev7/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/ci_integrations.py` & `cycode-0.2.5.dev7/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/code_scanner.py` & `cycode-0.2.5.dev7/cycode/cli/code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/consts.py` & `cycode-0.2.5.dev7/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.5.dev7/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.5.dev7/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.5.dev7/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.5.dev7/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.5.dev7/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/main.py` & `cycode-0.2.5.dev7/cycode/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,18 +61,18 @@
               default=False,
               help='Run scan without failing, always return a non-error status code',
               type=bool,
               required=False)
 @click.option('--output', default=None,
               help="""
               \b
-              Specify the results output (text/json), 
+              Specify the results output (text/json/table), 
               the default is text
               """,
-              type=click.Choice(['text', 'json']))
+              type=click.Choice(['text', 'json', 'table']))
 @click.option('--severity-threshold',
               default=None,
               help='Show only violations at the specified level or higher (supported for SCA scan type only).',
               type=click.Choice([e.name for e in Severity]),
               required=False)
 @click.option('--sca-scan',
               default=None,
@@ -138,16 +138,16 @@
 )
 @click.option(
     "--verbose", "-v", is_flag=True, default=False, help="Show detailed logs",
 )
 @click.option(
     '--output',
     default='text',
-    help='Specify the output (text/json), the default is text',
-    type=click.Choice(['text', 'json'])
+    help='Specify the output (text/json/table), the default is text',
+    type=click.Choice(['text', 'json', 'table'])
 )
 @click.option(
     '--user-agent',
     default=None,
     help='Characteristic JSON object that lets servers identify the application',
     type=str,
 )
```

### Comparing `cycode-0.2.5.dev6/cycode/cli/models.py` & `cycode-0.2.5.dev7/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/printers/base_printer.py` & `cycode-0.2.5.dev7/cycode/cli/printers/base_printer.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 import click
 
 from cycode.cli.models import DocumentDetections, CliResult, CliError
 
 
 class BasePrinter(ABC):
-    context: click.Context
+    RED_COLOR_NAME = 'red'
+    WHITE_COLOR_NAME = 'white'
+    GREEN_COLOR_NAME = 'green'
 
     def __init__(self, context: click.Context):
         self.context = context
 
     @abstractmethod
     def print_scan_results(self, results: List[DocumentDetections]) -> None:
         pass
```

### Comparing `cycode-0.2.5.dev6/cycode/cli/printers/console_printer.py` & `cycode-0.2.5.dev7/cycode/cli/printers/console_printer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import click
 from typing import List, TYPE_CHECKING
 
-from cycode.cli.consts import SCA_SCAN_TYPE
 from cycode.cli.exceptions.custom_exceptions import CycodeError
 from cycode.cli.models import DocumentDetections, CliResult, CliError
 from cycode.cli.printers.table_printer import TablePrinter
+from cycode.cli.printers.sca_table_printer import SCATablePrinter
 from cycode.cli.printers.json_printer import JsonPrinter
 from cycode.cli.printers.text_printer import TextPrinter
 
 if TYPE_CHECKING:
     from cycode.cli.printers.base_printer import BasePrinter
 
 
 class ConsolePrinter:
     _AVAILABLE_PRINTERS = {
         'text': TextPrinter,
         'json': JsonPrinter,
-        'text_sca': TablePrinter
+        'table': TablePrinter,
+        # overrides
+        'table_sca': SCATablePrinter,
+        'text_sca': SCATablePrinter,
     }
 
     def __init__(self, context: click.Context):
         self.context = context
+        self.scan_type = self.context.obj.get('scan_type')
         self.output_type = self.context.obj.get('output')
 
         self._printer_class = self._AVAILABLE_PRINTERS.get(self.output_type)
         if self._printer_class is None:
             raise CycodeError(f'"{self.output_type}" output type is not supported.')
 
     def print_scan_results(self, detections_results_list: List[DocumentDetections]) -> None:
         printer = self._get_scan_printer()
         printer.print_scan_results(detections_results_list)
 
     def _get_scan_printer(self) -> 'BasePrinter':
-        scan_type = self.context.obj.get('scan_type')
-
         printer_class = self._printer_class
-        if scan_type == SCA_SCAN_TYPE and self.output_type == 'text':
-            printer_class = TablePrinter
+
+        composite_printer = self._AVAILABLE_PRINTERS.get(f'{self.output_type}_{self.scan_type}')
+        if composite_printer:
+            printer_class = composite_printer
 
         return printer_class(self.context)
 
     def print_result(self, result: CliResult) -> None:
         self._printer_class(self.context).print_result(result)
 
     def print_error(self, error: CliError) -> None:
```

### Comparing `cycode-0.2.5.dev6/cycode/cli/printers/json_printer.py` & `cycode-0.2.5.dev7/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/printers/table_printer.py` & `cycode-0.2.5.dev7/cycode/cli/printers/sca_table_printer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import defaultdict
 from typing import List, Dict
 
 import click
 from texttable import Texttable
 
 from cycode.cli.consts import LICENSE_COMPLIANCE_POLICY_ID, PACKAGE_VULNERABILITY_POLICY_ID
-from cycode.cli.models import DocumentDetections, Detection, CliError, CliResult
-from cycode.cli.printers.base_printer import BasePrinter
+from cycode.cli.models import DocumentDetections, Detection
+from cycode.cli.printers.base_table_printer import BaseTablePrinter
 
 SEVERITY_COLUMN = 'Severity'
 LICENSE_COLUMN = 'License'
 UPGRADE_COLUMN = 'Upgrade'
 REPOSITORY_COLUMN = 'Repository'
 CVE_COLUMN = 'CVE'
 
@@ -19,44 +19,19 @@
     'Ecosystem',
     'Dependency Name',
     'Direct Dependency',
     'Development Dependency'
 ]
 
 
-class TablePrinter(BasePrinter):
-    RED_COLOR_NAME = 'red'
-    WHITE_COLOR_NAME = 'white'
-    GREEN_COLOR_NAME = 'green'
-
-    def __init__(self, context: click.Context):
-        super().__init__(context)
-        self.scan_id = context.obj.get('scan_id')
-
-    def print_result(self, result: CliResult) -> None:
-        raise NotImplemented
-
-    def print_error(self, error: CliError) -> None:
-        raise NotImplemented
-
-    def print_scan_results(self, results: List[DocumentDetections]):
-        click.secho(f"Scan Results: (scan_id: {self.scan_id})")
-
-        if not results:
-            click.secho("Good job! No issues were found!!! 👏👏👏", fg=self.GREEN_COLOR_NAME)
-            return
-
+class SCATablePrinter(BaseTablePrinter):
+    def _print_results(self, results: List[DocumentDetections]) -> None:
         detections_per_detection_type_id = self._extract_detections_per_detection_type_id(results)
-
         self._print_detection_per_detection_type_id(detections_per_detection_type_id)
 
-        report_url = self.context.obj.get('report_url')
-        if report_url:
-            click.secho(f'Report URL: {report_url}')
-
     @staticmethod
     def _extract_detections_per_detection_type_id(results: List[DocumentDetections]) -> Dict[str, List[Detection]]:
         detections_per_detection_type_id = defaultdict(list)
 
         for document_detection in results:
             for detection in document_detection.detections:
                 detections_per_detection_type_id[detection.detection_type_id].append(detection)
@@ -142,17 +117,14 @@
         ]
 
         if self._is_git_repository():
             row = [detection.detection_details.get('repository_name')] + row
 
         return row
 
-    def _is_git_repository(self) -> bool:
-        return self.context.obj.get("remote_url") is not None
-
     def _get_upgrade_package_vulnerability(self, detection: Detection) -> List[str]:
         alert = detection.detection_details.get('alert')
         row = [
             detection.detection_details.get('advisory_severity'),
             *self._get_common_detection_fields(detection),
             detection.detection_details.get('vulnerability_id')
         ]
```

### Comparing `cycode-0.2.5.dev6/cycode/cli/printers/text_printer.py` & `cycode-0.2.5.dev7/cycode/cli/printers/text_printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,18 @@
 
 import click
 
 from cycode.cli.printers.base_printer import BasePrinter
 from cycode.cli.models import DocumentDetections, Detection, Document, CliResult, CliError
 from cycode.cli.config import config
 from cycode.cli.consts import SECRET_SCAN_TYPE, COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES
-from cycode.cli.utils.string_utils import obfuscate_text
+from cycode.cli.utils.string_utils import obfuscate_text, get_position_in_line
 
 
 class TextPrinter(BasePrinter):
-    RED_COLOR_NAME = 'red'
-    WHITE_COLOR_NAME = 'white'
-    GREEN_COLOR_NAME = 'green'
-
     def __init__(self, context: click.Context):
         super().__init__(context)
         self.scan_id: str = context.obj.get('scan_id')
         self.scan_type: str = context.obj.get('scan_type')
         self.command_scan_type: str = context.info_name
         self.show_secret: bool = context.obj.get('show_secret', False)
 
@@ -128,17 +124,14 @@
             return self.GREEN_COLOR_NAME
 
         if line.startswith('-'):
             return self.RED_COLOR_NAME
 
         return self.WHITE_COLOR_NAME
 
-    def _get_position_in_line(self, text: str, position: int) -> int:
-        return position - text.rfind('\n', 0, position) - 1
-
     def _get_line_number_style(self, line_number: int):
         return f'{click.style(str(line_number), fg=self.WHITE_COLOR_NAME, bold=False)} ' \
                f'{click.style("|", fg=self.RED_COLOR_NAME, bold=False)}'
 
     def _get_lines_to_display_count(self) -> int:
         result_printer_configuration = config.get('result_printer')
         lines_to_display_of_scan = result_printer_configuration.get(self.scan_type, {}) \
@@ -154,15 +147,15 @@
             detection_details.get('line_in_file', -1)
         detection_position = detection_details.get('start_position', -1)
         violation_length = detection_details.get('length', -1)
 
         file_content = document.content
         file_lines = file_content.splitlines()
         start_line = self._get_code_segment_start_line(detection_line, code_segment_size)
-        detection_position_in_line = self._get_position_in_line(file_content, detection_position)
+        detection_position_in_line = get_position_in_line(file_content, detection_position)
 
         click.echo()
         for i in range(code_segment_size):
             current_line_index = start_line + i
             if current_line_index >= len(file_lines):
                 break
 
@@ -178,15 +171,15 @@
         detection_line_number_in_original_file = detection_details.get('line_in_file', -1)
         detection_position = detection_details.get('start_position', -1)
         violation_length = detection_details.get('length', -1)
 
         git_diff_content = document.content
         git_diff_lines = git_diff_content.splitlines()
         detection_line = git_diff_lines[detection_line_number]
-        detection_position_in_line = self._get_position_in_line(git_diff_content, detection_position)
+        detection_position_in_line = get_position_in_line(git_diff_content, detection_position)
 
         click.echo()
         self._print_detection_line(document, detection_line, detection_line_number_in_original_file,
                                    detection_position_in_line, violation_length)
         click.echo()
 
     def _is_git_diff_based_scan(self):
```

### Comparing `cycode-0.2.5.dev6/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.5.dev7/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.5.dev7/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.5.dev7/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.5.dev7/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.5.dev7/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/utils/path_utils.py` & `cycode-0.2.5.dev7/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/utils/shell_executor.py` & `cycode-0.2.5.dev7/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/utils/string_utils.py` & `cycode-0.2.5.dev7/cycode/cli/utils/string_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,7 +39,11 @@
     return hashlib.sha256(content.encode()).hexdigest()
 
 
 def generate_random_string(string_len: int):
     # letters, digits, and symbols
     characters = string.ascii_letters + string.digits + string.punctuation
     return ''.join(random.choice(characters) for _ in range(string_len))
+
+
+def get_position_in_line(text: str, position: int) -> int:
+    return position - text.rfind('\n', 0, position) - 1
```

### Comparing `cycode-0.2.5.dev6/cycode/cli/utils/task_timer.py` & `cycode-0.2.5.dev7/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.5.dev7/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cli/zip_file.py` & `cycode-0.2.5.dev7/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cyclient/auth_client.py` & `cycode-0.2.5.dev7/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cyclient/config.py` & `cycode-0.2.5.dev7/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cyclient/cycode_client_base.py` & `cycode-0.2.5.dev7/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.5.dev7/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.5.dev7/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cyclient/models.py` & `cycode-0.2.5.dev7/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cyclient/scan_client.py` & `cycode-0.2.5.dev7/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.5.dev7/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.5.dev7/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev6/pyproject.toml` & `cycode-0.2.5.dev7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.5.dev6" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.5.dev7" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-0.2.5.dev6/PKG-INFO` & `cycode-0.2.5.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.5.dev6
+Version: 0.2.5.dev7
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
@@ -244,20 +244,20 @@
 > Successful hook installation will result in the message:<br/>
 `Pre-commit installed at .git/hooks/pre-commit`
 
 # Cycode Command
 
 The following are the options and commands available with the Cycode CLI application:
 
-| Option                  | Description                                               |
-|-------------------------|-----------------------------------------------------------|
-| `--output [text\|json]` | Specify the output (`text`/`json`). The default is `text` |
-| `-v`, `--verbose`       | Show detailed logs                                        |
-| `--version`             | Show the version and exit.                                |
-| `--help`                | Show options for given command.                           |
+| Option                         | Description                                                       |
+|--------------------------------|-------------------------------------------------------------------|
+| `--output [text\|json\|table]` | Specify the output (`text`/`json`/`table`). The default is `text` |
+| `-v`, `--verbose`              | Show detailed logs                                                |
+| `--version`                    | Show the version and exit.                                        |
+| `--help`                       | Show options for given command.                                   |
 
 | Command                             | Description |
 |-------------------------------------|-------------|
 | [auth](#use-auth-command)           | Authenticates your machine to associate CLI with your Cycode account. |
 | [configure](#use-configure-command) | Initial command to authenticate your CLI client with Cycode using client ID and client secret. |
 | [ignore](#ingoring-scan-results)    | Ignore a specific value, path or rule ID |
 | [scan](#running-a-scan)             | Scan content for secrets/IaC/SCA/SAST violations. You need to specify which scan type: `ci`/`commit_history`/`path`/`repository`/etc |
```

