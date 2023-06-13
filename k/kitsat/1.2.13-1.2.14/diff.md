# Comparing `tmp/kitsat-1.2.13.tar.gz` & `tmp/kitsat-1.2.14.tar.gz`

## Comparing `kitsat-1.2.13.tar` & `kitsat-1.2.14.tar`

### file list

```diff
@@ -1,775 +1,775 @@
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/__init__.py
--rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/kitsat_cli.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/pyvenv.cfg
--rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/Scripts/activate
--rwxr-xr-x   0        0        0     1004 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/Scripts/activate.bat
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   108409 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108409 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/Scripts/pip3.11.exe
--rwxr-xr-x   0        0        0   108409 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   270608 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/Scripts/python.exe
--rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/Scripts/pythonw.exe
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/cfg/__init__.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/cfg/cli_commands.csv
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/cfg/sat_commands.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/__init__.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/cmd_parser.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/math_utils.py
--rw-r--r--   0        0        0    19805 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/modem.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/packet_parser.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/__init__.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/py.typed
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    24474 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7340 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18833 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0    10097 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    17009 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    38902 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15832 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7893 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25965 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    19348 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20994 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18959 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28417 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    28215 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    18424 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    33649 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    25328 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24728 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    19416 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    28575 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11834 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11980 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    22946 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7948 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18642 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    12053 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    23516 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    35547 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0    86413 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16855 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   279760 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31660 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10293 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13762 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    37301 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    21019 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    26121 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    44880 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27293 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   109211 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0   102881 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0   102576 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   106012 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   133760 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   107154 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    99752 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    31052 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    15210 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13912 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10972 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    42375 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    53047 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    21342 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    53291 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    15204 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    40877 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    11178 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    68194 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    44980 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    50729 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    13350 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    46526 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   215139 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    35554 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30912 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   112748 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    18522 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    32947 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63340 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0     9418 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    41326 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    36592 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    22583 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19872 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    11498 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72109 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    54776 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   219158 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    40217 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    26101 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24327 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    22027 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    19121 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    36322 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    31011 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    34326 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    21058 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10547 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   143845 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    20401 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10679 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7318 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0   101828 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14648 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    12192 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10882 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    36846 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    61408 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24986 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27869 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    36103 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    40686 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    46832 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    30360 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    21101 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20872 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    40238 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    20323 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    31520 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17599 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    35369 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    18151 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    14319 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    35741 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22623 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17672 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     7116 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14731 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10921 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10681 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/METADATA
--rw-r--r--   0        0        0    77077 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/REQUESTED
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/WHEEL
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/top_level.txt
--rw-r--r--   0        0        0   111864 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    25309 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    14040 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   136885 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    19108 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8800 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30912 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   219124 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    40217 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    26101 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24310 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0     8676 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_entry_points.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_importlib.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_itertools.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_path.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_reqs.py
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0   137216 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/cli-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    21399 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/discovery.py
--rw-r--r--   0        0        0    46800 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0   137728 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/gui-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/logging.py
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    49427 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    41146 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/py34compat.py
--rw-r--r--   0        0        0    14878 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    15197 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    48589 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    18409 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    51472 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    18380 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8475 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    14084 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    31067 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    24297 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    19416 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    16042 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    18641 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    13310 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0        0        0     5598 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    22666 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    32345 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    16975 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    31035 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19772 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0    89445 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0        0        0    31177 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    14037 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    16116 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   121783 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30912 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   219124 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    40217 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    26101 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24310 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/build.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    16204 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    14483 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    87974 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0        0        0    27558 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/__init__.py
--rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0        0        0    16781 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/expand.py
--rw-r--r--   0        0        0    19797 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0        0        0    25960 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0        0        0   270934 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/METADATA
--rw-r--r--   0        0        0    37694 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/WHEEL
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 kitsat-1.2.13/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 kitsat-1.2.13/LICENSE.md
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 kitsat-1.2.13/README.md
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 kitsat-1.2.13/pyproject.toml
--rw-r--r--   0        0        0    42710 2020-02-02 00:00:00.000000 kitsat-1.2.13/PKG-INFO
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/__init__.py
+-rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/kitsat_cli.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/pyvenv.cfg
+-rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/Scripts/activate
+-rwxr-xr-x   0        0        0     1004 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/Scripts/activate.bat
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/Scripts/deactivate.bat
+-rwxr-xr-x   0        0        0   108409 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/Scripts/pip.exe
+-rwxr-xr-x   0        0        0   108409 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/Scripts/pip3.11.exe
+-rwxr-xr-x   0        0        0   108409 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/Scripts/pip3.exe
+-rwxr-xr-x   0        0        0   270608 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/Scripts/python.exe
+-rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/Scripts/pythonw.exe
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/cfg/__init__.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/cfg/cli_commands.csv
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/cfg/sat_commands.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/__init__.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/cmd_parser.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/math_utils.py
+-rw-r--r--   0        0        0    19805 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/modem.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/packet_parser.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    24474 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7340 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18833 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0    10097 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    29497 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    17009 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    38902 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15832 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7893 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25965 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    19348 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20994 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18959 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    28417 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    28215 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    18424 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    33649 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    25328 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24728 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    19416 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    28575 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11834 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11980 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    22946 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7948 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18642 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    12053 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    23516 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    35547 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    86413 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16855 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   279760 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31660 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10293 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13762 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    37301 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    21019 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    26121 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    44880 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27293 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   109211 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0   102881 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0   102576 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   106012 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   133760 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   107154 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    99752 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    31052 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    15210 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13912 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10972 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    42375 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    53047 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    21342 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    53291 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    15204 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    40877 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    11178 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/scripts.py
+-rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/t32.exe
+-rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    68194 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/version.py
+-rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/w32.exe
+-rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    44980 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    50729 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    13350 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    46526 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   215139 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    35554 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30912 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   112748 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    18522 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    32947 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63340 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9418 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    41326 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    36592 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    22583 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19872 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11498 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    72109 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    54776 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   219158 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    40217 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    26101 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24327 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    22027 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    19121 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    36322 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    31011 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    34326 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    21058 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10547 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   143845 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    20401 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10679 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7318 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0   101828 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14648 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    12192 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10882 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    36846 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    61408 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24986 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27869 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    36103 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    40686 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    46832 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    30360 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    21101 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20872 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    40238 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    20323 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    31520 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17599 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    35369 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    18151 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    14319 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    35741 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22623 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17672 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     7116 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14731 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10921 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0    10681 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0    77077 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0   111864 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    25309 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/zipp.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    14040 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   136885 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    19108 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8800 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30912 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   219124 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    40217 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    26101 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24310 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0     8676 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_importlib.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_itertools.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_path.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_reqs.py
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/build_meta.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/cli-32.exe
+-rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/cli-64.exe
+-rwxr-xr-x   0        0        0   137216 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/cli-arm64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    21399 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/discovery.py
+-rw-r--r--   0        0        0    46800 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/glob.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/gui-32.exe
+-rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/gui-64.exe
+-rwxr-xr-x   0        0        0   137728 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/gui-arm64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/logging.py
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    49427 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    41146 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14878 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    15197 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    48589 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    18409 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    51472 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    18380 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8475 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    14084 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    31067 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    24297 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    19416 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    16042 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    18641 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    13310 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0        0        0     5598 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    22666 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    32345 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    16975 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    31035 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19772 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0    89445 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0        0        0    31177 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    14037 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    16116 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   121783 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30912 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   219124 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    40217 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    26101 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24310 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/build.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    16204 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0    14483 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    87974 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0        0        0    27558 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+-rw-r--r--   0        0        0    16781 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/expand.py
+-rw-r--r--   0        0        0    19797 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0        0        0    25960 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0        0        0   270934 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/METADATA
+-rw-r--r--   0        0        0    37694 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 kitsat-1.2.14/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 kitsat-1.2.14/LICENSE.md
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 kitsat-1.2.14/README.md
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 kitsat-1.2.14/pyproject.toml
+-rw-r--r--   0        0        0    42769 2020-02-02 00:00:00.000000 kitsat-1.2.14/PKG-INFO
```

