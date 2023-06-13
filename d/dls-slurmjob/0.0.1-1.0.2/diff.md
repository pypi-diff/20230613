# Comparing `tmp/dls-slurmjob-0.0.1.tar.gz` & `tmp/dls-slurmjob-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-slurmjob-0.0.1.tar", last modified: Tue Jun 13 05:42:22 2023, max compression
+gzip compressed data, was "dls-slurmjob-1.0.2.tar", last modified: Tue Jun 13 13:16:30 2023, max compression
```

## Comparing `dls-slurmjob-0.0.1.tar` & `dls-slurmjob-1.0.2.tar`

### file list

```diff
@@ -1,134 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.943910 dls-slurmjob-0.0.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.943910 dls-slurmjob-0.0.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.943910 dls-slurmjob-0.0.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.943910 dls-slurmjob-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.939910 dls-slurmjob-0.0.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.943910 dls-slurmjob-0.0.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.943910 dls-slurmjob-0.0.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.947910 dls-slurmjob-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.947910 dls-slurmjob-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.947910 dls-slurmjob-0.0.1/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/configurations/dummy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.947910 dls-slurmjob-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.939910 dls-slurmjob-0.0.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.947910 dls-slurmjob-0.0.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.947910 dls-slurmjob-0.0.1/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/explanations/slurm_openapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.947910 dls-slurmjob-0.0.1/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.947910 dls-slurmjob-0.0.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.947910 dls-slurmjob-0.0.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.951910 dls-slurmjob-0.0.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.943910 dls-slurmjob-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.951910 dls-slurmjob-0.0.1/src/dls_slurmjob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-06-13 05:42:22.000000 dls-slurmjob-0.0.1/src/dls_slurmjob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-13 05:42:22.000000 dls-slurmjob-0.0.1/src/dls_slurmjob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:42:22.000000 dls-slurmjob-0.0.1/src/dls_slurmjob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 05:42:22.000000 dls-slurmjob-0.0.1/src/dls_slurmjob.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 05:42:22.000000 dls-slurmjob-0.0.1/src/dls_slurmjob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 05:42:22.000000 dls-slurmjob-0.0.1/src/dls_slurmjob.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.951910 dls-slurmjob-0.0.1/src/dls_slurmjob_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.951910 dls-slurmjob-0.0.1/src/dls_slurmjob_api/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/interfaces/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.951910 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/job_summary_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.951910 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.951910 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/dbv0/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/dbv0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75101 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/dbv0/field_0.py
--rw-r--r--   0 runner    (1001) docker     (123)   531009 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/openapi.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.951910 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/v0/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109493 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/v0/field_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/restds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/src/dls_slurmjob_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/src/dls_slurmjob_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_cli/subcommands/query_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_cli/subcommands/submit_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/src/dls_slurmjob_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 05:42:22.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/src/dls_slurmjob_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/tests/configurations/dummy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:42:22.955910 dls-slurmjob-0.0.1/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/tests/scripts/hello.sh
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/tests/scripts/hello1.json
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/tests/scripts/hello2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-13 05:42:13.000000 dls-slurmjob-0.0.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.794449 dls-slurmjob-1.0.2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/configurations/dummy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.794449 dls-slurmjob-1.0.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/slurm_openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/interfaces/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/job_summary_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/dbv0/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/dbv0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75101 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/dbv0/field_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)   531009 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/openapi.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109493 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/v0/field_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/restds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/query_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/submit_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/configurations/dummy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello_bxflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello_bxflow.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/test_cli.py
```

### Comparing `dls-slurmjob-0.0.1/.dae-devops/Makefile` & `dls-slurmjob-1.0.2/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.dae-devops/docs/conventions.rst` & `dls-slurmjob-1.0.2/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.dae-devops/docs/developing.rst` & `dls-slurmjob-1.0.2/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.dae-devops/docs/devops.rst` & `dls-slurmjob-1.0.2/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.dae-devops/docs/docs_structure.rst` & `dls-slurmjob-1.0.2/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.dae-devops/docs/documenting.rst` & `dls-slurmjob-1.0.2/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.dae-devops/docs/installing.rst` & `dls-slurmjob-1.0.2/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.dae-devops/docs/testing.rst` & `dls-slurmjob-1.0.2/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.dae-devops/project.yaml` & `dls-slurmjob-1.0.2/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.devcontainer/Dockerfile` & `dls-slurmjob-1.0.2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.devcontainer/devcontainer.json` & `dls-slurmjob-1.0.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.github/CONTRIBUTING.rst` & `dls-slurmjob-1.0.2/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.github/actions/install_requirements/action.yml` & `dls-slurmjob-1.0.2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.github/dependabot.yml` & `dls-slurmjob-1.0.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.github/pages/index.html` & `dls-slurmjob-1.0.2/.github/pages/index.html`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.github/pages/make_switcher.py` & `dls-slurmjob-1.0.2/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.github/workflows/code.yml` & `dls-slurmjob-1.0.2/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.github/workflows/docs.yml` & `dls-slurmjob-1.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.github/workflows/docs_clean.yml` & `dls-slurmjob-1.0.2/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.github/workflows/linkcheck.yml` & `dls-slurmjob-1.0.2/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.gitignore` & `dls-slurmjob-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.gitlab-ci.yml` & `dls-slurmjob-1.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/.vscode/launch.json` & `dls-slurmjob-1.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/LICENSE` & `dls-slurmjob-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/PKG-INFO` & `dls-slurmjob-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-slurmjob
-Version: 0.0.1
+Version: 1.0.2
 Summary: Simplified job submit and status using Slurm REST.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-slurmjob-0.0.1/docs/conf.py` & `dls-slurmjob-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/docs/explanations/slurm_openapi.rst` & `dls-slurmjob-1.0.2/docs/explanations/slurm_openapi.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 OPENAPI
 =======================================================================
 
-The slurmrestd server conforms to OpenAPI.
+The slurmrestd server claims to conform to OpenAPI.
 
 To turn the OpenAPI schemas into pydantic models do these steps::
 
     $ export SLURM_JWT=<your token>
     $ curl -s -H X-SLURM-USER-NAME:${USER} -H X-SLURM-USER-TOKEN:${SLURM_JWT} -H "Content-Type: application/json" -X GET https://slurm-rest.diamond.ac.uk:8443/openapi/ > src/dls_slurmjob_api/models/openapi/openapi.json
     $ pip install datamodel-code-generator
     $ datamodel-codegen --input src/dls_slurmjob_api/models/openapi/openapi.json --input-file-type=openapi --force-optional --target-python-version=3.10 --output src/dls_slurmjob_api/models/openapi
```

