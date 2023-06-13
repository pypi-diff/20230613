# Comparing `tmp/spb-cli-0.8.1.tar.gz` & `tmp/spb-cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spb-cli-0.8.1.tar", last modified: Mon Nov 22 07:12:02 2021, max compression
+gzip compressed data, was "dist/spb-cli-0.9.0.tar", last modified: Mon Dec 20 08:45:59 2021, max compression
```

## Comparing `spb-cli-0.8.1.tar` & `spb-cli-0.9.0.tar`

### file list

```diff
@@ -1,165 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 07:09:25.000000 spb-cli-0.8.1/.github/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-11-22 07:09:25.000000 spb-cli-0.8.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      888 2021-11-22 07:09:25.000000 spb-cli-0.8.1/.github/workflows/cli_test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-22 07:09:25.000000 spb-cli-0.8.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-11-22 07:09:25.000000 spb-cli-0.8.1/.github/workflows/unit_test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2021-11-22 07:09:25.000000 spb-cli-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     9124 2021-11-22 07:12:02.000000 spb-cli-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-11-22 07:09:25.000000 spb-cli-0.8.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    90572 2021-11-22 07:09:25.000000 spb-cli-0.8.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)     7165 2021-11-22 07:09:25.000000 spb-cli-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/assets/
--rw-r--r--   0 runner    (1001) docker     (121)    50983 2021-11-22 07:09:25.000000 spb-cli-0.8.1/assets/account-name.png
--rw-r--r--   0 runner    (1001) docker     (121)  1363969 2021-11-22 07:09:25.000000 spb-cli-0.8.1/assets/configure-cli.gif
--rw-r--r--   0 runner    (1001) docker     (121)   801886 2021-11-22 07:09:25.000000 spb-cli-0.8.1/assets/describe-projects.gif
--rw-r--r--   0 runner    (1001) docker     (121)  1934101 2021-11-22 07:09:25.000000 spb-cli-0.8.1/assets/download.gif
--rw-r--r--   0 runner    (1001) docker     (121)  2592287 2021-11-22 07:09:25.000000 spb-cli-0.8.1/assets/upload.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/logo/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 07:09:25.000000 spb-cli-0.8.1/logo/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)     5936 2021-11-22 07:09:25.000000 spb-cli-0.8.1/logo/cool-tree.png
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-11-22 07:12:02.000000 spb-cli-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2021-11-22 07:09:25.000000 spb-cli-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6078 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/cli_core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/cli_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/cli_core/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/cli_core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19576 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/cli_core/commands/label_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/cli_core/commands/project.py
--rw-r--r--   0 runner    (1001) docker     (121)    15410 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/cli_core/commands/video_label_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/cli_core/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2901 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/cli_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/command/
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/command/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/command/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/core/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/core/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/core/models/attrs/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/models/attrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/models/attrs/attributes_container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/core/models/types/
--rw-r--r--   0 runner    (1001) docker     (121)      240 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/models/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8252 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/models/types/type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/models/types/type_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7147 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     6320 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/datauri/
--rw-r--r--   0 runner    (1001) docker     (121)     3991 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/datauri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/datauri/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)     3771 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/labels/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/labels/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     7960 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/labels/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/labels/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/labels/serializer/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/labels/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/labels/serializer/label_info_build_params.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/labels/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/phy_credit/
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (121)      238 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/
--rwxr-xr-x   0 runner    (1001) docker     (121)       23 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/imageV2/
--rwxr-xr-x   0 runner    (1001) docker     (121)      512 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/imageV2/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7317 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/imageV2/label_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/imageV2/legacy/
--rwxr-xr-x   0 runner    (1001) docker     (121)       25 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/imageV2/legacy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6543 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/imageV2/legacy/label_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/video/
--rwxr-xr-x   0 runner    (1001) docker     (121)      512 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/video/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9572 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/video/label_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/video/legacy/
--rwxr-xr-x   0 runner    (1001) docker     (121)       25 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/video/legacy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8059 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/video/legacy/label_info.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      416 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/phy_credit/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/phy_credit/test/image/
--rwxr-xr-x   0 runner    (1001) docker     (121)    58985 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/test/image/build_label_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/libs/phy_credit/test/video/
--rwxr-xr-x   0 runner    (1001) docker     (121)    19626 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/libs/phy_credit/test/video/build_label_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/models/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/models/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/models/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/models/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     1731 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/models/video_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/models/video_label.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/orm/
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/orm/json_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     4095 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/orm/loading.py
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/orm/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6156 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/orm/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/orm/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     4233 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/orm/type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/orm/type_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/orm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb/projects/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/projects/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/projects/project.py
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/projects/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/projects/session.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    20023 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/sdk.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/sdk_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8308 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2021-11-22 07:09:25.000000 spb-cli-0.8.1/spb/spb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9124 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      559 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-11-22 07:12:02.000000 spb-cli-0.8.1/spb_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/cli/cli_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/fixture/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/fixture/.credentials
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/sdk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/sdk/mocks/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/sdk/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/sdk/mocks/mock_data_handle.py
--rw-r--r--   0 runner    (1001) docker     (121)     5142 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/sdk/mocks/mock_label.py
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/sdk/mocks/mock_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/sdk/test_image_data_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/sdk/test_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/unit/core/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/unit/core/models/
--rw-r--r--   0 runner    (1001) docker     (121)     4758 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/core/models/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/unit/core/models/types/
--rw-r--r--   0 runner    (1001) docker     (121)    10224 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/core/models/types/test_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/core/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     8018 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/core/test_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/core/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/unit/labels/
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/labels/test_label.py
--rw-r--r--   0 runner    (1001) docker     (121)     8712 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/labels/test_label_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/unit/projects/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/projects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 07:12:02.000000 spb-cli-0.8.1/tests/unit/projects/mocks/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/projects/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4955 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/projects/mocks/get_project_response_mock.py
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2021-11-22 07:09:25.000000 spb-cli-0.8.1/tests/unit/projects/test_project_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     9052 2021-12-20 08:45:59.000000 spb-cli-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7093 2021-12-20 08:42:52.000000 spb-cli-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-12-20 08:45:59.000000 spb-cli-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1969 2021-12-20 08:42:52.000000 spb-cli-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/
+-rw-r--r--   0 runner    (1001) docker     (121)     2769 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6253 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/cli_core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/cli_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/cli_core/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/cli_core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19576 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/cli_core/commands/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4803 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/cli_core/commands/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15410 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/cli_core/commands/video_label_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/cli_core/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2901 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/cli_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/command/
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2540 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/command/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2754 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/command/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/core/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/core/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/core/models/attrs/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/models/attrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/models/attrs/attributes_container.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/core/models/types/
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/models/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8738 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/models/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1456 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/models/types/type_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7147 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6320 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/core/session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/datauri/
+-rw-r--r--   0 runner    (1001) docker     (121)     3991 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/datauri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/datauri/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (121)     3771 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/labels/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3094 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/labels/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7960 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/labels/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      929 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/labels/query.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/labels/serializer/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/labels/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1878 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/labels/serializer/label_info_build_params.py
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/labels/session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/libs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/libs/phy_credit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       23 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/imageV2/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      512 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/imageV2/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7317 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/imageV2/label_info.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/imageV2/legacy/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       25 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/imageV2/legacy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6543 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/imageV2/legacy/label_info.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/video/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      512 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/video/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9572 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/video/label_info.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/video/legacy/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       25 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/video/legacy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8059 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/video/legacy/label_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      416 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/libs/phy_credit/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1954 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3747 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1731 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/models/video_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/models/video_label.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/orm/
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/orm/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4095 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/orm/loading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1872 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/orm/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6156 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/orm/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4048 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/orm/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4233 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/orm/type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2567 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/orm/type_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/orm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb/projects/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1468 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/projects/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/projects/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/projects/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    20023 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/sdk_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8308 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/session.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2232 2021-12-20 08:42:52.000000 spb-cli-0.9.0/spb/spb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9052 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2190 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-12-20 08:45:59.000000 spb-cli-0.9.0/spb_cli.egg-info/top_level.txt
```

### Comparing `spb-cli-0.8.1/PKG-INFO` & `spb-cli-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spb-cli
-Version: 0.8.1
+Version: 0.9.0
 Summary: Suite Standard Library
 Home-page: https://github.com/Superb-AI-Suite/spb-cli.git
 Author: Super AI Dev Team
 Author-email: support@superb-ai.com
 License: MIT
 Description: <!-- <p align="center">
           <a href="http://suite-api.superb-ai.com/" target="blank"><img src="logo/cool-tree.png" width="200" height="200" alt="Cool-Tree Logo" /></a>
