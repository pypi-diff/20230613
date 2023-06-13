# Comparing `tmp/dvc-3.0.0a1.tar.gz` & `tmp/dvc-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-3.0.0a1.tar", last modified: Thu May 25 10:51:41 2023, max compression
+gzip compressed data, was "dvc-3.0.0a2.tar", last modified: Wed Jun  7 06:07:19 2023, max compression
```

## Comparing `dvc-3.0.0a1.tar` & `dvc-3.0.0a2.tar`

### file list

```diff
@@ -1,687 +1,684 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.021571 dvc-3.0.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.877570 dvc-3.0.0a1/.dvc/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.dvc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.dvc/config
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.dvcignore
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.881569 dvc-3.0.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.881569 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/epic_story.md
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.881569 dvc-3.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/packages.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/plugin_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-05-25 10:51:20.000000 dvc-3.0.0a1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-25 10:51:20.000000 dvc-3.0.0a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-25 10:51:20.000000 dvc-3.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-05-25 10:51:41.021571 dvc-3.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-05-25 10:51:20.000000 dvc-3.0.0a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.889570 dvc-3.0.0a1/dvc/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc/_dvc_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.889570 dvc-3.0.0a1/dvc/api/
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9452 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    11606 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     2089 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cachemgr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.889570 dvc-3.0.0a1/dvc/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     7647 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.897570 dvc-3.0.0a1/dvc/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.901570 dvc-3.0.0a1/dvc/commands/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/exec_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3481 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/install.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.901570 dvc-3.0.0a1/dvc/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/ls/ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/params.py
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.901570 dvc-3.0.0a1/dvc/commands/queue/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/kill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/start.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/stop.py
--rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/repro.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/compare.py
--rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    10948 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dagascii.py
--rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/data_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)     2962 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dependency/param.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dependency/repo.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    12574 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      673 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/env.py
--rw-r--r--   0 runner    (1001) docker     (122)    10279 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/fs/
--rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    13720 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/git.py
--rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     4990 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/machine/
--rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/machine/backend/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/machine/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/machine/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/machine/backend/terraform.py
--rw-r--r--   0 runner    (1001) docker     (122)    44224 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)    15488 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/parsing/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/parsing/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/render/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.909570 dvc-3.0.0a1/dvc/render/converter/
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/converter/image.py
--rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/converter/vega.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/match.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.913570 dvc-3.0.0a1/dvc/repo/
--rw-r--r--   0 runner    (1001) docker     (122)    18486 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9293 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/brancher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6613 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.917570 dvc-3.0.0a1/dvc/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/brancher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25405 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/executor/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7923 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/executor/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/executor/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/push.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24548 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    23073 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6834 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8879 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/refs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     6331 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     6759 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/stash.py
--rw-r--r--   0 runner    (1001) docker     (122)    24913 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/fetch.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/get.py
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      233 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4121 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)    20412 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/index.py
--rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      818 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/ls_url.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/metrics/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/metrics/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     8225 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/open_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/params/
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/params/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/params/show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)    17028 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/plots/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     7288 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/trie.py
--rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    14157 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/worktree.py
--rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     4303 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.925570 dvc-3.0.0a1/dvc/stage/
--rw-r--r--   0 runner    (1001) docker     (122)    24877 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9042 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     7439 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/params.py
--rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6907 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)     8604 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.925570 dvc-3.0.0a1/dvc/testing/
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4088 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/api_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.929570 dvc-3.0.0a1/dvc/testing/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.929570 dvc-3.0.0a1/dvc/testing/benchmarks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.929570 dvc-3.0.0a1/dvc/testing/benchmarks/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.933570 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_exp_show.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_help.py
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_push.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.933570 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/test_modify_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.933570 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/use_cases/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/path_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/remote_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/tmp_dir.py
--rw-r--r--   0 runner    (1001) docker     (122)    13091 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/workspace_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.933570 dvc-3.0.0a1/dvc/ui/
--rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ui/_rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ui/pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ui/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     5385 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.937570 dvc-3.0.0a1/dvc/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 10:51:24.000000 dvc-3.0.0a1/dvc/utils/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     5226 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/pkg.py
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.937570 dvc-3.0.0a1/dvc/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)      984 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_py.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.889570 dvc-3.0.0a1/dvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17149 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9367 2023-05-25 10:51:20.000000 dvc-3.0.0a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.937570 dvc-3.0.0a1/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/build-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/build.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      231 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/build_package.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.941570 dvc-3.0.0a1/scripts/fpm/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/after-install.sh
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/after-remove.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/notarize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.941570 dvc-3.0.0a1/scripts/innosetup/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/addSymLinkPermissions.ps1
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/addsymlink.iss
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/build.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/dvc.ico.dvc
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/dvc_left.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/dvc_up.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/modpath.iss
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/setup.iss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.941570 dvc-3.0.0a1/scripts/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/build.py
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.945570 dvc-3.0.0a1/scripts/pyinstaller/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-asyncssh.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.system.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc_task.py
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-fsspec.py
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-pydrive2.py
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/sign.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 10:51:41.021571 dvc-3.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.945570 dvc-3.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7176 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/dir_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6885 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/artifacts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/artifacts/test_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/data/db/test_index.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.961570 dvc-3.0.0a1/tests/func/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.961570 dvc-3.0.0a1/tests/func/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/executor/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    26233 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)    13387 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4928 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_save.py
--rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_set_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_stash_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.961570 dvc-3.0.0a1/tests/func/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/machine/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/machine/test_machine_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/machine/test_machine_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.961570 dvc-3.0.0a1/tests/func/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7112 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/metrics/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/metrics/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/func/params/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8152 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/params/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     6928 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/params/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/func/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10114 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    15835 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/test_foreach.py
--rw-r--r--   0 runner    (1001) docker     (122)     9670 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/test_interpolated_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/test_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/func/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/plots/test_modify.py
--rw-r--r--   0 runner    (1001) docker     (122)    12871 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/plots/test_show.py
--rw-r--r--   0 runner    (1001) docker     (122)    35171 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    26547 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     8797 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    16745 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_data_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    18824 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    12248 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     7554 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_external_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)    14728 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)     7625 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     5558 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     5057 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    17854 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_merge_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5734 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_move.py
--rw-r--r--   0 runner    (1001) docker     (122)     5936 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_odb.py
--rw-r--r--   0 runner    (1001) docker     (122)    15547 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)    10062 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (122)    34947 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)    13819 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_repro_multistage.py
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_root.py
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_run_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)    11484 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_run_multistage.py
--rw-r--r--   0 runner    (1001) docker     (122)    16626 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_run_single_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     9662 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)    14749 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_stage_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5156 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)    14335 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_used_objs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_virtual_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/func/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/utils/test_hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/utils/test_strict_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.969570 dvc-3.0.0a1/tests/integration/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/plots/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    13779 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/plots/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/plots/test_repo_plots_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/test_studio_live_experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.969570 dvc-3.0.0a1/tests/remotes/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.969570 dvc-3.0.0a1/tests/remotes/git-init/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/git_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/user.key
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/user.key.pub
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes_env.sample
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.977570 dvc-3.0.0a1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.981570 dvc-3.0.0a1/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/cli/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.985571 dvc-3.0.0a1/tests/unit/command/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.985571 dvc-3.0.0a1/tests/unit/command/ls/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/ls/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/ls/test_ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_compat_flag.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)    11210 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    11627 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4010 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.985571 dvc-3.0.0a1/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.989570 dvc-3.0.0a1/tests/unit/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/data/db/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.989570 dvc-3.0.0a1/tests/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/dependency/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/dependency/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.993570 dvc-3.0.0a1/tests/unit/fs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    19085 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_dvc_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.997571 dvc-3.0.0a1/tests/unit/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.997571 dvc-3.0.0a1/tests/unit/output/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/test_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/test_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/test_output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.001571 dvc-3.0.0a1/tests/unit/remote/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/test_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/test_webdav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/test_webhdfs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.001571 dvc-3.0.0a1/tests/unit/render/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/test_image_converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/test_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/test_vega_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.005571 dvc-3.0.0a1/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.005571 dvc-3.0.0a1/tests/unit/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.005571 dvc-3.0.0a1/tests/unit/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/queue/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/queue/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/test_executor_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.005571 dvc-3.0.0a1/tests/unit/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_open_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_scm_context.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.009571 dvc-3.0.0a1/tests/unit/scm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/scm/test_scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.009571 dvc-3.0.0a1/tests/unit/stage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5924 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     8626 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_loader_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_serialize_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_serialize_pipeline_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_hashinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     8869 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_tabular_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.013571 dvc-3.0.0a1/tests/unit/ui/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/ui/test_console.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/ui/test_pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/ui/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.017571 dvc-3.0.0a1/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.021571 dvc-3.0.0a1/tests/unit/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/serialize/test_python.py
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/serialize/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/serialize/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     5635 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.021571 dvc-3.0.0a1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      593 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.994876 dvc-3.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.858869 dvc-3.0.0a2/.dvc/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.dvc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.dvc/config
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.dvcignore
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.858869 dvc-3.0.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.858869 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/epic_story.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.858869 dvc-3.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/packages.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/plugin_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-07 06:07:00.000000 dvc-3.0.0a2/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-07 06:07:00.000000 dvc-3.0.0a2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-07 06:07:00.000000 dvc-3.0.0a2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-07 06:07:00.000000 dvc-3.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-06-07 06:07:19.994876 dvc-3.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-06-07 06:07:00.000000 dvc-3.0.0a2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.862869 dvc-3.0.0a2/dvc/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc/_dvc_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.866870 dvc-3.0.0a2/dvc/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9452 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11606 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/api/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2089 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cachemgr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.866870 dvc-3.0.0a2/dvc/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     7647 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.874870 dvc-3.0.0a2/dvc/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3963 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.878870 dvc-3.0.0a2/dvc/commands/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/exec_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3481 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/install.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.878870 dvc-3.0.0a2/dvc/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/ls/ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.878870 dvc-3.0.0a2/dvc/commands/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/kill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/start.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/queue/stop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10948 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dagascii.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/data_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.882870 dvc-3.0.0a2/dvc/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dependency/param.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dependency/repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10109 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.882870 dvc-3.0.0a2/dvc/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13922 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/fs/git.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4990 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.882870 dvc-3.0.0a2/dvc/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.882870 dvc-3.0.0a2/dvc/machine/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/machine/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/machine/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/machine/backend/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43972 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.886870 dvc-3.0.0a2/dvc/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)    13884 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/parsing/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/parsing/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.886870 dvc-3.0.0a2/dvc/render/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.886870 dvc-3.0.0a2/dvc/render/converter/
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/converter/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/converter/vega.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/render/match.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.898871 dvc-3.0.0a2/dvc/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)    18486 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7135 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4457 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.902871 dvc-3.0.0a2/dvc/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.902871 dvc-3.0.0a2/dvc/repo/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25405 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/executor/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7923 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/executor/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/executor/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/push.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.906871 dvc-3.0.0a2/dvc/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24548 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23073 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6834 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8879 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/queue/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/refs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6331 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6759 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/stash.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24913 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21484 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/ls_url.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.906871 dvc-3.0.0a2/dvc/repo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/metrics/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/metrics/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8225 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/open_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.906871 dvc-3.0.0a2/dvc/repo/params/
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/params/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/params/show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.906871 dvc-3.0.0a2/dvc/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)    17028 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/plots/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7492 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/trie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14157 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/repo/worktree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4191 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.910872 dvc-3.0.0a2/dvc/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)    24712 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9042 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7439 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6907 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8571 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/stage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.914872 dvc-3.0.0a2/dvc/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4088 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/api_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.914872 dvc-3.0.0a2/dvc/testing/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.914872 dvc-3.0.0a2/dvc/testing/benchmarks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.914872 dvc-3.0.0a2/dvc/testing/benchmarks/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.918872 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_exp_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.918872 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/test_modify_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.918872 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/benchmarks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/path_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/remote_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/tmp_dir.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13091 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/testing/workspace_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.922872 dvc-3.0.0a2/dvc/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ui/_rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ui/pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/ui/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5385 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.926872 dvc-3.0.0a2/dvc/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-07 06:07:03.000000 dvc-3.0.0a2/dvc/utils/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.926872 dvc-3.0.0a2/dvc/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_py.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/serialize/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/utils/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-07 06:07:00.000000 dvc-3.0.0a2/dvc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.866870 dvc-3.0.0a2/dvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17038 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-07 06:07:19.000000 dvc-3.0.0a2/dvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-06-07 06:07:00.000000 dvc-3.0.0a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.926872 dvc-3.0.0a2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/build-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/build.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      231 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/build_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.930873 dvc-3.0.0a2/scripts/fpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/after-install.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/after-remove.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/notarize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/fpm/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.930873 dvc-3.0.0a2/scripts/innosetup/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/addSymLinkPermissions.ps1
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/addsymlink.iss
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/dvc.ico.dvc
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/dvc_left.bmp.dvc
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/dvc_up.bmp.dvc
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/modpath.iss
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/innosetup/setup.iss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.934873 dvc-3.0.0a2/scripts/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/entitlements.plist
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.934873 dvc-3.0.0a2/scripts/pyinstaller/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-asyncssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.system.py
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc_task.py
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-pydrive2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2023-06-07 06:07:00.000000 dvc-3.0.0a2/scripts/pyinstaller/sign.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 06:07:19.994876 dvc-3.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.938873 dvc-3.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/dir_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.950873 dvc-3.0.0a2/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.950873 dvc-3.0.0a2/tests/func/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6887 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/api/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.950873 dvc-3.0.0a2/tests/func/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/artifacts/test_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.950873 dvc-3.0.0a2/tests/func/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.954874 dvc-3.0.0a2/tests/func/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/data/db/test_index.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.954874 dvc-3.0.0a2/tests/func/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/executor/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26286 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13387 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4928 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_set_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_stash_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/machine/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/machine/test_machine_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/machine/test_machine_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7730 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/metrics/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9854 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/metrics/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/params/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8161 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/params/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/params/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.958874 dvc-3.0.0a2/tests/func/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7479 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11227 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/test_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5484 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/test_interpolated_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/parsing/test_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.962874 dvc-3.0.0a2/tests/func/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/plots/test_modify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/plots/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31717 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24438 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8738 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16609 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_data_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18824 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11755 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7554 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_external_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14728 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11109 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20867 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7625 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5558 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5046 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17911 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_merge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5736 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5936 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_odb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15547 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10062 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33140 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20564 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_run_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9415 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14963 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_stage_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14871 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_used_objs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/test_virtual_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.962874 dvc-3.0.0a2/tests/func/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/utils/test_hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/func/utils/test_strict_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.962874 dvc-3.0.0a2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.962874 dvc-3.0.0a2/tests/integration/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/plots/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13779 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/plots/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/plots/test_repo_plots_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/integration/test_studio_live_experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.966874 dvc-3.0.0a2/tests/remotes/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.966874 dvc-3.0.0a2/tests/remotes/git-init/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/git_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/user.key
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes/user.key.pub
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/remotes_env.sample
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.970874 dvc-3.0.0a2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.970874 dvc-3.0.0a2/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/cli/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.978875 dvc-3.0.0a2/tests/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.978875 dvc-3.0.0a2/tests/unit/command/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/ls/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/ls/test_ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_compat_flag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11210 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11627 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4010 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/command/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.978875 dvc-3.0.0a2/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.982875 dvc-3.0.0a2/tests/unit/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/data/db/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.982875 dvc-3.0.0a2/tests/unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/dependency/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/dependency/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.982875 dvc-3.0.0a2/tests/unit/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7345 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19095 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_dvc_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/fs/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.982875 dvc-3.0.0a2/tests/unit/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.986875 dvc-3.0.0a2/tests/unit/output/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/output/test_output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.986875 dvc-3.0.0a2/tests/unit/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/test_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/test_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/remote/test_webhdfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.986875 dvc-3.0.0a2/tests/unit/render/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/test_image_converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/render/test_vega_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.986875 dvc-3.0.0a2/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/queue/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/queue/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/test_executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/test_open_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/test_reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/repo/test_scm_context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/scm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/scm/test_scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6074 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8626 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_loader_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_serialize_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_serialize_pipeline_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3705 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/stage/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_hashinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8869 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_tabular_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.990875 dvc-3.0.0a2/tests/unit/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/ui/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/ui/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/ui/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.994876 dvc-3.0.0a2/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.994876 dvc-3.0.0a2/tests/unit/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/serialize/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/serialize/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/serialize/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 06:07:19.994876 dvc-3.0.0a2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-07 06:07:00.000000 dvc-3.0.0a2/tests/utils/plots.py
```

### Comparing `dvc-3.0.0a1/.git-blame-ignore-revs` & `dvc-3.0.0a2/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md` & `dvc-3.0.0a2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/.github/ISSUE_TEMPLATE/epic_story.md` & `dvc-3.0.0a2/.github/ISSUE_TEMPLATE/epic_story.md`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/.github/workflows/codeql.yml` & `dvc-3.0.0a2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/.github/workflows/packages.yaml` & `dvc-3.0.0a2/.github/workflows/packages.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/.github/workflows/plugin_tests.yaml` & `dvc-3.0.0a2/.github/workflows/plugin_tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/.github/workflows/tests.yaml` & `dvc-3.0.0a2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/.pre-commit-config.yaml` & `dvc-3.0.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/.pre-commit-hooks.yaml` & `dvc-3.0.0a2/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/CODE_OF_CONDUCT.md` & `dvc-3.0.0a2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/LICENSE` & `dvc-3.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/PKG-INFO` & `dvc-3.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.0.0a1/README.rst` & `dvc-3.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/_debug.py` & `dvc-3.0.0a2/dvc/_debug.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/analytics.py` & `dvc-3.0.0a2/dvc/analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/annotations.py` & `dvc-3.0.0a2/dvc/annotations.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/api/data.py` & `dvc-3.0.0a2/dvc/api/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/api/experiments.py` & `dvc-3.0.0a2/dvc/api/experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/api/scm.py` & `dvc-3.0.0a2/dvc/api/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/api/show.py` & `dvc-3.0.0a2/dvc/api/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/cachemgr.py` & `dvc-3.0.0a2/dvc/cachemgr.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/cli/__init__.py` & `dvc-3.0.0a2/dvc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/cli/command.py` & `dvc-3.0.0a2/dvc/cli/command.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/cli/completion.py` & `dvc-3.0.0a2/dvc/cli/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/cli/parser.py` & `dvc-3.0.0a2/dvc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/cli/utils.py` & `dvc-3.0.0a2/dvc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/add.py` & `dvc-3.0.0a2/dvc/commands/add.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,32 +5,60 @@
 from dvc.cli.command import CmdBase
 from dvc.cli.utils import append_doc_link
 
 logger = logging.getLogger(__name__)
 
 
 class CmdAdd(CmdBase):
+    def validate_args(self) -> None:
+        from dvc.exceptions import InvalidArgumentError
+
+        args = self.args
+        invalid_opt = None
+
+        if args.to_remote or args.out:
+            message = "{option} can't be used with "
+            message += "--to-remote" if args.to_remote else "--out"
+            if len(args.targets) != 1:
+                invalid_opt = "multiple targets"
+            elif args.glob:
+                invalid_opt = "--glob option"
+            elif args.no_commit:
+                invalid_opt = "--no-commit option"
+            elif args.external:
+                invalid_opt = "--external option"
+        else:
+            message = "{option} can't be used without --to-remote"
+            if args.remote:
+                invalid_opt = "--remote"
+            elif args.remote_jobs:
+                invalid_opt = "--remote-jobs"
+
+        if invalid_opt is not None:
+            raise InvalidArgumentError(message.format(option=invalid_opt))
+
     def run(self):
-        from dvc.exceptions import DvcException, RecursiveAddingWhileUsingFilename
+        from dvc.exceptions import DvcException, InvalidArgumentError
 
         try:
-            if len(self.args.targets) > 1 and self.args.file:
-                raise RecursiveAddingWhileUsingFilename()
+            self.validate_args()
+        except InvalidArgumentError:
+            logger.exception("")
+            return 1
 
+        try:
             self.repo.add(
                 self.args.targets,
-                recursive=self.args.recursive,
                 no_commit=self.args.no_commit,
-                fname=self.args.file,
                 external=self.args.external,
                 glob=self.args.glob,
                 out=self.args.out,
                 remote=self.args.remote,
                 to_remote=self.args.to_remote,
-                jobs=self.args.jobs,
+                remote_jobs=self.args.remote_jobs,
                 force=self.args.force,
             )
         except FileNotFoundError:
             logger.exception("")
             return 1
         except DvcException:
             logger.exception("")
@@ -45,21 +73,14 @@
         "add",
         parents=[parent_parser],
         description=append_doc_link(ADD_HELP, "add"),
         help=ADD_HELP,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument(
-        "-R",
-        "--recursive",
-        action="store_true",
-        default=False,
-        help="Recursively add files under directory targets.",
-    )
-    parser.add_argument(
         "--no-commit",
         action="store_true",
         default=False,
         help="Don't put files/directories into cache.",
     )
     parser.add_argument(
         "--external",
@@ -70,19 +91,14 @@
     parser.add_argument(
         "--glob",
         action="store_true",
         default=False,
         help="Allows targets containing shell-style wildcards.",
     )
     parser.add_argument(
-        "--file",
-        help="Specify name of the .dvc file this command will generate.",
-        metavar="<filename>",
-    )
-    parser.add_argument(
         "-o",
         "--out",
         help="Destination path to put files to.",
         metavar="<path>",
     )
     parser.add_argument(
         "--to-remote",
@@ -93,16 +109,15 @@
     parser.add_argument(
         "-r",
         "--remote",
         help="Remote storage to download to",
         metavar="<name>",
     )
     parser.add_argument(
-        "-j",
-        "--jobs",
+        "--remote-jobs",
         type=int,
         help=(
             "Only used along with '--to-remote'. "
             "Number of jobs to run simultaneously "
             "when pushing data to remote."
             "The default value is 4 * cpu_count(). "
         ),
```

### Comparing `dvc-3.0.0a1/dvc/commands/cache.py` & `dvc-3.0.0a2/dvc/commands/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/check_ignore.py` & `dvc-3.0.0a2/dvc/commands/check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/checkout.py` & `dvc-3.0.0a2/dvc/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/commit.py` & `dvc-3.0.0a2/dvc/commands/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/completion.py` & `dvc-3.0.0a2/dvc/commands/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/config.py` & `dvc-3.0.0a2/dvc/commands/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/daemon.py` & `dvc-3.0.0a2/dvc/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/dag.py` & `dvc-3.0.0a2/dvc/commands/dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/data.py` & `dvc-3.0.0a2/dvc/commands/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/data_sync.py` & `dvc-3.0.0a2/dvc/commands/data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/destroy.py` & `dvc-3.0.0a2/dvc/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/diff.py` & `dvc-3.0.0a2/dvc/commands/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/__init__.py` & `dvc-3.0.0a2/dvc/commands/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/apply.py` & `dvc-3.0.0a2/dvc/commands/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/branch.py` & `dvc-3.0.0a2/dvc/commands/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/clean.py` & `dvc-3.0.0a2/dvc/commands/experiments/clean.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/diff.py` & `dvc-3.0.0a2/dvc/commands/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/exec_run.py` & `dvc-3.0.0a2/dvc/commands/experiments/exec_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/ls.py` & `dvc-3.0.0a2/dvc/commands/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/pull.py` & `dvc-3.0.0a2/dvc/commands/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/push.py` & `dvc-3.0.0a2/dvc/commands/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/queue_worker.py` & `dvc-3.0.0a2/dvc/commands/experiments/queue_worker.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/remove.py` & `dvc-3.0.0a2/dvc/commands/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/run.py` & `dvc-3.0.0a2/dvc/commands/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/save.py` & `dvc-3.0.0a2/dvc/commands/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/experiments/show.py` & `dvc-3.0.0a2/dvc/commands/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/freeze.py` & `dvc-3.0.0a2/dvc/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/gc.py` & `dvc-3.0.0a2/dvc/commands/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/get.py` & `dvc-3.0.0a2/dvc/commands/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/get_url.py` & `dvc-3.0.0a2/dvc/commands/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/git_hook.py` & `dvc-3.0.0a2/dvc/commands/git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/imp.py` & `dvc-3.0.0a2/dvc/commands/imp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/imp_url.py` & `dvc-3.0.0a2/dvc/commands/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/init.py` & `dvc-3.0.0a2/dvc/commands/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/install.py` & `dvc-3.0.0a2/dvc/commands/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/ls/__init__.py` & `dvc-3.0.0a2/dvc/commands/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/ls/ls_colors.py` & `dvc-3.0.0a2/dvc/commands/ls/ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/ls_url.py` & `dvc-3.0.0a2/dvc/commands/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/machine.py` & `dvc-3.0.0a2/dvc/commands/machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/metrics.py` & `dvc-3.0.0a2/dvc/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/move.py` & `dvc-3.0.0a2/dvc/commands/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/params.py` & `dvc-3.0.0a2/dvc/commands/params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/plots.py` & `dvc-3.0.0a2/dvc/commands/plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/queue/__init__.py` & `dvc-3.0.0a2/dvc/commands/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/queue/kill.py` & `dvc-3.0.0a2/dvc/commands/queue/kill.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/queue/logs.py` & `dvc-3.0.0a2/dvc/commands/queue/logs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/queue/remove.py` & `dvc-3.0.0a2/dvc/commands/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/queue/start.py` & `dvc-3.0.0a2/dvc/commands/queue/start.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/queue/status.py` & `dvc-3.0.0a2/dvc/commands/queue/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/queue/stop.py` & `dvc-3.0.0a2/dvc/commands/queue/stop.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/remote.py` & `dvc-3.0.0a2/dvc/commands/remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/remove.py` & `dvc-3.0.0a2/dvc/commands/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/repro.py` & `dvc-3.0.0a2/dvc/commands/repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/root.py` & `dvc-3.0.0a2/dvc/commands/root.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/stage.py` & `dvc-3.0.0a2/dvc/commands/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/status.py` & `dvc-3.0.0a2/dvc/commands/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/unprotect.py` & `dvc-3.0.0a2/dvc/commands/unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/update.py` & `dvc-3.0.0a2/dvc/commands/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/commands/version.py` & `dvc-3.0.0a2/dvc/commands/version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/compare.py` & `dvc-3.0.0a2/dvc/compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/config.py` & `dvc-3.0.0a2/dvc/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/config_schema.py` & `dvc-3.0.0a2/dvc/config_schema.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/daemon.py` & `dvc-3.0.0a2/dvc/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/dagascii.py` & `dvc-3.0.0a2/dvc/dagascii.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/data_cloud.py` & `dvc-3.0.0a2/dvc/data_cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/dependency/__init__.py` & `dvc-3.0.0a2/dvc/dependency/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # NOTE: schema for dependencies is basically the same as for outputs, but
 # without output-specific entries like 'cache' (whether or not output is
 # cached, see -o and -O flags for `dvc run`) and 'metric' (whether or not
 # output is a metrics file and how to parse it, see `-M` flag for `dvc run`).
 SCHEMA: Mapping[str, Any] = {
     **ARTIFACT_SCHEMA,
     **RepoDependency.REPO_SCHEMA,
-    **ParamsDependency.PARAM_SCHEMA,
     Output.PARAM_FILES: [DIR_FILES_SCHEMA],
 }
 
 
 def _get(stage, p, info, **kwargs):
     if info and info.get(RepoDependency.PARAM_REPO):
         repo = info.pop(RepoDependency.PARAM_REPO)
```

### Comparing `dvc-3.0.0a1/dvc/dependency/base.py` & `dvc-3.0.0a2/dvc/dependency/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/dependency/param.py` & `dvc-3.0.0a2/dvc/dependency/param.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import os
 import typing
 from collections import defaultdict
-from typing import Dict
+from typing import Any, Dict
 
 import dpath
-from voluptuous import Any
 
 from dvc.exceptions import DvcException
 from dvc.utils.serialize import ParseError, load_path
 from dvc_data.hashfile.hash_info import HashInfo
 
 from .base import Dependency
 
@@ -30,15 +29,14 @@
 
 class BadParamFileError(DvcException):
     pass
 
 
 class ParamsDependency(Dependency):
     PARAM_PARAMS = "params"
-    PARAM_SCHEMA = {PARAM_PARAMS: Any(dict, list, None)}
     DEFAULT_PARAMS_FILE = "params.yaml"
 
     def __init__(self, stage, path, params=None, repo=None):
         self.params = list(params) if params else []
         hash_info = HashInfo()
         if isinstance(params, dict):
             hash_info = HashInfo(
```

### Comparing `dvc-3.0.0a1/dvc/dependency/repo.py` & `dvc-3.0.0a2/dvc/dependency/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/dirs.py` & `dvc-3.0.0a2/dvc/dirs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/dvcfile.py` & `dvc-3.0.0a2/dvc/dvcfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     from .parsing import DataResolver
     from .stage import Stage
 
 logger = logging.getLogger(__name__)
 _T = TypeVar("_T")
 
-DVC_FILE = "Dvcfile"
 DVC_FILE_SUFFIX = ".dvc"
 PROJECT_FILE = "dvc.yaml"
 LOCK_FILE = "dvc.lock"
 
 
 class FileIsGitIgnored(DvcException):
     def __init__(self, path, pipeline_file=False):
@@ -51,18 +50,15 @@
 
 
 class ParametrizedDumpError(DvcException):
     pass
 
 
 def is_valid_filename(path):
-    return path.endswith(DVC_FILE_SUFFIX) or os.path.basename(path) in [
-        DVC_FILE,
-        PROJECT_FILE,
-    ]
+    return path.endswith(DVC_FILE_SUFFIX) or os.path.basename(path) == PROJECT_FILE
 
 
 def is_dvc_file(path):
     return os.path.isfile(path) and (is_valid_filename(path) or is_lock_file(path))
 
 
 def is_lock_file(path):
```

### Comparing `dvc-3.0.0a1/dvc/env.py` & `dvc-3.0.0a2/dvc/env.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/exceptions.py` & `dvc-3.0.0a2/dvc/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,19 +178,14 @@
             "the following metrics do not exist, "
             "are not metrics files or are malformed: {paths}".format(
                 paths=", ".join(f"'{path}'" for path in paths)
             )
         )
 
 
-class RecursiveAddingWhileUsingFilename(DvcException):
-    def __init__(self):
-        super().__init__("cannot use `fname` with multiple targets or `-R|--recursive`")
-
-
 class OverlappingOutputPathsError(DvcException):
     def __init__(self, parent, overlapping_out, message):
         self.parent = parent
         self.overlapping_out = overlapping_out
         super().__init__(message)
```

### Comparing `dvc-3.0.0a1/dvc/fs/__init__.py` & `dvc-3.0.0a2/dvc/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/fs/callbacks.py` & `dvc-3.0.0a2/dvc/fs/callbacks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/fs/data.py` & `dvc-3.0.0a2/dvc/fs/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/fs/dvc.py` & `dvc-3.0.0a2/dvc/fs/dvc.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,25 @@
 def _is_dvc_file(fname):
     from dvc.dvcfile import is_valid_filename
     from dvc.ignore import DvcIgnore
 
     return is_valid_filename(fname) or fname == DvcIgnore.DVCIGNORE_FILE
 
 
-def _merge_info(repo, fs_info, dvc_info):
+def _merge_info(repo, key, fs_info, dvc_info):
     from . import utils
 
     ret = {"repo": repo}
 
     if dvc_info:
