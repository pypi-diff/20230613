# Comparing `tmp/pdm-2.7.3.tar.gz` & `tmp/pdm-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.7.3.tar", last modified: Tue Jun 13 04:35:30 2023, max compression
+gzip compressed data, was "pdm-2.7.4.tar", last modified: Tue Jun 13 04:51:14 2023, max compression
```

## Comparing `pdm-2.7.3.tar` & `pdm-2.7.4.tar`

### file list

```diff
@@ -1,272 +1,272 @@
--rw-r--r--   0        0        0   124001 2023-06-13 04:35:18.115172 pdm-2.7.3/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-06-13 04:35:18.115172 pdm-2.7.3/LICENSE
--rw-r--r--   0        0        0     1075 2023-06-13 04:35:18.115172 pdm-2.7.3/LICENSE
--rw-r--r--   0        0        0     7986 2023-06-13 04:35:18.115172 pdm-2.7.3/README.md
--rw-r--r--   0        0        0     7986 2023-06-13 04:35:18.115172 pdm-2.7.3/README.md
--rw-r--r--   0        0        0     4396 2023-06-13 04:35:30.939237 pdm-2.7.3/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/__version__.py
--rw-r--r--   0        0        0     3282 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11850 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    14229 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     7095 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2657 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     4236 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6542 2023-06-13 04:35:18.119172 pdm-2.7.3/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     5812 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     3066 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     3689 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0     8612 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3589 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15754 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2196 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6596 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6782 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     4271 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15427 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9373 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     6898 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     6489 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1715 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2426 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6149 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      819 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1279 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2759 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5096 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    38130 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18583 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25158 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10461 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/options.py
--rw-r--r--   0        0        0    25081 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2226 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/compat.py
--rw-r--r--   0        0        0    10667 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8850 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/environments/base.py
--rw-r--r--   0        0        0     3560 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/environments/local.py
--rw-r--r--   0        0        0     1600 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1362 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1202 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5788 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2400 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7490 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7502 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2309 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1390 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10901 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18161 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10990 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     3162 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4698 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/models/backends.py
--rw-r--r--   0        0        0    11466 2023-06-13 04:35:18.123172 pdm-2.7.3/src/pdm/models/caches.py
--rw-r--r--   0        0        0    26568 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1845 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6323 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2195 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    21340 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    18726 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/search.py
--rw-r--r--   0        0        0     2426 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     1300 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5924 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2766 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16748 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/project/config.py
--rw-r--r--   0        0        0    26273 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/project/core.py
--rw-r--r--   0        0        0     2093 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/py.typed
--rw-r--r--   0        0        0    19876 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13119 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/signals.py
--rw-r--r--   0        0        0     8054 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/termui.py
--rw-r--r--   0        0        0    13866 2023-06-13 04:35:18.127173 pdm-2.7.3/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/__init__.py
--rw-r--r--   0        0        0     3723 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/conftest.py
--rw-r--r--   0        0        0    12362 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_add.py
--rw-r--r--   0        0        0     5799 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_cache.py
--rw-r--r--   0        0        0     9286 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4481 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_list.py
--rw-r--r--   0        0        0     6324 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7796 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_others.py
--rw-r--r--   0        0        0     6052 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3888 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_remove.py
--rw-r--r--   0        0        0    29259 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     8876 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_update.py
--rw-r--r--   0        0        0     2997 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_use.py
--rw-r--r--   0        0        0    10430 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.127173 pdm-2.7.3/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-06-13 04:35:18.131173 pdm-2.7.3/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-06-13 04:35:18.135172 pdm-2.7.3/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-06-13 04:35:18.135172 pdm-2.7.3/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-06-13 04:35:18.135172 pdm-2.7.3/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-06-13 04:35:18.135172 pdm-2.7.3/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-06-13 04:35:18.139172 pdm-2.7.3/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-06-13 04:35:18.143173 pdm-2.7.3/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-06-13 04:35:18.143173 pdm-2.7.3/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      574 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      728 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      332 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo/setup.py
--rw-r--r--   0        0        0       26 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1330 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/models/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/models/test_backends.py
--rw-r--r--   0        0        0    13344 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2556 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7704 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/test_integration.py
--rw-r--r--   0        0        0     3435 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/test_plugin.py
--rw-r--r--   0        0        0    12085 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/test_signals.py
--rw-r--r--   0        0        0     4419 2023-06-13 04:35:18.147173 pdm-2.7.3/tests/test_utils.py
--rw-r--r--   0        0        0     9611 1970-01-01 00:00:00.000000 pdm-2.7.3/PKG-INFO
+-rw-r--r--   0        0        0   124084 2023-06-13 04:51:05.335390 pdm-2.7.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-06-13 04:51:05.335390 pdm-2.7.4/LICENSE
+-rw-r--r--   0        0        0     1075 2023-06-13 04:51:05.335390 pdm-2.7.4/LICENSE
+-rw-r--r--   0        0        0     7986 2023-06-13 04:51:05.335390 pdm-2.7.4/README.md
+-rw-r--r--   0        0        0     7986 2023-06-13 04:51:05.335390 pdm-2.7.4/README.md
+-rw-r--r--   0        0        0     4396 2023-06-13 04:51:14.599513 pdm-2.7.4/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3282 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11850 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    14229 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     7095 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2857 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6542 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     5812 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     3066 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     3689 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0     8612 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3589 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15754 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2196 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6782 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     4271 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15427 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9373 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     6898 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     6489 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1715 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2426 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6149 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      819 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1279 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2759 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5096 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    38130 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18583 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25158 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10461 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/options.py
+-rw-r--r--   0        0        0    25081 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2226 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/compat.py
+-rw-r--r--   0        0        0    10667 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8850 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     3560 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1362 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1202 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2400 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7490 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7502 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2309 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1390 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10901 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18161 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10990 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4698 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    11466 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26568 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1845 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6323 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2195 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    21340 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18726 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/search.py
+-rw-r--r--   0        0        0     2426 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2766 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    16748 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26273 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2093 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/py.typed
+-rw-r--r--   0        0        0    19876 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     1954 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13119 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-06-13 04:51:05.347390 pdm-2.7.4/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-06-13 04:51:05.347390 pdm-2.7.4/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-06-13 04:51:05.347390 pdm-2.7.4/src/pdm/termui.py
+-rw-r--r--   0        0        0    13866 2023-06-13 04:51:05.347390 pdm-2.7.4/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12362 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5799 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4481 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6324 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6052 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3888 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29259 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     8876 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2997 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10430 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-06-13 04:51:05.355390 pdm-2.7.4/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-06-13 04:51:05.359390 pdm-2.7.4/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      574 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      728 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      332 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo/setup.py
+-rw-r--r--   0        0        0       26 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1330 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13344 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2556 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7704 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_plugin.py
+-rw-r--r--   0        0        0    12085 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_signals.py
+-rw-r--r--   0        0        0     4419 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_utils.py
+-rw-r--r--   0        0        0     9611 1970-01-01 00:00:00.000000 pdm-2.7.4/PKG-INFO
```

### Comparing `pdm-2.7.3/CHANGELOG.md` & `pdm-2.7.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Release v2.7.4 (2023-06-13)
+---------------------------
+
+No significant changes.
+
+
 Release v2.7.3 (2023-06-13)
 ---------------------------
 
 ### Bug Fixes
 
 - Fix the warning of extras not found due to extra names not normalized. [#2006](https://github.com/pdm-project/pdm/issues/2006)
 - Pop up a warning when the deprecated `parser` argument is passed to `BaseCommand.__init__()` method. [#2007](https://github.com/pdm-project/pdm/issues/2007)
```

### Comparing `pdm-2.7.3/LICENSE` & `pdm-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/README.md` & `pdm-2.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/pyproject.toml` & `pdm-2.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.7.3"
+version = "2.7.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
```

### Comparing `pdm-2.7.3/src/pdm/_types.py` & `pdm-2.7.4/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/builders/base.py` & `pdm-2.7.4/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/builders/editable.py` & `pdm-2.7.4/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/builders/sdist.py` & `pdm-2.7.4/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/builders/wheel.py` & `pdm-2.7.4/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/actions.py` & `pdm-2.7.4/src/pdm/cli/actions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/add.py` & `pdm-2.7.4/src/pdm/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/base.py` & `pdm-2.7.4/src/pdm/cli/commands/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,18 +19,21 @@
     name: str | None = None
     # The subcommand's help string, if not given, __doc__ will be used.
     description: str | None = None
     # A list of pre-defined options which will be loaded on initializing
     # Rewrite this if you don't want the default ones
     arguments: list[Option] = [verbose_option, global_option, project_option]
 
+    def __init__(self, parser: argparse.ArgumentParser | None = None) -> None:
+        """For compatibility, the parser is optional and won't be used."""
+
     @classmethod
     def init_parser(cls: type[C], parser: argparse.ArgumentParser) -> C:
         args = inspect.signature(cls).parameters
-        if "parser" in args:
+        if "parser" in args and args["parser"].default is inspect._empty:
             deprecation_warning(
                 f"The `parser` argument of `{cls.__name__}.__init__()` is deprecated. It won't be used."
             )
             cmd = cls(parser)  # type: ignore[call-arg]
         else:
             cmd = cls()
         for arg in cmd.arguments:
```

### Comparing `pdm-2.7.3/src/pdm/cli/commands/build.py` & `pdm-2.7.4/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/cache.py` & `pdm-2.7.4/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/completion.py` & `pdm-2.7.4/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/config.py` & `pdm-2.7.4/src/pdm/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/export.py` & `pdm-2.7.4/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.7.4/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.7.4/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/import_cmd.py` & `pdm-2.7.4/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/info.py` & `pdm-2.7.4/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/init.py` & `pdm-2.7.4/src/pdm/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/install.py` & `pdm-2.7.4/src/pdm/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/list.py` & `pdm-2.7.4/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/lock.py` & `pdm-2.7.4/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.7.4/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/publish/package.py` & `pdm-2.7.4/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/publish/repository.py` & `pdm-2.7.4/src/pdm/cli/commands/publish/repository.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/remove.py` & `pdm-2.7.4/src/pdm/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/run.py` & `pdm-2.7.4/src/pdm/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/search.py` & `pdm-2.7.4/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/self_cmd.py` & `pdm-2.7.4/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/show.py` & `pdm-2.7.4/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/sync.py` & `pdm-2.7.4/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/update.py` & `pdm-2.7.4/src/pdm/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/use.py` & `pdm-2.7.4/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.7.4/src/pdm/cli/commands/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/venv/activate.py` & `pdm-2.7.4/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/venv/backends.py` & `pdm-2.7.4/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/venv/create.py` & `pdm-2.7.4/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/venv/list.py` & `pdm-2.7.4/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/venv/purge.py` & `pdm-2.7.4/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/venv/remove.py` & `pdm-2.7.4/src/pdm/cli/commands/venv/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/commands/venv/utils.py` & `pdm-2.7.4/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/completions/pdm.bash` & `pdm-2.7.4/src/pdm/cli/completions/pdm.bash`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/completions/pdm.fish` & `pdm-2.7.4/src/pdm/cli/completions/pdm.fish`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/completions/pdm.ps1` & `pdm-2.7.4/src/pdm/cli/completions/pdm.ps1`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/completions/pdm.zsh` & `pdm-2.7.4/src/pdm/cli/completions/pdm.zsh`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/filters.py` & `pdm-2.7.4/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/hooks.py` & `pdm-2.7.4/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/options.py` & `pdm-2.7.4/src/pdm/cli/options.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/cli/utils.py` & `pdm-2.7.4/src/pdm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/compat.py` & `pdm-2.7.4/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/core.py` & `pdm-2.7.4/src/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/environments/__init__.py` & `pdm-2.7.4/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/environments/base.py` & `pdm-2.7.4/src/pdm/environments/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/environments/local.py` & `pdm-2.7.4/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/environments/python.py` & `pdm-2.7.4/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/exceptions.py` & `pdm-2.7.4/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/formats/__init__.py` & `pdm-2.7.4/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/formats/base.py` & `pdm-2.7.4/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/formats/flit.py` & `pdm-2.7.4/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/formats/pipfile.py` & `pdm-2.7.4/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/formats/poetry.py` & `pdm-2.7.4/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/formats/requirements.py` & `pdm-2.7.4/src/pdm/formats/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/formats/setup_py.py` & `pdm-2.7.4/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/installers/core.py` & `pdm-2.7.4/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/installers/installers.py` & `pdm-2.7.4/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/installers/manager.py` & `pdm-2.7.4/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/installers/packages.py` & `pdm-2.7.4/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/installers/synchronizers.py` & `pdm-2.7.4/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/installers/uninstallers.py` & `pdm-2.7.4/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/auth.py` & `pdm-2.7.4/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/backends.py` & `pdm-2.7.4/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/caches.py` & `pdm-2.7.4/src/pdm/models/caches.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/candidates.py` & `pdm-2.7.4/src/pdm/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/in_process/__init__.py` & `pdm-2.7.4/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.7.4/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/in_process/parse_setup.py` & `pdm-2.7.4/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/in_process/pep508.py` & `pdm-2.7.4/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.7.4/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/markers.py` & `pdm-2.7.4/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/project_info.py` & `pdm-2.7.4/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/python.py` & `pdm-2.7.4/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/repositories.py` & `pdm-2.7.4/src/pdm/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/requirements.py` & `pdm-2.7.4/src/pdm/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/search.py` & `pdm-2.7.4/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/session.py` & `pdm-2.7.4/src/pdm/models/session.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/setup.py` & `pdm-2.7.4/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/specifiers.py` & `pdm-2.7.4/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/venv.py` & `pdm-2.7.4/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/versions.py` & `pdm-2.7.4/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/models/working_set.py` & `pdm-2.7.4/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/pep582/sitecustomize.py` & `pdm-2.7.4/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/project/config.py` & `pdm-2.7.4/src/pdm/project/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/project/core.py` & `pdm-2.7.4/src/pdm/project/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/project/lockfile.py` & `pdm-2.7.4/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/project/project_file.py` & `pdm-2.7.4/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/project/toml_file.py` & `pdm-2.7.4/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/pytest.py` & `pdm-2.7.4/src/pdm/pytest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/resolver/core.py` & `pdm-2.7.4/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/resolver/providers.py` & `pdm-2.7.4/src/pdm/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/resolver/python.py` & `pdm-2.7.4/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/resolver/reporters.py` & `pdm-2.7.4/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/signals.py` & `pdm-2.7.4/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/termui.py` & `pdm-2.7.4/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/src/pdm/utils.py` & `pdm-2.7.4/src/pdm/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/conftest.py` & `pdm-2.7.4/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_add.py` & `pdm-2.7.4/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_build.py` & `pdm-2.7.4/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_cache.py` & `pdm-2.7.4/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_config.py` & `pdm-2.7.4/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_fix.py` & `pdm-2.7.4/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_hooks.py` & `pdm-2.7.4/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_init.py` & `pdm-2.7.4/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_install.py` & `pdm-2.7.4/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_list.py` & `pdm-2.7.4/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_lock.py` & `pdm-2.7.4/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_others.py` & `pdm-2.7.4/tests/cli/test_others.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_publish.py` & `pdm-2.7.4/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_remove.py` & `pdm-2.7.4/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_run.py` & `pdm-2.7.4/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_self_command.py` & `pdm-2.7.4/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_update.py` & `pdm-2.7.4/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_use.py` & `pdm-2.7.4/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/cli/test_venv.py` & `pdm-2.7.4/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/conftest.py` & `pdm-2.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.7.4/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.7.4/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.7.4/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.7.4/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.7.4/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.7.4/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.7.4/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.7.4/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.7.4/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.7.4/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.7.4/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/pypi.json` & `pdm-2.7.4/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/fixtures/pyproject.toml` & `pdm-2.7.4/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/models/test_backends.py` & `pdm-2.7.4/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/models/test_candidates.py` & `pdm-2.7.4/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/models/test_marker.py` & `pdm-2.7.4/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/models/test_requirements.py` & `pdm-2.7.4/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/models/test_setup_parsing.py` & `pdm-2.7.4/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/models/test_specifiers.py` & `pdm-2.7.4/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/models/test_versions.py` & `pdm-2.7.4/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/resolver/test_resolve.py` & `pdm-2.7.4/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/test_formats.py` & `pdm-2.7.4/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/test_installer.py` & `pdm-2.7.4/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/test_integration.py` & `pdm-2.7.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/test_plugin.py` & `pdm-2.7.4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/test_project.py` & `pdm-2.7.4/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/test_signals.py` & `pdm-2.7.4/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/tests/test_utils.py` & `pdm-2.7.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.3/PKG-INFO` & `pdm-2.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.7.3
+Version: 2.7.4
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.7.3 Summary: A modern Python package
+Metadata-Version: 2.1 Name: pdm Version: 2.7.4 Summary: A modern Python package
 and dependency manager supporting the latest PEP standards Keywords: packaging
 dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

