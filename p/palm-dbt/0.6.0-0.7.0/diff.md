# Comparing `tmp/palm-dbt-0.6.0.tar.gz` & `tmp/palm-dbt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palm-dbt-0.6.0.tar", last modified: Fri Jun  2 15:08:03 2023, max compression
+gzip compressed data, was "palm-dbt-0.7.0.tar", last modified: Tue Jun 13 19:56:17 2023, max compression
```

## Comparing `palm-dbt-0.6.0.tar` & `palm-dbt-0.7.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.119712 palm-dbt-0.6.0/palm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.119712 palm-dbt-0.6.0/palm/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.123712 palm-dbt-0.6.0/palm/plugins/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.127713 palm-dbt-0.6.0/palm/plugins/dbt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_containerize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_dbt-docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_model-doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_prod-artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/dbt_containerizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/dbt_palm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/dbt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/local_user_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.127713 palm-dbt-0.6.0/palm/plugins/dbt/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/macros/drop_branch_schemas.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/macros/generate_schema_name.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.119712 palm-dbt-0.6.0/palm/plugins/dbt/model_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/model_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/docs/base_model.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/docs/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/model_template/model/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/model/base_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/model/base_model.yml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/model/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/model_template/ref_files/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/ref_files/ref_file.sql
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/ref_files/ref_file_readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/parsers/project_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/plugin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/sql_to_dbt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.119712 palm-dbt-0.6.0/palm/plugins/dbt/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/Dockerfile.txt
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/entrypoint.sh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/palm/plugins/dbt/templates/model_docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/model_docs/model_doc.tpl.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/model_docs/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/palm_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.142179 palm-dbt-0.7.0/palm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.142179 palm-dbt-0.7.0/palm/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm/plugins/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm/plugins/dbt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_containerize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_dbt-docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_model-doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_prod-artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/dbt_containerizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/dbt_palm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/dbt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/local_user_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm/plugins/dbt/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/macros/drop_branch_schemas.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/macros/generate_schema_name.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.142179 palm-dbt-0.7.0/palm/plugins/dbt/model_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm/plugins/dbt/model_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/model_template/docs/base_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/model_template/docs/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm/plugins/dbt/model_template/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/model_template/model/base_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/model_template/model/base_model.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/model_template/model/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm/plugins/dbt/model_template/ref_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/model_template/ref_files/ref_file.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/model_template/ref_files/ref_file_readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm/plugins/dbt/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/parsers/project_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/sql_to_dbt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.142179 palm-dbt-0.7.0/palm/plugins/dbt/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm/plugins/dbt/templates/containerize/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/templates/containerize/Dockerfile.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/templates/containerize/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/templates/containerize/entrypoint.sh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/templates/containerize/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm/plugins/dbt/templates/model_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/templates/model_docs/model_doc.tpl.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/palm/plugins/dbt/templates/model_docs/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/palm_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-13 19:56:17.000000 palm-dbt-0.7.0/palm_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-13 19:56:17.000000 palm-dbt-0.7.0/palm_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:56:17.000000 palm-dbt-0.7.0/palm_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 19:56:17.000000 palm-dbt-0.7.0/palm_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 19:56:17.000000 palm-dbt-0.7.0/palm_dbt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:56:17.146179 palm-dbt-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-13 19:56:09.000000 palm-dbt-0.7.0/setup.py
```

### Comparing `palm-dbt-0.6.0/LICENSE` & `palm-dbt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/PKG-INFO` & `palm-dbt-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palm-dbt
-Version: 0.6.0
+Version: 0.7.0
 Summary: dbt extension for Palm CLI
 Home-page: https://github.com/palmetto/palm-dbt
 Author: Palmetto - Data & Analytics team
 Author-email: data-analytics-team@palmetto.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `palm-dbt-0.6.0/README.md` & `palm-dbt-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_cleanup.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_containerize.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_containerize.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_cycle.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_cycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ctx,
     count: int,
     persist: bool,
     seed: bool,
     models: Optional[Tuple] = tuple(),
     select: Optional[Tuple] = tuple(),
 ):
-    """Consecutive run-test of the DBT repo. `count` is the number of run/test cycles to execute, defaults to 2"""
+    """Consecutive run-test of the dbt repo. `count` is the number of run/test cycles to execute, defaults to 2"""
 
     def add_models(command: str) -> str:
         if models:
             command += " --models " + " ".join(models)
         return command
 
     def add_select(command: str) -> str:
```

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_dbt.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_dbt.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_install.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_install.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_model-doc.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_model-doc.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_model.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 valid_model_types = ['tmp', 'staging', 'intermediate', 'dim', 'fact']
 
 
 @click.group()
 def cli():