@@ -78,18 +78,18 @@
         
         <img src="./assets/describe-projects.gif" width="800">
         
         You can list all projects that belong to the currently configured profile by using the following command:
         ```shell
         $ spb describe projects
         
-        ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━┓
-        ┃ NAME                                               ┃ LABELS ┃ PROGRESS ┃
-        ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━┩
-        │ my-project                                         │   5837 │    13.7% │
+        ┏━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━┓
+        ┃ NAME        ┃ LABELS ┃   IN PROGRESS ┃   SUBMITTED ┃ SKIPPED ┃
+        ┡━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━┩
+        │ my-project  │   6000 │   1000 (16 %) │ 2000 (33 %) │ 0 (0 %) │
         ...
         Press any button to continue to the next page (1/10). Otherwise press ‘Q’ to quit.
         ```
         
         ## Uploading Dataset
         
         <img src="./assets/upload.gif" width="800">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spb-cli Version: 0.8.1 Summary: Suite Standard
+Metadata-Version: 2.1 Name: spb-cli Version: 0.9.0 Summary: Suite Standard
 Library Home-page: https://github.com/Superb-AI-Suite/spb-cli.git Author: Super
 AI Dev Team Author-email: support@superb-ai.com License: MIT Description:  #
 Superb AI Suite Command Line Tool ![Build](https://github.com/Superb-AI-Suite/
 spb-cli/workflows/Build/badge.svg) ![Version](https://img.shields.io/pypi/v/
 spb-cli) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]
 (https://opensource.org/licenses/MIT)  Official Superb AI Suite Command Line
 Interface for managing data and labels on [Superb AI Suite](https://
@@ -21,26 +21,26 @@
 to:** [./assets/account-name.png] ```shell $ spb configure Suite Team Name: foo
 Access Key: bar ``` Once configured, you can check the currently configured
 profile by using the `--list` option. ``` $ spb configure --list [default]
 access_key = foo team_name = bar ``` ## Resource Description ### Projects [./
 assets/describe-projects.gif] You can list all projects that belong to the
 currently configured profile by using the following command: ```shell $ spb
 describe projects
-ââââââââââââââââââââââââââââââââââââââââââââââââââââââ³âââââââââ³âââââââââââ
-â NAME â LABELS â PROGRESS â
-â¡âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ©
-â my-project â 5837 â 13.7% â ... Press any button to continue to the
-next page (1/10). Otherwise press âQâ to quit. ``` ## Uploading Dataset [./
-assets/upload.gif] You can upload data and create labels for your project with
-this command line interface. Move to the dataset directory that has image files
-(with extension of `.jpg`, `.png`, `.gif`) and upload images in the directory
-by using the following CLI command: ```shell $ cd some-folder $ spb upload
-dataset Project Name: my-project Dataset Name: my-dataset Uploading 3 data and
-0 labels to dataset 'my-dataset' under project 'my-project'. Proceed? [y/N]: y
-Uploading data:
+âââââââââââââââ³âââââââââ³ââââââââââââââââ³ââââââââââââââ³ââââââââââ
+â NAME â LABELS â IN PROGRESS â SUBMITTED â SKIPPED â
+â¡âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ©
+â my-project â 6000 â 1000 (16 %) â 2000 (33 %) â 0 (0 %) â ...
+Press any button to continue to the next page (1/10). Otherwise press âQâ
+to quit. ``` ## Uploading Dataset [./assets/upload.gif] You can upload data and
+create labels for your project with this command line interface. Move to the
+dataset directory that has image files (with extension of `.jpg`, `.png`,
+`.gif`) and upload images in the directory by using the following CLI command:
+```shell $ cd some-folder $ spb upload dataset Project Name: my-project Dataset
+Name: my-dataset Uploading 3 data and 0 labels to dataset 'my-dataset' under
+project 'my-project'. Proceed? [y/N]: y Uploading data:
 100%|ââââââââââââââââââââââââââââââââââââââââââââââââââ|
 3/3 [00:03<00:00, 1.06s/it] ``` If you wish to upload the **label** files along
 with the dataset, you can enable the `--include-label` option: ```shell $ cd
 some-folder $ spb upload dataset --include-label Project Name: my-project
 Dataset Name: my-dataset Uploading 3 data and 0 labels to dataset 'my-dataset'
 under project 'my-project'. Proceed? [y/N]: y Uploading data:
 100%|ââââââââââââââââââââââââââââââââââââââââââââââââââ|
```