### Comparing `kitsat-1.2.13/kitsat/kitsat_cli.py` & `kitsat-1.2.14/kitsat/kitsat_cli.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/Scripts/Activate.ps1` & `kitsat-1.2.14/kitsat/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/Scripts/activate` & `kitsat-1.2.14/kitsat/Scripts/activate`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/Scripts/activate.bat` & `kitsat-1.2.14/kitsat/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/Scripts/pip.exe` & `kitsat-1.2.14/kitsat/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/Scripts/pip3.11.exe` & `kitsat-1.2.14/kitsat/Scripts/pip3.11.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/Scripts/pip3.exe` & `kitsat-1.2.14/kitsat/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/Scripts/python.exe` & `kitsat-1.2.14/kitsat/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/Scripts/pythonw.exe` & `kitsat-1.2.14/kitsat/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/cfg/cli_commands.csv` & `kitsat-1.2.14/kitsat/cfg/cli_commands.csv`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/cfg/sat_commands.csv` & `kitsat-1.2.14/kitsat/cfg/sat_commands.csv`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/cmd_parser.py` & `kitsat-1.2.14/kitsat/lib/cmd_parser.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/math_utils.py` & `kitsat-1.2.14/kitsat/lib/math_utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/modem.py` & `kitsat-1.2.14/kitsat/lib/modem.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/packet_parser.py` & `kitsat-1.2.14/kitsat/lib/packet_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,9 +76,12 @@
                 data = parse_gps(data)
         elif orig == 5: #IMU
             if(cmd_id == 14):
                 data = parse_imu(data)
         elif orig == 8: # EPS
             if(cmd_id == 4):
                 data = parse_eps(data)