-    """DBT model tools"""
+    """dbt model tools"""
     pass
 
 
 @cli.command('new')
 @click.pass_context
 @click.option(
     "--name",
```

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_prod-artifacts.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_prod-artifacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 def cli(environment):
 
     """No-op command: Download your dbt artifacts from production.
 
     This command is a no-op as the implementation will differ depending on your
     production environment. You should override this command in your own
     project by running `palm override --name prod-artifacts` and then
-    implementing the logic to download your DBT artifacts from production.
+    implementing the logic to download your dbt artifacts from production.
     """
 
     plugin_config = environment.plugin_config("dbt")
     artifact_path = plugin_config.dbt_artifacts_prod
 
-    msg = "No-op command! Please override this command in your own project by running: palm override --name prod-artifacts'"
+    msg = "No-op command! Please override this command in your own project by running: 'palm override --name prod-artifacts'"
 
     env_vars = dbt_env_vars(environment.palm.branch)
     # success, msg = environment.run_in_docker(cmd, env_vars)
 
     click.secho(msg, fg="red")
     sys.exit(2)
```

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_run.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from palm.plugins.dbt.dbt_palm_utils import dbt_env_vars
 import sys
 
 
 @click.command("run")
 @click.option(
     "--no-fail-fast",
+    "-nx",
     is_flag=True,
     help="Turns off --fail-fast. See dbt docs on fail-fast flag.",
 )
 @click.option("--clean", is_flag=True, help="Drop the test schema after the run")
 @click.option("--models", "-m", multiple=True, help="See dbt docs on models flag")
 @click.option("--select", "-s", multiple=True, help="See dbt docs on select flag")
 @click.option("--exclude", "-e", multiple=True, help="See dbt docs on exclude flag")
-@click.option("--defer", is_flag=True, help="See dbt docs on defer flag")
-@click.option("--iterative", is_flag=True, help="Iterative stateful dbt run")
+@click.option("--defer", "-d", is_flag=True, help="See dbt docs on defer flag")
+@click.option("--iterative", "-i", is_flag=True, help="Iterative stateful dbt run")
 @click.option(
     "--full-refresh",
+    "-f",
     is_flag=True,
     help="Will perform a full refresh on incremental models",
 )
 @click.option("--seed", is_flag=True, help="Run dbt seed before dbt run")
 @click.pass_obj
 def cli(
     environment,
@@ -32,15 +34,15 @@
     defer: bool,
     seed: bool,
     models: Optional[Tuple] = tuple(),
     select: Optional[Tuple] = tuple(),
     exclude: Optional[Tuple] = tuple(),
     vars: Optional[str] = None,
 ):
-    """Runs the DBT repo."""
+    """Runs the dbt repo."""
     stateful = iterative or defer
 
     if defer:
         click.secho("Running 'palm prod-artifacts'...", fg='yellow')
         exit_code, _, _ = environment.run_on_host("palm prod-artifacts")
         if exit_code == 2:
             click.secho(
@@ -88,15 +90,15 @@
             )
             success, msg = environment.run_in_docker(stateful_run_cmd, env_vars)
 
     click.secho(msg, fg="green" if success else "red")
 
     if clean:
         success, msg = environment.run_in_docker(
-            "dbt run-operation drop_branch_schemas && dbt clean", env_vars
+            "dbt run-operation drop_branch_schemas", env_vars
         )
         click.secho(msg, fg="green" if success else "red")
 
 
 def build_run_command(
     full_refresh: bool = False,
     seed: bool = True,
```

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_seed.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_seed.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 @click.option("--exclude", '-e', multiple=True, help="see dbt docs on exclude flag")
 @click.option(
     "--no-full-refresh",
     "-nf",
     is_flag=True,
     help="Insert seeds instead of recreating the table",
 )
-@click.obj
+@click.pass_obj
 def cli(
     environment,
     clean: bool,
     no_full_refresh: bool,
     select: Optional[Tuple] = tuple(),
     exclude: Optional[Tuple] = tuple(),
 ):
```

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_test.py` & `palm-dbt-0.7.0/palm/plugins/dbt/commands/cmd_snapshot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 import click
 from typing import Optional, Tuple
 from palm.plugins.dbt.dbt_palm_utils import dbt_env_vars
 
 
-@click.command('test')
-@click.option(
-    "--clean", is_flag=True, help="drop the test schema after the run is complete"
-)
-@click.option("--models", multiple=True, help="see dbt docs on models flag")
-@click.option("--select", multiple=True, help="see dbt docs on select flag")
-@click.option("--exclude", multiple=True, help="see dbt docs on exclude flag")
-@click.option("--no-fail-fast", is_flag=True, help="will run all tests if one fails")
-@click.pass_context
+@click.command("snapshot")
+@click.option("--clean", is_flag=True, help="Drop the test schema after the run")
+@click.option("--select", "-s", multiple=True, help="See dbt docs on select flag")
+@click.option("--exclude", "-e", multiple=True, help="See dbt docs on exclude flag")
+@click.pass_obj
 def cli(
-    ctx,
+    environment,
     clean: bool,
-    no_fail_fast: bool,
-    models: Optional[Tuple] = tuple(),
     select: Optional[Tuple] = tuple(),
     exclude: Optional[Tuple] = tuple(),
 ):
-    """Tests the DBT repo"""
+    """Executes the dbt snapshots."""
+    env_vars = dbt_env_vars(environment.palm.branch)
 
-    cmd = ['dbt', 'test']
+    cmd = ["dbt snapshot"]
     if select:
-        cmd.append('--select')
+        cmd.append("--select")
         cmd.extend(select)
-    if models:
-        cmd.append('--models')
-        cmd.extend(models)
     if exclude:
         cmd.append('--exclude')
         cmd.extend(exclude)
-    if not no_fail_fast:
-        cmd.append('--fail-fast')
-    if clean:
-        cmd.append('&& dbt run-operation drop_branch_schemas')
 
-    env_vars = dbt_env_vars(ctx.obj.palm.branch)
-    success, msg = ctx.obj.run_in_docker(" ".join(cmd), env_vars)
+    success, msg = environment.run_in_docker(" ".join(cmd), env_vars)
     click.secho(msg, fg="green" if success else "red")
+
+    if clean:
+        success, msg = environment.run_in_docker(
+            "dbt run-operation drop_branch_schemas", env_vars
+        )
+        click.secho(msg, fg="green" if success else "red")
```

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/dbt_containerizer.py` & `palm-dbt-0.7.0/palm/plugins/dbt/dbt_containerizer.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/dbt_palm_utils.py` & `palm-dbt-0.7.0/palm/plugins/dbt/dbt_palm_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from typing import Dict
 from palm.plugins.dbt.local_user_lookup import local_user_lookup
 
-""" Shared DBT utilities to build out common CLI options """
+""" Shared dbt utilities to build out common CLI options """
 
 
 def dbt_env_vars(branch: str) -> Dict:
     return {
         'PDP_DEV_SCHEMA': _generate_schema_from_branch(branch),
         'PDP_ENV': 'DEVELOPMENT',  # Deprecated - this will be removed!
         'PALM_DBT_ENV': 'DEVELOPMENT',
```

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/dbt_plugin.py` & `palm-dbt-0.7.0/palm/plugins/dbt/dbt_plugin.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/macros/drop_branch_schemas.sql` & `palm-dbt-0.7.0/palm/plugins/dbt/macros/drop_branch_schemas.sql`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/macros/generate_schema_name.sql` & `palm-dbt-0.7.0/palm/plugins/dbt/macros/generate_schema_name.sql`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/model_template/ref_files/ref_file_readme.md` & `palm-dbt-0.7.0/palm/plugins/dbt/model_template/ref_files/ref_file_readme.md`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/parsers/__init__.py` & `palm-dbt-0.7.0/palm/plugins/dbt/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/parsers/project_parser.py` & `palm-dbt-0.7.0/palm/plugins/dbt/parsers/project_parser.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/plugin_config.py` & `palm-dbt-0.7.0/palm/plugins/dbt/plugin_config.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm/plugins/dbt/sql_to_dbt.py` & `palm-dbt-0.7.0/palm/plugins/dbt/sql_to_dbt.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/palm_dbt.egg-info/PKG-INFO` & `palm-dbt-0.7.0/palm_dbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palm-dbt
-Version: 0.6.0
+Version: 0.7.0
 Summary: dbt extension for Palm CLI
 Home-page: https://github.com/palmetto/palm-dbt
 Author: Palmetto - Data & Analytics team
 Author-email: data-analytics-team@palmetto.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `palm-dbt-0.6.0/palm_dbt.egg-info/SOURCES.txt` & `palm-dbt-0.7.0/palm_dbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.6.0/setup.py` & `palm-dbt-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # User-friendly description from README.md
 this_directory = Path(__file__).parent
 long_description = Path(this_directory, 'README.md').read_text()
 
 setup(
     name='palm-dbt',
-    version='0.6.0',
+    version='0.7.0',
     description='dbt extension for Palm CLI',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Palmetto - Data & Analytics team',
     author_email='data-analytics-team@palmetto.com',
     url='https://github.com/palmetto/palm-dbt',
     packages=find_namespace_packages(include=['palm', 'palm.*']),
```