### Comparing `spb-cli-0.8.1/README.md` & `spb-cli-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,18 @@
 
 <img src="./assets/describe-projects.gif" width="800">
 
 You can list all projects that belong to the currently configured profile by using the following command:
 ```shell
 $ spb describe projects
 
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━┓
-┃ NAME                                               ┃ LABELS ┃ PROGRESS ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━┩
-│ my-project                                         │   5837 │    13.7% │
+┏━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━┓
+┃ NAME        ┃ LABELS ┃   IN PROGRESS ┃   SUBMITTED ┃ SKIPPED ┃
+┡━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━┩
+│ my-project  │   6000 │   1000 (16 %) │ 2000 (33 %) │ 0 (0 %) │
 ...
 Press any button to continue to the next page (1/10). Otherwise press ‘Q’ to quit.
 ```
 
 ## Uploading Dataset
 
 <img src="./assets/upload.gif" width="800">
```

#### html2text {}

```diff
@@ -18,26 +18,26 @@
 to:** [./assets/account-name.png] ```shell $ spb configure Suite Team Name: foo
 Access Key: bar ``` Once configured, you can check the currently configured
 profile by using the `--list` option. ``` $ spb configure --list [default]
 access_key = foo team_name = bar ``` ## Resource Description ### Projects [./
 assets/describe-projects.gif] You can list all projects that belong to the
 currently configured profile by using the following command: ```shell $ spb
 describe projects
-ââââââââââââââââââââââââââââââââââââââââââââââââââââââ³âââââââââ³âââââââââââ
-â NAME â LABELS â PROGRESS â
-â¡âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ©
-â my-project â 5837 â 13.7% â ... Press any button to continue to the
-next page (1/10). Otherwise press âQâ to quit. ``` ## Uploading Dataset [./
-assets/upload.gif] You can upload data and create labels for your project with
-this command line interface. Move to the dataset directory that has image files
-(with extension of `.jpg`, `.png`, `.gif`) and upload images in the directory
-by using the following CLI command: ```shell $ cd some-folder $ spb upload
-dataset Project Name: my-project Dataset Name: my-dataset Uploading 3 data and
-0 labels to dataset 'my-dataset' under project 'my-project'. Proceed? [y/N]: y
-Uploading data:
+âââââââââââââââ³âââââââââ³ââââââââââââââââ³ââââââââââââââ³ââââââââââ
+â NAME â LABELS â IN PROGRESS â SUBMITTED â SKIPPED â
+â¡âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ©
+â my-project â 6000 â 1000 (16 %) â 2000 (33 %) â 0 (0 %) â ...
+Press any button to continue to the next page (1/10). Otherwise press âQâ
+to quit. ``` ## Uploading Dataset [./assets/upload.gif] You can upload data and
+create labels for your project with this command line interface. Move to the
+dataset directory that has image files (with extension of `.jpg`, `.png`,
+`.gif`) and upload images in the directory by using the following CLI command:
+```shell $ cd some-folder $ spb upload dataset Project Name: my-project Dataset
+Name: my-dataset Uploading 3 data and 0 labels to dataset 'my-dataset' under
+project 'my-project'. Proceed? [y/N]: y Uploading data:
 100%|ââââââââââââââââââââââââââââââââââââââââââââââââââ|
 3/3 [00:03<00:00, 1.06s/it] ``` If you wish to upload the **label** files along
 with the dataset, you can enable the `--include-label` option: ```shell $ cd
 some-folder $ spb upload dataset --include-label Project Name: my-project
 Dataset Name: my-dataset Uploading 3 data and 0 labels to dataset 'my-dataset'
 under project 'my-project'. Proceed? [y/N]: y Uploading data:
 100%|ââââââââââââââââââââââââââââââââââââââââââââââââââ|
```