### Comparing `dls-slurmjob-0.0.1/docs/images/dls-favicon.ico` & `dls-slurmjob-1.0.2/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/docs/images/dls-logo.svg` & `dls-slurmjob-1.0.2/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/pyproject.toml` & `dls-slurmjob-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 name = "dls-slurmjob"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
 ]
 description = "Simplified job submit and status using Slurm REST."
-dependencies = ["dls_mainiac", "dls_multiconf", "dls_normsql", "dls_utilpack", "aiohttp", "pydantic"]
+dependencies = ["dls_mainiac", "dls_multiconf", "dls_utilpack", "aiohttp", "pydantic"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.md"
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
@@ -96,8 +96,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 37a4d952a31722f99663f202e2ffb40e
+# dae_devops_fingerprint c93b5329a8dea01174b8b2fed54f9d11
```

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob.egg-info/PKG-INFO` & `dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-slurmjob
-Version: 0.0.1
+Version: 1.0.2
 Summary: Simplified job submit and status using Slurm REST.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob.egg-info/SOURCES.txt` & `dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -91,8 +91,10 @@
 tests/__init__.py
 tests/base_tester.py
 tests/conftest.py
 tests/test_cli.py
 tests/configurations/dummy.yaml
 tests/scripts/hello.sh
 tests/scripts/hello1.json
-tests/scripts/hello2.json
+tests/scripts/hello2.json
+tests/scripts/hello_bxflow.json
+tests/scripts/hello_bxflow.sh
```

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/aiohttp_client.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/interfaces/client.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/interfaces/client.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/job_summary_model.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/job_summary_model.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/dbv0/field_0.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/dbv0/field_0.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/openapi.json` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/openapi.json`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/models/openapi/v0/field_0.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/v0/field_0.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/aiohttp.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/aiohttp.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from dls_utilpack.callsign import callsign
 from dls_utilpack.describe import describe
 
 # Class for an aiohttp client.
 from dls_slurmjob_api.aiohttp_client import AiohttpClient
 
+# Job rejected by slurm engine, for example missing some required property.
+from dls_slurmjob_api.exceptions import Rejected
+
 # Client interface.
 from dls_slurmjob_api.interfaces.client import Interface
 
 # Job info.
 from dls_slurmjob_api.models.job_summary_model import JobSummaryModel
 from dls_slurmjob_api.models.openapi.v0.field_0 import (
     Field38JobProperties as OpenapiJobProperties,
@@ -81,19 +84,15 @@
         is_client_connection_possible = await self.is_client_connection_possible()
 
         if not is_client_connection_possible:
             raise RuntimeError(
                 f"{callsign(self)} no client connection possible to slurm server"
             )
 
-        # Make CSV of jobs and put in the url.
-        # In practice, slurmrestd seems to ignore this and always returns all jobs anyway.
-        job_ids_csv = ",".join(str(job_id) for job_id in job_ids)
-
-        url = f"jobs?job_ids={job_ids_csv}"
+        url = "jobs"
 
         logger.debug(f"{callsign(self)} client connection seems possible for {url}")
 
         # Talk to the slurmrestd server.
         response = await self.client_get(url)
 
         if "jobs" not in response:
@@ -161,56 +160,55 @@
         is_client_connection_possible = await self.is_client_connection_possible()
 
         if not is_client_connection_possible:
             raise RuntimeError(
                 f"{callsign(self)} no client connection possible to slurm server"
             )
 
-        with open(script_filename, "r") as script_stream:
-            script_contents = script_stream.read()
-
         properties.oversubscribe = None
 
         submission_model = OpenapiJobSubmission(
-            script=script_contents,
+            script=f"#!/bin/bash\nsource {script_filename}\n",
             job=properties,
             jobs=None,
         )
 
         submission_dict = submission_model.dict(exclude_none=True)
         submission_json = json.dumps(
             submission_dict,
             indent=4,
         )
 
         url = "job/submit"
 
         logger.debug(
-            f"{callsign(self)} client connection seems possible for {url}\n{submission_json}"
+            f"[SLRMSUB] {callsign(self)} client connection seems possible for {url}\n{submission_json}"
         )
 
         # Talk to the slurmrestd server.
         response_dict = await self.client_post(
             url, json=submission_dict, read_until_eof=False
         )
 
-        logger.debug(describe("job submit response", response_dict))
+        logger.debug(
+            describe(f"[SLRMSUB] {callsign(self)} job submit response", response_dict)
+        )
 
         # Check the response.
         jsr = OpenapiJobSubmissionResponse(**response_dict)
 
         if jsr.errors is not None and len(jsr.errors) > 0:
             error = jsr.errors[0]
             error_number = error.error_number
             # TODO: Figure out why the 0.0.38 spec says error_number, but the server is giving error_code instead.
             if error_number is None:
                 error_number = response_dict.get("errors")[0].get(
                     "error_code", "unknown"
                 )
-            raise RuntimeError(
+            raise Rejected(
                 f"{callsign(self)} slurmrestd error {error_number}: {error.error}"
             )
 
         logger.debug(
             f"{callsign(self)} submitted job_id {jsr.job_id}: {jsr.job_submit_user_msg}"
         )
```

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/context.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/context.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/dummy.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/dummy.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_api/restds/restds.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/restds.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_cli/main.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_cli/subcommands/base.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_cli/subcommands/query_jobs.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/query_jobs.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_cli/subcommands/submit_job.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/submit_job.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_cli/version.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_lib/__main__.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_lib/envvar.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/src/dls_slurmjob_lib/version.py` & `dls-slurmjob-1.0.2/src/dls_slurmjob_lib/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 When a string, it comes from the package __version__.
 When a dict, it also has __version__,
 as well as versions of other depdency packages.
 """
 
 from typing import Optional
 
-import dls_mainiac_lib.version
-import dls_normsql.version
-import dls_utilpack.version
-
 from dls_slurmjob_lib import __version__ as dls_slurmjob_lib_version
 
 
 # ----------------------------------------------------------
 def version() -> str:
     """
     Version of the dls_normsql package as a string.
@@ -30,24 +26,42 @@
     Returns version information from the dls_normsql package
     and its dependencies as a dict.
     Adds version information to a given meta dict if it was provided.
     """
 
     meta = {}
     meta["dls_slurmjob_lib"] = version()
-    meta.update(dls_mainiac_lib.version.meta())
-    meta.update(dls_normsql.version.meta())
-    meta.update(dls_utilpack.version.meta())
 
     try:
-        import setproctitle
+        import dls_utilpack.version
+
+        meta.update(dls_utilpack.version.meta())
+    except Exception:
+        meta["dls_utilpack"] = "unavailable"
+
+    try:
+        import dls_mainiac_lib.version
+
+        meta.update(dls_mainiac_lib.version.meta())
+    except Exception:
+        meta["dls_mainiac_lib"] = "unavailable"
+
+    try:
+        import dls_multiconf_lib.version
+
+        meta.update(dls_multiconf_lib.version.meta())
+    except Exception:
+        meta["dls_multiconf_lib"] = "unavailable"
+
+    try:
+        import aiohttp
 
-        setproctitle.__version__
-        meta["setproctitle"] = setproctitle.__version__
+        aiohttp.__version__
+        meta["aiohttp"] = aiohttp.__version__
     except Exception:
-        meta["setproctitle"] = "unavailable"
+        meta["aiohttp"] = "unavailable"
 
     if given_meta is not None:
         given_meta.update(meta)
     else:
         given_meta = meta
     return given_meta
```

### Comparing `dls-slurmjob-0.0.1/tests/base_tester.py` & `dls-slurmjob-1.0.2/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/tests/conftest.py` & `dls-slurmjob-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-0.0.1/tests/test_cli.py` & `dls-slurmjob-1.0.2/tests/test_cli.py`

 * *Files identical despite different names*

