# Comparing `tmp/hcs-cli-0.1.34.tar.gz` & `tmp/hcs-cli-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.34.tar", last modified: Mon Apr 24 21:14:15 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.36.tar", last modified: Tue Jun 13 19:58:39 2023, max compression
```

## Comparing `hcs-cli-0.1.34.tar` & `hcs-cli-0.1.36.tar`

### file list

```diff
@@ -1,141 +1,151 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.908372 hcs-cli-0.1.34/
--rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.34/.gitignore
--rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)      851 2023-04-24 20:31:20.000000 hcs-cli-0.1.34/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-24 21:14:15.907988 hcs-cli-0.1.34/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.720647 hcs-cli-0.1.34/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     3039 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.694623 hcs-cli-0.1.34/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.721841 hcs-cli-0.1.34/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-24 21:14:15.908471 hcs-cli-0.1.34/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      545 2023-04-24 21:13:25.000000 hcs-cli-0.1.34/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.723975 hcs-cli-0.1.34/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.724607 hcs-cli-0.1.34/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.725193 hcs-cli-0.1.34/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.727697 hcs-cli-0.1.34/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.728948 hcs-cli-0.1.34/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/test_auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.729995 hcs-cli-0.1.34/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.34/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       87 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.731158 hcs-cli-0.1.34/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.733469 hcs-cli-0.1.34/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.734065 hcs-cli-0.1.34/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.735787 hcs-cli-0.1.34/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      341 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.737841 hcs-cli-0.1.34/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      349 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/auth.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.739081 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.741277 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      382 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.745041 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1257 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      975 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.701395 hcs-cli-0.1.34/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.746332 hcs-cli-0.1.34/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      249 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      410 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.747436 hcs-cli-0.1.34/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      310 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      605 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.750788 hcs-cli-0.1.34/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.751869 hcs-cli-0.1.34/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      171 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/test.py
--rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.753947 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/redeem-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/request-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/test.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2264 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.755058 hcs-cli-0.1.34/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.762252 hcs-cli-0.1.34/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      107 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      611 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.763863 hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     4141 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     5748 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)      600 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2162 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     3974 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)      899 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     2180 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2656 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.899474 hcs-cli-0.1.34/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     3870 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-24 21:01:55.000000 hcs-cli-0.1.34/vhcs/common/sglib/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.900748 hcs-cli-0.1.34/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-04-24 20:24:09.000000 hcs-cli-0.1.34/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.904693 hcs-cli-0.1.34/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      823 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/admin.py
--rw-r--r--   0 nanw       (501) staff       (20)     3217 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/lcm.py
--rw-r--r--   0 nanw       (501) staff       (20)      995 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/service/org_service.py
--rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/pki.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/vmhub.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.907268 hcs-cli-0.1.34/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/util/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2159 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4688 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1160 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.564299 hcs-cli-0.1.36/
+-rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.36/.gitignore
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.36/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.36/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.36/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.36/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.36/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      851 2023-04-24 20:31:20.000000 hcs-cli-0.1.36/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.36/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     2375 2023-06-13 19:58:39.563914 hcs-cli-0.1.36/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1501 2023-06-13 18:55:03.000000 hcs-cli-0.1.36/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.471273 hcs-cli-0.1.36/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)     5685 2023-06-13 19:47:35.000000 hcs-cli-0.1.36/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.36/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5700 2023-06-13 18:48:47.000000 hcs-cli-0.1.36/doc/hcs-cli-cheatsheet.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.475237 hcs-cli-0.1.36/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     2375 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     3207 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      127 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-06-13 19:58:39.000000 hcs-cli-0.1.36/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.440331 hcs-cli-0.1.36/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.475964 hcs-cli-0.1.36/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.36/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-06-13 19:58:39.564418 hcs-cli-0.1.36/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1145 2023-06-13 19:57:53.000000 hcs-cli-0.1.36/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.477856 hcs-cli-0.1.36/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3025 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.478796 hcs-cli-0.1.36/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.479469 hcs-cli-0.1.36/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.482548 hcs-cli-0.1.36/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.484238 hcs-cli-0.1.36/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)      890 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.486056 hcs-cli-0.1.36/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.36/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.487842 hcs-cli-0.1.36/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.491122 hcs-cli-0.1.36/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.491964 hcs-cli-0.1.36/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.494915 hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      941 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.498417 hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1835 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/admin/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)      975 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/auth.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.500528 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.505405 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      796 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      787 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      982 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.512018 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1074 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      835 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1575 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)      706 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/lcm/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.447635 hcs-cli-0.1.36/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.513741 hcs-cli-0.1.36/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      849 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1010 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.515612 hcs-cli-0.1.36/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      910 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.521738 hcs-cli-0.1.36/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1135 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      886 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      755 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1784 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      706 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.523400 hcs-cli-0.1.36/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4323 2023-06-13 19:41:20.000000 hcs-cli-0.1.36/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      771 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/test.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.526704 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1238 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/redeem-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1147 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/request-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      710 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/cmds/vmhub/test.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.528155 hcs-cli-0.1.36/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.538231 hcs-cli-0.1.36/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      707 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.540463 hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1965 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2341 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4741 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      937 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6348 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2762 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4574 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1499 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2780 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.545318 hcs-cli-0.1.36/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3104 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4201 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4470 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1149 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      970 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/common/sglib/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.547906 hcs-cli-0.1.36/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-04-24 20:24:09.000000 hcs-cli-0.1.36/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.558641 hcs-cli-0.1.36/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.36/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1423 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/admin.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3817 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/lcm.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1595 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/org_service.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1210 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/pki.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1529 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/service/vmhub.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-06-13 19:58:39.563222 hcs-cli-0.1.36/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.36/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1760 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.36/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.34/.gitignore` & `hcs-cli-0.1.36/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.34/Makefile` & `hcs-cli-0.1.36/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.34/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.36/hcs_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 .gitignore
 CHANGELOG.md