### Comparing `spb-cli-0.8.1/setup.py` & `spb-cli-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/__init__.py` & `spb-cli-0.9.0/spb/__init__.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/cli.py` & `spb-cli-0.9.0/spb/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,17 +69,18 @@
 def describe():
     """Describe your RESOURCES in Suite"""
     _initiation_cli()
     spb.client()
     pass
 
 @describe.command()
-def projects():
+@click.option('-s', '--show', 'show_options', default='default', help='Show additional info about project for the given option : (default | reviews)')
+def projects(show_options):
     """Get all of your project in Suite"""
-    helper.describe_projects()
+    helper.describe_projects(show_options)
 
 @cli.group()
 def upload():
     """Upload your data to Suite"""
     _initiation_cli()
     pass
```

### Comparing `spb-cli-0.8.1/spb/cli_core/commands/label_data.py` & `spb-cli-0.9.0/spb/cli_core/commands/label_data.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/cli_core/commands/video_label_data.py` & `spb-cli-0.9.0/spb/cli_core/commands/video_label_data.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/cli_core/helper.py` & `spb-cli-0.9.0/spb/cli_core/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     project = Project()
     label_data = LabelData()
     video_label_data = VideoLabelData()
 
     def init_project(self, directory_path, project):
         return self.project.init_project(directory_path, project)
 