+        dvc_info["isout"] = any(
+            (len(out_key) <= len(key) and key[: len(out_key)] == out_key)
+            for out_key in repo.index.data_keys["repo"]
+        )
+        dvc_info["isdvc"] = dvc_info["isout"]
         ret["dvc_info"] = dvc_info
         ret["type"] = dvc_info["type"]
         ret["size"] = dvc_info["size"]
         if not fs_info and "md5" in dvc_info:
             ret["md5"] = dvc_info["md5"]
 
     if fs_info:
@@ -259,18 +264,18 @@
         kw = {}
         if kwargs.get("cache_remote_stream", False):
             kw["cache_odb"] = repo.cache.local
         return dvc_fs.open(dvc_path, mode=mode, **kw)
 
     def isdvc(self, path, **kwargs) -> bool:
         """Is this entry dvc-tracked?"""
-        key = self._get_key_from_relative(path)
-        _, dvc_fs, subkey = self._get_subrepo_info(key)
-        dvc_path = _get_dvc_path(dvc_fs, subkey)
-        return dvc_fs is not None and dvc_fs.isdvc(dvc_path, **kwargs)
+        try:
+            return self.info(path).get("dvc_info", {}).get("isout", False)
+        except FileNotFoundError:
+            return False
 
     def ls(  # pylint: disable=arguments-differ # noqa: C901
         self, path, detail=True, dvc_only=False, **kwargs
     ):
         key = self._get_key_from_relative(path)
         repo, dvc_fs, subkey = self._get_subrepo_info(key)
 
@@ -310,15 +315,17 @@
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), path)
 
         for name in names:
             if not dvcfiles and _is_dvc_file(name):
                 continue
 
             entry_path = self.path.join(path, name)
-            info = _merge_info(repo, fs_infos.get(name), dvc_infos.get(name))
+            info = _merge_info(
+                repo, (*subkey, name), fs_infos.get(name), dvc_infos.get(name)
+            )
             info["name"] = entry_path
             infos.append(info)
             paths.append(entry_path)
 
         if not detail:
             return paths
 
@@ -366,15 +373,15 @@
                         break
                 except FileNotFoundError:
                     continue
 
         if not dvc_info and not fs_info:
             raise FileNotFoundError
 
-        info = _merge_info(repo, fs_info, dvc_info)
+        info = _merge_info(repo, subkey, fs_info, dvc_info)
         info["name"] = path
         return info
 
     def get_file(self, rpath, lpath, **kwargs):  # pylint: disable=arguments-differ
         key = self._get_key_from_relative(rpath)
         fs_path = self._from_key(key)
         try:
```

### Comparing `dvc-3.0.0a1/dvc/fs/git.py` & `dvc-3.0.0a2/dvc/fs/git.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/ignore.py` & `dvc-3.0.0a2/dvc/ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/info.py` & `dvc-3.0.0a2/dvc/info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/lock.py` & `dvc-3.0.0a2/dvc/lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/logger.py` & `dvc-3.0.0a2/dvc/logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/machine/__init__.py` & `dvc-3.0.0a2/dvc/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/machine/backend/base.py` & `dvc-3.0.0a2/dvc/machine/backend/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/machine/backend/terraform.py` & `dvc-3.0.0a2/dvc/machine/backend/terraform.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/output.py` & `dvc-3.0.0a2/dvc/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,23 +294,14 @@
     PARAM_PLOT_TITLE = "title"
     PARAM_PLOT_HEADER = "header"
     PARAM_PERSIST = "persist"
     PARAM_REMOTE = "remote"
     PARAM_PUSH = "push"
     PARAM_CLOUD = "cloud"
 
-    METRIC_SCHEMA = Any(
-        None,
-        bool,
-        {
-            PARAM_METRIC_TYPE: Any(str, None),
-            PARAM_METRIC_XPATH: Any(str, None),
-        },
-    )
-
     DoesNotExistError: Type[DvcException] = OutputDoesNotExistError
     IsNotFileOrDirError: Type[DvcException] = OutputIsNotFileOrDirError
     IsStageFileError: Type[DvcException] = OutputIsStageFileError
     IsIgnoredError: Type[DvcException] = OutputIsIgnoredError
 
     def __init__(  # noqa: PLR0913
         self,
@@ -1413,15 +1404,14 @@
 
 CLOUD_SCHEMA = All({str: {**META_SCHEMA, **CHECKSUMS_SCHEMA}}, Length(max=1))
 
 ARTIFACT_SCHEMA = {
     **CHECKSUMS_SCHEMA,
     **META_SCHEMA,
     Required(Output.PARAM_PATH): str,
-    Output.PARAM_PLOT: bool,
     Output.PARAM_PERSIST: bool,
     Output.PARAM_CLOUD: CLOUD_SCHEMA,
 }
 
 DIR_FILES_SCHEMA: Dict[str, Any] = {
     **CHECKSUMS_SCHEMA,
     **META_SCHEMA,
@@ -1429,12 +1419,11 @@
     Output.PARAM_CLOUD: CLOUD_SCHEMA,
 }
 
 SCHEMA = {
     **ARTIFACT_SCHEMA,
     **ANNOTATION_SCHEMA,
     Output.PARAM_CACHE: bool,
-    Output.PARAM_METRIC: Output.METRIC_SCHEMA,
     Output.PARAM_REMOTE: str,
     Output.PARAM_PUSH: bool,
     Output.PARAM_FILES: [DIR_FILES_SCHEMA],
 }
```

### Comparing `dvc-3.0.0a1/dvc/parsing/__init__.py` & `dvc-3.0.0a2/dvc/parsing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,26 +228,14 @@
         self.wdir = self.resolver.wdir
         self.relpath = self.resolver.relpath
         self.context = context
         self.name = name
         self.definition = definition
         self.where = where
 
-    def _resolve_wdir(
-        self, context: Context, name: str, wdir: Optional[str] = None
-    ) -> str:
-        if not wdir:
-            return self.wdir
-
-        try:
-            wdir = to_str(context.resolve_str(wdir))
-        except (ContextError, ParseError) as exc:
-            format_and_raise(exc, f"'{self.where}.{name}.wdir'", self.relpath)
-        return self.resolver.fs.path.join(self.wdir, wdir)
-
     def resolve(self, **kwargs):
         try:
             return self.resolve_stage(**kwargs)
         except ContextError as exc:
             format_and_raise(exc, f"stage '{self.name}'", self.relpath)
 
     def resolve_stage(self, skip_checks: bool = False) -> "DictStrAny":
@@ -257,41 +245,15 @@
             # we can check for syntax errors as we go for interpolated entries,
             # but for foreach-generated ones, once is enough, which it does
             # that itself. See `ForeachDefinition.do_definition`.
             check_syntax_errors(self.definition, name, self.relpath)
 
         # we need to pop vars from generated/evaluated data
         definition = deepcopy(self.definition)
-
-        wdir = self._resolve_wdir(context, name, definition.get(WDIR_KWD))
-        vars_ = definition.pop(VARS_KWD, [])
-        # FIXME: Should `vars` be templatized?
-        check_interpolations(vars_, f"{self.where}.{name}.vars", self.relpath)
-        if vars_:
-            # Optimization: Lookahead if it has any vars, if it does not, we
-            # don't need to clone them.
-            context = Context.clone(context)
-
-        try:
-            fs = self.resolver.fs
-            context.load_from_vars(fs, vars_, wdir, stage_name=name)
-        except VarsAlreadyLoaded as exc:
-            format_and_raise(exc, f"'{self.where}.{name}.vars'", self.relpath)
-
-        logger.trace(  # type: ignore[attr-defined]
-            "Context during resolution of stage %s:\n%s", name, context
-        )
-
         with context.track() as tracked_data:
-            # NOTE: we do not pop "wdir", and resolve it again
-            # this does not affect anything and is done to try to
-            # track the source of `wdir` interpolation.
-            # This works because of the side-effect that we do not
-            # allow overwriting and/or str interpolating complex objects.
-            # Fix if/when those assumptions are no longer valid.
             resolved = {
                 key: self._resolve(context, value, key, skip_checks)
                 for key, value in definition.items()
             }
 
         self.resolver.track_vars(name, tracked_data)
         return {name: resolved}
```

### Comparing `dvc-3.0.0a1/dvc/parsing/context.py` & `dvc-3.0.0a2/dvc/parsing/context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/parsing/interpolate.py` & `dvc-3.0.0a2/dvc/parsing/interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/pathspec_math.py` & `dvc-3.0.0a2/dvc/pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/progress.py` & `dvc-3.0.0a2/dvc/progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/prompt.py` & `dvc-3.0.0a2/dvc/prompt.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/render/convert.py` & `dvc-3.0.0a2/dvc/render/convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/render/converter/__init__.py` & `dvc-3.0.0a2/dvc/render/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/render/converter/image.py` & `dvc-3.0.0a2/dvc/render/converter/image.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/render/converter/vega.py` & `dvc-3.0.0a2/dvc/render/converter/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/render/match.py` & `dvc-3.0.0a2/dvc/render/match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/__init__.py` & `dvc-3.0.0a2/dvc/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/artifacts.py` & `dvc-3.0.0a2/dvc/repo/artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/brancher.py` & `dvc-3.0.0a2/dvc/repo/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/checkout.py` & `dvc-3.0.0a2/dvc/repo/install.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,85 @@
-import logging
-import os
-from typing import TYPE_CHECKING, Dict, List, Set
+from typing import TYPE_CHECKING
 
-from dvc.exceptions import CheckoutError, CheckoutErrorSuggestGit, NoOutputOrStageError
-from dvc.utils import relpath
-
-from . import locked
+from dvc.exceptions import DvcException
 
 if TYPE_CHECKING:
-    from . import Repo
-    from .stage import StageInfo
+    from dvc.repo import Repo
+    from dvc.scm import Git
 
-logger = logging.getLogger(__name__)
 
+def pre_commit_install(scm: "Git") -> None:
+    import os
 
-def _fspath_dir(path):
-    if not os.path.exists(str(path)):
-        return str(path)
+    from dvc.utils.serialize import modify_yaml
 
-    path = relpath(path)
-    return os.path.join(path, "") if os.path.isdir(path) else path
+    config_path = os.path.join(scm.root_dir, ".pre-commit-config.yaml")
+    with modify_yaml(config_path) as config:
+        entry = {
+            "repo": "https://github.com/iterative/dvc",
+            "rev": "main",
+            "hooks": [
+                {
+                    "id": "dvc-pre-commit",
+                    "additional_dependencies": [".[all]"],
+                    "language_version": "python3",
+                    "stages": ["commit"],
+                },
+                {
+                    "id": "dvc-pre-push",
+                    "additional_dependencies": [".[all]"],
+                    "language_version": "python3",
+                    "stages": ["push"],
+                },
+                {
+                    "id": "dvc-post-checkout",
+                    "additional_dependencies": [".[all]"],
+                    "language_version": "python3",
+                    "stages": ["post-checkout"],
+                    "always_run": True,
+                },
+            ],
+        }
+
+        config["repos"] = config.get("repos", [])
+        if entry not in config["repos"]:
+            config["repos"].append(entry)
 
 
-def _remove_unused_links(repo):
-    used = [out.fspath for out in repo.index.outs if out.protocol == "local"]
-    unused = repo.state.get_unused_links(used, repo.fs)
-    ret = [_fspath_dir(u) for u in unused]
-    repo.state.remove_links(unused, repo.fs)
-    return ret
+def install_hooks(scm: "Git") -> None:
+    from scmrepo.exceptions import GitHookAlreadyExists
 
+    from dvc.utils import format_link
 
-def get_all_files_numbers(pairs):
-    return sum(stage.get_all_files_number(filter_info) for stage, filter_info in pairs)
+    hooks = ["post-checkout", "pre-commit", "pre-push"]
+    for hook in hooks:
+        try:
+            scm.verify_hook(hook)
+        except GitHookAlreadyExists as exc:
+            link = format_link("https://man.dvc.org/install")
+            raise DvcException(  # noqa: B904
+                f"{exc}. Please refer to {link} for more info."
+            )
 
+    for hook in hooks:
+        scm.install_hook(hook, f"exec dvc git-hook {hook} $@")
 
-def _collect_pairs(
-    self: "Repo", targets, with_deps: bool, recursive: bool
-) -> Set["StageInfo"]:
-    from dvc.stage.exceptions import StageFileBadNameError, StageFileDoesNotExistError
 
-    pairs: Set["StageInfo"] = set()
-    for target in targets:
-        try:
-            pairs.update(
-                self.stage.collect_granular(
-                    target, with_deps=with_deps, recursive=recursive
-                )
-            )
-        except (
-            StageFileDoesNotExistError,
-            StageFileBadNameError,
-            NoOutputOrStageError,
-        ) as exc:
-            if not target:
-                raise
-            raise CheckoutErrorSuggestGit(target) from exc
-
-    return pairs
-
-
-@locked
-def checkout(
-    self,
-    targets=None,
-    with_deps=False,
-    force=False,
-    relink=False,
-    recursive=False,
-    allow_missing=False,
-    **kwargs,
-):
-    from dvc.fs.callbacks import Callback
-
-    stats: Dict[str, List[str]] = {
-        "added": [],
-        "deleted": [],
-        "modified": [],
-        "failed": [],
-    }
-    if not targets:
-        targets = [None]
-        stats["deleted"] = _remove_unused_links(self)
-
-    if isinstance(targets, str):
-        targets = [targets]
-
-    pairs = _collect_pairs(self, targets, with_deps, recursive)
-    total = get_all_files_numbers(pairs)
-    with Callback.as_tqdm_callback(
-        unit="file",
-        desc="Checkout",
-        disable=total == 0,
-    ) as cb:
-        cb.set_size(total)
-        for stage, filter_info in pairs:
-            result = stage.checkout(
-                force=force,
-                progress_callback=cb,
-                relink=relink,
-                filter_info=filter_info,
-                allow_missing=allow_missing,
-                **kwargs,
-            )
-            for key, items in result.items():
-                stats[key].extend(_fspath_dir(path) for path in items)
+def install(self: "Repo", use_pre_commit_tool: bool = False) -> None:
+    """Adds dvc commands to SCM hooks for the repo.
+
+    If use_pre_commit_tool is set and pre-commit is installed it will be used
+    to install the hooks.
+    """
+    from dvc.scm import Git
+
+    scm = self.scm
+    if not isinstance(scm, Git):
+        return
+
+    driver = "dvc git-hook merge-driver --ancestor %O --our %A --their %B "
+    scm.install_merge_driver("dvc", "DVC merge driver", driver)
 
-    if stats.get("failed"):
-        raise CheckoutError(stats["failed"], stats)
+    if use_pre_commit_tool:
+        return pre_commit_install(scm)
 
-    del stats["failed"]
-    return stats
+    return install_hooks(scm)
```

### Comparing `dvc-3.0.0a1/dvc/repo/collect.py` & `dvc-3.0.0a2/dvc/repo/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/commit.py` & `dvc-3.0.0a2/dvc/repo/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/data.py` & `dvc-3.0.0a2/dvc/repo/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,18 +69,16 @@
         with_unchanged=True,
         shallow=not granular,
         hash_only=True,
         with_unknown=True,
     ):
         if (
             change.typ == UNCHANGED
-            and change.old
-            and change.new
-            and not change.old.hash_info
-            and not change.new.hash_info
+            and (not change.old or not change.old.hash_info)
+            and (not change.new or not change.new.hash_info)
         ):
             # NOTE: emulating previous behaviour
             continue
 
         if change.typ == UNKNOWN and not change.new:
             # NOTE: emulating previous behaviour
             continue
```

### Comparing `dvc-3.0.0a1/dvc/repo/destroy.py` & `dvc-3.0.0a2/dvc/repo/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/diff.py` & `dvc-3.0.0a2/dvc/repo/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/__init__.py` & `dvc-3.0.0a2/dvc/repo/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/apply.py` & `dvc-3.0.0a2/dvc/repo/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/branch.py` & `dvc-3.0.0a2/dvc/repo/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/brancher.py` & `dvc-3.0.0a2/dvc/repo/experiments/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/cache.py` & `dvc-3.0.0a2/dvc/repo/experiments/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/collect.py` & `dvc-3.0.0a2/dvc/repo/experiments/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/diff.py` & `dvc-3.0.0a2/dvc/repo/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/exceptions.py` & `dvc-3.0.0a2/dvc/repo/experiments/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/executor/base.py` & `dvc-3.0.0a2/dvc/repo/experiments/executor/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/executor/local.py` & `dvc-3.0.0a2/dvc/repo/experiments/executor/local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/executor/ssh.py` & `dvc-3.0.0a2/dvc/repo/experiments/executor/ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/ls.py` & `dvc-3.0.0a2/dvc/repo/experiments/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/pull.py` & `dvc-3.0.0a2/dvc/repo/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/push.py` & `dvc-3.0.0a2/dvc/repo/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/queue/base.py` & `dvc-3.0.0a2/dvc/repo/experiments/queue/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/queue/celery.py` & `dvc-3.0.0a2/dvc/repo/experiments/queue/celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/queue/remove.py` & `dvc-3.0.0a2/dvc/repo/experiments/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/queue/tasks.py` & `dvc-3.0.0a2/dvc/repo/experiments/queue/tasks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/queue/tempdir.py` & `dvc-3.0.0a2/dvc/repo/experiments/queue/tempdir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/queue/utils.py` & `dvc-3.0.0a2/dvc/repo/experiments/queue/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/queue/workspace.py` & `dvc-3.0.0a2/dvc/repo/experiments/queue/workspace.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/refs.py` & `dvc-3.0.0a2/dvc/repo/experiments/refs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/remove.py` & `dvc-3.0.0a2/dvc/repo/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/run.py` & `dvc-3.0.0a2/dvc/repo/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/save.py` & `dvc-3.0.0a2/dvc/repo/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/serialize.py` & `dvc-3.0.0a2/dvc/repo/experiments/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/show.py` & `dvc-3.0.0a2/dvc/repo/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/stash.py` & `dvc-3.0.0a2/dvc/repo/experiments/stash.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/experiments/utils.py` & `dvc-3.0.0a2/dvc/repo/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/fetch.py` & `dvc-3.0.0a2/dvc/repo/fetch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/gc.py` & `dvc-3.0.0a2/dvc/repo/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/get.py` & `dvc-3.0.0a2/dvc/repo/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/get_url.py` & `dvc-3.0.0a2/dvc/repo/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/graph.py` & `dvc-3.0.0a2/dvc/repo/graph.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/imp_url.py` & `dvc-3.0.0a2/dvc/repo/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/imports.py` & `dvc-3.0.0a2/dvc/repo/imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         if not cache.fs.exists(cache.path):
             os.makedirs(cache.path)
         with TemporaryDirectory(dir=cache.path) as tmpdir:
             with Callback.as_tqdm_callback(
                 desc="Downloading imports from source",
                 unit="files",
             ) as cb:
-                checkout(data_view, tmpdir, cache.fs, callback=cb, storage="data")
+                checkout(data_view, tmpdir, cache.fs, callback=cb, storage="remote")
             md5(data_view)
             save(data_view, odb=cache, hardlink=True)
 
         downloaded.update(
             entry.hash_info
             for _, entry in data_view.iteritems()
             if entry.meta is not None
```

### Comparing `dvc-3.0.0a1/dvc/repo/index.py` & `dvc-3.0.0a2/dvc/repo/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,23 @@
     Tuple,
     Union,
 )
 
 from funcy.debug import format_time
 
 from dvc.fs import LocalFileSystem
+from dvc.fs.callbacks import DEFAULT_CALLBACK
 from dvc.utils.objects import cached_property
 
 if TYPE_CHECKING:
     from networkx import DiGraph
     from pygtrie import Trie
 
     from dvc.dependency import Dependency, ParamsDependency
+    from dvc.fs.callbacks import Callback
     from dvc.output import Output
     from dvc.repo import Repo
     from dvc.repo.stage import StageInfo
     from dvc.stage import Stage
     from dvc.types import TargetType
     from dvc_data.hashfile.hash_info import HashInfo
     from dvc_data.index import DataIndex, DataIndexKey, DataIndexView
@@ -109,22 +111,26 @@
                 if out.protocol == "local"
             )
             yield file_path, index
         dirs[:] = [d for d in dirs if not is_out_or_ignored(root, d)]
 
 
 def _load_data_from_outs(index, prefix, outs):
-    from dvc_data.index import DataIndexEntry
+    from dvc_data.index import DataIndexEntry, Meta
 
+    parents = set()
     for out in outs:
         if not out.use_cache:
             continue
 
         ws, key = out.index_key
 
+        for key_len in range(1, len(key)):
+            parents.add((ws, key[:key_len]))
+
         entry = DataIndexEntry(
             key=key,
             meta=out.meta,
             hash_info=out.hash_info,
         )
 
         if out.stage.is_import and not out.stage.is_repo_import:
@@ -133,14 +139,19 @@
             entry.hash_info = dep.hash_info
 
         # FIXME PyGTrie-based DataIndex doesn't remove entry.key during
         # index.add, so we have to set the entry manually here to make
         # index.view() work correctly.
         index[(*prefix, ws, *key)] = entry
 
+    for ws, key in parents:
+        index[(*prefix, ws, *key)] = DataIndexEntry(
+            key=key, meta=Meta(isdir=True), loaded=True
+        )
+
 
 def _load_storage_from_out(storage_map, key, out):
     from dvc.config import NoRemoteError
     from dvc_data.index import FileStorage, ObjectStorage
 
     if out.odb:
         storage_map.add_data(ObjectStorage(key, out.odb))
@@ -159,15 +170,15 @@
         else:
             storage_map.add_remote(ObjectStorage(key, remote.odb, index=remote.index))
     except NoRemoteError:
         pass
 
     if out.stage.is_import:
         dep = out.stage.deps[0]