+CODE_OF_CONDUCT.md
+CONTRIBUTING_CLA.md
+GOVERNANCE.md
+LICENSE
 Makefile
+NOTICE
 README.md
 mypy.ini
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
+doc/dev-setup.md
+doc/get-csp-user-api-token.md
+doc/hcs-cli-cheatsheet.md
 hcs_cli.egg-info/PKG-INFO
 hcs_cli.egg-info/SOURCES.txt
 hcs_cli.egg-info/dependency_links.txt
 hcs_cli.egg-info/entry_points.txt
 hcs_cli.egg-info/requires.txt
 hcs_cli.egg-info/top_level.txt
 payload/lcm/zero.json
@@ -98,11 +106,12 @@
 vhcs/service/_util.py
 vhcs/service/admin.py
 vhcs/service/lcm.py
 vhcs/service/org_service.py
 vhcs/service/pki.py
 vhcs/service/vmhub.py
 vhcs/util/__init__.py
+vhcs/util/check_license.py
 vhcs/util/duration.py
 vhcs/util/pki_util.py
 vhcs/util/query_util.py
 vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.34/payload/lcm/zero.json` & `hcs-cli-0.1.36/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.34/pyproject.toml` & `hcs-cli-0.1.36/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 dynamic = ["version", "dependencies"]
 
 [project.scripts]
 hcs = "vhcs.cli.main:main"
 
 [project.urls]
-Homepage = "https://github.com/nanw1103/hcs-cli"
-"Bug Tracker" = "https://github.com/nanw1103/hcs-cli/issues"
+Homepage = "https://github.com/vmware/horizon-cloud-service-cli"
+"Bug Tracker" = "https://github.com/vmware/horizon-cloud-service-cli/issues"
 documentation = "https://readthedocs.org"
-repository = "https://github.com/nanw1103/hcs-cli"
-changelog = "https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md"
+repository = "https://github.com/vmware/horizon-cloud-service-cli"
+changelog = "https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md"
 
 [tool.black]
 line-length = 120
 target-version = ['py310']
 include = '\.pyi?$'
 extend-exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
```

### Comparing `hcs-cli-0.1.34/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.36/tests/vhcs/cli/cmds/test_context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+Copyright 2023-2023 VMware Inc.
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import unittest
 from test_utils import CliTest
 
 
 class TestContext(CliTest):
     def test1_default_help(self):
         self.verify("hcs context", CliTest.NON_EMPTY_STRING)
```

### Comparing `hcs-cli-0.1.34/vhcs/cli/main.py` & `hcs-cli-0.1.36/vhcs/cli/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 #!/usr/bin/env -S python3 -W ignore
 
+"""
+Copyright 2023-2023 VMware Inc.
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+
 import sys
 import json
 import httpx
 import click
 import os.path as path
 import logging
```

### Comparing `hcs-cli-0.1.34/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.36/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.34/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.36/vhcs/common/ctxp/fstore.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+Copyright 2023-2023 VMware Inc.
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import os
 import logging
 from os import path, listdir
 from typing import Any
 from collections.abc import Generator
 from . import jsondot
 from .jsondot import dotdict
```

### Comparing `hcs-cli-0.1.34/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.36/vhcs/common/ctxp/profile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+Copyright 2023-2023 VMware Inc.
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 from typing import Any
 from .util import CtxpException, panic
 from .jsondot import dotdict
 from .fstore import fstore
 
 _store: fstore = None
 _active_profile_name: str = None
```

### Comparing `hcs-cli-0.1.34/vhcs/common/logger.py` & `hcs-cli-0.1.36/vhcs/common/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+Copyright 2023-2023 VMware Inc.
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import sys
 import os
 import re
 import logging
 import coloredlogs
 from logging.handlers import RotatingFileHandler
```

### Comparing `hcs-cli-0.1.34/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.36/vhcs/common/sglib/csp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+Copyright 2023-2023 VMware Inc.
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import httpx
 import jwt
 import time
 import logging
 from vhcs.common.ctxp import jsondot
 
 log = logging.getLogger(__name__)
```

### Comparing `hcs-cli-0.1.34/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.36/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.34/vhcs/service/lcm.py` & `hcs-cli-0.1.36/vhcs/service/lcm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+Copyright 2023-2023 VMware Inc.
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import time
 import json
 from typing import Any
 from ._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("lcm")
```

### Comparing `hcs-cli-0.1.34/vhcs/util/duration.py` & `hcs-cli-0.1.36/vhcs/util/duration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+Copyright 2023-2023 VMware Inc.
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import re
 
 PATTERN = re.compile("^(([0-9]+)D)?(([0-9]+)H)?(([0-9]+)M)?(([0-9]+)S)?$")
 
 
 # Examples
```

### Comparing `hcs-cli-0.1.34/vhcs/util/pki_util.py` & `hcs-cli-0.1.36/vhcs/util/pki_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+Copyright 2023-2023 VMware Inc.
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import base64
 import os
 import subprocess
 from typing import List
 from OpenSSL import crypto
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
```