-    def describe_projects(self):
-        self.project.describe_projects()
+    def describe_projects(self, show_options):
+        self.project.describe_projects(show_options)
 
     def upload(self, dataset_name, project, directory_path, include_label, is_forced):
         return self.label_data.upload_data(project, dataset_name, directory_path, include_label, is_forced)
     
     def upload_video(self, dataset_name, project, directory_path, include_label, is_forced):
         return self.video_label_data.upload_data(project, dataset_name, directory_path, include_label, is_forced)
```

### Comparing `spb-cli-0.8.1/spb/cli_core/utils.py` & `spb-cli-0.9.0/spb/cli_core/utils.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/command/__init__.py` & `spb-cli-0.9.0/spb/command/__init__.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/command/builder.py` & `spb-cli-0.9.0/spb/command/builder.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/command/commands.py` & `spb-cli-0.9.0/spb/command/commands.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/core/manager.py` & `spb-cli-0.9.0/spb/core/manager.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/core/model.py` & `spb-cli-0.9.0/spb/core/model.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/core/models/attrs/attributes_container.py` & `spb-cli-0.9.0/spb/core/models/attrs/attributes_container.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/core/models/types/type.py` & `spb-cli-0.9.0/spb/core/models/types/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,28 @@
             elif isinstance(value, dict):
                 json.dumps(value)
         except Exception as e:
             raise AttributeTypeException(f'Invalid JsonObject type for {self.attr_name}: value is of {str(type(value))} type')
         return value
 
 
+class JsonList(Type):
+    GRAPHQL_TYPE='JSON'
+
+    def _validation(self, value):
+        try:
+            if isinstance(value, str):
+                value = json.loads(value)
+            if isinstance(value, list):
+                value = [json.loads(item) if isinstance(item, str) else item for item in value]
+        except Exception as e:
+            raise AttributeTypeException(f'Invalid Json type for {self.attr_name}: value is of {str(type(value))} type')
+        return value
+
+
 @abc.abstractmethod
 class Number(Type):
     """
     Top level class to define all number types in SDK
     """
     def _validation(self, value):
         return value