-        storage_map.add_data(FileStorage(key, dep.fs, dep.fs_path))
+        storage_map.add_remote(FileStorage(key, dep.fs, dep.fs_path))
 
 
 class Index:
     def __init__(
         self,
         repo: "Repo",
         stages: Optional[List["Stage"]] = None,
@@ -530,30 +541,35 @@
     def _data_prefixes(self) -> Dict[str, "_DataPrefixes"]:
         from collections import defaultdict
 
         prefixes: Dict[str, "_DataPrefixes"] = defaultdict(
             lambda: _DataPrefixes(set(), set())
         )
         for out, filter_info in self._filtered_outs:
+            if not out.use_cache:
+                continue
             workspace, key = out.index_key
             if filter_info and out.fs.path.isin(filter_info, out.fs_path):
                 key = key + out.fs.path.relparts(filter_info, out.fs_path)
-            entry = self._index.data[workspace][key]
+            entry = self._index.data[workspace].get(key)
             if entry and entry.meta and entry.meta.isdir:
                 prefixes[workspace].recursive.add(key)
             prefixes[workspace].explicit.update(key[:i] for i in range(len(key), 0, -1))
         return prefixes
 
     @cached_property
     def data_keys(self) -> Dict[str, Set["DataIndexKey"]]:
         from collections import defaultdict
 
         ret: Dict[str, Set["DataIndexKey"]] = defaultdict(set)
 
         for out, filter_info in self._filtered_outs:
+            if not out.use_cache:
+                continue
+
             workspace, key = out.index_key
             if filter_info and out.fs.path.isin(filter_info, out.fs_path):
                 key = key + out.fs.path.relparts(filter_info, out.fs_path)
             ret[workspace].add(key)
 
         return dict(ret)
 
@@ -575,45 +591,54 @@
             if self.stages:
                 data[workspace] = view(data_index, partial(key_filter, workspace))
             else:
                 data[workspace] = DataIndex()
         return data
 
 
-def build_data_index(
+def build_data_index(  # noqa: C901
     index: Union["Index", "IndexView"],
     path: str,
     fs: "FileSystem",
     workspace: str = "repo",
     compute_hash: Optional[bool] = False,
+    callback: "Callback" = DEFAULT_CALLBACK,
 ) -> "DataIndex":
-    from dvc_data.index import DataIndex, DataIndexEntry
+    from dvc_data.index import DataIndex, DataIndexEntry, Meta
     from dvc_data.index.build import build_entries, build_entry
     from dvc_data.index.save import build_tree
 
     ignore = None
     if workspace == "repo" and isinstance(fs, LocalFileSystem):
         ignore = index.repo.dvcignore
 
     data = DataIndex()
+    parents = set()
     for key in index.data_keys.get(workspace, set()):
         out_path = fs.path.join(path, *key)
 
+        for key_len in range(1, len(key)):
+            parents.add(key[:key_len])
+
+        if not fs.exists(out_path):
+            continue
+
         try:
             out_entry = build_entry(
                 out_path,
                 fs,
                 compute_hash=compute_hash,
                 state=index.repo.state,
             )
         except FileNotFoundError:
-            out_entry = DataIndexEntry()
+            continue
 
         out_entry.key = key
         data.add(out_entry)
+        callback.relative_update(1)
 
         if not out_entry.meta or not out_entry.meta.isdir:
             continue
 
         for entry in build_entries(
             out_path,
             fs,
@@ -624,16 +649,26 @@
             if not entry.key or entry.key == ("",):
                 # NOTE: whether the root will be returned by build_entries
                 # depends on the filesystem (e.g. local doesn't, but s3 does).
                 continue
 
             entry.key = key + entry.key
             data.add(entry)
+            callback.relative_update(1)
 
         if compute_hash:
             tree_meta, tree = build_tree(data, key)
             out_entry.meta = tree_meta
             out_entry.hash_info = tree.hash_info
             out_entry.loaded = True
             data.add(out_entry)
+            callback.relative_update(1)
+
+    for key in parents:
+        parent_path = fs.path.join(path, *key)
+        if not fs.exists(parent_path):
+            continue
+        direntry = DataIndexEntry(key=key, meta=Meta(isdir=True), loaded=True)
+        data.add(direntry)
+        callback.relative_update(1)
 
     return data
```

### Comparing `dvc-3.0.0a1/dvc/repo/init.py` & `dvc-3.0.0a2/dvc/repo/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/ls.py` & `dvc-3.0.0a2/dvc/repo/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/ls_url.py` & `dvc-3.0.0a2/dvc/repo/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/metrics/diff.py` & `dvc-3.0.0a2/dvc/repo/metrics/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/metrics/show.py` & `dvc-3.0.0a2/dvc/repo/metrics/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/move.py` & `dvc-3.0.0a2/dvc/repo/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/open_repo.py` & `dvc-3.0.0a2/dvc/repo/open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/params/diff.py` & `dvc-3.0.0a2/dvc/repo/params/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/params/show.py` & `dvc-3.0.0a2/dvc/repo/params/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/plots/__init__.py` & `dvc-3.0.0a2/dvc/repo/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/plots/diff.py` & `dvc-3.0.0a2/dvc/repo/plots/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/pull.py` & `dvc-3.0.0a2/dvc/repo/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/push.py` & `dvc-3.0.0a2/dvc/repo/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/remove.py` & `dvc-3.0.0a2/dvc/repo/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/reproduce.py` & `dvc-3.0.0a2/dvc/repo/reproduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from typing import TYPE_CHECKING, Iterator, List
 
 from dvc.exceptions import ReproductionError
 from dvc.repo.scm_context import scm_context
+from dvc.stage.cache import RunCacheNotSupported
 
 from . import locked
 
 if TYPE_CHECKING:
     from dvc.stage import Stage
 
     from . import Repo
@@ -102,17 +103,20 @@
                 self.stage.collect(
                     target,
                     recursive=recursive,
                     glob=glob,
                 )
             )
 
-    if kwargs.get("pull", False):
+    if kwargs.get("pull", False) and kwargs.get("run_cache", True):
         logger.debug("Pulling run cache")
-        self.stage_cache.pull(None)
+        try:
+            self.stage_cache.pull(None)
+        except RunCacheNotSupported as e:
+            logger.warning("Failed to pull run cache: %s", e)
 
     return _reproduce_stages(self.index.graph, list(stages), **kwargs)
 
 
 def _reproduce_stages(  # noqa: C901
     graph,
     stages,
```

### Comparing `dvc-3.0.0a1/dvc/repo/run.py` & `dvc-3.0.0a2/dvc/repo/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     self: "Repo",
     no_exec: bool = False,
     no_commit: bool = False,
     run_cache: bool = True,
     force: bool = True,
     **kwargs,
 ) -> Union["Stage", "PipelineStage"]:
+    assert not kwargs.get("single_stage")
+    assert not kwargs.get("fname")
     kwargs.update({"force": force, "params": parse_params(kwargs.get("params", []))})
     stage = self.stage.create(**kwargs)
 
     if no_exec:
         stage.ignore_outs()
     else:
         stage.run(no_commit=no_commit, run_cache=run_cache)
```

### Comparing `dvc-3.0.0a1/dvc/repo/scm_context.py` & `dvc-3.0.0a2/dvc/repo/scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/stage.py` & `dvc-3.0.0a2/dvc/repo/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/status.py` & `dvc-3.0.0a2/dvc/repo/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/trie.py` & `dvc-3.0.0a2/dvc/repo/trie.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/update.py` & `dvc-3.0.0a2/dvc/repo/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/repo/worktree.py` & `dvc-3.0.0a2/dvc/repo/worktree.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/rwlock.py` & `dvc-3.0.0a2/dvc/rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/schema.py` & `dvc-3.0.0a2/dvc/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 )
 from dvc.parsing import DO_KWD, FOREACH_KWD, VARS_KWD
 from dvc.stage.params import StageParams
 
 STAGES = "stages"
 SINGLE_STAGE_SCHEMA = {
     StageParams.PARAM_MD5: output.CHECKSUM_SCHEMA,
-    StageParams.PARAM_CMD: Any(str, list, None),
     StageParams.PARAM_WDIR: Any(str, None),
     StageParams.PARAM_DEPS: Any([dependency.SCHEMA], None),
     StageParams.PARAM_OUTS: Any([output.SCHEMA], None),
     StageParams.PARAM_LOCKED: bool,  # backward compatibility
     StageParams.PARAM_FROZEN: bool,
     StageParams.PARAM_META: object,
     StageParams.PARAM_ALWAYS_CHANGED: bool,
@@ -69,22 +68,20 @@
     Output.PARAM_PLOT_HEADER: bool,
 }
 PLOT_PROPS_SCHEMA = {**OUT_PSTAGE_DETAILED_SCHEMA[str], **PLOT_PROPS}
 PLOT_PSTAGE_SCHEMA = {str: Any(PLOT_PROPS_SCHEMA, [PLOT_PROPS_SCHEMA])}
 
 PARAM_PSTAGE_NON_DEFAULT_SCHEMA = {str: [str]}
 
-VARS_SCHEMA = [str, dict]
 
 STAGE_DEFINITION = {
     Required(StageParams.PARAM_CMD): Any(str, list),
     Optional(StageParams.PARAM_WDIR): str,
     Optional(StageParams.PARAM_DEPS): [str],
     Optional(StageParams.PARAM_PARAMS): [Any(str, dict)],
-    Optional(VARS_KWD): VARS_SCHEMA,
     Optional(StageParams.PARAM_FROZEN): bool,
     Optional(StageParams.PARAM_META): object,
     Optional(StageParams.PARAM_DESC): str,
     Optional(StageParams.PARAM_ALWAYS_CHANGED): bool,
     Optional(StageParams.PARAM_OUTS): [Any(str, OUT_PSTAGE_DETAILED_SCHEMA)],
     Optional(StageParams.PARAM_METRICS): [Any(str, OUT_PSTAGE_DETAILED_SCHEMA)],
     Optional(StageParams.PARAM_PLOTS): [Any(str, PLOT_PSTAGE_SCHEMA)],
@@ -118,15 +115,15 @@
 }
 SINGLE_PIPELINE_STAGE_SCHEMA = {
     str: either_or(STAGE_DEFINITION, FOREACH_IN, [FOREACH_KWD, DO_KWD])
 }
 MULTI_STAGE_SCHEMA = {
     PLOTS: [Any(str, SINGLE_PLOT_SCHEMA)],
     STAGES: SINGLE_PIPELINE_STAGE_SCHEMA,
-    VARS_KWD: VARS_SCHEMA,
+    VARS_KWD: [str, dict],
     StageParams.PARAM_PARAMS: [str],
     StageParams.PARAM_METRICS: [str],
     ARTIFACTS: SINGLE_ARTIFACT_SCHEMA,
 }
 
 COMPILED_SINGLE_STAGE_SCHEMA = Schema(SINGLE_STAGE_SCHEMA)
 COMPILED_MULTI_STAGE_SCHEMA = Schema(MULTI_STAGE_SCHEMA)
```

### Comparing `dvc-3.0.0a1/dvc/scm.py` & `dvc-3.0.0a2/dvc/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/stage/__init__.py` & `dvc-3.0.0a2/dvc/stage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,21 +386,22 @@
             self.dvcfile.remove_stage(self)
 
     def transfer(
         self,
         source: str,
         odb: Optional["ObjectDB"] = None,
         to_remote: bool = False,
-        **kwargs: Any,
+        jobs: Optional[int] = None,
+        force: bool = False,
     ) -> None:
         assert len(self.outs) == 1
         (out,) = self.outs
-        out.transfer(source, odb=odb, jobs=kwargs.get("jobs"))
+        out.transfer(source, odb=odb, jobs=jobs)
         if not to_remote:
-            out.checkout(force=kwargs.get("force"))
+            out.checkout(force=force)
             out.ignore()
 
     @rwlocked(read=["deps"], write=["outs"])
     def reproduce(self, interactive=False, **kwargs) -> Optional["Stage"]:
         if not (
             kwargs.get("force", False)
             or self.changed(kwargs.get("allow_missing", False))
@@ -712,19 +713,14 @@
 
     def outs_cached(self) -> bool:
         return all(
             not out.changed_cache() if out.use_cache else not out.changed()
             for out in self.outs
         )
 
-    def get_all_files_number(self, filter_info=None) -> int:
-        return sum(
-            out.get_files_number(filter_info) for out in self.filter_outs(filter_info)
-        )
-
     def get_used_objs(
         self, *args, **kwargs
     ) -> Dict[Optional["ObjectDB"], Set["HashInfo"]]:
         """Return set of object IDs used by this stage."""
         if self.is_partial_import and not self.is_repo_import:
             return {}
```

### Comparing `dvc-3.0.0a1/dvc/stage/cache.py` & `dvc-3.0.0a2/dvc/stage/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/stage/decorators.py` & `dvc-3.0.0a2/dvc/stage/decorators.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/stage/exceptions.py` & `dvc-3.0.0a2/dvc/stage/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/stage/imports.py` & `dvc-3.0.0a2/dvc/stage/imports.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def _update_import_on_remote(stage, remote, jobs):
     if stage.is_repo_import:
         raise InvalidArgumentError(
             "Data imported from other DVC or Git repositories can't "
             "be updated with --to-remote"
         )
 
+    stage.save_deps()
     url = stage.deps[0].def_path
     odb = stage.repo.cloud.get_remote_odb(remote, "update")
     stage.outs[0].transfer(url, odb=odb, jobs=jobs, update=True)
 
 
 def update_import(
     stage, rev=None, to_remote=False, remote=None, no_download=None, jobs=None
```

### Comparing `dvc-3.0.0a1/dvc/stage/loader.py` & `dvc-3.0.0a2/dvc/stage/loader.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/stage/run.py` & `dvc-3.0.0a2/dvc/stage/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/stage/serialize.py` & `dvc-3.0.0a2/dvc/stage/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/stage/utils.py` & `dvc-3.0.0a2/dvc/stage/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,32 +221,30 @@
 
 
 def prepare_file_path(kwargs) -> str:
     """Determine file path from the first output name.
 
     Used in creating .dvc files.
     """
-    from dvc.dvcfile import DVC_FILE, DVC_FILE_SUFFIX
+    from dvc.dvcfile import DVC_FILE_SUFFIX
 
     out = first(
         concat(
             kwargs.get("outs", []),
             kwargs.get("outs_no_cache", []),
             kwargs.get("metrics", []),
             kwargs.get("metrics_no_cache", []),
             kwargs.get("plots", []),
             kwargs.get("plots_no_cache", []),
             kwargs.get("outs_persist", []),
             kwargs.get("outs_persist_no_cache", []),
         )
     )
-
-    return (
-        os.path.basename(os.path.normpath(out)) + DVC_FILE_SUFFIX if out else DVC_FILE
-    )
+    assert out
+    return os.path.basename(os.path.normpath(out)) + DVC_FILE_SUFFIX
 
 
 def check_stage_exists(repo: "Repo", stage: Union["Stage", "PipelineStage"], path: str):
     from dvc.dvcfile import load_file
     from dvc.stage import PipelineStage
     from dvc.stage.exceptions import DuplicateStageName, StageFileAlreadyExistsError
```

### Comparing `dvc-3.0.0a1/dvc/testing/README.rst` & `dvc-3.0.0a2/dvc/testing/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/api_tests.py` & `dvc-3.0.0a2/dvc/testing/api_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_checkout.py` & `dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_data_status.py` & `dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_plots.py` & `dvc-3.0.0a2/dvc/testing/benchmarks/cli/commands/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/test_modify_data.py` & `dvc-3.0.0a2/dvc/testing/benchmarks/cli/stories/test_modify_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/benchmarks/fixtures.py` & `dvc-3.0.0a2/dvc/testing/benchmarks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/benchmarks/plugin.py` & `dvc-3.0.0a2/dvc/testing/benchmarks/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/cloud.py` & `dvc-3.0.0a2/dvc/testing/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/fixtures.py` & `dvc-3.0.0a2/dvc/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/path_info.py` & `dvc-3.0.0a2/dvc/testing/path_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/plugin.py` & `dvc-3.0.0a2/dvc/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/remote_tests.py` & `dvc-3.0.0a2/dvc/testing/remote_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/tmp_dir.py` & `dvc-3.0.0a2/dvc/testing/tmp_dir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/testing/workspace_tests.py` & `dvc-3.0.0a2/dvc/testing/workspace_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/ui/__init__.py` & `dvc-3.0.0a2/dvc/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/ui/_rich_progress.py` & `dvc-3.0.0a2/dvc/ui/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/ui/pager.py` & `dvc-3.0.0a2/dvc/ui/pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/ui/table.py` & `dvc-3.0.0a2/dvc/ui/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/updater.py` & `dvc-3.0.0a2/dvc/updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/__init__.py` & `dvc-3.0.0a2/dvc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/cli_parse.py` & `dvc-3.0.0a2/dvc/utils/cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/diff.py` & `dvc-3.0.0a2/dvc/utils/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/fs.py` & `dvc-3.0.0a2/dvc/utils/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/humanize.py` & `dvc-3.0.0a2/dvc/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/hydra.py` & `dvc-3.0.0a2/dvc/utils/hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/serialize/__init__.py` & `dvc-3.0.0a2/dvc/utils/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/serialize/_common.py` & `dvc-3.0.0a2/dvc/utils/serialize/_common.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/serialize/_json.py` & `dvc-3.0.0a2/dvc/utils/serialize/_json.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/serialize/_py.py` & `dvc-3.0.0a2/dvc/utils/serialize/_py.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/serialize/_toml.py` & `dvc-3.0.0a2/dvc/utils/serialize/_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/serialize/_yaml.py` & `dvc-3.0.0a2/dvc/utils/serialize/_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/strictyaml.py` & `dvc-3.0.0a2/dvc/utils/strictyaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/studio.py` & `dvc-3.0.0a2/dvc/utils/studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/table.py` & `dvc-3.0.0a2/dvc/utils/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc/utils/threadpool.py` & `dvc-3.0.0a2/dvc/utils/threadpool.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/dvc.egg-info/PKG-INFO` & `dvc-3.0.0a2/dvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.0.0a1/dvc.egg-info/SOURCES.txt` & `dvc-3.0.0a2/dvc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -384,19 +384,17 @@
 tests/func/test_move.py
 tests/func/test_odb.py
 tests/func/test_remote.py
 tests/func/test_remove.py
 tests/func/test_repo.py
 tests/func/test_repo_index.py
 tests/func/test_repro.py
-tests/func/test_repro_multistage.py
 tests/func/test_root.py
+tests/func/test_run.py
 tests/func/test_run_cache.py
-tests/func/test_run_multistage.py
-tests/func/test_run_single_stage.py
 tests/func/test_scm.py
 tests/func/test_scm_context.py
 tests/func/test_stage.py
 tests/func/test_stage_load.py
 tests/func/test_state.py
 tests/func/test_status.py
 tests/func/test_unprotect.py
@@ -555,15 +553,14 @@
 tests/unit/render/test_image_converter.py
 tests/unit/render/test_match.py
 tests/unit/render/test_vega_converter.py
 tests/unit/repo/__init__.py
 tests/unit/repo/test_open_repo.py
 tests/unit/repo/test_repo.py
 tests/unit/repo/test_reproduce.py
-tests/unit/repo/test_run.py
 tests/unit/repo/test_scm_context.py
 tests/unit/repo/experiments/__init__.py
 tests/unit/repo/experiments/conftest.py
 tests/unit/repo/experiments/test_executor_status.py
 tests/unit/repo/experiments/test_remove.py
 tests/unit/repo/experiments/test_utils.py
 tests/unit/repo/experiments/queue/__init__.py
```

### Comparing `dvc-3.0.0a1/dvc.egg-info/requires.txt` & `dvc-3.0.0a2/dvc.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 colorama>=0.3.9
 configobj>=5.0.6
 distro>=1.3
 dpath<3,>=2.1.0
-dvc-data<0.52,>=0.51.0
+dvc-data<0.55,>=0.54.3
 dvc-http>=2.29.0
 dvc-render<1,>=0.3.1
 dvc-studio-client<1,>=0.9.2
 dvc-task<1,>=0.2.1
 flatten_dict<1,>=0.4.1
 flufl.lock>=5
 funcy>=1.14
@@ -33,15 +33,15 @@
 voluptuous>=0.11.7
 zc.lockfile>=1.2.1
 
 [all]
 dvc[azure,gdrive,gs,hdfs,oss,s3,ssh,webdav,webhdfs]
 
 [azure]
-dvc-azure==2.21.1
+dvc-azure>=2.21.2
 
 [dev]
 dvc[azure,gdrive,gs,hdfs,lint,oss,s3,ssh,terraform,tests,webdav,webhdfs]
 
 [gdrive]
 dvc-gdrive==2.19.2
 
@@ -94,14 +94,15 @@
 pytest-mock
 pytest-test-utils
 pytest-timeout>=2
 pytest-xdist>=3.2
 
 [tests:sys_platform == "win32"]
 pywin32>=225
+tzdata
 
 [webdav]
 dvc-webdav==2.19.1
 
 [webhdfs]
 dvc-webhdfs==2.19
```

### Comparing `dvc-3.0.0a1/pyproject.toml` & `dvc-3.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 dynamic = ["version"]
 dependencies = [
     "colorama>=0.3.9",
     "configobj>=5.0.6",
     "distro>=1.3",
     "dpath<3,>=2.1.0",
-    "dvc-data>=0.51.0,<0.52",
+    "dvc-data>=0.54.3,<0.55",
     "dvc-http>=2.29.0",
     "dvc-render>=0.3.1,<1",
     "dvc-studio-client>=0.9.2,<1",
     "dvc-task>=0.2.1,<1",
     "flatten_dict<1,>=0.4.1",
     "flufl.lock>=5",
     "funcy>=1.14",
@@ -63,15 +63,15 @@
     "tomlkit>=0.11.1",
     "tqdm<5,>=4.63.1",
     "voluptuous>=0.11.7",
     "zc.lockfile>=1.2.1",
 ]
 [project.optional-dependencies]
 all = ["dvc[azure,gdrive,gs,hdfs,oss,s3,ssh,webdav,webhdfs]"]
-azure = ["dvc-azure==2.21.1"]
+azure = ["dvc-azure>=2.21.2"]
 dev = ["dvc[azure,gdrive,gs,hdfs,lint,oss,s3,ssh,terraform,tests,webdav,webhdfs]"]
 gdrive = ["dvc-gdrive==2.19.2"]
 gs = ["dvc-gs==2.22.1"]
 hdfs = ["dvc-hdfs==2.19"]
 lint = [
     "mypy==1.3.0",
     "pylint==2.17.4",
@@ -103,14 +103,15 @@
     "pytest-docker>=1,<2",
     "pytest-lazy-fixture",
     "pytest-mock",
     "pytest-test-utils",
     "pytest-timeout>=2",
     "pytest-xdist>=3.2",
     'pywin32>=225; sys_platform == "win32"', # optional test dependency
+    'tzdata; sys_platform == "win32"',  # for testing with celery
 ]
 webdav = ["dvc-webdav==2.19.1"]
 webhdfs = ["dvc-webhdfs==2.19"]
 webhdfs_kerberos = ["dvc-webhdfs[kerberos]==2.19"]
 [project.urls]
 Documentation = "https://dvc.org/doc"
 Issues = "https://github.com/iterative/dvc/issues"
```

### Comparing `dvc-3.0.0a1/scripts/build.py` & `dvc-3.0.0a2/scripts/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/fpm/build.py` & `dvc-3.0.0a2/scripts/fpm/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/fpm/notarize.py` & `dvc-3.0.0a2/scripts/fpm/notarize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/fpm/sign.py` & `dvc-3.0.0a2/scripts/fpm/sign.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/innosetup/addSymLinkPermissions.ps1` & `dvc-3.0.0a2/scripts/innosetup/addSymLinkPermissions.ps1`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/innosetup/addsymlink.iss` & `dvc-3.0.0a2/scripts/innosetup/addsymlink.iss`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/innosetup/build.py` & `dvc-3.0.0a2/scripts/innosetup/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/innosetup/modpath.iss` & `dvc-3.0.0a2/scripts/innosetup/modpath.iss`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/innosetup/setup.iss` & `dvc-3.0.0a2/scripts/innosetup/setup.iss`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/pyinstaller/build.py` & `dvc-3.0.0a2/scripts/pyinstaller/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.py` & `dvc-3.0.0a2/scripts/pyinstaller/hooks/hook-dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/scripts/pyinstaller/sign.py` & `dvc-3.0.0a2/scripts/pyinstaller/sign.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/conftest.py` & `dvc-3.0.0a2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import sys
 from contextlib import suppress
 
 import pytest
 
 from dvc import env
+from dvc.stage import PipelineStage
 from dvc.testing.fixtures import *  # noqa, pylint: disable=wildcard-import
 
 from .dir_helpers import *  # noqa, pylint: disable=wildcard-import
 from .remotes import *  # noqa, pylint: disable=wildcard-import
 from .scripts import *  # noqa, pylint: disable=wildcard-import
 
 # Prevent updater and analytics from running their processes
@@ -237,14 +238,16 @@
             single_stage=single_stage,
             name=name,
             **kwargs,
         )
 
         if hasattr(tmp_dir.dvc, "scm"):
             files = [stage.path]
+            if isinstance(stage, PipelineStage):
+                files += [stage.dvcfile._lockfile.path]
             files += [out.fs_path for out in stage.outs if not out.use_cache]
             tmp_dir.dvc.scm.add(files)
             if commit:
                 tmp_dir.dvc.scm.commit(commit)
             if tag:
                 tmp_dir.dvc.scm.tag(tag)
         return stage
```

### Comparing `dvc-3.0.0a1/tests/dir_helpers.py` & `dvc-3.0.0a2/tests/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/api/test_data.py` & `dvc-3.0.0a2/tests/func/api/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 def test_open_not_cached(dvc):
     metric_file = "metric.txt"
     metric_content = "0.6"
     metric_code = f"open('{metric_file}', 'w').write('{metric_content}')"
     dvc.run(
-        single_stage=True,
+        name="write-metric",
         metrics_no_cache=[metric_file],
         cmd=f'python -c "{metric_code}"',
     )
 
     with api.open(metric_file) as fd:
         assert fd.read() == metric_content
```

### Comparing `dvc-3.0.0a1/tests/func/api/test_experiments.py` & `dvc-3.0.0a2/tests/func/api/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/api/test_scm.py` & `dvc-3.0.0a2/tests/func/api/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/api/test_show.py` & `dvc-3.0.0a2/tests/func/api/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/artifacts/test_artifacts.py` & `dvc-3.0.0a2/tests/func/artifacts/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/data/db/test_index.py` & `dvc-3.0.0a2/tests/func/data/db/test_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/conftest.py` & `dvc-3.0.0a2/tests/func/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/executor/test_ssh.py` & `dvc-3.0.0a2/tests/func/experiments/executor/test_ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_apply.py` & `dvc-3.0.0a2/tests/func/experiments/test_apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_diff.py` & `dvc-3.0.0a2/tests/func/experiments/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_experiments.py` & `dvc-3.0.0a2/tests/func/experiments/test_experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,15 +580,19 @@
         assert (tmp_dir / "metrics.yaml").read_text().strip() == params
         assert (tmp_dir / "data").read_text().strip() == "modified"
 
 
 def test_exp_run_recursive(tmp_dir, scm, dvc, run_copy_metrics):
     tmp_dir.dvc_gen("metric_t.json", '{"foo": 1}')
     run_copy_metrics(
-        "metric_t.json", "metric.json", metrics=["metric.json"], no_exec=True
+        "metric_t.json",
+        "metric.json",
+        metrics=["metric.json"],
+        no_exec=True,
+        name="copy-metric",
     )
     assert dvc.experiments.run(".", recursive=True)
     assert (tmp_dir / "metric.json").parse() == {"foo": 1}
 
 
 def test_experiment_name_invalid(tmp_dir, scm, dvc, exp_stage, mocker):
     from dvc.exceptions import InvalidArgumentError
```

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_queue.py` & `dvc-3.0.0a2/tests/func/experiments/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_remote.py` & `dvc-3.0.0a2/tests/func/experiments/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_remove.py` & `dvc-3.0.0a2/tests/func/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_save.py` & `dvc-3.0.0a2/tests/func/experiments/test_save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_set_params.py` & `dvc-3.0.0a2/tests/func/experiments/test_set_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_show.py` & `dvc-3.0.0a2/tests/func/experiments/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_stash_exp.py` & `dvc-3.0.0a2/tests/func/experiments/test_stash_exp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/experiments/test_utils.py` & `dvc-3.0.0a2/tests/func/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/machine/conftest.py` & `dvc-3.0.0a2/tests/func/machine/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/machine/test_machine_config.py` & `dvc-3.0.0a2/tests/func/machine/test_machine_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/machine/test_machine_status.py` & `dvc-3.0.0a2/tests/func/machine/test_machine_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/metrics/test_diff.py` & `dvc-3.0.0a2/tests/func/metrics/test_diff.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from dvc.cli import main
 from dvc.utils import relpath
 
 
 def test_metrics_diff_simple(tmp_dir, scm, dvc, run_copy_metrics):
     def _gen(val):
         tmp_dir.gen({"m_temp.yaml": str(val)})
-        run_copy_metrics("m_temp.yaml", "m.yaml", metrics=["m.yaml"])
+        run_copy_metrics(
+            "m_temp.yaml", "m.yaml", name="copy-metrics", metrics=["m.yaml"]
+        )
         dvc.scm.commit(str(val))
 
     _gen(1)
     _gen(2)
     _gen(3)
 
     expected = {"m.yaml": {"": {"old": 1, "new": 3, "diff": 2}}}
@@ -22,15 +24,21 @@
     assert dvc.metrics.diff(a_rev="HEAD~2") == expected
 
 
 def test_metrics_diff_yaml(tmp_dir, scm, dvc, run_copy_metrics):
     def _gen(val):
         metrics = {"a": {"b": {"c": val, "d": 1, "e": str(val)}}}
         (tmp_dir / "m_temp.yaml").dump(metrics)
-        run_copy_metrics("m_temp.yaml", "m.yaml", metrics=["m.yaml"], commit=str(val))
+        run_copy_metrics(
+            "m_temp.yaml",
+            "m.yaml",
+            name="copy-metrics",
+            metrics=["m.yaml"],
+            commit=str(val),
+        )
 
     _gen(1)
     _gen(2)
     _gen(3)
 
     expected = {
         "m.yaml": {
@@ -42,15 +50,21 @@
     assert dvc.metrics.diff(a_rev="HEAD~2") == expected
 
 
 def test_metrics_diff_json(tmp_dir, scm, dvc, run_copy_metrics):
     def _gen(val):
         metrics = {"a": {"b": {"c": val, "d": 1, "e": str(val)}}}
         (tmp_dir / "m_temp.json").dump(metrics)
-        run_copy_metrics("m_temp.json", "m.json", metrics=["m.json"], commit=str(val))
+        run_copy_metrics(
+            "m_temp.json",
+            "m.json",
+            name="copy-metrics",
+            metrics=["m.json"],
+            commit=str(val),
+        )
 
     _gen(1)
     _gen(2)
     _gen(3)
 
     expected = {
         "m.json": {
@@ -61,29 +75,36 @@
     assert dvc.metrics.diff(a_rev="HEAD~2") == expected
 
 
 def test_metrics_diff_json_unchanged(tmp_dir, scm, dvc, run_copy_metrics):
     def _gen(val):
         metrics = {"a": {"b": {"c": val, "d": 1, "e": str(val)}}}
         (tmp_dir / "m_temp.json").dump(metrics)
-        run_copy_metrics("m_temp.json", "m.json", metrics=["m.json"], commit=str(val))
+        run_copy_metrics(
+            "m_temp.json",
+            "m.json",
+            name="copy-metrics",
+            metrics=["m.json"],
+            commit=str(val),
+        )
 
     _gen(1)
     _gen(2)
     _gen(1)
 
     assert dvc.metrics.diff(a_rev="HEAD~2") == {}
 
 
 def test_metrics_diff_broken_json(tmp_dir, scm, dvc, run_copy_metrics):
     metrics = {"a": {"b": {"c": 1, "d": 1, "e": "3"}}}
     (tmp_dir / "m_temp.json").dump(metrics)
     run_copy_metrics(
         "m_temp.json",
         "m.json",
+        name="copy-metrics",
         metrics_no_cache=["m.json"],
         commit="add metrics",
     )
 
     (tmp_dir / "m.json").write_text(json.dumps(metrics) + "ma\nlformed\n")
 
     assert dvc.metrics.diff() == {
@@ -99,15 +120,17 @@
     tmp_dir.scm_gen({"foo": "foo"}, commit="add foo")
     assert dvc.metrics.diff(a_rev="HEAD~1") == {}
 
 
 def test_metrics_diff_new_metric(tmp_dir, scm, dvc, run_copy_metrics):
     metrics = {"a": {"b": {"c": 1, "d": 1, "e": "3"}}}
     (tmp_dir / "m_temp.json").dump(metrics)
-    run_copy_metrics("m_temp.json", "m.json", metrics_no_cache=["m.json"])
+    run_copy_metrics(
+        "m_temp.json", "m.json", name="copy-metrics", metrics_no_cache=["m.json"]
+    )
 
     assert dvc.metrics.diff() == {
         "m.json": {
             "a.b.e": {"old": None, "new": "3"},
             "a.b.c": {"old": None, "new": 1},
             "a.b.d": {"old": None, "new": 1},
         }
@@ -116,14 +139,15 @@
 
 def test_metrics_diff_deleted_metric(tmp_dir, scm, dvc, run_copy_metrics):
     metrics = {"a": {"b": {"c": 1, "d": 1, "e": "3"}}}
     (tmp_dir / "m_temp.json").dump(metrics)
     run_copy_metrics(
         "m_temp.json",
         "m.json",
+        name="copy-metrics",
         metrics_no_cache=["m.json"],
         commit="add metrics",
     )
 
     (tmp_dir / "m.json").unlink()
 
     assert dvc.metrics.diff() == {
@@ -136,14 +160,15 @@
 
 
 def test_metrics_diff_with_unchanged(tmp_dir, scm, dvc, run_copy_metrics):
     tmp_dir.gen("metrics_temp.yaml", "foo: 1\nxyz: 10")
     run_copy_metrics(
         "metrics_temp.yaml",
         "metrics.yaml",
+        name="copy-metrics",
         metrics_no_cache=["metrics.yaml"],
         commit="1",
     )
 
     tmp_dir.scm_gen("metrics.yaml", "foo: 2\nxyz: 10", commit="2")
     tmp_dir.scm_gen("metrics.yaml", "foo: 3\nxyz: 10", commit="3")
 
@@ -164,15 +189,17 @@
 
     assert Repo.init().metrics.diff() == {}
 
 
 def test_metrics_diff_dirty(tmp_dir, scm, dvc, run_copy_metrics):
     def _gen(val):
         tmp_dir.gen({"m_temp.yaml": str(val)})
-        run_copy_metrics("m_temp.yaml", "m.yaml", metrics=["m.yaml"])
+        run_copy_metrics(
+            "m_temp.yaml", "m.yaml", name="copy-metrics", metrics=["m.yaml"]
+        )
         dvc.scm.commit(str(val))
 
     _gen(1)
     _gen(2)
     _gen(3)
 
     tmp_dir.gen({"m.yaml": "4"})
@@ -181,15 +208,17 @@
 
     assert dvc.metrics.diff() == expected
 
 
 def test_metrics_diff_cli(tmp_dir, scm, dvc, run_copy_metrics, caplog, capsys):
     def _gen(val):
         tmp_dir.gen({"m_temp.yaml": f"foo: {val}"})
-        run_copy_metrics("m_temp.yaml", "m.yaml", metrics=["m.yaml"])
+        run_copy_metrics(
+            "m_temp.yaml", "m.yaml", name="copy-metrics", metrics=["m.yaml"]
+        )
         dvc.scm.commit(str(val))
 
     _gen(1.23456789)
     _gen(2.34567891011)
     _gen(3.45678910111213)
 
     caplog.clear()
@@ -239,14 +268,20 @@
     }
 
 
 def test_metrics_diff_active_branch_unchanged(tmp_dir, scm, dvc, run_copy_metrics):
     def _gen(val):
         metrics = {"a": {"b": {"c": val, "d": 1, "e": str(val)}}}
         (tmp_dir / "m_temp.yaml").dump(metrics)
-        run_copy_metrics("m_temp.yaml", "m.yaml", metrics=["m.yaml"], commit=str(val))
+        run_copy_metrics(
+            "m_temp.yaml",
+            "m.yaml",
+            name="copy-metric",
+            metrics=["m.yaml"],
+            commit=str(val),
+        )
 
     _gen(1)
     _gen(2)
     _gen(1)
 
     assert dvc.metrics.diff(a_rev=tmp_dir.scm.active_branch()) == {}
```

### Comparing `dvc-3.0.0a1/tests/func/metrics/test_show.py` & `dvc-3.0.0a2/tests/func/metrics/test_show.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 from dvc.repo import Repo
 from dvc.utils.fs import remove
 from dvc.utils.serialize import JSONFileCorruptedError, YAMLFileCorruptedError
 
 
 def test_show_simple(tmp_dir, dvc, run_copy_metrics):
     tmp_dir.gen("metrics_t.yaml", "1.1")
-    run_copy_metrics("metrics_t.yaml", "metrics.yaml", metrics=["metrics.yaml"])
+    run_copy_metrics(
+        "metrics_t.yaml", "metrics.yaml", name="copy-metrics", metrics=["metrics.yaml"]
+    )
     assert dvc.metrics.show() == {"": {"data": {"metrics.yaml": {"data": 1.1}}}}
 
 
 def test_show_simple_from_subdir(tmp_dir, dvc, run_copy_metrics):
     subdir = tmp_dir / "subdir"
     subdir.mkdir()
     tmp_dir.gen("metrics_t.yaml", "1.1")
     run_copy_metrics(
         "metrics_t.yaml",
         "subdir/metrics.yaml",
+        name="copy-metrics",
         metrics=["subdir/metrics.yaml"],
     )
 
     expected_path = os.path.join("subdir", "metrics.yaml")
     assert dvc.metrics.show() == {"": {"data": {expected_path: {"data": 1.1}}}}
 
     expected_path = os.path.join("..", "subdir", "metrics.yaml")
@@ -36,50 +39,59 @@
     subdir2.mkdir()
     with subdir2.chdir():
         assert dvc.metrics.show() == {"": {"data": {expected_path: {"data": 1.1}}}}
 
 
 def test_show(tmp_dir, dvc, run_copy_metrics):
     tmp_dir.gen("metrics_t.yaml", "foo: 1.1")
-    run_copy_metrics("metrics_t.yaml", "metrics.yaml", metrics=["metrics.yaml"])
+    run_copy_metrics(
+        "metrics_t.yaml", "metrics.yaml", name="copy-metrics", metrics=["metrics.yaml"]
+    )
     assert dvc.metrics.show() == {
         "": {"data": {"metrics.yaml": {"data": {"foo": 1.1}}}}
     }
 
 
 def test_show_toml(tmp_dir, dvc, run_copy_metrics):
     tmp_dir.gen("metrics_t.toml", "[foo]\nbar = 1.2")
-    run_copy_metrics("metrics_t.toml", "metrics.toml", metrics=["metrics.toml"])
+    run_copy_metrics(
+        "metrics_t.toml", "metrics.toml", name="copy-metrics", metrics=["metrics.toml"]
+    )
     assert dvc.metrics.show() == {
         "": {"data": {"metrics.toml": {"data": {"foo": {"bar": 1.2}}}}}
     }
 
 
 def test_show_targets(tmp_dir, dvc, run_copy_metrics):
     tmp_dir.gen("metrics_t.yaml", "foo: 1.1")
-    run_copy_metrics("metrics_t.yaml", "metrics.yaml", metrics=["metrics.yaml"])
+    run_copy_metrics(
+        "metrics_t.yaml", "metrics.yaml", name="copy-metrics", metrics=["metrics.yaml"]
+    )
     expected = {"": {"data": {"metrics.yaml": {"data": {"foo": 1.1}}}}}
     assert dvc.metrics.show(targets=["metrics.yaml"]) == expected
     assert dvc.metrics.show(targets=(tmp_dir / "metrics.yaml").fs_path) == expected
 
 
 def test_show_multiple(tmp_dir, dvc, run_copy_metrics):
     tmp_dir.gen("foo_temp", "foo: 1\n")
     tmp_dir.gen("baz_temp", "baz: 2\n")
-    run_copy_metrics("foo_temp", "foo", fname="foo.dvc", metrics=["foo"])
-    run_copy_metrics("baz_temp", "baz", fname="baz.dvc", metrics=["baz"])
+    run_copy_metrics("foo_temp", "foo", name="copy-to-foo", metrics=["foo"])
+    run_copy_metrics("baz_temp", "baz", name="copy-to-baz", metrics=["baz"])
     assert dvc.metrics.show() == {
         "": {"data": {"foo": {"data": {"foo": 1}}, "baz": {"data": {"baz": 2}}}}
     }
 
 
 def test_show_branch(tmp_dir, scm, dvc, run_copy_metrics):
     tmp_dir.gen("metrics_temp.yaml", "foo: 1")
     run_copy_metrics(
-        "metrics_temp.yaml", "metrics.yaml", metrics_no_cache=["metrics.yaml"]
+        "metrics_temp.yaml",
+        "metrics.yaml",
+        name="copy-metrics",
+        metrics_no_cache=["metrics.yaml"],
     )
     scm.add(["metrics.yaml", "metrics.yaml.dvc"])
     scm.commit("init")
 
     with tmp_dir.branch("branch", new=True):
         tmp_dir.scm_gen("metrics.yaml", "foo: 2", commit="branch")
 
@@ -100,40 +112,46 @@
     with subrepo_dir.chdir():
         dvc = Repo.init(subdir=True)
         scm.commit("init dvc")
 
         dvc.run(
             cmd="echo foo: 1 > metrics.yaml",
             metrics=["metrics.yaml"],
-            single_stage=True,
+            name="generate-metrics",
         )
 
     scm.add(
         [
             str(subrepo_dir / "metrics.yaml"),
-            str(subrepo_dir / "metrics.yaml.dvc"),
+            str(subrepo_dir / "dvc.yaml"),
+            str(subrepo_dir / "dvc.lock"),
         ]
     )
     scm.commit("init metrics")
     scm.tag("v1")
 
     expected_path = os.path.join("subdir", "metrics.yaml")
     assert dvc.metrics.show(all_tags=True) == {
         "workspace": {"data": {expected_path: {"data": {"foo": 1}}}},
         "v1": {"data": {expected_path: {"data": {"foo": 1}}}},
     }
 
 
 def test_missing_cache(tmp_dir, dvc, run_copy_metrics):
     tmp_dir.gen("metrics_t.yaml", "1.1")
-    run_copy_metrics("metrics_t.yaml", "metrics.yaml", metrics=["metrics.yaml"])
+    run_copy_metrics(
+        "metrics_t.yaml", "metrics.yaml", name="copy-metrics", metrics=["metrics.yaml"]
+    )
 
     # This one should be skipped
     stage = run_copy_metrics(
-        "metrics_t.yaml", "metrics2.yaml", metrics=["metrics2.yaml"]
+        "metrics_t.yaml",
+        "metrics2.yaml",
+        name="copy-metrics2",
+        metrics=["metrics2.yaml"],
     )
     remove(stage.outs[0].fspath)
     remove(stage.outs[0].cache_path)
 
     result = dvc.metrics.show()
     metrics2 = result[""]["data"].pop("metrics2.yaml")
     assert isinstance(metrics2["error"], FileNotFoundError)
@@ -179,19 +197,19 @@
         "branch": {"data": {"metrics.yaml": {"data": {"foo": 2.2}}}},
     }
 
     if not use_dvc:
         assert not (tmp_dir / ".dvc").exists()
 
 
-def test_non_metric_and_recurisve_show(tmp_dir, dvc, run_copy_metrics):
+def test_non_metric_and_recursive_show(tmp_dir, dvc, run_copy_metrics):
     tmp_dir.gen({"metrics_t.yaml": "foo: 1.1", "metrics": {"metric1.yaml": "bar: 1.2"}})
 
     metric2 = os.fspath(tmp_dir / "metrics" / "metric2.yaml")
-    run_copy_metrics("metrics_t.yaml", metric2, metrics=[metric2])
+    run_copy_metrics("metrics_t.yaml", metric2, name="copy-metric2", metrics=[metric2])
 
     assert dvc.metrics.show(targets=["metrics_t.yaml", "metrics"], recursive=True) == {
         "": {
             "data": {
                 os.path.join("metrics", "metric1.yaml"): {"data": {"bar": 1.2}},
                 os.path.join("metrics", "metric2.yaml"): {"data": {"foo": 1.1}},
                 "metrics_t.yaml": {"data": {"foo": 1.1}},
```

### Comparing `dvc-3.0.0a1/tests/func/params/test_diff.py` & `dvc-3.0.0a2/tests/func/params/test_diff.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,95 +7,95 @@
 
 def test_diff_no_params(tmp_dir, scm, dvc):
     assert dvc.params.diff() == {}
 
 
 def test_diff_no_changes(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo: bar")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     scm.add(["params.yaml", "Dvcfile"])
     scm.commit("bar")
     assert dvc.params.diff() == {}
 
 
 def test_diff(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo: bar")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     scm.add(["params.yaml", "Dvcfile"])
     scm.commit("bar")
 
     tmp_dir.scm_gen("params.yaml", "foo: baz", commit="baz")
     tmp_dir.scm_gen("params.yaml", "foo: qux", commit="qux")
 
     assert dvc.params.diff(a_rev="HEAD~2") == {
         "params.yaml": {"foo": {"old": "bar", "new": "qux"}}
     }
 
 
 def test_diff_dirty(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo: bar")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     scm.add(["params.yaml", "Dvcfile"])
     scm.commit("bar")
 
     tmp_dir.scm_gen("params.yaml", "foo: baz", commit="baz")
     tmp_dir.gen("params.yaml", "foo: qux")
 
     assert dvc.params.diff() == {"params.yaml": {"foo": {"old": "baz", "new": "qux"}}}
 
 
 def test_diff_new(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo: bar")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
 
     assert dvc.params.diff() == {"params.yaml": {"foo": {"old": None, "new": "bar"}}}
 
 
 def test_diff_deleted(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo: bar")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     scm.add(["params.yaml", "Dvcfile"])
     scm.commit("bar")
 
     (tmp_dir / "params.yaml").unlink()
 
     assert dvc.params.diff() == {"params.yaml": {"foo": {"old": "bar", "new": None}}}
 
 
 def test_diff_list(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo:\n- bar\n- baz")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     scm.add(["params.yaml", "Dvcfile"])
     scm.commit("foo")
 
     tmp_dir.gen("params.yaml", "foo:\n- bar\n- baz\n- qux")
 
     assert dvc.params.diff() == {
         "params.yaml": {
             "foo": {"old": "['bar', 'baz']", "new": "['bar', 'baz', 'qux']"}
         }
     }
 
 
 def test_diff_dict(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo:\n  bar: baz")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     scm.add(["params.yaml", "Dvcfile"])
     scm.commit("foo")
 
     tmp_dir.gen("params.yaml", "foo:\n  bar: qux")
 
     assert dvc.params.diff() == {
         "params.yaml": {"foo.bar": {"old": "baz", "new": "qux"}}
     }
 
 
 def test_diff_with_unchanged(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo: bar\nxyz: val")
-    dvc.run(cmd="echo params.yaml", params=["foo,xyz"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo,xyz"], name="echo-params")
     scm.add(["params.yaml", "Dvcfile"])
     scm.commit("bar")
 
     tmp_dir.scm_gen("params.yaml", "foo: baz\nxyz: val", commit="baz")
     tmp_dir.scm_gen("params.yaml", "foo: qux\nxyz: val", commit="qux")
 
     assert dvc.params.diff(a_rev="HEAD~2", all=True) == {
@@ -257,11 +257,11 @@
     assert dvc.params.diff() == {
         relpath(directory / params_file): {"foo": {"diff": 2, "new": 5, "old": 3}}
     }
 
 
 def test_diff_active_branch_no_changes(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo: bar")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     scm.add(["params.yaml", "Dvcfile"])
     scm.commit("bar")
     assert dvc.params.diff(a_rev=tmp_dir.scm.active_branch()) == {}
```

### Comparing `dvc-3.0.0a1/tests/func/params/test_show.py` & `dvc-3.0.0a2/tests/func/params/test_show.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,87 +10,77 @@
 
 def test_show_empty(dvc):
     assert dvc.params.show() == {}
 
 
 def test_show(tmp_dir, dvc):
     tmp_dir.gen("params.yaml", "foo: bar")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     assert dvc.params.show() == {
         "": {"data": {"params.yaml": {"data": {"foo": "bar"}}}}
     }
 
 
 def test_show_targets(tmp_dir, dvc):
     tmp_dir.gen("params.yaml", "foo: bar")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     expected = {"": {"data": {"params.yaml": {"data": {"foo": "bar"}}}}}
     assert dvc.params.show(targets=["params.yaml"]) == expected
     assert dvc.params.show(targets=(tmp_dir / "params.yaml").fs_path) == expected
 
 
 def test_show_toml(tmp_dir, dvc):
     tmp_dir.gen("params.toml", "[foo]\nbar = 42\nbaz = [1, 2]\n")
-    dvc.run(cmd="echo params.toml", params=["params.toml:foo"], single_stage=True)
+    dvc.run(cmd="echo params.toml", params=["params.toml:foo"], name="echo-params")
     assert dvc.params.show() == {
         "": {"data": {"params.toml": {"data": {"foo": {"bar": 42, "baz": [1, 2]}}}}}
     }
 
 
 def test_show_py(tmp_dir, dvc):
     tmp_dir.gen(
         "params.py",
         "CONST = 1\nIS_DIR: bool = True\n\n\nclass Config:\n    foo = 42\n",
     )
     dvc.run(
         cmd="echo params.py",
         params=["params.py:CONST,IS_DIR,Config.foo"],
-        single_stage=True,
+        name="echo-params",
     )
     assert dvc.params.show() == {
         "": {
             "data": {
                 "params.py": {
                     "data": {"CONST": 1, "Config": {"foo": 42}, "IS_DIR": True}
                 }
             }
         }
     }
 
 
 def test_show_multiple(tmp_dir, dvc):
     tmp_dir.gen("params.yaml", "foo: bar\nbaz: qux\n")
-    dvc.run(
-        cmd="echo params.yaml",
-        fname="foo.dvc",
-        params=["foo"],
-        single_stage=True,
-    )
-    dvc.run(
-        cmd="echo params.yaml",
-        fname="baz.dvc",
-        params=["baz"],
-        single_stage=True,
-    )
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params1")
+    dvc.run(cmd="echo params.yaml", params=["baz"], name="echo-params2")
     assert dvc.params.show() == {
         "": {"data": {"params.yaml": {"data": {"baz": "qux", "foo": "bar"}}}}
     }
 
 
 def test_show_list(tmp_dir, dvc):
     tmp_dir.gen("params.yaml", "foo:\n- bar\n- baz\n")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     assert dvc.params.show() == {
         "": {"data": {"params.yaml": {"data": {"foo": ["bar", "baz"]}}}}
     }
 
 
 def test_show_branch(tmp_dir, scm, dvc):
     tmp_dir.gen("params.yaml", "foo: bar")
-    dvc.run(cmd="echo params.yaml", params=["foo"], single_stage=True)
+    dvc.run(cmd="echo params.yaml", params=["foo"], name="echo-params")
     scm.add(["params.yaml", "Dvcfile"])
     scm.commit("init")
 
     with tmp_dir.branch("branch", new=True):
         tmp_dir.scm_gen("params.yaml", "foo: baz", commit="branch")
 
     assert dvc.params.show(revs=["branch"]) == {
```

### Comparing `dvc-3.0.0a1/tests/func/parsing/__init__.py` & `dvc-3.0.0a2/tests/func/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/parsing/test_errors.py` & `dvc-3.0.0a2/tests/func/parsing/test_errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,39 +5,26 @@
 import re
 
 import pytest
 
 from dvc.parsing import ResolveError
 from dvc.parsing.context import Context
 from dvc.parsing.interpolate import embrace
-from dvc.utils.humanize import join
 
 from . import make_entry_definition, make_foreach_def
 
 
 def escape_ansi(line):
     ansi_escape = re.compile(r"(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]")
     return ansi_escape.sub("", line)
 
 
 # Tests for the interpolated entries
 
 
-@pytest.mark.parametrize("vars_", ["${file}_params.yaml", {"foo": "${foo}"}])
-def test_vars_interpolation_errors(tmp_dir, dvc, vars_):
-    definition = make_entry_definition(tmp_dir, "build", {"vars": [vars_]})
-    with pytest.raises(ResolveError) as exc_info:
-        definition.resolve()
-
-    assert (
-        str(exc_info.value) == "failed to parse 'stages.build.vars' in 'dvc.yaml': "
-        "interpolating is not allowed"
-    )
-
-
 def test_failed_to_interpolate(tmp_dir, dvc):
     context = Context(models={"foo": "bar"})
     definition = make_entry_definition(
         tmp_dir, "build", {"cmd": "echo ${models.foo.}"}, context
     )
 
     with pytest.raises(ResolveError) as exc_info:
@@ -50,31 +37,14 @@
         "            ^\n"
         "ParseException: Expected end of text, found '.'"
         "  (at char 12), (line:1, col:13)"
     )
     assert definition.context == {"models": {"foo": "bar"}}
 
 
-def test_local_vars_params_file_not_exist(tmp_dir, dvc):
-    definition = make_entry_definition(
-        tmp_dir,
-        "build",
-        {"vars": ["not_existing_params.yaml"], "cmd": "echo ${models.foo}"},
-    )
-
-    with pytest.raises(ResolveError) as exc_info:
-        definition.resolve()
-
-    assert (
-        str(exc_info.value) == "failed to parse stage 'build' in 'dvc.yaml': "
-        "'not_existing_params.yaml' does not exist"
-    )
-    assert not definition.context
-
-
 def test_specified_key_does_not_exist(tmp_dir, dvc):
     definition = make_entry_definition(
         tmp_dir,
         "build",
         {"cmd": "echo ${models.foobar}"},
         Context(models={"foo": "foo"}),
     )
@@ -145,33 +115,14 @@
 
     assert (
         str(exc_info.value) == "failed to parse 'stages.build.cmd' in 'dvc.yaml':\n"
         "Cannot interpolate nested iterable in 'list'"
     )
 
 
-def test_partial_vars_doesnot_exist(tmp_dir, dvc):
-    (tmp_dir / "test_params.yaml").dump({"sub1": "sub1", "sub2": "sub2"})
-
-    definition = make_entry_definition(
-        tmp_dir,
-        "build",
-        {"vars": ["test_params.yaml:sub3"], "cmd": "echo ${sub1} ${sub2}"},
-    )
-
-    with pytest.raises(ResolveError) as exc_info:
-        definition.resolve()
-
-    assert (
-        str(exc_info.value) == "failed to parse stage 'build' in 'dvc.yaml': "
-        "could not find 'sub3' in 'test_params.yaml'"
-    )
-    assert not definition.context
-
-
 # Tests foreach generated stages and their error messages
 
 
 def test_foreach_data_syntax_error(tmp_dir, dvc):
     definition = make_foreach_def(tmp_dir, "build", "${syntax.[error}", {})
     with pytest.raises(ResolveError) as exc_info:
         definition.resolve_all()
@@ -280,55 +231,14 @@
         == f"failed to parse '{loc}' in 'dvc.yaml': Could not find '{key}'"
     )
 
     # should have no `item` and `key` even though it failed to resolve.
     assert context == {"foo": "bar"}
 
 
-@pytest.mark.parametrize(
-    "redefine",
-    [
-        {"item": 5},
-        {"key": 5},
-        {"item": 5, "key": 10},
-        {"item": {"epochs": 10}},
-    ],
-)
-@pytest.mark.parametrize("from_file", [True, False])
-def test_item_key_in_generated_stage_vars(tmp_dir, dvc, redefine, from_file):
-    context = Context(foo="bar")
-    vars_ = [redefine]
-    if from_file:
-        (tmp_dir / "test_params.yaml").dump(redefine)
-        vars_ = ["test_params.yaml"]
-
-    definition = make_foreach_def(
-        tmp_dir,
-        "build",
-        {"model1": {"thresh": "10"}, "model2": {"thresh": 5}},
-        {"vars": vars_, "cmd": "${item}"},
-        context,
-    )
-
-    with pytest.raises(ResolveError) as exc_info:
-        definition.resolve_all()
-
-    message = str(exc_info.value)
-    assert (
-        "failed to parse stage 'build@model1' in 'dvc.yaml': "
-        "attempted to modify reserved" in message
-    )
-
-    key_or_keys = "keys" if len(redefine) > 1 else "key"
-    assert f"{key_or_keys} {join(redefine)}" in message
-    if from_file:
-        assert "in 'test_params.yaml'" in message
-    assert context == {"foo": "bar"}
-
-
 def test_foreach_wdir_key_does_not_exist(tmp_dir, dvc):
     definition = make_foreach_def(
         tmp_dir,
         "build",
         "${models}",
         {"wdir": "${ite}", "cmd": "echo ${item}"},
         Context(models=["foo", "bar"]),
```

### Comparing `dvc-3.0.0a1/tests/func/parsing/test_foreach.py` & `dvc-3.0.0a2/tests/func/parsing/test_foreach.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Testing happy paths for the foreach."""
-import os
 
 import pytest
 
-from dvc.parsing import DEFAULT_PARAMS_FILE, DataResolver, ForeachDefinition
+from dvc.parsing import DataResolver, ForeachDefinition
 from dvc.parsing.context import Context
 
 
 def test_with_simple_list_data(tmp_dir, dvc):
     """Testing a simple non-nested list as a foreach data"""
     resolver = DataResolver(dvc, tmp_dir.fs_path, {})
 
@@ -266,142 +265,14 @@
         "build@bar": {"wdir": "bar", "cmd": "echo hello"},
     }
 
     assert not resolver.context
     assert not any(item for item in resolver.tracked_vars.values())
 
 
-def test_foreach_with_local_vars(tmp_dir, dvc):
-    resolver = DataResolver(dvc, (tmp_dir / "data").fs_path, {})
-    foreach_data = ["foo", "bar"]
-    data = {
-        "foreach": foreach_data,
-        "do": {
-            "vars": [{"foobar": "foobar"}],
-            "cmd": "echo ${item} ${foobar}",
-        },
-    }
-    definition = ForeachDefinition(resolver, resolver.context, "build", data)
-
-    assert definition.resolve_all() == {
-        # note that the resolver generates `wdir` relative to file's wdir
-        # so, this is just `foo`, not `data/foo`.
-        # figuring out `wdir` is the responsibility of the `load_stage`/`Stage`
-        "build@foo": {"cmd": "echo foo foobar"},
-        "build@bar": {"cmd": "echo bar foobar"},
-    }
-    assert not resolver.context
-    assert not any(item for item in resolver.tracked_vars.values())
-
-
-@pytest.mark.parametrize(
-    "local_import",
-    [
-        "test_params.yaml",
-        "test_params.yaml:train",
-        "test_params.yaml:train,prepare",
-    ],
-)
-def test_foreach_with_imported_vars(tmp_dir, dvc, local_import):
-    (tmp_dir / "params.yaml").dump({"models": {"model1": {"thresh": "foo"}}})
-    (tmp_dir / "test_params.yaml").dump(
-        {"train": {"epochs": 10}, "prepare": {"nums": 25}}
-    )
-    resolver = DataResolver(dvc, tmp_dir.fs_path, {})
-    foreach_data = ["foo", "bar"]
-    data = {
-        "foreach": foreach_data,
-        "do": {"vars": [local_import], "cmd": "echo ${item} ${train.epochs}"},
-    }
-    definition = ForeachDefinition(resolver, resolver.context, "build", data)
-
-    assert definition.resolve_all() == {
-        # note that the resolver generates `wdir` relative to file's wdir
-        # so, this is just `foo`, not `data/foo`.
-        # figuring out `wdir` is the responsibility of the `load_stage`/`Stage`
-        "build@foo": {"cmd": "echo foo 10"},
-        "build@bar": {"cmd": "echo bar 10"},
-    }
-
-    assert resolver.context == {"models": {"model1": {"thresh": "foo"}}}
-    assert resolver.tracked_vars == {
-        "build@foo": {"test_params.yaml": {"train.epochs": 10}},
-        "build@bar": {"test_params.yaml": {"train.epochs": 10}},
-    }
-
-
-@pytest.mark.parametrize("local_import", ["params.yaml", "params.yaml:train,prepare"])
-def test_foreach_with_interpolated_wdir_and_local_vars(tmp_dir, dvc, local_import):
-    (tmp_dir / "params.yaml").dump({"models": {"model1": {"thresh": "foo"}}})
-
-    for i in range(5):
-        build_dir = tmp_dir / ("model-" + str(i))
-        build_dir.mkdir()
-        (build_dir / "params.yaml").dump(
-            {"train": {"epochs": 1 + i}, "prepare": {"nums": 10 * i}},
-        )
-
-    resolver = DataResolver(dvc, tmp_dir.fs_path, {})
-    data = {
-        "foreach": [0, 1, 2, 3, 4],
-        "do": {
-            "wdir": "model-${item}",
-            "vars": [local_import],
-            "cmd": "echo ${item} ${train.epochs} ${prepare.nums}",
-        },
-    }
-    definition = ForeachDefinition(resolver, resolver.context, "build", data)
-
-    assert definition.resolve_all() == {
-        # note that the resolver generates `wdir` relative to file's wdir
-        # so, this is just `foo`, not `data/foo`.
-        # figuring out `wdir` is the responsibility of the `load_stage`/`Stage`
-        "build@0": {"wdir": "model-0", "cmd": "echo 0 1 0"},
-        "build@1": {"wdir": "model-1", "cmd": "echo 1 2 10"},
-        "build@2": {"wdir": "model-2", "cmd": "echo 2 3 20"},
-        "build@3": {"wdir": "model-3", "cmd": "echo 3 4 30"},
-        "build@4": {"wdir": "model-4", "cmd": "echo 4 5 40"},
-    }
-
-    assert resolver.context == {"models": {"model1": {"thresh": "foo"}}}
-    assert resolver.tracked_vars == {
-        "build@0": {
-            os.path.join("model-0", "params.yaml"): {
-                "train.epochs": 1,
-                "prepare.nums": 0,
-            }
-        },
-        "build@1": {
-            os.path.join("model-1", "params.yaml"): {
-                "train.epochs": 2,
-                "prepare.nums": 10,
-            }
-        },
-        "build@2": {
-            os.path.join("model-2", "params.yaml"): {
-                "train.epochs": 3,
-                "prepare.nums": 20,
-            }
-        },
-        "build@3": {
-            os.path.join("model-3", "params.yaml"): {
-                "train.epochs": 4,
-                "prepare.nums": 30,
-            }
-        },
-        "build@4": {
-            os.path.join("model-4", "params.yaml"): {
-                "train.epochs": 5,
-                "prepare.nums": 40,
-            }
-        },
-    }
-    assert resolver.context.imports == {DEFAULT_PARAMS_FILE: None}
-
-
 def test_foreach_do_syntax_is_checked_once(tmp_dir, dvc, mocker):
     do_def = {"cmd": "python script.py --epochs ${item}"}
     data = {"foreach": [0, 1, 2, 3, 4], "do": do_def}
     definition = ForeachDefinition(
         DataResolver(dvc, tmp_dir.fs_path, {}), Context(), "build", data
     )
     mock = mocker.patch("dvc.parsing.check_syntax_errors", return_value=True)
```

### Comparing `dvc-3.0.0a1/tests/func/parsing/test_interpolated_entry.py` & `dvc-3.0.0a2/tests/func/parsing/test_interpolated_entry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from copy import deepcopy
 
 import pytest
 
 from dvc.dependency import _merge_params
 from dvc.parsing import DEFAULT_PARAMS_FILE, DataResolver
 from dvc.parsing.context import recurse_not_a_node
@@ -68,155 +67,14 @@
         resolver.resolve(), {"stages": {"stage1": {"cmd": "echo foobar bar"}}}
     )
     assert resolver.tracked_vars == {
         "stage1": {DEFAULT_PARAMS_FILE: {"dict.bar": "bar"}}
     }
 
 
-def test_stage_with_wdir(tmp_dir, dvc):
-    """
-    Test that params file from wdir are also loaded
-    """
-    d = {
-        "stages": {
-            "stage1": {
-                "cmd": "echo ${dict.foo} ${dict.bar}",
-                "params": ["value1"],
-                "wdir": "data",
-                "vars": [DEFAULT_PARAMS_FILE],
-            }
-        }
-    }
-
-    data_dir = tmp_dir / "data"
-    data_dir.mkdir()
-    (tmp_dir / DEFAULT_PARAMS_FILE).dump({"dict": {"bar": "bar"}})
-    (data_dir / DEFAULT_PARAMS_FILE).dump({"dict": {"foo": "foo"}})
-    resolver = DataResolver(dvc, tmp_dir.fs_path, d)
-
-    assert_stage_equal(
-        resolver.resolve(),
-        {
-            "stages": {
-                "stage1": {
-                    "cmd": "echo foo bar",
-                    "wdir": "data",
-                    "params": ["value1"],
-                }
-            }
-        },
-    )
-    assert resolver.tracked_vars == {
-        "stage1": {
-            os.path.join("data", DEFAULT_PARAMS_FILE): {"dict.foo": "foo"},
-            DEFAULT_PARAMS_FILE: {"dict.bar": "bar"},
-        }
-    }
-
-
-def test_with_templated_wdir(tmp_dir, dvc):
-    """
-    Test that params from the resolved wdir are still loaded
-    and is used in the interpolation.
-    """
-    d = {
-        "stages": {
-            "stage1": {
-                "cmd": "echo ${dict.foo} ${dict.bar}",
-                "params": ["value1"],
-                "wdir": "${dict.ws}",
-                "vars": [DEFAULT_PARAMS_FILE],
-            }
-        }
-    }
-    (tmp_dir / DEFAULT_PARAMS_FILE).dump({"dict": {"bar": "bar", "ws": "data"}})
-    data_dir = tmp_dir / "data"
-    data_dir.mkdir()
-    (data_dir / DEFAULT_PARAMS_FILE).dump({"dict": {"foo": "foo"}})
-    resolver = DataResolver(dvc, tmp_dir.fs_path, d)
-
-    assert_stage_equal(
-        resolver.resolve(),
-        {
-            "stages": {
-                "stage1": {
-                    "cmd": "echo foo bar",
-                    "wdir": "data",
-                    "params": ["value1"],
-                }
-            }
-        },
-    )
-    assert resolver.tracked_vars == {
-        "stage1": {
-            os.path.join("data", DEFAULT_PARAMS_FILE): {"dict.foo": "foo"},
-            DEFAULT_PARAMS_FILE: {"dict.bar": "bar", "dict.ws": "data"},
-        }
-    }
-    assert resolver.context.imports == {"params.yaml": None}
-    assert resolver.context == {"dict": {"bar": "bar", "ws": "data"}}
-
-
-def test_resolve_local_tries_to_load_globally_used_files(tmp_dir, dvc):
-    iterable = {"bar": "bar", "foo": "foo"}
-    (tmp_dir / "params.json").dump(iterable)
-
-    d = {
-        "vars": ["params.json"],
-        "stages": {
-            "build": {
-                "cmd": "command --value ${bar}",
-                "params": [{"params.json": ["foo"]}],
-                "vars": ["params.json"],
-            }
-        },
-    }
-    resolver = DataResolver(dvc, tmp_dir.fs_path, d)
-    assert_stage_equal(
-        resolver.resolve(),
-        {
-            "stages": {
-                "build": {
-                    "cmd": "command --value bar",
-                    "params": [{"params.json": ["foo"]}],
-                }
-            }
-        },
-    )
-    assert resolver.tracked_vars == {"build": {"params.json": {"bar": "bar"}}}
-
-
-def test_resolve_local_tries_to_load_globally_used_params_yaml(tmp_dir, dvc):
-    iterable = {"bar": "bar", "foo": "foo"}
-    (tmp_dir / "params.yaml").dump(iterable)
-
-    d = {
-        "stages": {
-            "build": {
-                "cmd": "command --value ${bar}",
-                "params": [{"params.yaml": ["foo"]}],
-                "vars": ["params.yaml"],
-            }
-        }
-    }
-    resolver = DataResolver(dvc, tmp_dir.fs_path, d)
-    assert_stage_equal(
-        resolver.resolve(),
-        {
-            "stages": {
-                "build": {
-                    "cmd": "command --value bar",
-                    "params": [{"params.yaml": ["foo"]}],
-                }
-            }
-        },
-    )
-    assert resolver.tracked_vars == {"build": {"params.yaml": {"bar": "bar"}}}
-
-
 def test_vars_relpath_overwrite(tmp_dir, dvc):
     iterable = {"bar": "bar", "foo": "foo"}
     (tmp_dir / "params.yaml").dump(iterable)
     d = {
         "vars": ["params.yaml"],
         "stages": {
             "build": {
@@ -227,32 +85,27 @@
         },
     }
     resolver = DataResolver(dvc, tmp_dir.fs_path, d)
     resolver.resolve()
     assert resolver.context.imports == {"params.yaml": None}
 
 
-@pytest.mark.parametrize("local", [True, False])
 @pytest.mark.parametrize(
     "vars_",
     [
         ["test_params.yaml:bar", "test_params.yaml:foo"],
         ["test_params.yaml:foo,bar"],
         ["test_params.yaml"],
         ["test_params.yaml", "test_params.yaml"],
     ],
 )
-def test_vars_load_partial(tmp_dir, dvc, local, vars_):
+def test_vars_load_partial(tmp_dir, dvc, vars_):
     iterable = {"bar": "bar", "foo": "foo"}
     (tmp_dir / "test_params.yaml").dump(iterable)
-    d = {"stages": {"build": {"cmd": "echo ${bar}"}}}
-    if local:
-        d["stages"]["build"]["vars"] = vars_
-    else:
-        d["vars"] = vars_
+    d = {"vars": vars_, "stages": {"build": {"cmd": "echo ${bar}"}}}
     resolver = DataResolver(dvc, tmp_dir.fs_path, d)
     resolver.resolve()
 
 
 @pytest.mark.parametrize(
     "bool_config, list_config",
     [(None, None), ("store_true", "nargs"), ("boolean_optional", "append")],
```

### Comparing `dvc-3.0.0a1/tests/func/parsing/test_resolver.py` & `dvc-3.0.0a2/tests/func/parsing/test_resolver.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,48 +140,23 @@
 
     assert (
         str(exc_info.value) == "failed to parse 'vars' in 'dvc.yaml': "
         "'not_existing_params.yaml' does not exist"
     )
 
 
-@pytest.mark.parametrize("local", [True, False])
 @pytest.mark.parametrize(
     "vars_",
     [
         ["test_params.yaml", "test_params.yaml:sub1"],
         ["test_params.yaml:sub1", "test_params.yaml"],
         ["test_params.yaml:sub1", "test_params.yaml:sub1,sub2"],
     ],
 )
-def test_vars_already_loaded_message(tmp_dir, dvc, local, vars_):
-    d = {"stages": {"build": {"cmd": "echo ${sub1} ${sub2}"}}}
+def test_vars_already_loaded_message(tmp_dir, dvc, vars_):
+    d = {"vars": vars_, "stages": {"build": {"cmd": "echo ${sub1} ${sub2}"}}}
     (tmp_dir / "test_params.yaml").dump({"sub1": "sub1", "sub2": "sub2"})
-    if not local:
-        d["vars"] = vars_
-    else:
-        d["stages"]["build"]["vars"] = vars_
 
     with pytest.raises(ResolveError) as exc_info:  # noqa: PT012
         resolver = DataResolver(dvc, tmp_dir.fs_path, d)
         resolver.resolve()
     assert "partially" in str(exc_info.value)
-
-
-@pytest.mark.parametrize(
-    "vars_, loc", [(DATA, "build.vars[0]"), ("params.json", "params.json")]
-)
-def test_local_overwrite_error(tmp_dir, dvc, vars_, loc):
-    (tmp_dir / DEFAULT_PARAMS_FILE).dump(DATA)
-    (tmp_dir / "params.json").dump(DATA)
-
-    d = {"stages": {"build": {"cmd": "echo ${models.foo}", "vars": [vars_]}}}
-
-    resolver = DataResolver(dvc, tmp_dir.fs_path, d)
-    with pytest.raises(ResolveError) as exc_info:
-        resolver.resolve()
-
-    assert (
-        str(exc_info.value) == "failed to parse stage 'build' in 'dvc.yaml':\n"
-        f"cannot redefine 'models.bar' from '{loc}' "
-        "as it already exists in 'params.yaml'"
-    )
```

### Comparing `dvc-3.0.0a1/tests/func/plots/test_diff.py` & `dvc-3.0.0a2/tests/func/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/plots/test_modify.py` & `dvc-3.0.0a2/tests/func/plots/test_modify.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/plots/test_show.py` & `dvc-3.0.0a2/tests/func/plots/test_show.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 def test_plot_cache_missing(tmp_dir, scm, dvc, caplog, run_copy_metrics):
     metric1 = [{"y": 2}, {"y": 3}]
     (tmp_dir / "metric_t.json").dump_json(metric1, sort_keys=True)
     run_copy_metrics(
         "metric_t.json",
         "metric.json",
         plots=["metric.json"],
+        name="copy-metric",
         commit="there is metric",
     )
     scm.tag("v1")
 
     # Make a different plot and then remove its datafile
     metric2 = [{"y": 3}, {"y": 4}]
     (tmp_dir / "metric_t.json").dump_json(metric2, sort_keys=True)
     stage = run_copy_metrics(
         "metric_t.json",
         "metric.json",
         plots=["metric.json"],
+        name="copy-metric",
         commit="there is an another metric",
     )
     scm.tag("v2")
     remove(stage.outs[0].fspath)
     remove(stage.outs[0].cache_path)
 
     plots_data = dvc.plots.show(revs=["v1", "v2"], targets=["metric.json"])
@@ -60,14 +62,15 @@
 
 def test_plot_wrong_metric_type(tmp_dir, scm, dvc, run_copy_metrics):
     tmp_dir.gen("metric_t.txt", "some text")
     run_copy_metrics(
         "metric_t.txt",
         "metric.txt",
         plots_no_cache=["metric.txt"],
+        name="copy-metric",
         commit="add text metric",
     )
 
     result = dvc.plots.show(targets=["metric.txt"], onerror=onerror_collect)
     assert isinstance(
         get_plot(result, "workspace", file="metric.txt", endkey="error"),
         PlotMetricTypeError,
@@ -206,15 +209,17 @@
     }
 
 
 def test_ignore_parsing_error(tmp_dir, dvc, run_copy_metrics):
     with open("file", "wb", encoding=None) as fobj:
         fobj.write(b"\xc1")
 
-    run_copy_metrics("file", "plot_file.json", plots=["plot_file.json"])
+    run_copy_metrics(
+        "file", "plot_file.json", plots=["plot_file.json"], name="copy-metric"
+    )
     result = dvc.plots.show(onerror=onerror_collect)
 
     assert isinstance(
         get_plot(result, "workspace", file="plot_file.json", endkey="error"),
         EncodingError,
     )
 
@@ -300,23 +305,23 @@
     p2 = os.path.join("subdir", "p2.json")
     subdir_stage = tmp_dir.dvc.run(
         cmd=(
             f"mkdir subdir && python copy.py {sname} {p1} && "
             f"python copy.py {sname} {p2}"
         ),
         deps=[sname],
-        single_stage=False,
         plots=["subdir"],
         name="copy_double",
     )
 
     run_copy_metrics(
         pname,
         "plot.json",
         plots=["plot.json"],
+        name="copy-metric",
         commit="there is metric",
     )
 
     remove(subdir_stage.outs[0].cache_path)
     remove(subdir_stage.outs[0].fs_path)
 
     result = dvc.plots.show()
```

### Comparing `dvc-3.0.0a1/tests/func/test_add.py` & `dvc-3.0.0a2/tests/func/test_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,48 +2,41 @@
 import filecmp
 import os
 import shutil
 import stat
 import textwrap
 from unittest.mock import call
 
-import colorama
 import pytest
 
-import dvc as dvc_module
 import dvc_data
 from dvc.cachemgr import CacheManager
 from dvc.cli import main
 from dvc.config import ConfigError
 from dvc.dvcfile import DVC_FILE_SUFFIX
-from dvc.exceptions import (
-    DvcException,
-    InvalidArgumentError,
-    OverlappingOutputPathsError,
-    RecursiveAddingWhileUsingFilename,
-)
+from dvc.exceptions import DvcException, OverlappingOutputPathsError
 from dvc.fs import LocalFileSystem, system
 from dvc.output import (
     OutputAlreadyTrackedError,
     OutputDoesNotExistError,
     OutputIsStageFileError,
 )
 from dvc.stage import Stage
 from dvc.stage.exceptions import StageExternalOutputsError, StagePathNotFoundError
 from dvc.testing.workspace_tests import TestAdd
-from dvc.utils import LARGE_DIR_SIZE
 from dvc.utils.fs import path_isin
 from dvc.utils.serialize import YAMLFileCorruptedError
 from dvc_data.hashfile.hash import file_md5
 from dvc_data.hashfile.hash_info import HashInfo
 from tests.utils import get_gitignore_content
 
 
 def test_add(tmp_dir, dvc):
-    (stage,) = tmp_dir.dvc_gen({"foo": "foo"})
+    tmp_dir.gen("foo", "foo")
+    (stage,) = dvc.add("foo")
     md5 = file_md5("foo", dvc.fs)
 
     assert stage is not None
 
     assert isinstance(stage, Stage)
     assert os.path.isfile(stage.path)
     assert len(stage.outs) == 1
@@ -110,40 +103,14 @@
 
     obj = load(dvc.cache.local, hash_info)
     for key, _, _ in obj:
         for part in key:
             assert "\\" not in part
 
 
-def test_add_directory_recursive(tmp_dir, dvc):
-    tmp_dir.gen("data", {"file1": "file1", "sub": {"file2": "file2"}})
-    stages = dvc.add("data", recursive=True)
-    assert len(stages) == 2
-
-
-def test_add_cmd_directory_recursive(tmp_dir, dvc):
-    tmp_dir.gen("data", {"file1": "file1", "sub": {"file2": "file2"}})
-    assert main(["add", "--recursive", "data"]) == 0
-
-
-def test_warn_about_large_directories_recursive_add(tmp_dir, dvc, capsys):
-    warning = (
-        "You are adding a large directory 'large-dir' recursively."
-        "\nConsider tracking it as a whole instead with "
-        "`{cyan}dvc add large-dir{nc}`"
-    ).format(
-        cyan=colorama.Fore.CYAN,
-        nc=colorama.Style.RESET_ALL,
-    )
-
-    tmp_dir.gen("large-dir", {f"{i}": f"{i}" for i in range(LARGE_DIR_SIZE + 1)})
-    assert main(["add", "--recursive", "large-dir"]) == 0
-    assert warning in capsys.readouterr()[1]
-
-
 def test_add_directory_with_forward_slash(tmp_dir, dvc):
     tmp_dir.gen("directory", {"file": "file"})
     (stage,) = dvc.add("directory/")
     assert stage.relpath == "directory.dvc"
 
 
 def test_add_tracked_file(tmp_dir, scm, dvc):
@@ -361,19 +328,19 @@
     ret = main(["status"])
     assert ret == 0
     assert file_md5_counter.mock.call_count == 1
 
     os.rename("foo", "foo.back")
     ret = main(["checkout"])
     assert ret == 0
-    assert file_md5_counter.mock.call_count == 1
+    assert file_md5_counter.mock.call_count == 2
 
     ret = main(["status"])
     assert ret == 0
-    assert file_md5_counter.mock.call_count == 1
+    assert file_md5_counter.mock.call_count == 2
 
 
 def test_should_update_state_entry_for_directory_after_add(mocker, dvc, tmp_dir):
     file_md5_counter = mocker.spy(dvc_data.hashfile.hash, "file_md5")
 
     tmp_dir.gen({"data/data": "foo", "data/data_sub/sub_data": "foo"})
 
@@ -387,19 +354,19 @@
     ret = main(["status"])
     assert ret == 0
     assert file_md5_counter.mock.call_count == 5
 
     os.rename("data", "data.back")
     ret = main(["checkout"])
     assert ret == 0
-    assert file_md5_counter.mock.call_count == 5
+    assert file_md5_counter.mock.call_count == 6
 
     ret = main(["status"])
     assert ret == 0
-    assert file_md5_counter.mock.call_count == 6
+    assert file_md5_counter.mock.call_count == 7
 
 
 def test_add_commit(tmp_dir, dvc):
     tmp_dir.gen("foo", "foo")
     ret = main(["add", "foo", "--no-commit"])
     assert ret == 0
     assert os.path.isfile("foo")
@@ -475,42 +442,14 @@
     tmp_dir.gen({"foo": "foo"})
     (tmp_dir / "out").write_text("old contents")
 
     assert main(["add", "foo", "--out", "out", "--force"]) == 0
     assert (tmp_dir / "foo").read_text() == "foo"
 
 
-def test_add_filename(tmp_dir, dvc):
-    tmp_dir.gen({"foo": "foo", "bar": "bar", "data": {"file": "file"}})
-    ret = main(["add", "foo", "bar", "--file", "error.dvc"])
-    assert ret != 0
-
-    ret = main(["add", "-R", "data", "--file", "error.dvc"])
-    assert ret != 0
-
-    with pytest.raises(RecursiveAddingWhileUsingFilename):
-        dvc.add("data", recursive=True, fname="error.dvc")
-
-    ret = main(["add", "data", "--file", "data_directory.dvc"])
-    assert ret == 0
-    assert (tmp_dir / "data_directory.dvc").exists()
-
-    ret = main(["add", "foo", "--file", "bar.dvc"])
-    assert ret == 0
-    assert (tmp_dir / "bar.dvc").exists()
-    assert not (tmp_dir / "foo.dvc").exists()
-
-    (tmp_dir / "bar.dvc").unlink()
-
-    ret = main(["add", "foo", "--file", "bar.dvc"])
-    assert ret == 0
-    assert (tmp_dir / "bar.dvc").exists()
-    assert not (tmp_dir / "foo.dvc").exists()
-
-
 def test_failed_add_cleanup(tmp_dir, scm, dvc):
     tmp_dir.gen({"foo": "foo", "bar": "bar"})
 
     # Add and corrupt a stage file
     dvc.add("foo")
     tmp_dir.gen("foo.dvc", "- broken\nyaml")
 
@@ -519,25 +458,14 @@
 
     assert not os.path.exists("bar.dvc")
 
     gitignore_content = get_gitignore_content()
     assert "/bar" not in gitignore_content
 
 
-def test_should_not_track_git_internal_files(mocker, dvc, tmp_dir):
-    stage_creator_spy = mocker.spy(dvc_module.repo.add, "create_stages")
-
-    ret = main(["add", "-R", dvc.root_dir])
-    assert ret == 0
-
-    created_stages_filenames = stage_creator_spy.mock.call_args[0][1]
-    for fname in created_stages_filenames:
-        assert ".git" not in fname
-
-
 def test_add_unprotected(tmp_dir, dvc):
     tmp_dir.gen("foo", "foo")
     ret = main(["config", "cache.type", "hardlink"])
     assert ret == 0
 
     ret = main(["add", "foo"])
     assert ret == 0
@@ -709,18 +637,18 @@
 
     dvc.add(os.path.join("dir", "file2"))
 
 
 def test_add_parent_dir(tmp_dir, scm, dvc):
     tmp_dir.gen({"dir": {"file1": "file1 content"}})
     out_path = os.path.join("dir", "file1")
-    dvc.add(out_path, fname=out_path + ".dvc")
+    dvc.add(out_path)
 
     with pytest.raises(OverlappingOutputPathsError) as e:
-        dvc.add("dir", fname="dir.dvc")
+        dvc.add("dir")
     assert str(e.value) == (
         "Cannot add 'dir', because it is overlapping with other DVC "
         "tracked output: '{out}'.\n"
         "To include '{out}' in 'dir', run 'dvc remove {out}.dvc' "
         "and then 'dvc add dir'"
     ).format(out=os.path.join("dir", "file1"))
 
@@ -764,15 +692,19 @@
         assert os.path.exists(stage.path)
         assert os.path.exists(stage.outs[0].cache_path)
 
 
 def test_try_adding_pipeline_tracked_output(tmp_dir, dvc, run_copy):
     tmp_dir.dvc_gen("foo", "foo")
     run_copy("foo", "bar", name="copy-foo-bar")
-    with pytest.raises(DvcException, match="cannot update 'bar': not a data source"):
+    msg = (
+        "cannot update 'bar': overlaps with an output of stage: 'copy-foo-bar' in "
+        "'dvc.yaml'.\nRun the pipeline or use 'dvc commit' to force update it."
+    )
+    with pytest.raises(DvcException, match=msg):
         dvc.add("bar")
 
 
 def test_add_pipeline_file(tmp_dir, dvc, run_copy):
     from dvc.dvcfile import PROJECT_FILE
 
     tmp_dir.dvc_gen("foo", "foo")
@@ -934,28 +866,14 @@
     assert foo.read_text() == "foo"
 
     tmp_bar = tmp_abs_dir / "bar"
     with pytest.raises(StageExternalOutputsError):
         dvc.add(str(tmp_foo), out=str(tmp_bar), to_remote=True)
 
 
-@pytest.mark.parametrize(
-    "invalid_opt, kwargs",
-    [
-        ("multiple targets", {"targets": ["foo", "bar", "baz"]}),
-        ("--no-commit", {"targets": ["foo"], "no_commit": True}),
-        ("--recursive", {"targets": ["foo"], "recursive": True}),
-        ("--external", {"targets": ["foo"], "external": True}),
-    ],
-)
-def test_add_to_remote_invalid_combinations(dvc, invalid_opt, kwargs):
-    with pytest.raises(InvalidArgumentError, match=invalid_opt):
-        dvc.add(to_remote=True, **kwargs)
-
-
 def test_add_to_cache_dir(tmp_dir, dvc, local_cloud):
     local_cloud.gen({"data": {"foo": "foo", "bar": "bar"}})
 
     (stage,) = dvc.add(str(local_cloud / "data"), out="data")
     assert len(stage.deps) == 0
     assert len(stage.outs) == 1
     assert stage.outs[0].meta.size == len("foo") + len("bar")
@@ -1023,27 +941,14 @@
     dest_dir.parent.mkdir(parents=True)
     dvc.add(str(local_cloud / "data"), out=str(dest_dir))
 
     assert dest_dir.read_text() == {"foo": "foo", "bar": "bar"}
     assert dest_dir.with_suffix(".dvc").exists()
 
 
-@pytest.mark.parametrize(
-    "invalid_opt, kwargs",
-    [
-        ("multiple targets", {"targets": ["foo", "bar", "baz"]}),
-        ("--no-commit", {"targets": ["foo"], "no_commit": True}),
-        ("--recursive", {"targets": ["foo"], "recursive": True}),
-    ],
-)
-def test_add_to_cache_invalid_combinations(dvc, invalid_opt, kwargs):
-    with pytest.raises(InvalidArgumentError, match=invalid_opt):
-        dvc.add(out="bar", **kwargs)
-
-
 def test_add_to_cache_from_remote(tmp_dir, dvc, workspace):
     workspace.gen("foo", "foo")
 
     url = "remote://workspace/foo"
     dvc.add(url, out="foo")
 
     foo = tmp_dir / "foo"
@@ -1101,23 +1006,14 @@
 
     with pytest.raises(DvcException, match=exc_msg):
         dvc.add("foo")
     assert (tmp_dir / "foo.dvc").exists()
     assert (tmp_dir / stage.path).read_text() == dvcfile_contents
 
 
-def test_add_ignore_duplicated_targets(tmp_dir, dvc, capsys):
-    tmp_dir.gen({"foo": "foo", "bar": "bar", "foobar": "foobar"})
-    stages = dvc.add(["foo", "bar", "foobar", "bar", "foo"])
-
-    _, err = capsys.readouterr()
-    assert len(stages) == 3
-    assert "ignoring duplicated targets: foo, bar" in err
-
-
 def test_add_updates_to_cloud_versioning_dir(tmp_dir, dvc):
     data_dvc = tmp_dir / "data.dvc"
     data_dvc.dump(
         {
             "outs": [
                 {
                     "path": "data",
```

### Comparing `dvc-3.0.0a1/tests/func/test_analytics.py` & `dvc-3.0.0a2/tests/func/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_check_ignore.py` & `dvc-3.0.0a2/tests/func/test_check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_checkout.py` & `dvc-3.0.0a2/tests/func/test_checkout.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,62 +4,53 @@
 import stat
 import textwrap
 
 import pytest
 
 from dvc.cli import main
 from dvc.dvcfile import PROJECT_FILE, load_file
-from dvc.exceptions import (
-    CheckoutError,
-    CheckoutErrorSuggestGit,
-    ConfirmRemoveError,
-    NoOutputOrStageError,
-)
-from dvc.fs import LocalFileSystem, system
-from dvc.stage import Stage
+from dvc.exceptions import CheckoutError, CheckoutErrorSuggestGit, NoOutputOrStageError
+from dvc.fs import system
 from dvc.stage.exceptions import StageFileDoesNotExistError
 from dvc.utils import relpath
 from dvc.utils.fs import remove
-from dvc.utils.serialize import dump_yaml, load_yaml
 from tests.utils import get_gitignore_content
 
 logger = logging.getLogger("dvc")
 
 
 def walk_files(directory):
     for root, _, files in os.walk(directory):
         for f in files:
             yield os.path.join(root, f)
 
 
 def test_checkout(tmp_dir, dvc, copy_script):
     tmp_dir.dvc_gen({"foo": "foo", "data": {"file": "file"}})
     dvc.run(
-        fname="file1.dvc",
         outs=["file1"],
         deps=["foo", "copy.py"],
         cmd="python copy.py foo file1",
-        single_stage=True,
+        name="copy-foo-file1",
     )
     remove(tmp_dir / "foo")
     remove("data")
 
     dvc.checkout(force=True)
     assert (tmp_dir / "foo").read_text() == "foo"
     assert (tmp_dir / "data").read_text() == {"file": "file"}
 
 
 def test_checkout_cli(tmp_dir, dvc, copy_script):
     tmp_dir.dvc_gen({"foo": "foo", "data": {"file": "file"}})
     dvc.run(
-        fname="file1.dvc",
         outs=["file1"],
         deps=["foo", "copy.py"],
         cmd="python copy.py foo file1",
-        single_stage=True,
+        name="copy-foo-file1",
     )
     remove(tmp_dir / "foo")
     remove("data")
 
     assert main(["checkout", "--force"]) == 0
     assert (tmp_dir / "foo").read_text() == "foo"
     assert (tmp_dir / "data").read_text() == {"file": "file"}
@@ -78,15 +69,15 @@
     cache = foo_stage.outs[0].cache_path
 
     os.chmod(cache, 0o644)
     with open(cache, "a", encoding="utf-8") as fd:
         fd.write("1")
 
     with pytest.raises(CheckoutError):
-        dvc.checkout(force=True)
+        dvc.checkout(force=True, relink=True)
 
     assert not os.path.isfile("foo")
     assert not os.path.isfile(cache)
 
 
 def test_checkout_corrupted_cache_dir(tmp_dir, dvc):
     from dvc_data.hashfile import load
@@ -110,15 +101,15 @@
     cache = dvc.cache.local.oid_to_path(entry_oid.value)
 
     os.chmod(cache, 0o644)
     with open(cache, "w+", encoding="utf-8") as fobj:
         fobj.write("1")
 
     with pytest.raises(CheckoutError):
-        dvc.checkout(force=True)
+        dvc.checkout(force=True, relink=True)
 
     assert not os.path.exists(cache)
 
 
 def test_remove_files_when_checkout(tmp_dir, dvc, scm):
     # add the file into a separate branch
     scm.checkout("branch", True)
@@ -180,18 +171,18 @@
 def test_gitignore_basic(tmp_dir, dvc, scm):
     tmp_dir.gen("foo", "foo")
     assert not os.path.exists(scm.GITIGNORE)
 
     tmp_dir.dvc_gen("file1", "random text1", commit="add file1")
     tmp_dir.dvc_gen("file2", "random text2", commit="add file2")
     dvc.run(
-        single_stage=True,
         cmd="cp foo file3",
         deps=["foo"],
         outs_no_cache=["file3"],
+        name="cp-foo-file3",
     )
     assert get_gitignore_content() == ["/file1", "/file2"]
 
 
 def test_gitignore_when_checkout(tmp_dir, dvc, scm):
     tmp_dir.dvc_gen("file_in_a_master", "master", commit="master")
 
@@ -212,27 +203,22 @@
     scm.checkout("branch")
     ret = main(["checkout", "--force"])
     assert ret == 0
     ignored = get_gitignore_content()
     assert "/file_in_a_branch" in ignored
 
 
-def test_checkout_missing_md5_in_stage_file(tmp_dir, dvc, copy_script):
+def test_checkout_missing_md5_in_lock_file_for_outs_deps(tmp_dir, dvc, copy_script):
     tmp_dir.dvc_gen({"foo": "foo", "data": {"file": "file"}})
-    stage = dvc.run(
-        fname="file1.dvc",
+    dvc.stage.add(
         outs=["file1"],
         deps=["foo", "copy.py"],
         cmd="python copy.py foo file1",
-        single_stage=True,
+        name="copy-file",
     )
-    d = load_yaml(stage.relpath)
-    del d[Stage.PARAM_OUTS][0][LocalFileSystem.PARAM_CHECKSUM]
-    del d[Stage.PARAM_DEPS][0][LocalFileSystem.PARAM_CHECKSUM]
-    dump_yaml(stage.relpath, d)
 
     with pytest.raises(CheckoutError):
         dvc.checkout(force=True)
 
 
 def test_checkout_empty_dir(tmp_dir, dvc):
     empty_dir = tmp_dir / "empty_dir"
@@ -250,36 +236,35 @@
 
 def test_checkout_not_cached_file(tmp_dir, dvc):
     tmp_dir.dvc_gen("foo", "foo")
     dvc.run(
         cmd="cp foo bar",
         deps=["foo"],
         outs_no_cache=["bar"],
-        single_stage=True,
+        name="copy-file",
     )
     stats = dvc.checkout(force=True)
     assert not any(stats.values())
 
 
 def test_checkout_with_deps_cli(tmp_dir, dvc, copy_script):
     tmp_dir.dvc_gen({"foo": "foo", "data": {"file": "file"}})
     dvc.run(
-        fname="file1.dvc",
         outs=["file1"],
         deps=["foo", "copy.py"],
         cmd="python copy.py foo file1",
-        single_stage=True,
+        name="copy-file",
     )
     remove("foo")
     remove("file1")
 
     assert not os.path.exists("foo")
     assert not os.path.exists("file1")
 
-    ret = main(["checkout", "--force", "file1.dvc", "--with-deps"])
+    ret = main(["checkout", "--force", "copy-file", "--with-deps"])
     assert ret == 0
 
     assert os.path.exists("foo")
     assert os.path.exists("file1")
 
 
 def test_checkout_directory(tmp_dir, dvc):
@@ -290,27 +275,14 @@
 
     ret = main(["checkout", stage.path])
     assert ret == 0
 
     assert os.path.exists("data")
 
 
-def test_checkout_hook(mocker, tmp_dir, dvc):
-    """Test that dvc checkout handles EOFError gracefully, which is what
-    it will experience when running in a git hook.
-    """
-    tmp_dir.dvc_gen({"data": {"foo": "foo"}})
-    mocker.patch("sys.stdout.isatty", return_value=True)
-    mocker.patch("dvc.prompt.input", side_effect=EOFError)
-
-    (tmp_dir / "data").gen("test", "test")
-    with pytest.raises(ConfirmRemoveError):
-        dvc.checkout()
-
-
 def test_checkout_suggest_git(tmp_dir, dvc, scm):
     with pytest.raises(CheckoutErrorSuggestGit) as e:
         dvc.checkout(targets="gitbranch")
     assert isinstance(e.value.__cause__, NoOutputOrStageError)
     assert isinstance(e.value.__cause__.__cause__, StageFileDoesNotExistError)
 
     with pytest.raises(CheckoutErrorSuggestGit) as e:
@@ -378,18 +350,18 @@
     assert relpath(old_data_link, old_cache_dir) == relpath(
         new_data_link, new_cache_dir
     )
 
 
 def test_checkout_no_checksum(tmp_dir, dvc):
     tmp_dir.gen("file", "file content")
-    stage = dvc.run(outs=["file"], no_exec=True, cmd="somecmd", single_stage=True)
+    dvc.run(outs=["file"], no_exec=True, cmd="somecmd", name="stage1")
 
     with pytest.raises(CheckoutError):
-        dvc.checkout([stage.path], force=True)
+        dvc.checkout(["stage1"], force=True)
 
     assert not os.path.exists("file")
 
 
 @pytest.mark.parametrize(
     "link, link_test_func",
     [("hardlink", system.is_hardlink), ("symlink", system.is_symlink)],
@@ -600,67 +572,45 @@
     stats = dvc.checkout(relink=True)
     assert stats == {**empty_checkout, "added": ["foo"]}
 
 
 def test_checkout_with_deps(tmp_dir, dvc):
     tmp_dir.dvc_gen({"foo": "foo"})
     dvc.run(
-        fname="copy_file.dvc",
         cmd="echo foo > bar",
         outs=["bar"],
         deps=["foo"],
-        single_stage=True,
+        name="copy-file",
     )
 
     (tmp_dir / "bar").unlink()
     (tmp_dir / "foo").unlink()
 
-    stats = dvc.checkout(["copy_file.dvc"], with_deps=False)
+    stats = dvc.checkout(["copy-file"], with_deps=False)
     assert stats == {**empty_checkout, "added": ["bar"]}
 
     (tmp_dir / "bar").unlink()
-    stats = dvc.checkout(["copy_file.dvc"], with_deps=True)
+    stats = dvc.checkout(["copy-file"], with_deps=True)
     assert set(stats["added"]) == {"foo", "bar"}
 
 
 def test_checkout_recursive(tmp_dir, dvc):
     tmp_dir.gen({"dir": {"foo": "foo", "bar": "bar"}})
-    dvc.add("dir", recursive=True)
+    dvc.add("dir/*", glob=True)
 
     (tmp_dir / "dir" / "foo").unlink()
     (tmp_dir / "dir" / "bar").unlink()
 
     stats = dvc.checkout(["dir"], recursive=True)
     assert set(stats["added"]) == {
         os.path.join("dir", "foo"),
         os.path.join("dir", "bar"),
     }
 
 
-def test_checkout_for_external_outputs(tmp_dir, dvc, workspace):
-    workspace.gen("foo", "foo")
-
-    file_path = workspace / "foo"
-    dvc.add("remote://workspace/foo")
-
-    odb = dvc.cloud.get_remote_odb("workspace")
-    odb.fs.remove(str(file_path))
-    assert not file_path.exists()
-
-    stats = dvc.checkout(force=True)
-    assert stats == {**empty_checkout, "added": ["remote://workspace/foo"]}
-    assert file_path.exists()
-
-    workspace.gen("foo", "foo\nfoo")
-
-    stats = dvc.checkout(force=True)
-    assert stats == {**empty_checkout, "modified": ["remote://workspace/foo"]}
-    assert file_path.read_text() == "foo"
-
-
 def test_checkouts_with_different_addressing(tmp_dir, dvc, run_copy):
     tmp_dir.gen({"foo": "foo", "lorem": "lorem"})
     run_copy("foo", "bar", name="copy-foo-bar")
     run_copy("lorem", "ipsum", name="copy-lorem-ipsum")
 
     (tmp_dir / "bar").unlink()
     (tmp_dir / "ipsum").unlink()
@@ -721,30 +671,14 @@
     (tmp_dir / "bar").unlink()
     assert set(dvc.checkout([stage2.addressing])["added"]) == {"ipsum"}
 
     (tmp_dir / "ipsum").unlink()
     assert set(dvc.checkout()["added"]) == {"bar", "ipsum"}
 
 
-def test_checkout_external_modified_file(tmp_dir, dvc, scm, mocker, workspace):
-    # regression: happened when file in external output changed and checkout
-    # was attempted without force, dvc checks if it's present in its cache
-    # before asking user to remove it.
-    workspace.gen("foo", "foo")
-    dvc.add("remote://workspace/foo", external=True)
-    scm.add(["foo.dvc"])
-    scm.commit("add foo")
-
-    workspace.gen("foo", "foobar")  # messing up the external outputs
-    mocker.patch("dvc.prompt.confirm", return_value=True)
-    dvc.checkout()
-
-    assert (workspace / "foo").read_text() == "foo"
-
-
 def test_checkout_executable(tmp_dir, dvc):
     tmp_dir.dvc_gen("foo", "foo")
 
     contents = (tmp_dir / "foo.dvc").parse()
     contents["outs"][0]["isexec"] = True
     (tmp_dir / "foo.dvc").dump(contents)
 
@@ -813,15 +747,15 @@
 
     # Relevant change, one modified
     sub_dir_file.unlink()
     stats = dvc.checkout(str(sub_dir))
     assert len(stats["modified"]) == 1
 
     stats = dvc.checkout(str(data_dir / "empty_sub_dir"))
-    assert not any(stats.values())
+    assert stats == {**empty_checkout, "modified": ["data" + os.sep]}
 
     dvc.checkout(str(data_dir))
 
     # Everything is in place, no action taken
     stats = dvc.checkout(str(data_dir))
     assert not any(stats.values())
```

### Comparing `dvc-3.0.0a1/tests/func/test_cli.py` & `dvc-3.0.0a2/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_commit.py` & `dvc-3.0.0a2/tests/func/test_commit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import textwrap
 
 import pytest
 
 from dvc.dependency.base import DependencyDoesNotExistError
 from dvc.dvcfile import PROJECT_FILE
+from dvc.fs import localfs
 from dvc.output import OutputDoesNotExistError
 from dvc.stage.exceptions import StageCommitError
 
 
 def test_commit_recursive(tmp_dir, dvc):
     tmp_dir.gen({"dir": {"file": "text1", "subdir": {"file2": "text2"}}})
-    stages = dvc.add("dir", recursive=True, no_commit=True)
+    stages = dvc.add(localfs.find("dir"), no_commit=True)
 
     assert len(stages) == 2
     assert dvc.status() != {}
 
     dvc.commit("dir", recursive=True)
     assert dvc.status() == {}
 
@@ -79,22 +80,21 @@
           md5: acbd18db4cc2f85cedef654fccc4a4d8
           size: 3
         meta: some metadata
     """
     )
 
 
-@pytest.mark.parametrize("run_kw", [{"single_stage": True}, {"name": "copy"}])
-def test_commit_with_deps(tmp_dir, dvc, run_copy, run_kw):
+def test_commit_with_deps(tmp_dir, dvc, run_copy):
     tmp_dir.gen("foo", "foo")
     (foo_stage,) = dvc.add("foo", no_commit=True)
     assert foo_stage is not None
     assert len(foo_stage.outs) == 1
 
-    stage = run_copy("foo", "file", no_commit=True, **run_kw)
+    stage = run_copy("foo", "file", no_commit=True, name="copy")
     assert stage is not None
     assert len(stage.outs) == 1
 
     assert foo_stage.outs[0].changed_cache()
     assert stage.outs[0].changed_cache()
 
     dvc.commit(stage.path, with_deps=True)
```

### Comparing `dvc-3.0.0a1/tests/func/test_config.py` & `dvc-3.0.0a2/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_data_cloud.py` & `dvc-3.0.0a2/tests/func/test_data_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from dvc.exceptions import CheckoutError
 from dvc.repo.open_repo import clean_repos
 from dvc.stage.exceptions import StageNotFound
 from dvc.testing.remote_tests import TestRemote  # noqa, pylint: disable=unused-import
 from dvc.utils.fs import remove
 from dvc_data.hashfile.db import HashFileDB
 from dvc_data.hashfile.db.local import LocalHashFileDB
+from dvc_data.hashfile.hash_info import HashInfo
 
 
 def test_cloud_cli(tmp_dir, dvc, remote, mocker):  # noqa: PLR0915
     jobs = 2
     args = ["-v", "-j", str(jobs)]
 
     (stage,) = tmp_dir.dvc_gen("foo", "foo")
@@ -114,27 +115,25 @@
     assert main(["status", "-c", f])
     assert main(["push", f])
     assert main(["pull", f])
     assert main(["fetch", f])
 
 
 def test_warn_on_outdated_stage(tmp_dir, dvc, local_remote, caplog):
-    stage = dvc.run(outs=["bar"], cmd="echo bar > bar", single_stage=True)
-    assert main(["push"]) == 0
+    stage = dvc.run(outs=["bar"], cmd="echo bar > bar", name="gen-bar")
+    dvc.push()
 
-    stage_file_path = stage.relpath
-    content = (tmp_dir / stage_file_path).parse()
-    del content["outs"][0]["md5"]
-    (tmp_dir / stage_file_path).dump(content)
+    stage.outs[0].hash_info = HashInfo()
+    stage.dump()
 
     with caplog.at_level(logging.WARNING, logger="dvc"):
         caplog.clear()
         assert main(["status", "-c"]) == 0
         expected_warning = (
-            "Output 'bar'(stage: 'bar.dvc') is missing version info. "
+            "Output 'bar'(stage: 'gen-bar') is missing version info. "
             "Cache for it will not be collected. "
             "Use `dvc repro` to get your pipeline up to date."
         )
 
         assert expected_warning in caplog.text
 
 
@@ -307,15 +306,15 @@
     return [
         os.path.join(root, f) for root, _, filenames in os.walk(d) for f in filenames
     ]
 
 
 def test_dvc_pull_pipeline_stages(tmp_dir, dvc, run_copy, local_remote):
     (stage0,) = tmp_dir.dvc_gen("foo", "foo")
-    stage1 = run_copy("foo", "bar", single_stage=True)
+    stage1 = run_copy("foo", "bar", name="copy-foo-bar")
     stage2 = run_copy("bar", "foobar", name="copy-bar-foobar")
     dvc.push()
 
     outs = ["foo", "bar", "foobar"]
 
     clean(outs, dvc)
     dvc.pull()
@@ -339,29 +338,28 @@
     stats = dvc.pull([os.curdir], recursive=True)
     assert set(stats["added"]) == set(outs)
 
 
 def test_pipeline_file_target_ops(tmp_dir, dvc, run_copy, local_remote):
     path = local_remote.url
     tmp_dir.dvc_gen("foo", "foo")
-    run_copy("foo", "bar", single_stage=True)
 
     tmp_dir.dvc_gen("lorem", "lorem")
     run_copy("lorem", "lorem2", name="copy-lorem-lorem2")
 
     tmp_dir.dvc_gen("ipsum", "ipsum")
     run_copy("ipsum", "baz", name="copy-ipsum-baz")
 
-    outs = ["foo", "bar", "lorem", "ipsum", "baz", "lorem2"]
+    outs = ["foo", "lorem", "ipsum", "baz", "lorem2"]
 
     remove(dvc.stage_cache.cache_dir)
 
     dvc.push()
 
-    outs = ["foo", "bar", "lorem", "ipsum", "baz", "lorem2"]
+    outs = ["foo", "lorem", "ipsum", "baz", "lorem2"]
 
     # each one's a copy of other, hence 3
     assert len(recurse_list_dir(path)) == 3
 
     clean(outs, dvc)
     assert set(dvc.pull(["dvc.yaml"])["added"]) == {"lorem2", "baz"}
```

### Comparing `dvc-3.0.0a1/tests/func/test_data_status.py` & `dvc-3.0.0a2/tests/func/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_diff.py` & `dvc-3.0.0a2/tests/func/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_dvcfile.py` & `dvc-3.0.0a2/tests/func/test_dvcfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,22 +61,15 @@
         always_changed=True,
     )
     with pytest.raises(StageNotFound):
         assert load_file(dvc, stage.path).stages["random-name"]
 
 
 def test_run_load_one_on_single_stage(tmp_dir, dvc):
-    tmp_dir.gen("foo", "foo")
-    stage = dvc.run(
-        cmd="cp foo foo2",
-        deps=["foo"],
-        metrics=["foo2"],
-        always_changed=True,
-        single_stage=True,
-    )
+    (stage,) = tmp_dir.dvc_gen("foo", "foo")
     assert isinstance(load_file(dvc, stage.path), SingleStageFile)
     assert load_file(dvc, stage.path).stages.get("random-name") == stage
     assert load_file(dvc, stage.path).stage == stage
 
 
 def test_has_stage_with_name(tmp_dir, dvc):
     tmp_dir.gen("foo", "foo")
@@ -116,23 +109,16 @@
     assert set(load_file(dvc, PROJECT_FILE).stages.values()) == {
         stage2,
         stage1,
     }
 
 
 def test_load_all_singlestage(tmp_dir, dvc):
-    tmp_dir.gen("foo", "foo")
-    stage1 = dvc.run(
-        cmd="cp foo foo2",
-        deps=["foo"],
-        metrics=["foo2"],
-        always_changed=True,
-        single_stage=True,
-    )
-    dvcfile = load_file(dvc, "foo2.dvc")
+    (stage1,) = tmp_dir.dvc_gen("foo", "foo")
+    dvcfile = load_file(dvc, "foo.dvc")
     assert isinstance(dvcfile, SingleStageFile)
     assert len(dvcfile.stages) == 1
     stages = dvcfile.stages.values()
     assert len(stages) == 1
     assert list(stages) == [stage1]
 
 
@@ -163,22 +149,15 @@
     stage2 = dvc.run(
         cmd="cp foo foo2",
         deps=["foo"],
         name="copy-foo-foo2",
         metrics=["foo2"],
         always_changed=True,
     )
-    stage3 = dvc.run(
-        cmd="cp bar bar2",
-        deps=["bar"],
-        metrics=["bar2"],
-        always_changed=True,
-        single_stage=True,
-    )
-    assert set(dvc.index.stages) == {stage1, stage3, stage2}
+    assert set(dvc.index.stages) == {stage1, stage2}
 
 
 def test_remove_stage(tmp_dir, dvc, run_copy):
     tmp_dir.gen("foo", "foo")
     stage = run_copy("foo", "bar", name="copy-foo-bar")
     stage2 = run_copy("bar", "foobar", name="copy-bar-foobar")
 
@@ -223,16 +202,15 @@
     lock_file.remove_stage(stage)
     lock_file.remove()
     # should not fail when there's no file at all.
     lock_file.remove_stage(stage)
 
 
 def test_remove_stage_dvcfiles(tmp_dir, dvc, run_copy):
-    tmp_dir.gen("foo", "foo")
-    stage = run_copy("foo", "bar", single_stage=True)
+    (stage,) = tmp_dir.dvc_gen("foo", "foo")
 
     dvc_file = load_file(dvc, stage.path)
     assert dvc_file.exists()
     dvc_file.remove_stage(stage)
     assert not dvc_file.exists()
 
     # re-check to see if it fails if there's no stage entry
```

### Comparing `dvc-3.0.0a1/tests/func/test_external_repo.py` & `dvc-3.0.0a2/tests/func/test_external_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_fs.py` & `dvc-3.0.0a2/tests/func/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_gc.py` & `dvc-3.0.0a2/tests/func/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_get.py` & `dvc-3.0.0a2/tests/func/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,19 +145,17 @@
 
 def test_non_cached_output(tmp_dir, erepo_dir):
     src = "non_cached_file"
     dst = src + "_imported"
 
     with erepo_dir.chdir():
         erepo_dir.dvc.run(
-            outs_no_cache=[src],
-            cmd="echo hello > non_cached_file",
-            single_stage=True,
+            outs_no_cache=[src], cmd="echo hello > non_cached_file", name="gen"
         )
-        erepo_dir.scm_add([src, src + ".dvc"], commit="add non-cached output")
+        erepo_dir.scm_add(["dvc.lock", "dvc.yaml"], commit="add non-cached output")
 
     Repo.get(os.fspath(erepo_dir), src, dst)
 
     assert (tmp_dir / dst).is_file()
     # NOTE: using strip() to account for `echo` differences on win and *nix
     assert (tmp_dir / dst).read_text().strip() == "hello"
```

### Comparing `dvc-3.0.0a1/tests/func/test_get_url.py` & `dvc-3.0.0a2/tests/func/test_get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_ignore.py` & `dvc-3.0.0a2/tests/func/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_import.py` & `dvc-3.0.0a2/tests/func/test_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,17 @@
 
 def test_import_non_cached(erepo_dir, tmp_dir, dvc, scm):
     src = "non_cached_output"
     dst = src + "_imported"
 
     with erepo_dir.chdir():
         erepo_dir.dvc.run(
-            cmd=f"echo hello > {src}", outs_no_cache=[src], single_stage=True
+            cmd=f"echo hello > {src}",
+            outs_no_cache=[src],
+            name="gen",
         )
 
     erepo_dir.scm_add([os.fspath(erepo_dir / src)], commit="add a non-cached out")
 
     stage = tmp_dir.dvc.imp(os.fspath(erepo_dir), src, dst)
 
     assert (tmp_dir / dst).is_file()
```

### Comparing `dvc-3.0.0a1/tests/func/test_import_url.py` & `dvc-3.0.0a2/tests/func/test_import_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_init.py` & `dvc-3.0.0a2/tests/func/test_init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_install.py` & `dvc-3.0.0a2/tests/func/test_install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_lock.py` & `dvc-3.0.0a2/tests/func/test_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_lockfile.py` & `dvc-3.0.0a2/tests/func/test_lockfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import OrderedDict
 from operator import itemgetter
 
 from dvc.dvcfile import LOCK_FILE
 from dvc.stage.utils import split_params_deps
 from dvc.utils.fs import remove
 from dvc.utils.serialize import dumps_yaml, parse_yaml_for_update
-from tests.func.test_run_multistage import supported_params
+from tests.func.test_run import supported_params
 
 FS_STRUCTURE = {
     "foo": "bar\nfoobar",
     "bar": "foo\nfoobar",
     "foobar": "foobar\nbar",
     "params.yaml": dumps_yaml(supported_params),
     "params2.yaml": dumps_yaml(supported_params),
```

### Comparing `dvc-3.0.0a1/tests/func/test_ls.py` & `dvc-3.0.0a2/tests/func/test_ls.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,17 @@
     )
     tmp_dir.scm_gen({"script.py": script}, commit="init")
     tmp_dir.dvc_gen({"dep": "content"}, commit="init dvc")
     dvc.run(
         cmd="python script.py {}".format(os.path.join("out", "file")),
         outs=[os.path.join("out", "file")],
         deps=["dep"],
-        fname="out.dvc",
-        single_stage=True,
+        name="touch",
     )
-    tmp_dir.scm_add(["out.dvc"], commit="run")
+    tmp_dir.scm_add(["dvc.yaml", "dvc.lock"], commit="run")
     shutil.rmtree("out")
 
 
 def test_ls_repo(tmp_dir, dvc, scm):
     tmp_dir.scm_gen(FS_STRUCTURE, commit="init")
     tmp_dir.dvc_gen(DVC_STRUCTURE, commit="dvc")
 
@@ -239,15 +238,16 @@
 
     files = Repo.ls(os.fspath(tmp_dir))
     match_files(
         files,
         (
             (("script.py",), False),
             (("dep.dvc",), False),
-            (("out.dvc",), False),
+            (("dvc.yaml",), False),
+            (("dvc.lock",), False),
             (("dep",), True),
             (("out",), False),
             ((".dvcignore",), False),
             ((".gitignore",), False),
         ),
     )
 
@@ -257,15 +257,16 @@
 
     files = Repo.ls(os.fspath(tmp_dir), recursive=True)
     match_files(
         files,
         (
             (("script.py",), False),
             (("dep.dvc",), False),
-            (("out.dvc",), False),
+            (("dvc.yaml",), False),
+            (("dvc.lock",), False),
             (("dep",), True),
             (("out", "file"), True),
             ((".dvcignore",), False),
             ((".gitignore",), False),
         ),
     )
```

### Comparing `dvc-3.0.0a1/tests/func/test_merge_driver.py` & `dvc-3.0.0a2/tests/func/test_merge_driver.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_move.py` & `dvc-3.0.0a2/tests/func/test_move.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import shutil
 import textwrap
 
 import pytest
 
 from dvc.cli import main
 from dvc.exceptions import MoveNotDataSourceError, OutputNotFoundError
 
@@ -35,15 +36,15 @@
 
 def test_move_not_data_source(tmp_dir, dvc):
     tmp_dir.dvc_gen("foo", "foo")
     dvc.run(
         cmd="cp foo file1",
         outs=["file1"],
         deps=["foo"],
-        single_stage=True,
+        name="copy-foo-file1",
     )
 
     with pytest.raises(MoveNotDataSourceError):
         dvc.move("file1", "dst")
 
     assert main(["move", "file1", "dst"]) != 0
     assert (tmp_dir / "file1").exists()
@@ -134,18 +135,18 @@
 
     dvc.move("old_name", "new_name")
 
     assert dvc.status() == {}
 
 
 def test_should_move_to_dir_on_non_default_stage_file(tmp_dir, dvc):
-    stage_file_name = "stage.dvc"
     tmp_dir.gen({"file": "file_content"})
 
-    dvc.add("file", fname=stage_file_name)
+    dvc.add("file")
+    shutil.move("file.dvc", "stage.dvc")
     os.mkdir("directory")
 
     dvc.move("file", "directory")
 
     assert os.path.exists(os.path.join("directory", "file"))
```

### Comparing `dvc-3.0.0a1/tests/func/test_odb.py` & `dvc-3.0.0a2/tests/func/test_odb.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_remote.py` & `dvc-3.0.0a2/tests/func/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_remove.py` & `dvc-3.0.0a2/tests/func/test_remove.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dvc_objects.errors import ObjectDBError
 from tests.utils import get_gitignore_content
 
 
 @pytest.mark.parametrize("remove_outs", [True, False])
 def test_remove(tmp_dir, scm, dvc, run_copy, remove_outs):
     (stage1,) = tmp_dir.dvc_gen("foo", "foo")
-    stage2 = run_copy("foo", "bar", single_stage=True)
+    stage2 = run_copy("foo", "bar", name="copy-foo-bar")
     stage3 = run_copy("bar", "foobar", name="copy-bar-foobar")
 
     assert "/foo" in get_gitignore_content()
     assert "/bar" in get_gitignore_content()
     assert "/foobar" in get_gitignore_content()
 
     for stage in [stage1, stage2, stage3]:
@@ -92,15 +92,15 @@
     assert not (tmp_dir / stage.relpath).exists()
     assert not (stage.dvcfile._lockfile).exists()
     assert not (tmp_dir / ".gitignore").exists()
 
 
 def test_cmd_remove_gitignore_multistage(tmp_dir, scm, dvc, run_copy):
     (stage,) = tmp_dir.dvc_gen("foo", "foo")
-    stage1 = run_copy("foo", "foo1", single_stage=True)
+    stage1 = run_copy("foo", "foo1", name="copy-foo-foo1")
     stage2 = run_copy("foo1", "foo2", name="copy-foo1-foo2")
 
     assert (tmp_dir / ".gitignore").exists()
 
     assert main(["remove", stage2.addressing]) == 0
     assert main(["remove", stage1.addressing]) == 0
     assert main(["remove", stage.addressing]) == 0
```

### Comparing `dvc-3.0.0a1/tests/func/test_repo.py` & `dvc-3.0.0a2/tests/func/test_repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,26 +32,25 @@
 def test_destroy(tmp_dir, dvc, run_copy):
     dvc.config["cache"]["type"] = ["symlink"]
     dvc.cache = CacheManager(dvc)
 
     tmp_dir.dvc_gen("file", "text")
     tmp_dir.dvc_gen({"dir": {"file": "lorem", "subdir/file": "ipsum"}})
 
-    run_copy("file", "file2", single_stage=True)
+    run_copy("file", "file2", name="copy-file-file2")
     run_copy("file2", "file3", name="copy-file2-file3")
     run_copy("file3", "file4", name="copy-file3-file4")
 
     dvc.destroy()
 
     # Remove all the files related to DVC
     for path in [
         ".dvc",
         ".dvcignore",
         "file.dvc",
-        "file2.dvc",
         "dir.dvc",
         PROJECT_FILE,
         LOCK_FILE,
     ]:
         assert not (tmp_dir / path).exists()
 
     # Leave the rest of the files
```

### Comparing `dvc-3.0.0a1/tests/func/test_repo_index.py` & `dvc-3.0.0a2/tests/func/test_repo_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_repro_multistage.py` & `dvc-3.0.0a2/tests/func/test_run.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,483 +1,718 @@
+import logging
 import os
-from copy import deepcopy
-from textwrap import dedent
+import textwrap
+import uuid
 
 import pytest
-from funcy import lsplit
+from funcy import get_in
 
 from dvc.cli import main
-from dvc.dvcfile import LOCK_FILE, PROJECT_FILE
-from dvc.exceptions import CyclicGraphError, ReproductionError
+from dvc.dependency import ParamsDependency
+from dvc.dependency.base import DependencyDoesNotExistError
+from dvc.dvcfile import LOCK_FILE, PROJECT_FILE, load_file
+from dvc.exceptions import (
+    ArgumentDuplicationError,
+    CircularDependencyError,
+    CyclicGraphError,
+    InvalidArgumentError,
+    OutputDuplicationError,
+    OverlappingOutputPathsError,
+)
 from dvc.stage import PipelineStage
-from dvc.stage.exceptions import StageNotFound
-from dvc.utils.fs import remove
+from dvc.stage.exceptions import (
+    DuplicateStageName,
+    InvalidStageName,
+    StagePathNotDirectoryError,
+    StagePathNotFoundError,
+    StagePathOutsideError,
+)
+from dvc.utils.serialize import load_yaml
 
 
-def test_non_existing_stage_name(tmp_dir, dvc, run_copy):
-    tmp_dir.gen("file1", "file1")
-    run_copy("file1", "file2", name="copy-file1-file2")
+def test_run(tmp_dir, dvc, copy_script):
+    tmp_dir.dvc_gen("foo", "foo")
+    assert not os.path.exists(PROJECT_FILE)
+    stage = dvc.run(
+        cmd="python copy.py foo bar",
+        deps=["foo", "copy.py"],
+        outs=["bar"],
+        name="copy-foo-to-bar",
+    )
+    assert isinstance(stage, PipelineStage)
+    assert stage.name == "copy-foo-to-bar"
+    assert os.path.exists(PROJECT_FILE)
+    assert os.path.exists(LOCK_FILE)
+    assert stage.cmd == "python copy.py foo bar"
+    assert len(stage.deps) == 2
+    assert len(stage.outs) == 1
 
-    with pytest.raises(StageNotFound):
-        dvc.freeze(":copy-file1-file3")
+    with pytest.raises(OutputDuplicationError):
+        dvc.run(
+            cmd="python copy.py foo bar",
+            deps=["foo", "copy.py"],
+            outs=["bar"],
+            name="duplicate",
+        )
 
-    assert main(["freeze", ":copy-file1-file3"]) != 0
 
+def test_run_empty(dvc):
+    dvc.run(
+        cmd="echo hello world",
+        deps=[],
+        outs=[],
+        outs_no_cache=[],
+        name="empty",
+    )
 
-def test_repro_frozen(tmp_dir, dvc, run_copy):
-    (data_stage,) = tmp_dir.dvc_gen("data", "foo")
-    stage0 = run_copy("data", "stage0", name="copy-data-stage0")
-    run_copy("stage0", "stage1", name="copy-data-stage1")
-    run_copy("stage1", "stage2", name="copy-data-stage2")
 
-    dvc.freeze("copy-data-stage1")
+def test_run_missing_dep(dvc):
+    with pytest.raises(DependencyDoesNotExistError):
+        dvc.run(
+            cmd="command",
+            deps=["non-existing-dep"],
+            outs=[],
+            outs_no_cache=[],
+            name="missing-dep",
+        )
 
-    tmp_dir.gen("data", "bar")
-    stages = dvc.reproduce()
-    assert stages == [data_stage, stage0]
 
+def test_run_no_exec(tmp_dir, dvc, scm, run_copy):
+    tmp_dir.dvc_gen("foo", "foo")
+    assert not os.path.exists(PROJECT_FILE)
+    stage = run_copy("foo", "bar", name="copy-foo-to-bar", no_exec=True)
+    assert isinstance(stage, PipelineStage)
+    assert stage.name == "copy-foo-to-bar"
+    assert os.path.exists(PROJECT_FILE)
+    assert not os.path.exists(LOCK_FILE)
+    assert not os.path.exists("bar")
 
-def test_downstream(M, tmp_dir, dvc):
-    # The dependency graph should look like this:
-    #
-    #       E
-    #      / \
-    #     D   F
-    #    / \   \
-    #   B   C   G
-    #    \ /
-    #     A
-    #
-    assert main(["stage", "add", "--run", "-n", "A-gen", "-o", "A", "echo A>A"]) == 0
-    assert (
-        main(["stage", "add", "--run", "-n", "B-gen", "-d", "A", "-o", "B", "echo B>B"])
-        == 0
-    )
-    assert (
-        main(
-            [
-                "stage",
-                "add",
-                "--run",
-                "-n",
-                "C-gen",
-                "-d",
-                "A",
-                "-o",
-                "C",
-                "echo C>C",
-            ]
-        )
-        == 0
-    )
-    assert (
-        main(
-            [
-                "stage",
-                "add",
-                "--run",
-                "-n",
-                "D-gen",
-                "-d",
-                "B",
-                "-d",
-                "C",
-                "-o",
-                "D",
-                "echo D>D",
-            ]
-        )
-        == 0
-    )
-    assert main(["stage", "add", "--run", "-n", "G-gen", "-o", "G", "echo G>G"]) == 0
-    assert (
-        main(["stage", "add", "--run", "-n", "F-gen", "-d", "G", "-o", "F", "echo F>F"])
-        == 0
-    )
-    assert (
-        main(
-            [
-                "stage",
-                "add",
-                "--run",
-                "-n",
-                "E-gen",
-                "-d",
-                "D",
-                "-d",
-                "F",
-                "-o",
-                "E",
-                "echo E>E",
-            ]
-        )
-        == 0
-    )
+    data, _ = stage.dvcfile._load()
+    assert data["stages"]["copy-foo-to-bar"] == {
+        "cmd": "python copy.py foo bar",
+        "deps": ["copy.py", "foo"],
+        "outs": ["bar"],
+    }
+    with open(".gitignore", encoding="utf-8") as fobj:
+        assert fobj.read() == "/foo\n/bar\n"
 
-    # We want the evaluation to move from B to E
-    #
-    #       E
-    #      /
-    #     D
-    #    /
-    #   B
-    #
-    evaluation = dvc.reproduce(PROJECT_FILE + ":B-gen", downstream=True, force=True)
-
-    assert len(evaluation) == 3
-    assert all(isinstance(stage, PipelineStage) for stage in evaluation)
-    assert all(stage.relpath == PROJECT_FILE for stage in evaluation)
-    assert [stage.name for stage in evaluation] == ["B-gen", "D-gen", "E-gen"]
-
-    # B, C should be run (in any order) before D
-    # See https://github.com/iterative/dvc/issues/3602
-    evaluation = dvc.reproduce(PROJECT_FILE + ":A-gen", downstream=True, force=True)
-
-    assert len(evaluation) == 5
-    assert all(isinstance(stage, PipelineStage) for stage in evaluation)
-    assert all(stage.relpath == PROJECT_FILE for stage in evaluation)
-    assert [stage.name for stage in evaluation] == [
-        "A-gen",
-        M.any_of("B-gen", "C-gen"),
-        M.any_of("B-gen", "C-gen"),
-        "D-gen",
-        "E-gen",
-    ]
 
+def test_run_repeat(tmp_dir, dvc, run_copy):
+    from dvc.dvcfile import PROJECT_FILE, load_file
+    from dvc.stage import PipelineStage
+
+    tmp_dir.dvc_gen("foo", "foo")
+    run_copy("foo", "foo1", name="copy-foo-foo1")
+    run_copy("foo1", "foo2", name="copy-foo1-foo2")
+    run_copy("foo2", "foo3", name="copy-foo2-foo3")
+
+    stages = list(load_file(dvc, PROJECT_FILE).stages.values())
+    assert len(stages) == 3
+    assert all(isinstance(stage, PipelineStage) for stage in stages)
+    assert {stage.name for stage in stages} == {
+        "copy-foo-foo1",
+        "copy-foo1-foo2",
+        "copy-foo2-foo3",
+    }
 
-def test_repro_when_cmd_changes(tmp_dir, dvc, run_copy, mocker):
-    from dvc.dvcfile import ProjectFile
 
-    tmp_dir.gen("foo", "foo")
-    stage = run_copy("foo", "bar", name="copy-file")
-    target = "copy-file"
-    assert not dvc.reproduce(target)
+def test_run_cached(tmp_dir, dvc, run_copy, mocker):
+    from dvc.stage.run import subprocess
 
-    from dvc.stage.run import cmd_run
+    tmp_dir.dvc_gen("foo", "foo")
 
-    m = mocker.patch("dvc.stage.run.cmd_run", wraps=cmd_run)
-    stage.cmd = "  ".join(stage.cmd.split())  # change cmd spacing by two
-    ProjectFile(dvc, PROJECT_FILE)._dump_pipeline_file(stage)
+    run_copy("foo", "foo2", name="copy-foo1-foo2")
+    spy = mocker.spy(subprocess, "Popen")
+    run_copy("foo", "foo2", name="copy-foo1-foo2")
+    assert not spy.called
 
-    assert dvc.status([target]) == {target: ["changed command"]}
-    assert dvc.reproduce(target)[0] == stage
-    m.assert_called_once_with(stage, dry=False, run_env=None)
 
+def test_dump_on_non_cached_outputs(tmp_dir, dvc):
+    tmp_dir.dvc_gen("foo")
+    dvc.run(
+        cmd="cp foo foo1",
+        deps=["foo"],
+        name="copy-foo1-foo2",
+        outs_no_cache=["foo1"],
+    )
 
-def test_repro_when_new_deps_is_added_in_dvcfile(tmp_dir, dvc, run_copy, copy_script):
-    from dvc.dvcfile import load_file
 
-    tmp_dir.gen({"foo": "foo", "bar": "bar"})
+def test_with_wdir(tmp_dir, dvc):
+    tmp_dir.gen({"dir": {"foo": "foo", "bar": "bar"}})
     stage = dvc.run(
-        cmd="python copy.py {} {}".format("foo", "foobar"),
-        outs=["foobar"],
+        cmd="cp foo foo1",
         deps=["foo"],
-        name="copy-file",
+        name="copy-foo1-foo2",
+        outs=["foo1"],
+        wdir="dir",
     )
-    target = PROJECT_FILE + ":copy-file"
-    assert not dvc.reproduce(target)
 
-    dvcfile = load_file(dvc, stage.path)
-    data, _ = dvcfile._load()
-    data["stages"]["copy-file"]["deps"] += ["copy.py"]
-    (tmp_dir / stage.path).dump(data)
+    data, _ = load_file(dvc, stage.path)._load()
+    assert data["stages"]["copy-foo1-foo2"]["wdir"] == "dir"
 
-    assert dvc.reproduce(target)[0] == stage
 
-
-def test_repro_when_new_outs_is_added_in_dvcfile(tmp_dir, dvc, copy_script):
+def test_always_changed(tmp_dir, dvc):
     from dvc.dvcfile import load_file
 
     tmp_dir.gen({"foo": "foo", "bar": "bar"})
     stage = dvc.run(
-        cmd="python copy.py {} {}".format("foo", "foobar"),
-        outs=[],  # scenario where user forgot to add
+        cmd="cp foo foo1",
         deps=["foo"],
-        name="copy-file",
+        name="copy-foo1-foo2",
+        outs=["foo1"],
+        always_changed=True,
     )
-    target = ":copy-file"
-    assert not dvc.reproduce(target)
 
-    dvcfile = load_file(dvc, stage.path)
-    data, _ = dvcfile._load()
-    data["stages"]["copy-file"]["outs"] = ["foobar"]
-    (tmp_dir / stage.path).dump(data)
+    data, _ = load_file(dvc, stage.path)._load()
+    assert data["stages"]["copy-foo1-foo2"]["always_changed"]
 
-    assert dvc.reproduce(target)[0] == stage
 
+def test_graph(tmp_dir, dvc):
+    from dvc.exceptions import CyclicGraphError
 
-def test_repro_when_new_deps_is_moved(tmp_dir, dvc, copy_script):
-    from dvc.dvcfile import load_file
+    tmp_dir.gen({"foo": "foo", "bar": "bar"})
 
-    tmp_dir.gen({"foo": "foo", "bar": "foo"})
-    stage = dvc.run(
-        cmd="python copy.py {} {}".format("foo", "foobar"),
-        outs=["foobar"],
-        deps=["foo"],
-        name="copy-file",
-    )
-    target = ":copy-file"
-    assert not dvc.reproduce(target)
+    dvc.run(deps=["foo"], outs=["bar"], cmd="echo foo > bar", name="1")
 
-    # hardcode values in source code, ignore sys.argv
-    tmp_dir.gen(
-        "copy.py",
-        """
-import shutil
+    dvc.run(deps=["bar"], outs=["baz"], cmd="echo bar > baz", name="2")
 
-shutil.copyfile('bar', 'foobar')
-""",
-    )
-    from shutil import move
+    with pytest.raises(CyclicGraphError):
+        dvc.run(deps=["baz"], outs=["foo"], cmd="echo baz > foo", name="3")
 
-    move("foo", "bar")
 
-    dvcfile = load_file(dvc, stage.path)
-    data, _ = dvcfile._load()
-    data["stages"]["copy-file"]["deps"] = ["bar"]
-    (tmp_dir / stage.path).dump(data)
+class TestRunCircularDependency:
+    def test(self, dvc):
+        with pytest.raises(CircularDependencyError):
+            dvc.run(
+                cmd="command",
+                deps=["foo"],
+                outs=["foo"],
+                name="circular-dependency",
+            )
+
+    def test_outs_no_cache(self, dvc):
+        with pytest.raises(CircularDependencyError):
+            dvc.run(
+                cmd="command",
+                deps=["foo"],
+                outs_no_cache=["foo"],
+                name="circular-dependency",
+            )
+
+    def test_non_normalized_paths(self, dvc):
+        with pytest.raises(CircularDependencyError):
+            dvc.run(
+                cmd="command",
+                deps=["./foo"],
+                outs=["foo"],
+                name="circular-dependency",
+            )
+
+    def test_graph(self, tmp_dir, dvc):
+        tmp_dir.gen("foo", "foo")
+        dvc.run(
+            deps=["foo"],
+            outs=["bar.txt"],
+            cmd="echo bar > bar.txt",
+            name="gen-bar-txt",
+        )
 
-    assert dvc.reproduce(target)[0] == stage
+        dvc.run(
+            deps=["bar.txt"],
+            outs=["baz.txt"],
+            cmd="echo baz > baz.txt",
+            name="gen-baz-txt",
+        )
 
+        with pytest.raises(CyclicGraphError):
+            dvc.run(
+                deps=["baz.txt"],
+                outs=["foo"],
+                cmd="echo baz > foo",
+                name="gen-foo",
+            )
+
+
+class TestRunDuplicatedArguments:
+    def test(self, dvc):
+        with pytest.raises(ArgumentDuplicationError):
+            dvc.run(
+                cmd="command",
+                deps=[],
+                outs=["foo", "foo"],
+                name="circular-dependency",
+            )
+
+    def test_outs_no_cache(self, dvc):
+        with pytest.raises(ArgumentDuplicationError):
+            dvc.run(
+                cmd="command",
+                outs=["foo"],
+                outs_no_cache=["foo"],
+                name="circular-dependency",
+            )
+
+    def test_non_normalized_paths(self, dvc):
+        with pytest.raises(ArgumentDuplicationError):
+            dvc.run(
+                cmd="command",
+                deps=[],
+                outs=["foo", "./foo"],
+                name="circular-dependency",
+            )
+
+
+class TestRunBadWdir:
+    def test(self, make_tmp_dir, dvc):
+        with pytest.raises(StagePathOutsideError):
+            dvc.run(
+                cmd="command",
+                wdir=make_tmp_dir("tmp"),
+                name="bad-wdir",
+            )
+
+    def test_same_prefix(self, tmp_dir, dvc):
+        path = f"{tmp_dir}-{uuid.uuid4()}"
+        os.mkdir(path)
+        with pytest.raises(StagePathOutsideError):
+            dvc.run(cmd="command", wdir=path, name="bad-wdir")
+
+    def test_not_found(self, tmp_dir, dvc):
+        path = os.path.join(tmp_dir, str(uuid.uuid4()))
+        with pytest.raises(StagePathNotFoundError):
+            dvc.run(cmd="command", wdir=path, name="bad-wdir")
+
+    def test_not_dir(self, tmp_dir, dvc):
+        path = tmp_dir / str(uuid.uuid4())
+        path.mkdir()
+        path = path / str(uuid.uuid4())
+        path.touch()
+        with pytest.raises(StagePathNotDirectoryError):
+            dvc.run(
+                cmd="command",
+                wdir=os.fspath(path),
+                name="bad-wdir",
+            )
+
+
+class TestCmdRunWorkingDirectory:
+    def test_default_wdir_is_not_written(self, tmp_dir, dvc):
+        dvc.run(
+            cmd="echo test > foo",
+            outs=["foo"],
+            wdir=".",
+            name="echo-foo",
+        )
 
-def test_repro_when_new_out_overlaps_others_stage_outs(tmp_dir, dvc):
-    from dvc.exceptions import OverlappingOutputPathsError
+        d = load_yaml("dvc.yaml")
+        assert "wdir" not in get_in(d, ["stages", "echo-foo"])
 
-    tmp_dir.gen({"dir": {"file1": "file1"}, "foo": "foo"})
-    dvc.add("dir")
-    (tmp_dir / PROJECT_FILE).dump(
-        {
-            "stages": {
-                "run-copy": {
-                    "cmd": "python copy {} {}".format("foo", "dir/foo"),
-                    "deps": ["foo"],
-                    "outs": ["dir/foo"],
-                }
-            }
-        },
-    )
-    with pytest.raises(OverlappingOutputPathsError):
-        dvc.reproduce(":run-copy")
+        dvc.run(cmd="echo test > bar", outs=["bar"], name="echo-bar")
+        d = load_yaml("dvc.yaml")
+        assert "wdir" not in get_in(d, ["stages", "echo-bar"])
+
+    def test_fname_changes_path_and_wdir(self, tmp_dir, dvc):
+        dirpath = tmp_dir / "dir"
+        dirpath.mkdir()
+
+        with dirpath.chdir():
+            stage = dvc.run(
+                cmd="echo test > foo",
+                outs=["foo"],
+                wdir=os.fspath(tmp_dir),
+                name="echo",
+            )
+        assert stage.wdir == os.path.realpath(tmp_dir)
+
+        # Check that it is dumped properly
+        d = load_yaml("dir/dvc.yaml")
+        assert get_in(d, ["stages", "echo", "wdir"]) == ".."
 
 
-def test_repro_when_new_deps_added_does_not_exist(tmp_dir, dvc, copy_script):
-    tmp_dir.gen("foo", "foo")
-    (tmp_dir / PROJECT_FILE).dump(
+def test_run_dump(tmp_dir, dvc, run_head):
+    from dvc.dvcfile import load_file
+
+    tmp_dir.gen(
         {
-            "stages": {
-                "run-copy": {
-                    "cmd": "python copy.py {} {}".format("foo", "foobar"),
-                    "deps": ["foo", "bar"],
-                    "outs": ["foobar"],
-                }
+            "dir": {
+                "foo": "foo\nfoo",
+                "bar": "bar\nbar",
+                "foobar": "foobar\foobar",
             }
-        },
+        }
     )
-    with pytest.raises(ReproductionError):
-        dvc.reproduce(":run-copy")
 
-
-def test_repro_when_new_outs_added_does_not_exist(tmp_dir, dvc, copy_script):
-    tmp_dir.gen("foo", "foo")
-    (tmp_dir / PROJECT_FILE).dump(
-        {
-            "stages": {
-                "run-copy": {
-                    "cmd": "python copy.py {} {}".format("foo", "foobar"),
-                    "deps": ["foo"],
-                    "outs": ["foobar", "bar"],
-                }
+    dvc.run(
+        cmd="cp foo foo2",
+        deps=["foo"],
+        name="copy-foo-foo2",
+        wdir="dir",
+        outs_persist=["foo2"],
+        always_changed=True,
+    )
+    data = load_file(dvc, PROJECT_FILE)._load()[0]
+    assert data == {
+        "stages": {
+            "copy-foo-foo2": {
+                "cmd": "cp foo foo2",
+                "deps": ["foo"],
+                "outs": [{"foo2": {"persist": True}}],
+                "always_changed": True,
+                "wdir": "dir",
             }
-        },
-    )
-    with pytest.raises(ReproductionError):
-        dvc.reproduce(":run-copy")
+        }
+    }
 
+    run_head(
+        "foo",
+        "bar",
+        "foobar",
+        name="head-files",
+        outs=["bar-1"],
+        outs_persist=["foo-1"],
+        metrics_no_cache=["foobar-1"],
+        wdir="dir",
+    )
+    assert load_file(dvc, PROJECT_FILE)._load()[0] == {
+        "stages": {
+            "head-files": {
+                "cmd": "python {} foo bar foobar".format(
+                    (tmp_dir / "head.py").resolve()
+                ),
+                "wdir": "dir",
+                "deps": ["bar", "foo", "foobar"],
+                "outs": ["bar-1", {"foo-1": {"persist": True}}],
+                "metrics": [{"foobar-1": {"cache": False}}],
+            },
+            **data["stages"],
+        }
+    }
 
-def test_repro_when_lockfile_gets_deleted(tmp_dir, dvc, copy_script):
-    tmp_dir.gen("foo", "foo")
-    (tmp_dir / PROJECT_FILE).dump(
-        {
-            "stages": {
-                "run-copy": {
-                    "cmd": "python copy.py {} {}".format("foo", "foobar"),
-                    "deps": ["foo"],
-                    "outs": ["foobar"],
-                }
-            }
-        },
-    )
-    assert dvc.reproduce(":run-copy")
-    assert os.path.exists(LOCK_FILE)
 
-    assert not dvc.reproduce(":run-copy")
-    os.unlink(LOCK_FILE)
-    stages = dvc.reproduce(":run-copy")
-    assert stages
-    assert stages[0].relpath == PROJECT_FILE
-    assert stages[0].name == "run-copy"
+@pytest.mark.parametrize("char", ["@:", "#", "$", ":", "/", "\\", ".", ";", ","])
+def test_run_with_invalid_stage_name(run_copy, char):
+    with pytest.raises(InvalidStageName):
+        run_copy("foo", "bar", name=f"copy_name-{char}")
 
 
-def test_cyclic_graph_error(tmp_dir, dvc, run_copy):
-    tmp_dir.gen("foo", "foo")
-    run_copy("foo", "bar", name="copy-foo-bar")
-    run_copy("bar", "baz", name="copy-bar-baz")
-    run_copy("baz", "foobar", name="copy-baz-foobar")
+def test_run_with_name_having_hyphen_underscore(tmp_dir, dvc, run_copy):
+    tmp_dir.dvc_gen("foo", "foo")
+    run_copy("foo", "bar", name="copy-foo_bar")
 
-    data = (tmp_dir / PROJECT_FILE).parse()
-    data["stages"]["copy-baz-foo"] = {
-        "cmd": "echo baz > foo",
-        "deps": ["baz"],
-        "outs": ["foo"],
-    }
-    (tmp_dir / PROJECT_FILE).dump(data)
-    with pytest.raises(CyclicGraphError):
-        dvc.reproduce(":copy-baz-foo")
 
+def test_run_already_exists(tmp_dir, dvc, run_copy):
+    tmp_dir.dvc_gen("foo", "foo")
+    run_copy("foo", "bar", name="copy")
+    with pytest.raises(DuplicateStageName):
+        run_copy("bar", "foobar", name="copy", force=False)
+    run_copy("bar", "foobar", name="copy", force=True)
 
-def test_repro_multiple_params(tmp_dir, dvc):
-    from dvc.stage.utils import split_params_deps
-    from tests.func.test_run_multistage import supported_params
 
-    (tmp_dir / "params2.yaml").dump(supported_params)
-    (tmp_dir / "params.yaml").dump(supported_params)
+supported_params = {
+    "name": "Answer",
+    "answer": 42,
+    "floats": 42.0,
+    "lists": [42, 42.0, "42"],
+    "nested": {"nested1": {"nested2": "42", "nested2-2": 41.99999}},
+}
+
 
-    (tmp_dir / "foo").write_text("foo")
+def test_run_params_default(tmp_dir, dvc):
+    (tmp_dir / "params.yaml").dump(supported_params)
     stage = dvc.run(
         name="read_params",
-        deps=["foo"],
-        outs=["bar"],
-        params=[
-            "params2.yaml:lists,floats,name",
-            "answer,floats,nested.nested1",
-        ],
-        cmd="cat params2.yaml params.yaml > bar",
+        params=["nested.nested1.nested2"],
+        cmd="cat params.yaml",
     )
+    assert isinstance(stage.deps[0], ParamsDependency)
+    assert stage.deps[0].params == ["nested.nested1.nested2"]
 
-    params, deps = split_params_deps(stage)
-    assert len(params) == 2
-    assert len(deps) == 1
-    assert len(stage.outs) == 1
+    lockfile = stage.dvcfile._lockfile
+    assert lockfile.load()["stages"]["read_params"]["params"] == {
+        "params.yaml": {"nested.nested1.nested2": "42"}
+    }
+
+    data, _ = stage.dvcfile._load()
+    assert data["stages"]["read_params"]["params"] == ["nested.nested1.nested2"]
+
+
+def test_run_params_custom_file(tmp_dir, dvc):
+    (tmp_dir / "params2.yaml").dump(supported_params)
+    stage = dvc.run(
+        name="read_params",
+        params=["params2.yaml:lists"],
+        cmd="cat params2.yaml",
+    )
 
+    isinstance(stage.deps[0], ParamsDependency)
+    assert stage.deps[0].params == ["lists"]
     lockfile = stage.dvcfile._lockfile
     assert lockfile.load()["stages"]["read_params"]["params"] == {
-        "params2.yaml": {
-            "lists": [42, 42.0, "42"],
-            "floats": 42.0,
-            "name": "Answer",
-        },
-        "params.yaml": {
-            "answer": 42,
-            "floats": 42.0,
-            "nested.nested1": {"nested2": "42", "nested2-2": 41.99999},
-        },
+        "params2.yaml": {"lists": [42, 42.0, "42"]}
     }
+
     data, _ = stage.dvcfile._load()
-    params = data["stages"]["read_params"]["params"]
+    assert data["stages"]["read_params"]["params"] == [{"params2.yaml": ["lists"]}]
 
-    custom, defaults = lsplit(lambda v: isinstance(v, dict), params)
-    assert set(custom[0]["params2.yaml"]) == {"name", "lists", "floats"}
-    assert set(defaults) == {"answer", "floats", "nested.nested1"}
-
-    assert not dvc.reproduce(stage.addressing)
-    params = deepcopy(supported_params)
-    params["answer"] = 43
-    (tmp_dir / "params.yaml").dump(params)
-
-    assert dvc.reproduce(stage.addressing) == [stage]
-
-
-@pytest.mark.parametrize("multiline", [True, False])
-def test_repro_list_of_commands_in_order(tmp_dir, dvc, multiline):
-    cmd = ["echo foo>foo", "echo bar>bar"]
-    if multiline:
-        cmd = "\n".join(cmd)
-
-    (tmp_dir / "dvc.yaml").dump({"stages": {"multi": {"cmd": cmd}}})
-
-    (tmp_dir / "dvc.yaml").write_text(
-        dedent(
-            """\
-            stages:
-              multi:
-                cmd:
-                - echo foo>foo
-                - echo bar>bar
-        """
-        )
+
+def test_run_params_no_exec(tmp_dir, dvc):
+    (tmp_dir / "params2.yaml").dump(supported_params)
+    stage = dvc.run(
+        name="read_params",
+        params=["params2.yaml:lists"],
+        cmd="cat params2.yaml",
+        no_exec=True,
+    )
+
+    isinstance(stage.deps[0], ParamsDependency)
+    assert stage.deps[0].params == ["lists"]
+    assert not stage.dvcfile._lockfile.exists()
+
+    data, _ = stage.dvcfile._load()
+    assert data["stages"]["read_params"]["params"] == [{"params2.yaml": ["lists"]}]
+
+
+@pytest.mark.parametrize(
+    "kwargs",
+    [
+        {"outs": ["foo"], "deps": ["bar"]},
+        {"outs": ["foo"], "deps": ["bar"], "name": "copy-foo-bar"},
+    ],
+)
+def test_run_without_cmd(tmp_dir, dvc, kwargs):
+    with pytest.raises(InvalidArgumentError) as exc:
+        dvc.run(**kwargs)
+    assert str(exc.value) == "command is not specified"
+
+
+def test_run_overwrite_order(tmp_dir, dvc, run_copy):
+    tmp_dir.gen({"foo": "foo", "foo1": "foo1"})
+    run_copy("foo", "bar", name="copy-foo-bar")
+    run_copy("bar", "foobar", name="copy-bar-foobar")
+
+    run_copy("foo1", "bar1", name="copy-foo-bar", force=True)
+
+    data = (tmp_dir / PROJECT_FILE).parse()
+    assert list(data["stages"].keys()) == ["copy-foo-bar", "copy-bar-foobar"]
+
+
+def test_run_overwrite_preserves_meta_and_comment(tmp_dir, dvc, run_copy):
+    tmp_dir.gen({"foo": "foo", "foo1": "foo1"})
+    text = textwrap.dedent(
+        """\
+        stages:
+          copy-foo-bar:
+            cmd: python copy.py {src} {dest}
+            deps:
+            - copy.py
+            - {src}
+            outs:
+            # comments are preserved
+            - {dest}
+            meta:
+              name: meta is preserved too
+    """
+    )
+    (tmp_dir / PROJECT_FILE).write_text(text.format(src="foo", dest="bar"))
+    assert dvc.reproduce(PROJECT_FILE)
+
+    assert run_copy("foo1", "bar1", name="copy-foo-bar", force=True)
+
+    assert (tmp_dir / PROJECT_FILE).read_text() == text.format(src="foo1", dest="bar1")
+
+
+def test_run_external_outputs(
+    tmp_dir,
+    dvc,
+    local_workspace,
+):
+    hash_name = "md5"
+    foo_hash = "acbd18db4cc2f85cedef654fccc4a4d8"
+    bar_hash = "37b51d194a7513e45b56f6524f2d51f2"
+
+    local_workspace.gen("foo", "foo")
+    dvc.run(
+        name="mystage",
+        cmd="mycmd",
+        deps=["remote://workspace/foo"],
+        outs=["remote://workspace/bar"],
+        no_exec=True,
+    )
+
+    dvc_yaml = (
+        "stages:\n"
+        "  mystage:\n"
+        "    cmd: mycmd\n"
+        "    deps:\n"
+        "    - remote://workspace/foo\n"
+        "    outs:\n"
+        "    - remote://workspace/bar\n"
+    )
+
+    assert (tmp_dir / "dvc.yaml").read_text() == dvc_yaml
+    assert not (tmp_dir / "dvc.lock").exists()
+
+    local_workspace.gen("bar", "bar")
+    dvc.commit("dvc.yaml", force=True)
+
+    assert (tmp_dir / "dvc.yaml").read_text() == dvc_yaml
+    assert (tmp_dir / "dvc.lock").read_text() == (
+        "schema: '2.0'\n"
+        "stages:\n"
+        "  mystage:\n"
+        "    cmd: mycmd\n"
+        "    deps:\n"
+        "    - path: remote://workspace/foo\n"
+        f"      {hash_name}: {foo_hash}\n"
+        "      size: 3\n"
+        "    outs:\n"
+        "    - path: remote://workspace/bar\n"
+        f"      {hash_name}: {bar_hash}\n"
+        "      size: 3\n"
     )
-    dvc.reproduce(targets=["multi"])
-    assert (tmp_dir / "foo").read_text() == "foo\n"
-    assert (tmp_dir / "bar").read_text() == "bar\n"
 
+    assert (local_workspace / "foo").read_text() == "foo"
+    assert (local_workspace / "bar").read_text() == "bar"
+    assert (
+        local_workspace / "cache" / bar_hash[:2] / bar_hash[2:]
+    ).read_text() == "bar"
+
+
+def test_rerun_callback(dvc):
+    def run_callback(force=False):
+        return dvc.run(cmd="echo content > out", force=force, name="echo")
+
+    assert run_callback() is not None
+    with pytest.raises(DuplicateStageName):
+        assert run_callback() is not None
+    assert run_callback(force=True) is not None
+
+
+def test_rerun_changed_dep(tmp_dir, run_copy):
+    tmp_dir.gen("foo", "foo content")
+    assert run_copy("foo", "out", name="copy") is not None
+
+    tmp_dir.gen("foo", "changed content")
+    with pytest.raises(DuplicateStageName):
+        run_copy("foo", "out", force=False, name="copy")
+    assert run_copy("foo", "out", force=True, name="copy")
+
+
+def test_run_remove_outs(tmp_dir, dvc, append_foo_script):
+    tmp_dir.gen("foo", "foo")
+    dvc.run(
+        deps=["append_foo.py"],
+        outs=["foo"],
+        cmd="python append_foo.py foo",
+        name="append-foo",
+    )
+
+
+@pytest.mark.parametrize("metrics_type", ["metrics", "metrics_no_cache"])
+def test_metrics_dir(tmp_dir, dvc, caplog, run_copy_metrics, metrics_type):
+    copyargs = {metrics_type: ["dir_metric"]}
+    tmp_dir.gen({"dir": {"file": "content"}})
+    with caplog.at_level(logging.DEBUG, "dvc"):
+        run_copy_metrics("dir", "dir_metric", name="copy-metrics", **copyargs)
+    assert "directory 'dir_metric' cannot be used as metrics." in caplog.messages
 
-@pytest.mark.parametrize("multiline", [True, False])
-def test_repro_list_of_commands_raise_and_stops_after_failure(tmp_dir, dvc, multiline):
-    cmd = ["echo foo>foo", "failed_command", "echo baz>bar"]
-    if multiline:
-        cmd = "\n".join(cmd)
 
-    (tmp_dir / "dvc.yaml").dump({"stages": {"multi": {"cmd": cmd}}})
+def test_rerun_deterministic(tmp_dir, run_copy, mocker):
+    from dvc.stage.run import subprocess
 
-    with pytest.raises(ReproductionError):
-        dvc.reproduce(targets=["multi"])
-    assert (tmp_dir / "foo").read_text() == "foo\n"
-    assert not (tmp_dir / "bar").exists()
+    tmp_dir.gen("foo", "foo content")
 
+    spy = mocker.spy(subprocess, "Popen")
 
-def test_repro_pulls_mising_data_source(tmp_dir, dvc, mocker, local_remote):
-    (foo,) = tmp_dir.dvc_gen("foo", "foo")
+    run_copy("foo", "out", name="copy")
+    assert spy.called
 
-    dvc.push()
+    spy.reset_mock()
+    run_copy("foo", "out", name="copy")
+    assert not spy.called
 
-    dvc.stage.add(name="copy-foo", cmd="cp foo bar", deps=["foo"], outs=["bar"])
-    remove("foo")
-    remove(foo.outs[0].cache_path)
 
-    assert dvc.reproduce(pull=True)
+def test_rerun_deterministic_ignore_cache(tmp_dir, run_copy, mocker):
+    from dvc.stage.run import subprocess
 
+    tmp_dir.gen("foo", "foo content")
 
-def test_repro_pulls_mising_import(tmp_dir, dvc, mocker, erepo_dir, local_remote):
-    with erepo_dir.chdir():
-        erepo_dir.dvc_gen("foo", "foo", commit="first")
+    spy = mocker.spy(subprocess, "Popen")
 
-    foo_import = dvc.imp(os.fspath(erepo_dir), "foo")
+    run_copy("foo", "out", name="copy")
+    assert spy.called
 
-    dvc.push()
+    spy.reset_mock()
+    run_copy("foo", "out", run_cache=False, name="copy")
+    assert spy.called
 
-    dvc.stage.add(name="copy-foo", cmd="cp foo bar", deps=["foo"], outs=["bar"])
-    remove("foo")
-    remove(foo_import.outs[0].cache_path)
 
-    assert dvc.reproduce(pull=True)
+def test_rerun_changed_stage(tmp_dir, run_copy):
+    tmp_dir.gen("foo", "foo content")
+    assert run_copy("foo", "out", name="copy") is not None
 
+    tmp_dir.gen("bar", "bar content")
+    with pytest.raises(DuplicateStageName):
+        run_copy("bar", "out", force=False, name="copy")
 
-def test_repro_allow_missing(tmp_dir, dvc):
-    tmp_dir.gen("fixed", "fixed")
-    dvc.stage.add(name="create-foo", cmd="echo foo > foo", deps=["fixed"], outs=["foo"])
-    dvc.stage.add(name="copy-foo", cmd="cp foo bar", deps=["foo"], outs=["bar"])
-    (create_foo, copy_foo) = dvc.reproduce()
 
-    remove("foo")
-    remove(create_foo.outs[0].cache_path)
-    remove(dvc.stage_cache.cache_dir)
+def test_rerun_changed_out(tmp_dir, run_copy):
+    tmp_dir.gen("foo", "foo content")
+    assert run_copy("foo", "out", name="copy") is not None
 
-    ret = dvc.reproduce(allow_missing=True)
-    # both stages are skipped
-    assert not ret
+    tmp_dir.gen("out", "modification")
+    with pytest.raises(DuplicateStageName):
+        run_copy("foo", "out", force=False, name="copy")
+
+
+def test_should_raise_on_overlapping_output_paths(tmp_dir, dvc, append_foo_script):
+    tmp_dir.gen("data", {"foo": "foo", "bar": "bar"})
+    ret = main(["add", "data"])
+    assert ret == 0
+
+    foo_file = os.path.join("data", "foo")
+    with pytest.raises(OverlappingOutputPathsError) as err:
+        dvc.run(
+            outs=["data/foo"],
+            cmd=f"python append_foo.py {foo_file}",
+            name="append-foo",
+        )
+
+    error_output = str(err.value)
+
+    assert "The output paths:\n" in error_output
+    assert "\n'data'('data.dvc')\n" in error_output
+    assert f"\n'{foo_file}'('append-foo')\n" in error_output
+    assert (
+        "overlap and are thus in the same tracked directory.\n"
+        "To keep reproducibility, outputs should be in separate "
+        "tracked directories or tracked individually." in error_output
+    )
+
+
+def test_should_not_checkout_upon_corrupted_local_hardlink_cache(
+    mocker, tmp_dir, dvc, copy_script
+):
+    tmp_dir.gen("foo", "foo")
+    dvc.cache.local.cache_types = ["hardlink"]
+
+    stage = dvc.run(
+        deps=["foo"],
+        outs=["bar"],
+        cmd="python copy.py foo bar",
+        name="copy",
+    )
 
+    os.chmod("bar", 0o644)
+    with open("bar", "w", encoding="utf-8") as fd:
+        fd.write("corrupting the output cache")
 
-def test_repro_allow_missing_and_pull(tmp_dir, dvc, mocker, local_remote):
-    tmp_dir.gen("fixed", "fixed")
-    dvc.stage.add(name="create-foo", cmd="echo foo > foo", deps=["fixed"], outs=["foo"])
-    dvc.stage.add(name="copy-foo", cmd="cp foo bar", deps=["foo"], outs=["bar"])
-    (create_foo,) = dvc.reproduce("create-foo")
+    spy_checkout = mocker.spy(stage.outs[0], "checkout")
+    from dvc.stage import run as stage_run
 
-    dvc.push()
+    spy_run = mocker.spy(stage_run, "cmd_run")
 
-    remove("foo")
-    remove(create_foo.outs[0].cache_path)
-    remove(dvc.stage_cache.cache_dir)
+    with dvc.lock:
+        stage.run()
 
-    ret = dvc.reproduce(pull=True, allow_missing=True)
-    # create-foo is skipped ; copy-foo pulls missing dep
-    assert len(ret) == 1
+        spy_run.assert_called_once()
+        spy_checkout.assert_not_called()
```

### Comparing `dvc-3.0.0a1/tests/func/test_run_cache.py` & `dvc-3.0.0a2/tests/func/test_run_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_scm.py` & `dvc-3.0.0a2/tests/func/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_scm_context.py` & `dvc-3.0.0a2/tests/func/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_stage.py` & `dvc-3.0.0a2/tests/func/test_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,18 @@
 
 
 def test_cmd_obj():
     with pytest.raises(YAMLValidationError):
         SingleStageFile.validate({Stage.PARAM_CMD: {}})
 
 
-def test_cmd_none():
-    SingleStageFile.validate({Stage.PARAM_CMD: None})
-
-
 def test_no_cmd():
     SingleStageFile.validate({})
 
 
-def test_cmd_str():
-    SingleStageFile.validate({Stage.PARAM_CMD: "cmd"})
-
-
 def test_object():
     with pytest.raises(YAMLValidationError):
         SingleStageFile.validate({Stage.PARAM_DEPS: {}})
 
     with pytest.raises(YAMLValidationError):
         SingleStageFile.validate({Stage.PARAM_OUTS: {}})
 
@@ -85,43 +77,38 @@
 
     d = load_yaml(stage.relpath)
     assert d[stage.PARAM_MD5] == md5
 
 
 def test_default_wdir_ignored_in_checksum(tmp_dir, dvc):
     tmp_dir.gen("bar", "bar")
-    stage = dvc.run(
-        cmd="cp bar foo",
-        deps=["bar"],
-        outs=["foo"],
-        single_stage=True,
-    )
+    stage = dvc.run(cmd="cp bar foo", deps=["bar"], outs=["foo"], name="copy-foo-bar")
 
     d = stage.dumpd()
     assert Stage.PARAM_WDIR not in d.keys()
 
-    d = load_yaml(stage.relpath)
-    assert Stage.PARAM_WDIR not in d.keys()
+    d = load_yaml("dvc.yaml")
+    assert Stage.PARAM_WDIR not in d["stages"]["copy-foo-bar"]
 
     with dvc.lock:
-        stage = SingleStageFile(dvc, stage.relpath).stage
+        stage = stage.reload()
         assert not stage.changed()
 
 
 def test_external_remote_output_resolution(tmp_dir, dvc, make_remote):
     tmp_path = make_remote("tmp", default=False)
     tmp_dir.add_remote(url="remote://tmp/storage", name="storage", default=False)
     storage = tmp_path / "storage"
     storage.mkdir()
     file_path = storage / "file"
 
     dvc.run(
         cmd=f"echo file > {file_path}",
         outs_no_cache=["remote://storage/file"],
-        single_stage=True,
+        name="gen-file",
     )
     assert os.path.exists(file_path)
 
 
 def test_external_remote_dependency_resolution(tmp_dir, dvc, make_remote):
     tmp_path = make_remote("tmp", default=False)
     tmp_dir.add_remote(url="remote://tmp/storage", name="storage", default=False)
@@ -241,24 +228,23 @@
         dvc.stage.collect(target=str(data_link / "foo.dvc"), with_deps=with_deps)
     )[0]
 
     assert stage.addressing == f"{foo_path}.dvc"
 
 
 def test_stage_strings_representation(tmp_dir, dvc, run_copy):
-    tmp_dir.dvc_gen("foo", "foo")
-    stage1 = run_copy("foo", "bar", single_stage=True)
-    assert stage1.addressing == "bar.dvc"
-    assert repr(stage1) == "Stage: 'bar.dvc'"
-    assert str(stage1) == "stage: 'bar.dvc'"
-
-    stage2 = run_copy("bar", "baz", name="copy-bar-baz")
-    assert stage2.addressing == "copy-bar-baz"
-    assert repr(stage2) == "Stage: 'copy-bar-baz'"
-    assert str(stage2) == "stage: 'copy-bar-baz'"
+    (stage1,) = tmp_dir.dvc_gen("foo", "foo")
+    assert stage1.addressing == "foo.dvc"
+    assert repr(stage1) == "Stage: 'foo.dvc'"
+    assert str(stage1) == "stage: 'foo.dvc'"
+
+    stage2 = run_copy("foo", "bar", name="copy-foo-bar")
+    assert stage2.addressing == "copy-foo-bar"
+    assert repr(stage2) == "Stage: 'copy-foo-bar'"
+    assert str(stage2) == "stage: 'copy-foo-bar'"
 
     folder = tmp_dir / "dir"
     folder.mkdir()
     with folder.chdir():
         # `Stage` caches `relpath` results, forcing it to reset
         stage1.path = stage1.path
         stage2.path = stage2.path
```

### Comparing `dvc-3.0.0a1/tests/func/test_stage_load.py` & `dvc-3.0.0a2/tests/func/test_stage_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,50 +22,56 @@
         return {
             str(out)
             for stage in dvc.stage.collect(*args, **kwargs)
             for out in stage.outs
         }
 
     tmp_dir.dvc_gen("foo", "foo")
-    run_copy("foo", "bar", single_stage=True)
-    scm.add([".gitignore", "foo.dvc", "bar.dvc"])
+    run_copy("foo", "bar", name="copy-foo-bar")
+    scm.add([".gitignore", "foo.dvc", "dvc.yaml", "dvc.lock"])
     scm.commit("Add foo and bar")
 
     scm.checkout("new-branch", create_new=True)
 
-    run_copy("bar", "buzz", single_stage=True)
-    scm.add([".gitignore", "buzz.dvc"])
+    run_copy("bar", "buzz", name="copy-bar-buzz")
+    scm.add([".gitignore", "dvc.yaml", "dvc.lock"])
     scm.commit("Add buzz")
 
-    assert collect_outs("bar.dvc", with_deps=True) == {"foo", "bar"}
-    assert collect_outs("buzz.dvc", with_deps=True) == {"foo", "bar", "buzz"}
-    assert collect_outs("buzz.dvc", with_deps=False) == {"buzz"}
+    assert collect_outs("copy-foo-bar", with_deps=True) == {"foo", "bar"}
+    assert collect_outs("copy-bar-buzz", with_deps=True) == {"foo", "bar", "buzz"}
+    assert collect_outs("copy-bar-buzz", with_deps=False) == {"buzz"}
 
     run_copy("foo", "foobar", name="copy-foo-foobar")
     assert collect_outs(":copy-foo-foobar") == {"foobar"}
     assert collect_outs(":copy-foo-foobar", with_deps=True) == {
         "foobar",
         "foo",
     }
     assert collect_outs("dvc.yaml:copy-foo-foobar", recursive=True) == {"foobar"}
     assert collect_outs("copy-foo-foobar") == {"foobar"}
     assert collect_outs("copy-foo-foobar", with_deps=True) == {"foobar", "foo"}
     assert collect_outs("copy-foo-foobar", recursive=True) == {"foobar"}
 
     run_copy("foobar", "baz", name="copy-foobar-baz")
-    assert collect_outs("dvc.yaml") == {"foobar", "baz"}
-    assert collect_outs("dvc.yaml", with_deps=True) == {"foobar", "baz", "foo"}
+    assert collect_outs("dvc.yaml") == {"foobar", "baz", "bar", "buzz"}
+    assert collect_outs("dvc.yaml", with_deps=True) == {
+        "foobar",
+        "baz",
+        "bar",
+        "buzz",
+        "foo",
+    }
 
 
 def test_collect_dir_recursive(tmp_dir, dvc, run_head):
     tmp_dir.gen({"dir": {"foo": "foo"}})
-    (stage1,) = dvc.add("dir", recursive=True)
+    (stage1,) = dvc.add("dir/*", glob=True)
     with (tmp_dir / "dir").chdir():
-        stage2 = run_head("foo", name="copy-foo-bar")
-        stage3 = run_head("foo-1", single_stage=True)
+        stage2 = run_head("foo", name="head-foo")
+        stage3 = run_head("foo-1", name="head-foo1")
     assert set(dvc.stage.collect("dir", recursive=True)) == {
         stage1,
         stage2,
         stage3,
     }
 
 
@@ -97,15 +103,15 @@
 
 @pytest.fixture
 def stages(tmp_dir, run_copy):
     stage1, stage2 = tmp_dir.dvc_gen({"foo": "foo", "lorem": "lorem"})
     return {
         "foo-generate": stage1,
         "lorem-generate": stage2,
-        "copy-foo-bar": run_copy("foo", "bar", single_stage=True),
+        "copy-foo-bar": run_copy("foo", "bar", name="copy-foo-bar"),
         "copy-bar-foobar": run_copy("bar", "foobar", name="copy-bar-foobar"),
         "copy-lorem-ipsum": run_copy("lorem", "ipsum", name="copy-lorem-ipsum"),
     }
 
 
 def test_collect_not_a_group_stage_with_group_flag(tmp_dir, dvc, stages):
     assert set(dvc.stage.collect("copy-bar-foobar")) == {stages["copy-bar-foobar"]}
@@ -143,35 +149,37 @@
     stages_info = {(stage, None) for stage in all_stages}
     assert set(dvc.stage.collect_granular("build")) == stages_info
     assert set(dvc.stage.collect_granular("build", with_deps=True)) == stages_info
 
 
 def test_collect_glob(tmp_dir, dvc, stages):
     assert set(dvc.stage.collect("copy*", glob=True)) == {
-        stages[key] for key in ["copy-bar-foobar", "copy-lorem-ipsum"]
+        stages[key] for key in ["copy-bar-foobar", "copy-foo-bar", "copy-lorem-ipsum"]
     }
     assert set(dvc.stage.collect("copy-lorem*", glob=True, with_deps=True)) == {
         stages[key] for key in ["copy-lorem-ipsum", "lorem-generate"]
     }
 
 
 def test_collect_granular_with_no_target(tmp_dir, dvc, stages):
     assert set(map(itemgetter(0), dvc.stage.collect_granular())) == set(stages.values())
     assert list(map(itemgetter(1), dvc.stage.collect_granular())) == [None] * len(
         stages
     )
 
 
 def test_collect_granular_with_target(tmp_dir, dvc, stages):
-    assert dvc.stage.collect_granular("bar.dvc") == [(stages["copy-foo-bar"], None)]
+    assert dvc.stage.collect_granular("foo.dvc") == [(stages["foo-generate"], None)]
     assert dvc.stage.collect_granular(PROJECT_FILE) == [
+        (stages["copy-foo-bar"], None),
         (stages["copy-bar-foobar"], None),
         (stages["copy-lorem-ipsum"], None),
     ]
     assert dvc.stage.collect_granular(":") == [
+        (stages["copy-foo-bar"], None),
         (stages["copy-bar-foobar"], None),
         (stages["copy-lorem-ipsum"], None),
     ]
     assert dvc.stage.collect_granular("copy-bar-foobar") == [
         (stages["copy-bar-foobar"], None)
     ]
     assert dvc.stage.collect_granular(":copy-bar-foobar") == [
@@ -214,15 +222,15 @@
         dvc.stage.collect_granular("some_file", recursive=True)
 
 
 def test_collect_granular_with_deps(tmp_dir, dvc, stages):
     assert set(
         map(
             itemgetter(0),
-            dvc.stage.collect_granular("bar.dvc", with_deps=True),
+            dvc.stage.collect_granular("copy-foo-bar", with_deps=True),
         )
     ) == {stages["copy-foo-bar"], stages["foo-generate"]}
     assert set(
         map(
             itemgetter(0),
             dvc.stage.collect_granular("copy-bar-foobar", with_deps=True),
         )
@@ -256,15 +264,15 @@
     assert dvc.stage.collect_granular("./copy-foo-bar", with_deps=True) == [
         (stage2, os.path.join(tmp_dir / "copy-foo-bar"))
     ]
 
 
 def test_collect_granular_priority_on_collision(tmp_dir, dvc, run_copy):
     tmp_dir.gen({"dir": {"foo": "foo"}, "foo": "foo"})
-    (stage1,) = dvc.add("dir", recursive=True)
+    (stage1,) = dvc.add("dir/*", glob=True)
     stage2 = run_copy("foo", "bar", name="dir")
 
     assert dvc.stage.collect_granular("dir") == [(stage2, None)]
     assert dvc.stage.collect_granular("dir", recursive=True) == [(stage1, None)]
 
     remove(tmp_dir / "dir")
```

### Comparing `dvc-3.0.0a1/tests/func/test_state.py` & `dvc-3.0.0a2/tests/func/test_state.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_status.py` & `dvc-3.0.0a2/tests/func/test_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 
 from dvc.cli import main
+from dvc.fs import localfs
 
 
 def test_quiet(tmp_dir, dvc, capsys):
     tmp_dir.dvc_gen("foo", "foo")
 
     # clear
     capsys.readouterr()
@@ -92,15 +93,15 @@
             "changed command",
         ],
     }
 
 
 def test_status_recursive(tmp_dir, dvc):
     tmp_dir.gen({"dir": {"file": "text1", "subdir": {"file2": "text2"}}})
-    stages = dvc.add("dir", recursive=True, no_commit=True)
+    stages = dvc.add(localfs.find("dir"), no_commit=True)
 
     assert len(stages) == 2
 
     assert dvc.status(targets=["dir"], recursive=True) == {
         os.path.join("dir", "file.dvc"): [
             {"changed outs": {os.path.join("dir", "file"): "not in cache"}}
         ],
```

### Comparing `dvc-3.0.0a1/tests/func/test_unprotect.py` & `dvc-3.0.0a2/tests/func/test_unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_update.py` & `dvc-3.0.0a2/tests/func/test_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -370,15 +370,18 @@
 
 
 def test_update_import_url_to_remote(tmp_dir, dvc, workspace, local_remote):
     workspace.gen("foo", "foo")
     stage = dvc.imp_url("remote://workspace/foo", to_remote=True)
 
     workspace.gen("foo", "bar")
-    stage = dvc.update(stage.path, to_remote=True)
+    (updated,) = dvc.update(stage.path, to_remote=True)
+
+    assert stage.deps[0].hash_info != updated.deps[0].hash_info
+    assert stage.outs[0].hash_info != updated.outs[0].hash_info
 
     dvc.pull("foo")
     assert (tmp_dir / "foo").read_text() == "bar"
 
 
 def test_update_import_url_to_remote_directory(
     mocker, tmp_dir, dvc, workspace, local_remote
@@ -396,15 +399,18 @@
                     "baz": "baz",
                     "foo_with_different_name": "foo",
                 },
             }
         }
     )
 
-    stage = dvc.update(stage.path, to_remote=True)
+    (updated,) = dvc.update(stage.path, to_remote=True)
+
+    assert stage.deps[0].hash_info != updated.deps[0].hash_info
+    assert stage.outs[0].hash_info != updated.outs[0].hash_info
 
     dvc.pull("data")
     assert (tmp_dir / "data").read_text() == {
         "foo": "foo",
         "foo2": "foo2",
         "bar": {"baz": "baz", "baz2": "baz2"},
         "repeated_hashes": {
@@ -420,15 +426,18 @@
 ):
     local_workspace.gen({"data": {"foo": "foo", "bar": {"baz": "baz"}}})
     stage = dvc.imp_url("remote://workspace/data", to_remote=True)
 
     local_workspace.gen(
         {"data": {"foo": "not_foo", "foo2": "foo", "bar": {"baz2": "baz2"}}}
     )
-    stage = dvc.update(stage.path, to_remote=True)
+    (updated,) = dvc.update(stage.path, to_remote=True)
+
+    assert stage.deps[0].hash_info != updated.deps[0].hash_info
+    assert stage.outs[0].hash_info != updated.outs[0].hash_info
 
     dvc.pull("data")
     assert (tmp_dir / "data").read_text() == {
         "foo": "not_foo",
         "foo2": "foo",
         "bar": {"baz": "baz", "baz2": "baz2"},
     }
@@ -437,15 +446,18 @@
 def test_update_import_url_to_remote_directory_same_hash(
     tmp_dir, dvc, local_workspace, local_remote
 ):
     local_workspace.gen({"data": {"foo": "foo", "bar": {"baz": "baz"}, "same": "same"}})
     stage = dvc.imp_url("remote://workspace/data", to_remote=True)
 
     local_workspace.gen({"data": {"foo": "baz", "bar": {"baz": "foo"}, "same": "same"}})
-    stage = dvc.update(stage.path, to_remote=True)
+    (updated,) = dvc.update(stage.path, to_remote=True)
+
+    assert stage.deps[0].hash_info != updated.deps[0].hash_info
+    assert stage.outs[0].hash_info != updated.outs[0].hash_info
 
     dvc.pull("data")
     assert (tmp_dir / "data").read_text() == {
         "foo": "baz",
         "bar": {"baz": "foo"},
         "same": "same",
     }
```

### Comparing `dvc-3.0.0a1/tests/func/test_used_objs.py` & `dvc-3.0.0a2/tests/func/test_used_objs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_utils.py` & `dvc-3.0.0a2/tests/func/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_version.py` & `dvc-3.0.0a2/tests/func/test_version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/test_virtual_directory.py` & `dvc-3.0.0a2/tests/func/test_virtual_directory.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/utils/test_hydra.py` & `dvc-3.0.0a2/tests/func/utils/test_hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/func/utils/test_strict_yaml.py` & `dvc-3.0.0a2/tests/func/utils/test_strict_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/integration/plots/conftest.py` & `dvc-3.0.0a2/tests/integration/plots/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/integration/plots/test_plots.py` & `dvc-3.0.0a2/tests/integration/plots/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/integration/plots/test_repo_plots_api.py` & `dvc-3.0.0a2/tests/integration/plots/test_repo_plots_api.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/integration/test_studio_live_experiments.py` & `dvc-3.0.0a2/tests/integration/test_studio_live_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/remotes/git_server.py` & `dvc-3.0.0a2/tests/remotes/git_server.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/remotes/user.key` & `dvc-3.0.0a2/tests/remotes/user.key`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/remotes_env.sample` & `dvc-3.0.0a2/tests/remotes_env.sample`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/scripts.py` & `dvc-3.0.0a2/tests/scripts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/cli/test_main.py` & `dvc-3.0.0a2/tests/unit/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/ls/test_ls.py` & `dvc-3.0.0a2/tests/unit/command/ls/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/ls/test_ls_colors.py` & `dvc-3.0.0a2/tests/unit/command/ls/test_ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_add.py` & `dvc-3.0.0a2/tests/unit/command/test_add.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,41 +4,36 @@
 from dvc.commands.add import CmdAdd
 
 
 def test_add(mocker, dvc):
     cli_args = parse_args(
         [
             "add",
-            "--recursive",
             "--no-commit",
             "--external",
             "--glob",
-            "--file",
-            "file",
             "data",
         ]
     )
     assert cli_args.func == CmdAdd
 
     cmd = cli_args.func(cli_args)
     m = mocker.patch.object(cmd.repo, "add", autospec=True)
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         ["data"],
-        recursive=True,
         no_commit=True,
         glob=True,
-        fname="file",
         external=True,
         out=None,
         remote=None,
         to_remote=False,
-        jobs=None,
+        remote_jobs=None,
         force=False,
     )
 
 
 def test_add_to_remote(mocker):
     cli_args = parse_args(
         [
@@ -56,38 +51,36 @@
     cmd = cli_args.func(cli_args)
     m = mocker.patch.object(cmd.repo, "add", autospec=True)
 
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         ["s3://bucket/foo"],
-        recursive=False,
         no_commit=False,
         glob=False,
-        fname=None,
         external=False,
         out="bar",
         remote="remote",
         to_remote=True,
-        jobs=None,
+        remote_jobs=None,
         force=False,
     )
 
 
 def test_add_to_remote_invalid_combinations(mocker, caplog):
     cli_args = parse_args(["add", "s3://bucket/foo", "s3://bucket/bar", "--to-remote"])
     assert cli_args.func == CmdAdd
 
     cmd = cli_args.func(cli_args)
     with caplog.at_level(logging.ERROR, logger="dvc"):
         assert cmd.run() == 1
         expected_msg = "multiple targets can't be used with --to-remote"
         assert expected_msg in caplog.text
 
-    for option, value in (("--remote", "remote"), ("--jobs", "4")):
+    for option, value in (("--remote", "remote"), ("--remote-jobs", "4")):
         cli_args = parse_args(["add", "foo", option, value])
 
         cmd = cli_args.func(cli_args)
         with caplog.at_level(logging.ERROR, logger="dvc"):
             assert cmd.run() == 1
             expected_msg = f"{option} can't be used without --to-remote"
             assert expected_msg in caplog.text
@@ -96,9 +89,9 @@
 def test_add_to_cache_invalid_combinations(mocker, caplog):
     cli_args = parse_args(["add", "s3://bucket/foo", "s3://bucket/bar", "-o", "foo"])
     assert cli_args.func == CmdAdd
 
     cmd = cli_args.func(cli_args)
     with caplog.at_level(logging.ERROR, logger="dvc"):
         assert cmd.run() == 1
-        expected_msg = "multiple targets can't be used with -o"
+        expected_msg = "multiple targets can't be used with --out"
         assert expected_msg in caplog.text
```

### Comparing `dvc-3.0.0a1/tests/unit/command/test_cache.py` & `dvc-3.0.0a2/tests/unit/command/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_checkout.py` & `dvc-3.0.0a2/tests/unit/command/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_compat_flag.py` & `dvc-3.0.0a2/tests/unit/command/test_compat_flag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_config.py` & `dvc-3.0.0a2/tests/unit/command/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_dag.py` & `dvc-3.0.0a2/tests/unit/command/test_dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_data_status.py` & `dvc-3.0.0a2/tests/unit/command/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_data_sync.py` & `dvc-3.0.0a2/tests/unit/command/test_data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_diff.py` & `dvc-3.0.0a2/tests/unit/command/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_experiments.py` & `dvc-3.0.0a2/tests/unit/command/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_gc.py` & `dvc-3.0.0a2/tests/unit/command/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_get.py` & `dvc-3.0.0a2/tests/unit/command/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_git_hook.py` & `dvc-3.0.0a2/tests/unit/command/test_git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_imp.py` & `dvc-3.0.0a2/tests/unit/command/test_imp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_imp_url.py` & `dvc-3.0.0a2/tests/unit/command/test_imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_ls_url.py` & `dvc-3.0.0a2/tests/unit/command/test_ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_machine.py` & `dvc-3.0.0a2/tests/unit/command/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_metrics.py` & `dvc-3.0.0a2/tests/unit/command/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_params.py` & `dvc-3.0.0a2/tests/unit/command/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_plots.py` & `dvc-3.0.0a2/tests/unit/command/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_queue.py` & `dvc-3.0.0a2/tests/unit/command/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_repro.py` & `dvc-3.0.0a2/tests/unit/command/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_stage.py` & `dvc-3.0.0a2/tests/unit/command/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_status.py` & `dvc-3.0.0a2/tests/unit/command/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/command/test_update.py` & `dvc-3.0.0a2/tests/unit/command/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/data/db/test_local.py` & `dvc-3.0.0a2/tests/unit/data/db/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/dependency/test_params.py` & `dvc-3.0.0a2/tests/unit/dependency/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/fs/test_azure.py` & `dvc-3.0.0a2/tests/unit/fs/test_azure.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/fs/test_data.py` & `dvc-3.0.0a2/tests/unit/fs/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import posixpath
 import shutil
 
 import pytest
 
 import dvc_data
+from dvc.fs import localfs
 from dvc.fs.data import DataFileSystem
 from dvc.utils.fs import remove
 from dvc_data.hashfile.build import build
 from dvc_data.hashfile.hash_info import HashInfo
 
 
 @pytest.mark.parametrize(
@@ -133,15 +134,15 @@
                 "subdir2": {"foo2": "foo2"},
                 "foo": "foo",
                 "bar": "bar",
             }
         }
     )
 
-    dvc.add("dir", recursive=True)
+    dvc.add(localfs.find("dir"))
     fs = DataFileSystem(index=dvc.index.data["repo"])
 
     expected = [
         "dir/subdir1",
         "dir/subdir2",
         "dir/subdir1/foo1",
         "dir/subdir1/bar1",
@@ -204,22 +205,14 @@
     tmp_dir.dvc_gen("foo", "foo")
     fs = DataFileSystem(index=dvc.index.data["repo"])
 
     for _ in fs.walk("foo"):
         pass
 
 
-def test_isdvc(tmp_dir, dvc):
-    tmp_dir.gen({"foo": "foo", "bar": "bar"})
-    dvc.add("foo")
-    fs = DataFileSystem(index=dvc.index.data["repo"])
-    assert fs.isdvc("foo")
-    assert not fs.isdvc("bar")
-
-
 def test_get_hash_file(tmp_dir, dvc):
     tmp_dir.dvc_gen({"foo": "foo"})
     fs = DataFileSystem(index=dvc.index.data["repo"])
     assert fs.info("foo")["md5"] == "acbd18db4cc2f85cedef654fccc4a4d8"
 
 
 def test_get_hash_dir(tmp_dir, dvc, mocker):
```

### Comparing `dvc-3.0.0a1/tests/unit/fs/test_dvc.py` & `dvc-3.0.0a2/tests/unit/fs/test_dvc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import posixpath
 import shutil
 from unittest import mock
 
 import pytest
 
+from dvc.fs import localfs
 from dvc.fs.dvc import DVCFileSystem
 from dvc.testing.tmp_dir import make_subrepo
 from dvc_data.hashfile.build import build
 from dvc_data.hashfile.hash_info import HashInfo
 
 
 def test_exists(tmp_dir, dvc):
@@ -181,15 +182,15 @@
         {
             "dir": {
                 "subdir1": {"foo1": "foo1", "bar1": "bar1"},
                 "subdir2": {"foo2": "foo2"},
             }
         }
     )
-    dvc.add(str(tmp_dir / "dir"), recursive=True)
+    dvc.add(localfs.find("dir"))
     tmp_dir.gen({"dir": {"foo": "foo", "bar": "bar"}})
     fs = DVCFileSystem(repo=dvc)
 
     expected = [
         "dir/subdir1",
         "dir/subdir2",
         "dir/subdir1/foo1",
```

### Comparing `dvc-3.0.0a1/tests/unit/fs/test_dvc_info.py` & `dvc-3.0.0a2/tests/unit/fs/test_dvc_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/fs/test_fs.py` & `dvc-3.0.0a2/tests/unit/fs/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/fs/test_path.py` & `dvc-3.0.0a2/tests/unit/fs/test_path.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/fs/test_s3.py` & `dvc-3.0.0a2/tests/unit/fs/test_s3.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/fs/test_tree.py` & `dvc-3.0.0a2/tests/unit/fs/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/machine/test_machine.py` & `dvc-3.0.0a2/tests/unit/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/output/test_load.py` & `dvc-3.0.0a2/tests/unit/output/test_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/output/test_local.py` & `dvc-3.0.0a2/tests/unit/output/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/output/test_output.py` & `dvc-3.0.0a2/tests/unit/output/test_output.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/remote/test_oss.py` & `dvc-3.0.0a2/tests/unit/remote/test_oss.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/remote/test_remote.py` & `dvc-3.0.0a2/tests/unit/remote/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/remote/test_webdav.py` & `dvc-3.0.0a2/tests/unit/remote/test_webdav.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/remote/test_webhdfs.py` & `dvc-3.0.0a2/tests/unit/remote/test_webhdfs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/render/test_convert.py` & `dvc-3.0.0a2/tests/unit/render/test_convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/render/test_image_converter.py` & `dvc-3.0.0a2/tests/unit/render/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/render/test_match.py` & `dvc-3.0.0a2/tests/unit/render/test_match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/render/test_vega_converter.py` & `dvc-3.0.0a2/tests/unit/render/test_vega_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/repo/experiments/conftest.py` & `dvc-3.0.0a2/tests/unit/repo/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/repo/experiments/queue/test_celery.py` & `dvc-3.0.0a2/tests/unit/repo/experiments/queue/test_celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/repo/experiments/queue/test_remove.py` & `dvc-3.0.0a2/tests/unit/repo/experiments/queue/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/repo/experiments/test_executor_status.py` & `dvc-3.0.0a2/tests/unit/repo/experiments/test_executor_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/repo/experiments/test_remove.py` & `dvc-3.0.0a2/tests/unit/repo/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/repo/experiments/test_utils.py` & `dvc-3.0.0a2/tests/unit/repo/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/repo/plots/test_diff.py` & `dvc-3.0.0a2/tests/unit/repo/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/repo/test_open_repo.py` & `dvc-3.0.0a2/tests/unit/repo/test_open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/repo/test_repo.py` & `dvc-3.0.0a2/tests/unit/repo/test_repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,29 +78,29 @@
     from dvc.repo.index import Index
 
     mock_build_graph = mocker.spy(Index.graph, "fget")
 
     # sanity check
     tmp_dir.gen("foo", "foo text")
     dvc.add("foo")
-    run_copy("foo", "bar", single_stage=True)
+    run_copy("foo", "bar", name="copy-foo-bar")
     assert mock_build_graph.called
 
     # check that our hack can be enabled
     mock_build_graph.reset_mock()
     dvc._skip_graph_checks = True
     tmp_dir.gen("baz", "baz text")
-    run_copy("baz", "qux", single_stage=True)
+    run_copy("baz", "qux", name="copy-baz-qux")
     assert not mock_build_graph.called
 
     # check that our hack can be disabled
     mock_build_graph.reset_mock()
     dvc._skip_graph_checks = False
     tmp_dir.gen("quux", "quux text")
-    run_copy("quux", "quuz", single_stage=True)
+    run_copy("quux", "quuz", name="copy-quux-quuz")
     assert mock_build_graph.called
 
 
 def test_branch_config(tmp_dir, scm):
     tmp_dir.scm_gen("foo", "foo", commit="init")
 
     # sanity check
```

### Comparing `dvc-3.0.0a1/tests/unit/repo/test_reproduce.py` & `dvc-3.0.0a2/tests/unit/repo/test_reproduce.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 def test_number_reproduces(tmp_dir, dvc, mocker):
     reproduce_stage_mock = mocker.patch(
         "dvc.repo.reproduce._reproduce_stage", returns=[]
     )
     tmp_dir.dvc_gen({"pre-foo": "pre-foo"})
 
-    dvc.run(single_stage=True, deps=["pre-foo"], outs=["foo"], cmd="echo foo > foo")
-    dvc.run(single_stage=True, deps=["foo"], outs=["bar"], cmd="echo bar > bar")
-    dvc.run(single_stage=True, deps=["foo"], outs=["baz"], cmd="echo baz > baz")
-    dvc.run(single_stage=True, deps=["bar"], outs=["boop"], cmd="echo boop > boop")
+    dvc.run(name="echo-foo", outs=["foo"], cmd="echo foo > foo")
+    dvc.run(name="echo-bar", deps=["foo"], outs=["bar"], cmd="echo bar > bar")
+    dvc.run(name="echo-baz", deps=["foo"], outs=["baz"], cmd="echo baz > baz")
+    dvc.run(name="echo-boop", deps=["bar"], outs=["boop"], cmd="echo boop > boop")
 
     reproduce_stage_mock.reset_mock()
 
     dvc.reproduce(all_pipelines=True)
 
     assert reproduce_stage_mock.call_count == 5
```

### Comparing `dvc-3.0.0a1/tests/unit/repo/test_scm_context.py` & `dvc-3.0.0a2/tests/unit/repo/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/scm/test_scm.py` & `dvc-3.0.0a2/tests/unit/scm/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/stage/test_cache.py` & `dvc-3.0.0a2/tests/unit/stage/test_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,23 @@
         "script.py",
         'open("out", "w+").write("out"); ',
     )
     stage = dvc.run(
         cmd="python script.py",
         deps=["script.py", "dep"],
         outs=["out"],
-        single_stage=True,
+        name="write-out",
     )
 
     with dvc.lock:
         stage.remove(remove_outs=True, force=True)
 
     assert not (tmp_dir / "out").exists()
-    assert not (tmp_dir / "out.dvc").exists()
+    assert not (tmp_dir / "dvc.yaml").exists()
+    assert not (tmp_dir / "dvc.lock").exists()
 
     cache_dir = os.path.join(
         dvc.stage_cache.cache_dir,
         "4b",
         "4b495dc2b14e1ca5bd5f2765a99ddd8785523a8342efe6bcadac012c2db01165",
     )
     cache_file = os.path.join(
@@ -57,22 +58,23 @@
         "script.py",
         'open("out", "w+").write("out"); ',
     )
     stage = dvc.run(
         cmd="python script.py",
         params=["foo,bar", "myparams.yaml:baz,qux"],
         outs=["out"],
-        single_stage=True,
+        name="write-out",
     )
 
     with dvc.lock:
         stage.remove(remove_outs=True, force=True)
 
     assert not (tmp_dir / "out").exists()
-    assert not (tmp_dir / "out.dvc").exists()
+    assert not (tmp_dir / "dvc.yaml").exists()
+    assert not (tmp_dir / "dvc.lock").exists()
 
     cache_dir = os.path.join(
         dvc.stage_cache.cache_dir,
         "8f",
         "8fdb377d1b4c0a303b788771b122dfba9bbbbc43f14ce41d35715cf4fea08459",
     )
     cache_file = os.path.join(
@@ -103,23 +105,24 @@
         'open("out", "w+").write("out"); ',
     )
     tmp_dir.gen({"wdir": {}})
     stage = dvc.run(
         cmd="python ../script.py",
         deps=["../script.py", "../dep"],
         outs=["out"],
-        single_stage=True,
+        name="write-out",
         wdir="wdir",
     )
 
     with dvc.lock:
         stage.remove(remove_outs=True, force=True)
 
     assert not (tmp_dir / "wdir" / "out").exists()
-    assert not (tmp_dir / "wdir" / "out.dvc").exists()
+    assert not (tmp_dir / "wdir" / "dvc.yaml").exists()
+    assert not (tmp_dir / "wdir" / "dvc.lock").exists()
 
     cache_dir = os.path.join(
         dvc.stage_cache.cache_dir,
         "b5",
         "b5d5548c43725139aa3419eb50717e062fe9b81f866f401fd6fd778d2a97822d",
     )
     cache_file = os.path.join(
```

### Comparing `dvc-3.0.0a1/tests/unit/stage/test_loader_pipeline_file.py` & `dvc-3.0.0a2/tests/unit/stage/test_loader_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/stage/test_run.py` & `dvc-3.0.0a2/tests/unit/stage/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/stage/test_serialize_pipeline_file.py` & `dvc-3.0.0a2/tests/unit/stage/test_serialize_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/stage/test_serialize_pipeline_lock.py` & `dvc-3.0.0a2/tests/unit/stage/test_serialize_pipeline_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/stage/test_stage.py` & `dvc-3.0.0a2/tests/unit/stage/test_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 def test_stage_run_ignore_sigint(dvc, mocker):
     proc = mocker.Mock()
     communicate = mocker.Mock()
     proc.configure_mock(returncode=0, communicate=communicate)
     popen = mocker.patch.object(subprocess, "Popen", return_value=proc)
     signal_mock = mocker.patch("signal.signal")
 
-    dvc.run(cmd="path", single_stage=True)
+    dvc.run(cmd="path", name="train")
 
     assert popen.called_once()
     assert communicate.called_once_with()
     signal_mock.assert_any_call(signal.SIGINT, signal.SIG_IGN)
     assert signal.getsignal(signal.SIGINT) == signal.default_int_handler
```

### Comparing `dvc-3.0.0a1/tests/unit/stage/test_utils.py` & `dvc-3.0.0a2/tests/unit/stage/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_analytics.py` & `dvc-3.0.0a2/tests/unit/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_collect.py` & `dvc-3.0.0a2/tests/unit/test_collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_compare.py` & `dvc-3.0.0a2/tests/unit/test_compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_config.py` & `dvc-3.0.0a2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_context.py` & `dvc-3.0.0a2/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_daemon.py` & `dvc-3.0.0a2/tests/unit/test_daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_dvcfile.py` & `dvc-3.0.0a2/tests/unit/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_ignore.py` & `dvc-3.0.0a2/tests/unit/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_imports.py` & `dvc-3.0.0a2/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_info.py` & `dvc-3.0.0a2/tests/unit/test_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_interpolate.py` & `dvc-3.0.0a2/tests/unit/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_lockfile.py` & `dvc-3.0.0a2/tests/unit/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_logger.py` & `dvc-3.0.0a2/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_metrics.py` & `dvc-3.0.0a2/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_params.py` & `dvc-3.0.0a2/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_pathspec_math.py` & `dvc-3.0.0a2/tests/unit/test_pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_progress.py` & `dvc-3.0.0a2/tests/unit/test_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_rwlock.py` & `dvc-3.0.0a2/tests/unit/test_rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_tabular_data.py` & `dvc-3.0.0a2/tests/unit/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/test_updater.py` & `dvc-3.0.0a2/tests/unit/test_updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/ui/test_console.py` & `dvc-3.0.0a2/tests/unit/ui/test_console.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/ui/test_pager.py` & `dvc-3.0.0a2/tests/unit/ui/test_pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/ui/test_table.py` & `dvc-3.0.0a2/tests/unit/ui/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/utils/serialize/test_python.py` & `dvc-3.0.0a2/tests/unit/utils/serialize/test_python.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/utils/serialize/test_toml.py` & `dvc-3.0.0a2/tests/unit/utils/serialize/test_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/utils/serialize/test_yaml.py` & `dvc-3.0.0a2/tests/unit/utils/serialize/test_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/utils/test_cli_parse.py` & `dvc-3.0.0a2/tests/unit/utils/test_cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/utils/test_executors.py` & `dvc-3.0.0a2/tests/unit/utils/test_executors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/utils/test_fs.py` & `dvc-3.0.0a2/tests/unit/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/utils/test_humanize.py` & `dvc-3.0.0a2/tests/unit/utils/test_humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/utils/test_studio.py` & `dvc-3.0.0a2/tests/unit/utils/test_studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/unit/utils/test_utils.py` & `dvc-3.0.0a2/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/utils/__init__.py` & `dvc-3.0.0a2/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a1/tests/utils/asserts.py` & `dvc-3.0.0a2/tests/utils/asserts.py`

 * *Files identical despite different names*