+        elif orig == 14: # Beacon
+            # TODO
+            pass
 
     return(data)
```

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/_distutils_hack/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/__main__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/__pip-runner__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/build_env.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cache.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/configuration.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/exceptions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/pyproject.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/self_outdated_check.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/wheel_builder.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/autocompletion.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/base_command.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/cmdoptions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/command_context.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/main.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/main_parser.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/parser.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/progress_bars.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/req_command.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/cli/spinners.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/cache.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/check.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/completion.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/configuration.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/debug.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/download.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/freeze.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/hash.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/help.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/index.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/inspect.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/install.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/list.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/search.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/show.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/uninstall.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/commands/wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/base.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/installed.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/sdist.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/distributions/wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/index/collector.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/index/package_finder.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/index/sources.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/locations/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/locations/_distutils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/locations/_sysconfig.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/locations/base.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/_json.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/base.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_dists.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_envs.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/candidate.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/direct_url.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/format_control.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/index.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/installation_report.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/link.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/scheme.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/search_scope.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/selection_prefs.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/target_python.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/models/wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/auth.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/cache.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/download.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/lazy_wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/session.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/utils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/network/xmlrpc.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/check.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/freeze.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/prepare.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/build_tracker.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/metadata.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/metadata_editable.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/wheel_editable.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/operations/install/wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/constructors.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/req_file.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/req_install.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/req_set.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/req/req_uninstall.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/base.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/_jaraco_text.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/_log.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/appdirs.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/deprecation.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/egg_link.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/encoding.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/entrypoints.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/filesystem.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/filetypes.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/glibc.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/hashes.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/inject_securetransport.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/logging.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/misc.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/models.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/packaging.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/setuptools_build.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/subprocess.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/temp_dir.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/unpacking.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/urls.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/virtualenv.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/utils/wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/bazaar.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/git.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/mercurial.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/subversion.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/six.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/typing_extensions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/certifi/cacert.pem` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/certifi/core.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/big5freq.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/big5prober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/enums.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/escprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/escsm.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/johabfreq.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/johabprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/macromanprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/utf1632prober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/ansi.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/initialise.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/win32.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/winterm.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/utils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/database.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/index.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/locators.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/manifest.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/markers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/metadata.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/resources.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/scripts.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/t32.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/t64-arm.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/t64.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/version.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/w32.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/w64-arm.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/w64.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distlib/wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distro/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/distro/distro.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/codec.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/core.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/idnadata.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/intranges.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/idna/uts46data.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/msgpack/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/msgpack/ext.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/msgpack/fallback.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/__about__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/_structures.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/markers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/requirements.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/specifiers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/tags.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/utils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/packaging/version.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/android.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/api.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/macos.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/unix.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/platformdirs/windows.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/cmdline.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/console.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/filter.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatter.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/lexer.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/modeline.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/plugin.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/regexopt.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/scanner.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/sphinxext.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/style.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/token.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/unistring.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/filters/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/groff.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/html.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/img.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/irc.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/latex.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/other.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/svg.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/python.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pygments/styles/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/actions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/common.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/core.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/exceptions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/helpers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/results.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/testing.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/unicode.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/adapters.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/api.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/auth.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/certs.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/cookies.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/exceptions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/help.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/hooks.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/models.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/packages.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/sessions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/status_codes.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/structures.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/requests/utils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/providers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/resolvelib/structs.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/__main__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_cell_widths.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_emoji_codes.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_emoji_replace.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_export_format.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_fileno.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_inspect.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_log_render.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_loop.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_null_file.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_palettes.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_ratio.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_spinners.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_win32_console.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_windows.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_windows_renderer.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/_wrap.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/abc.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/align.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/ansi.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/bar.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/box.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/cells.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/color.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/color_triplet.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/columns.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/console.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/constrain.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/containers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/control.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/default_styles.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/diagnose.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/emoji.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/errors.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/file_proxy.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/filesize.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/highlighter.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/json.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/jupyter.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/layout.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/live.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/live_render.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/logging.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/markup.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/measure.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/padding.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/pager.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/palette.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/panel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/pretty.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/progress.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/progress_bar.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/prompt.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/protocol.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/repr.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/rule.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/scope.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/screen.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/segment.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/spinner.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/status.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/style.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/styled.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/syntax.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/table.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/terminal_theme.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/text.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/theme.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/traceback.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/rich/tree.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/_utils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/after.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/before.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/nap.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/retry.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/stop.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tenacity/wait.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tomli/_parser.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/tomli/_re.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/_collections.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/connection.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/fields.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/filepost.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/request.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/response.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/queue.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/queue.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/request.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/response.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/url.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/labels.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/tests.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt` & `kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt` & `kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/METADATA` & `kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pip-23.1.2.dist-info/RECORD` & `kitsat-1.2.14/kitsat/lib/site-packages/pip-23.1.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/appdirs.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/zipp.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/context.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/markers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/tags.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/utils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/version.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/pkg_resources/extern/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_entry_points.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_imp.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_importlib.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_itertools.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_path.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_reqs.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_reqs.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/archive_util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/build_meta.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/cli-32.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/cli-64.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/cli-arm64.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/cli-arm64.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/cli.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/dep_util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/depends.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/discovery.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/dist.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/errors.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/extension.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/glob.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/gui-32.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/gui-64.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/gui-arm64.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/gui-arm64.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/gui.exe` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/installer.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/launch.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/logging.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/monkey.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/msvc.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/namespaces.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/package_index.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/sandbox.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/unicode_utils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/windows_support.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/_collections.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/_msvccompiler.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/archive_util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/bcppcompiler.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/ccompiler.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/cmd.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/config.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/core.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/cygwinccompiler.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/dep_util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/dir_util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/dist.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/errors.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/extension.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/fancy_getopt.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/file_util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/filelist.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/log.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/msvc9compiler.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/msvccompiler.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/py39compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/spawn.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/sysconfig.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/text_file.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/unixccompiler.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/version.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/versionpredicate.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/_framework_compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/bdist.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build_clib.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build_ext.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build_py.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/build_scripts.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/check.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/clean.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/config.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_data.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_egg_info.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_headers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_lib.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/install_scripts.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/py37compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/register.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/sdist.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_distutils/command/upload.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/ordered_set.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/typing_extensions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/zipp.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/jaraco/context.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/jaraco/functools.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/more.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/__about__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/_structures.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/markers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/requirements.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/specifiers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/tags.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/utils.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/packaging/version.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/actions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/common.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/core.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/results.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/testing.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/util.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/tomli/_parser.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/_vendor/tomli/_re.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/alias.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/bdist_egg.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/bdist_rpm.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/build.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/build_clib.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/build_ext.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/build_py.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/develop.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/dist_info.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/easy_install.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/editable_wheel.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/egg_info.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/install.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/install_egg_info.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/install_lib.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/install_scripts.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/launcher manifest.xml` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/py36compat.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/rotate.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/saveopts.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/sdist.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/setopt.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/command/upload_docs.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/expand.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/pyprojecttoml.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/setupcfg.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/formats.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools/extern/__init__.py` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/LICENSE` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/METADATA` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/RECORD` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt` & `kitsat-1.2.14/kitsat/lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/LICENSE.md` & `kitsat-1.2.14/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kitsat-1.2.13/README.md` & `kitsat-1.2.14/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,11 +47,12 @@
 print(mod.read())
 
 mod.disconnect()
 ```
 
 ## Contributors
  * Tuomas Simula - <tuomas@simu.la>
- * Samuli Nyman
+ * Tessa Nikander - <tessa@kitsat.fi>
+ * Samuli Nyman - <samuli@kitsat.fi>
 
 ## License
 [GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0)
```