```

### Comparing `spb-cli-0.8.1/spb/core/models/types/type_base.py` & `spb-cli-0.9.0/spb/core/models/types/type_base.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/core/query.py` & `spb-cli-0.9.0/spb/core/query.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/core/session.py` & `spb-cli-0.9.0/spb/core/session.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/datauri/__init__.py` & `spb-cli-0.9.0/spb/datauri/__init__.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/exceptions/__init__.py` & `spb-cli-0.9.0/spb/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/labels/label.py` & `spb-cli-0.9.0/spb/labels/label.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/labels/manager.py` & `spb-cli-0.9.0/spb/labels/manager.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/labels/query.py` & `spb-cli-0.9.0/spb/labels/query.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/labels/serializer/label_info_build_params.py` & `spb-cli-0.9.0/spb/labels/serializer/label_info_build_params.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/labels/session.py` & `spb-cli-0.9.0/spb/labels/session.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/imageV2/__init__.py` & `spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/imageV2/__init__.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/imageV2/label_info.py` & `spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/imageV2/label_info.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/imageV2/legacy/label_info.py` & `spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/imageV2/legacy/label_info.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/video/__init__.py` & `spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/video/__init__.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/video/label_info.py` & `spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/video/label_info.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/libs/phy_credit/phy_credit/video/legacy/label_info.py` & `spb-cli-0.9.0/spb/libs/phy_credit/phy_credit/video/legacy/label_info.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/models/data.py` & `spb-cli-0.9.0/spb/models/data.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/models/label.py` & `spb-cli-0.9.0/spb/models/label.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/models/project.py` & `spb-cli-0.9.0/spb/models/project.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/models/video_data.py` & `spb-cli-0.9.0/spb/models/video_data.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/models/video_label.py` & `spb-cli-0.9.0/spb/models/video_label.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/orm/__init__.py` & `spb-cli-0.9.0/spb/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/orm/json_type.py` & `spb-cli-0.9.0/spb/orm/json_type.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/orm/loading.py` & `spb-cli-0.9.0/spb/orm/loading.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/orm/manager.py` & `spb-cli-0.9.0/spb/orm/manager.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/orm/model.py` & `spb-cli-0.9.0/spb/orm/model.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/orm/query.py` & `spb-cli-0.9.0/spb/orm/query.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/orm/type.py` & `spb-cli-0.9.0/spb/orm/type.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/orm/type_base.py` & `spb-cli-0.9.0/spb/orm/type_base.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/orm/utils.py` & `spb-cli-0.9.0/spb/orm/utils.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/projects/manager.py` & `spb-cli-0.9.0/spb/projects/manager.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/projects/project.py` & `spb-cli-0.9.0/spb/projects/project.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from spb.core import Model
 from spb.core.models.attrs import AttributeModel
 from spb.core.models.types import (
     JsonObject,
     String,
     ID,
     Int,
-    PlainObject
+    JsonList,
 )
 
 
 class Project(Model):
     id = ID(property_name='id', default_value=uuid.uuid4())
     name = String(property_name='name')
 
     label_interface = JsonObject(property_name='labelInterface')
     workapp = String(property_name='workapp')
 
     label_count = Int(property_name='labelCount')
     progress = Int(property_name='progress')
     submitted_label_count = Int(property_name='submittedLabelCount', default = 0)
     in_progress_label_count = Int(property_name='inProgressLabelCount', default = 0)
-    skipped_label_count = Int(property_name='skippedLabelCount', default = 0)
+    skipped_label_count = Int(property_name='skippedLabelCount', default = 0)
+    stats = JsonList(property_name='stats', default = [])
```

### Comparing `spb-cli-0.8.1/spb/projects/session.py` & `spb-cli-0.9.0/spb/projects/session.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/sdk.py` & `spb-cli-0.9.0/spb/sdk.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/session.py` & `spb-cli-0.9.0/spb/session.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb/spb_logger.py` & `spb-cli-0.9.0/spb/spb_logger.py`

 * *Files identical despite different names*

### Comparing `spb-cli-0.8.1/spb_cli.egg-info/PKG-INFO` & `spb-cli-0.9.0/spb_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spb-cli
-Version: 0.8.1
+Version: 0.9.0
 Summary: Suite Standard Library
 Home-page: https://github.com/Superb-AI-Suite/spb-cli.git
 Author: Super AI Dev Team
 Author-email: support@superb-ai.com
 License: MIT
 Description: <!-- <p align="center">
           <a href="http://suite-api.superb-ai.com/" target="blank"><img src="logo/cool-tree.png" width="200" height="200" alt="Cool-Tree Logo" /></a>
@@ -78,18 +78,18 @@
         
         <img src="./assets/describe-projects.gif" width="800">
         
         You can list all projects that belong to the currently configured profile by using the following command:
         ```shell
         $ spb describe projects
         
-        ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━┓
-        ┃ NAME                                               ┃ LABELS ┃ PROGRESS ┃
-        ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━┩
-        │ my-project                                         │   5837 │    13.7% │
+        ┏━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━┓
+        ┃ NAME        ┃ LABELS ┃   IN PROGRESS ┃   SUBMITTED ┃ SKIPPED ┃
+        ┡━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━┩
+        │ my-project  │   6000 │   1000 (16 %) │ 2000 (33 %) │ 0 (0 %) │
         ...
         Press any button to continue to the next page (1/10). Otherwise press ‘Q’ to quit.
         ```
         
         ## Uploading Dataset
         
         <img src="./assets/upload.gif" width="800">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spb-cli Version: 0.8.1 Summary: Suite Standard
+Metadata-Version: 2.1 Name: spb-cli Version: 0.9.0 Summary: Suite Standard
 Library Home-page: https://github.com/Superb-AI-Suite/spb-cli.git Author: Super
 AI Dev Team Author-email: support@superb-ai.com License: MIT Description:  #
 Superb AI Suite Command Line Tool ![Build](https://github.com/Superb-AI-Suite/
 spb-cli/workflows/Build/badge.svg) ![Version](https://img.shields.io/pypi/v/
 spb-cli) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]
 (https://opensource.org/licenses/MIT)  Official Superb AI Suite Command Line
 Interface for managing data and labels on [Superb AI Suite](https://
@@ -21,26 +21,26 @@
 to:** [./assets/account-name.png] ```shell $ spb configure Suite Team Name: foo
 Access Key: bar ``` Once configured, you can check the currently configured
 profile by using the `--list` option. ``` $ spb configure --list [default]
 access_key = foo team_name = bar ``` ## Resource Description ### Projects [./
 assets/describe-projects.gif] You can list all projects that belong to the
 currently configured profile by using the following command: ```shell $ spb
 describe projects
-ââââââââââââââââââââââââââââââââââââââââââââââââââââââ³âââââââââ³âââââââââââ
-â NAME â LABELS â PROGRESS â
-â¡âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ©
-â my-project â 5837 â 13.7% â ... Press any button to continue to the
-next page (1/10). Otherwise press âQâ to quit. ``` ## Uploading Dataset [./
-assets/upload.gif] You can upload data and create labels for your project with
-this command line interface. Move to the dataset directory that has image files
-(with extension of `.jpg`, `.png`, `.gif`) and upload images in the directory
-by using the following CLI command: ```shell $ cd some-folder $ spb upload
-dataset Project Name: my-project Dataset Name: my-dataset Uploading 3 data and
-0 labels to dataset 'my-dataset' under project 'my-project'. Proceed? [y/N]: y
-Uploading data:
+âââââââââââââââ³âââââââââ³ââââââââââââââââ³ââââââââââââââ³ââââââââââ
+â NAME â LABELS â IN PROGRESS â SUBMITTED â SKIPPED â
+â¡âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ©
+â my-project â 6000 â 1000 (16 %) â 2000 (33 %) â 0 (0 %) â ...
+Press any button to continue to the next page (1/10). Otherwise press âQâ
+to quit. ``` ## Uploading Dataset [./assets/upload.gif] You can upload data and
+create labels for your project with this command line interface. Move to the
+dataset directory that has image files (with extension of `.jpg`, `.png`,
+`.gif`) and upload images in the directory by using the following CLI command:
+```shell $ cd some-folder $ spb upload dataset Project Name: my-project Dataset
+Name: my-dataset Uploading 3 data and 0 labels to dataset 'my-dataset' under
+project 'my-project'. Proceed? [y/N]: y Uploading data:
 100%|ââââââââââââââââââââââââââââââââââââââââââââââââââ|
 3/3 [00:03<00:00, 1.06s/it] ``` If you wish to upload the **label** files along
 with the dataset, you can enable the `--include-label` option: ```shell $ cd
 some-folder $ spb upload dataset --include-label Project Name: my-project
 Dataset Name: my-dataset Uploading 3 data and 0 labels to dataset 'my-dataset'
 under project 'my-project'. Proceed? [y/N]: y Uploading data:
 100%|ââââââââââââââââââââââââââââââââââââââââââââââââââ|
```

### Comparing `spb-cli-0.8.1/spb_cli.egg-info/requires.txt` & `spb-cli-0.9.0/spb_cli.egg-info/requires.txt`

 * *Files identical despite different names*