### Comparing `kitsat-1.2.13/pyproject.toml` & `kitsat-1.2.14/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 [tool.hatch.build]
 include = [
   "kitsat/*"
 ]
 [project]
 name = "kitsat"
-version = "1.2.13"
+version = "1.2.14"
 authors = [
   { name="Tuomas Simula", email="tuomas@simu.la" }, { name="Samuli Nyman", email="samuli@kitsat.fi" },
   { name="Tessa Nikander", email="tessa@kitsat.fi" }
 ]
 description = "CLI and python library for communicating with the Kitsat educational satellite"
 readme = "README.md"
 license = {file = "LICENSE.md"}
```

### Comparing `kitsat-1.2.13/PKG-INFO` & `kitsat-1.2.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitsat
-Version: 1.2.13
+Version: 1.2.14
 Summary: CLI and python library for communicating with the Kitsat educational satellite
 Project-URL: Homepage, https://github.com/netnspace/Kitsat-Python-Library
 Author-email: Tuomas Simula <tuomas@simu.la>, Samuli Nyman <samuli@kitsat.fi>, Tessa Nikander <tessa@kitsat.fi>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -736,11 +736,12 @@
 print(mod.read())
 
 mod.disconnect()
 ```
 
 ## Contributors
  * Tuomas Simula - <tuomas@simu.la>
- * Samuli Nyman
+ * Tessa Nikander - <tessa@kitsat.fi>
+ * Samuli Nyman - <samuli@kitsat.fi>
 
 ## License
 [GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0)
```

