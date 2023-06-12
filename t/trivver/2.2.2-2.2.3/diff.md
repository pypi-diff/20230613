# Comparing `tmp/trivver-2.2.2.tar.gz` & `tmp/trivver-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trivver-2.2.2.tar", last modified: Sun Jun 26 12:45:32 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `trivver-2.2.2.tar` & `trivver-2.2.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-06-26 12:45:32.266227 trivver-2.2.2/
--rw-r--r--   0 roam      (1000) roam      (1000)      415 2022-06-26 12:39:13.000000 trivver-2.2.2/.editorconfig
--rw-r--r--   0 roam      (1000) roam      (1000)      140 2022-06-26 12:39:13.000000 trivver-2.2.2/MANIFEST.in
--rw-r--r--   0 roam      (1000) roam      (1000)     4973 2022-06-26 12:45:32.266227 trivver-2.2.2/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)     4019 2022-06-26 12:44:48.000000 trivver-2.2.2/README.md
--rw-r--r--   0 roam      (1000) roam      (1000)      122 2022-06-26 12:39:13.000000 trivver-2.2.2/pyproject.toml
--rw-r--r--   0 roam      (1000) roam      (1000)     1247 2022-06-26 12:45:32.266227 trivver-2.2.2/setup.cfg
--rwxr-xr-x   0 roam      (1000) roam      (1000)     1499 2021-03-21 21:49:16.000000 trivver-2.2.2/setup.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-06-26 12:45:32.262227 trivver-2.2.2/src/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-06-26 12:45:32.262227 trivver-2.2.2/src/test_cargo/
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2022-06-26 12:39:13.000000 trivver-2.2.2/src/test_cargo/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     8145 2022-06-26 12:39:13.000000 trivver-2.2.2/src/test_cargo/__main__.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-06-26 12:45:32.262227 trivver-2.2.2/src/trivver/
--rw-r--r--   0 roam      (1000) roam      (1000)     2116 2022-06-26 05:06:30.000000 trivver-2.2.2/src/trivver/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     5132 2022-06-26 12:39:13.000000 trivver-2.2.2/src/trivver/__main__.py
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-03-19 23:54:14.000000 trivver-2.2.2/src/trivver/py.typed
--rw-r--r--   0 roam      (1000) roam      (1000)     4126 2021-03-21 21:49:16.000000 trivver-2.2.2/src/trivver/trivver.1
--rw-r--r--   0 roam      (1000) roam      (1000)     6645 2022-06-26 12:39:13.000000 trivver-2.2.2/src/trivver/trivver.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-06-26 12:45:32.266227 trivver-2.2.2/src/trivver.egg-info/
--rw-r--r--   0 roam      (1000) roam      (1000)     4973 2022-06-26 12:45:31.000000 trivver-2.2.2/src/trivver.egg-info/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)      582 2022-06-26 12:45:32.000000 trivver-2.2.2/src/trivver.egg-info/SOURCES.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2022-06-26 12:45:31.000000 trivver-2.2.2/src/trivver.egg-info/dependency_links.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       50 2022-06-26 12:45:32.000000 trivver-2.2.2/src/trivver.egg-info/entry_points.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        8 2022-06-26 12:45:32.000000 trivver-2.2.2/src/trivver.egg-info/top_level.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2022-06-26 05:20:05.000000 trivver-2.2.2/src/trivver.egg-info/zip-safe
--rw-r--r--   0 roam      (1000) roam      (1000)     1634 2022-06-26 12:39:13.000000 trivver-2.2.2/tox.ini
--rw-r--r--   0 roam      (1000) roam      (1000)     4099 2021-03-21 21:49:16.000000 trivver-2.2.2/trivver.scd
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-06-26 12:45:32.266227 trivver-2.2.2/unit_tests/
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2020-03-21 23:02:19.000000 trivver-2.2.2/unit_tests/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     4967 2021-11-11 23:11:10.000000 trivver-2.2.2/unit_tests/data.py
--rw-r--r--   0 roam      (1000) roam      (1000)     4970 2022-06-26 12:39:13.000000 trivver-2.2.2/unit_tests/test_main.py
--rwxr-xr-x   0 roam      (1000) roam      (1000)     2705 2021-03-20 22:08:17.000000 trivver-2.2.2/unit_tests/test_main.sh
--rw-r--r--   0 roam      (1000) roam      (1000)     2543 2022-06-26 12:43:08.000000 trivver-2.2.2/unit_tests/test_version.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 trivver-2.2.3/.editorconfig
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 trivver-2.2.3/.shellcheckrc
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 trivver-2.2.3/mkdocs.yml
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 trivver-2.2.3/tox.ini
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 trivver-2.2.3/trivver.scd
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 trivver-2.2.3/.reuse/dep5
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 trivver-2.2.3/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 trivver-2.2.3/config/ruff-all/pyproject.toml
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 trivver-2.2.3/config/ruff-base/pyproject.toml
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 trivver-2.2.3/config/ruff-most/pyproject.toml
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 trivver-2.2.3/docs/changes.md
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 trivver-2.2.3/docs/index.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 trivver-2.2.3/nix/python-tox.nix
+-rwxr-xr-x   0        0        0      434 2020-02-02 00:00:00.000000 trivver-2.2.3/nix/run-tox.sh
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 trivver-2.2.3/requirements/docs.txt
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 trivver-2.2.3/src/test_cargo/__init__.py
+-rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 trivver-2.2.3/src/test_cargo/__main__.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 trivver-2.2.3/src/trivver/__init__.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 trivver-2.2.3/src/trivver/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trivver-2.2.3/src/trivver/py.typed
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 trivver-2.2.3/src/trivver/trivver.1
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 trivver-2.2.3/src/trivver/trivver.py
+-rwxr-xr-x   0        0        0      546 2020-02-02 00:00:00.000000 trivver-2.2.3/tools/cleanpy.sh
+-rwxr-xr-x   0        0        0     1325 2020-02-02 00:00:00.000000 trivver-2.2.3/tools/test-docker.sh
+-rwxr-xr-x   0        0        0     3277 2020-02-02 00:00:00.000000 trivver-2.2.3/tools/test-in-docker.sh
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 trivver-2.2.3/unit_tests/__init__.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 trivver-2.2.3/unit_tests/data.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 trivver-2.2.3/unit_tests/test_main.py
+-rwxr-xr-x   0        0        0     2807 2020-02-02 00:00:00.000000 trivver-2.2.3/unit_tests/test_main.sh
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 trivver-2.2.3/unit_tests/test_version.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 trivver-2.2.3/.gitignore
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 trivver-2.2.3/README.md
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 trivver-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 trivver-2.2.3/PKG-INFO
```

### Comparing `trivver-2.2.2/setup.py` & `trivver-2.2.3/LICENSES/BSD-2-Clause.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,9 @@
-#!/usr/bin/python3
-#
-# Copyright (c) 2020, 2021  Peter Pentchev <roam@ringlet.net>
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions
-# are met:
-# 1. Redistributions of source code must retain the above copyright
-#    notice, this list of conditions and the following disclaimer.
-# 2. Redistributions in binary form must reproduce the above copyright
-#    notice, this list of conditions and the following disclaimer in the
-#    documentation and/or other materials provided with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS ``AS IS'' AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
-# OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-# OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-# SUCH DAMAGE.
-#
-"""Setup configuration for the trivial version comparison module."""
+Copyright (c) <year> <owner> 
 
-import setuptools  # type: ignore
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
-setuptools.setup()
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `trivver-2.2.2/src/test_cargo/__main__.py` & `trivver-2.2.3/src/test_cargo/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
+#
 """Run some tests using the crates.io index."""
 
+from __future__ import annotations
+
 import argparse
 import functools
 import json
 import os
 import pathlib
-import posix
-import pwd
 import random
 import re
 import subprocess
 import sys
-import tempfile
-import time
-
-from typing import Dict, List, NamedTuple  # noqa: H301
+from typing import NamedTuple
 
-import typedload
 import utf8_locale
 
 
 class GitTree(NamedTuple):
     """A single line in the `git ls-tree` output."""
 
     git_id: str
@@ -35,24 +34,23 @@
     vers: str
 
 
 class TestedCrate(NamedTuple):
     """A single crate to test."""
 
     name: str
-    versions: List[str]
+    versions: list[str]
 
 
 class Config(NamedTuple):
     """Runtime configuration for the test program."""
 
     cachedir: pathlib.Path
-    cargo: str
     program: pathlib.Path
-    utf8_env: Dict[str, str]
+    utf8_env: dict[str, str]
 
 
 RE_CARGO_FETCH_HEAD = re.compile(r"^ (?P<cid> [0-9a-f]+ ) \s .*? (?P<url> \S+ ) $", re.X)
 
 CARGO_FETCH_URL = "https://github.com/rust-lang/crates.io-index"
 CARGO_CACHE_TIMEOUT = 4 * 3600
 
@@ -93,148 +91,148 @@
             ),
             "18446744073709551615.18446744073709551615.18446744073709551615",
         ],
     ),
 ]
 
 
-def find_cargo_cache() -> pathlib.Path:
+def find_cargo_cache(cargo_index: pathlib.Path, utf8_env: dict[str, str]) -> pathlib.Path:
     """Find the cargo cache directory."""
-    home = pathlib.Path(os.environ.get("HOME", pwd.getpwuid(posix.getuid()).pw_dir))
-    index = home / ".cargo/registry/index"
-    for regdir in index.iterdir():
-        fetch_head = regdir / ".git/FETCH_HEAD"
-        if not fetch_head.is_file():
-            continue
-
-        lines = fetch_head.read_text(encoding="UTF-8").splitlines()
-        if len(lines) != 1:
-            sys.exit(f"Expected a single line in {fetch_head}, got {lines!r}")
-        fields = RE_CARGO_FETCH_HEAD.match(lines[0])
-        if not fields:
-            sys.exit(f"Invalid format for the first line of {fetch_head}: {lines[0]!r}")
-
-        if fields.group("url") == CARGO_FETCH_URL:
-            return regdir
-
-    sys.exit(f"Could not find {CARGO_FETCH_URL} in {index}")
-
-
-def update_if_needed(cfg: Config) -> None:
-    """Update the Cargo cache if needed."""
-    lastf = cfg.cachedir / ".last-updated"
-    lastupd = lastf.stat().st_mtime
-    if time.time() <= lastupd + CARGO_CACHE_TIMEOUT:
-        print(f"No need to update the Cargo cache at {cfg.cachedir}")
-        return
-
-    with tempfile.TemporaryDirectory() as tempd_obj:
-        tempd = pathlib.Path(tempd_obj)
-        print(f"Using {tempd} as a temporary directory for updating the Cargo cache")
-        subprocess.check_call(
-            [cfg.cargo, "install", "--root", tempd / "root", "expect-exit"], env=cfg.utf8_env
+    remotes: dict[str, dict[str, str]] = {}
+    for line in subprocess.check_output(
+        ["git", "--no-pager", "config", "--get-regexp", r"^remote\.[^.]+\.(url|fetch)$"],
+        cwd=cargo_index,
+        encoding="UTF-8",
+        env=utf8_env,
+    ).splitlines():
+        name, value = line.split(maxsplit=1)
+        fields = name.split(".")
+        if (
+            len(fields) != 3  # noqa: PLR2004
+            or fields[0] != "remote"
+            or fields[2] not in ("fetch", "url")
+        ):
+            sys.exit(f"Unexpected 'git config get-regexp' output line at {cargo_index}: {line!r}")
+        remote = fields[1]
+        if remote not in remotes:
+            remotes[remote] = {}
+        remotes[remote][fields[2]] = value
+
+    found = [item[0] for item in remotes.items() if item[1]["url"] == CARGO_FETCH_URL]
+    if len(found) != 1:
+        sys.exit(
+            f"Expected exactly one {CARGO_FETCH_URL} Git remote repo at "
+            f"{cargo_index}, got {found!r}"
         )
+    remote = found[0]
 
-    lastupd = lastf.stat().st_mtime
-    if time.time() > lastupd + CARGO_CACHE_TIMEOUT:
-        sys.exit(f"Could not get Cargo to update the modification time of {lastf}")
+    subprocess.check_call(["git", "fetch", remote], cwd=cargo_index)
+    subprocess.check_call(["git", "merge", "--ff-only"], cwd=cargo_index)
+    return cargo_index
 
 
-def get_crate_versions(cfg: Config, crate: str) -> List[str]:
-    """Fetch some data about a crate."""
+def _parse_ver_line(line: str) -> GitTree:
+    """Parse a `git ls-tree` output line."""
+    mtree = RE_GIT_TREE_LINE.match(line)
+    if not mtree:
+        sys.exit(f"Unexpected `git ls-tree` output line: {line!r}")
+    return GitTree(
+        git_id=mtree.group("obj_id"), git_type=mtree.group("obj_type"), name=mtree.group("name")
+    )
 
-    def parse_line(line: str) -> GitTree:
-        """Parse a `git ls-tree` output line."""
-        mtree = RE_GIT_TREE_LINE.match(line)
-        if not mtree:
-            sys.exit(f"Unexpected `git ls-tree` output line: {line!r}")
-        return GitTree(
-            git_id=mtree.group("obj_id"), git_type=mtree.group("obj_type"), name=mtree.group("name")
-        )
 
-    def parse_tree(treeish: str) -> Dict[str, GitTree]:
-        """Parse the `git ls-tree` output for the specified tree-like name."""
-        lines = subprocess.check_output(
-            ["git", "ls-tree", treeish], cwd=cfg.cachedir, encoding="UTF-8", env=cfg.utf8_env
-        ).splitlines()
-        print(f"Got {len(lines)} lines of `git ls-tree` output")
-        return {tree.name: tree for tree in (parse_line(line) for line in lines)}
-
-    def get_next_tree(treeish: str, part: str, exp_type: str) -> str:
-        """Get the next part of the tree chain."""
-        tree = parse_tree(treeish).get(part)
-        if tree is None:
-            sys.exit(f"Could not find '{part}' in the {treeish} Git tree.")
-        elif tree.git_type != exp_type:
-            sys.exit(f"Not a {exp_type}: {tree!r}")
-        return tree.git_id
+def _parse_ver_tree(cfg: Config, treeish: str) -> dict[str, GitTree]:
+    """Parse the `git ls-tree` output for the specified tree-like name."""
+    lines = subprocess.check_output(
+        ["git", "ls-tree", treeish], cwd=cfg.cachedir, encoding="UTF-8", env=cfg.utf8_env
+    ).splitlines()
+    print(f"Got {len(lines)} lines of `git ls-tree` output")
+    return {tree.name: tree for tree in (_parse_ver_line(line) for line in lines)}
+
+
+def _get_next_ver_tree(cfg: Config, treeish: str, part: str, exp_type: str) -> str:
+    """Get the next part of the tree chain."""
+    tree = _parse_ver_tree(cfg, treeish).get(part)
+    if tree is None:
+        sys.exit(f"Could not find '{part}' in the {treeish} Git tree.")
+    elif tree.git_type != exp_type:
+        sys.exit(f"Not a {exp_type}: {tree!r}")
+    return tree.git_id
+
+
+def get_crate_versions(cfg: Config, crate: str) -> list[str]:
+    """Fetch some data about a crate."""
 
     def get_tree_id() -> str:
         """Parse the trees until we find the crate."""
         if len(crate) in (1, 2):
             parts = [str(len(crate))]
-        elif len(crate) == 3:
+        elif len(crate) == 3:  # noqa: PLR2004
             parts = [str(len(crate)), crate[:1]]
         else:
             parts = [crate[:2], crate[2:4]]
 
         return functools.reduce(
-            lambda current, part: get_next_tree(current, part, "blob" if part == crate else "tree"),
-            parts + [crate],
+            lambda current, part: _get_next_ver_tree(
+                cfg, current, part, "blob" if part == crate else "tree"
+            ),
+            [*parts, crate],
             "FETCH_HEAD",
         )
 
+    def parse_vers_line(line: str) -> str:
+        """Parse a single crates.io crate version line."""
+        raw = json.loads(line)
+        if (
+            not isinstance(raw, dict)
+            or "name" not in raw
+            or raw["name"] != crate
+            or "vers" not in raw
+            or not isinstance(raw["vers"], str)
+        ):
+            sys.exit(f"Unexpected Cargo version line for {crate}: {line}")
+        return raw["vers"]
+
     print(f"Fetching crates.io data for {crate}")
     tree_id = get_tree_id()
     jlines = subprocess.check_output(
         ["git", "show", tree_id], cwd=cfg.cachedir, encoding="UTF-8", env=cfg.utf8_env
     ).splitlines()
-    raw = [json.loads(line) for line in jlines]
-    data = typedload.load(raw, List[CrateVersion])
-    if any(vers.name != crate for vers in data):
-        sys.exit(f"Unexpected Cargo versions: {data!r}")
-    return [vers.vers for vers in data]
+    return [parse_vers_line(line) for line in jlines]
 
 
-def parse_args() -> Config:
+def parse_args(cargo_index: pathlib.Path) -> Config:
     """Parse the command-line arguments."""
     parser = argparse.ArgumentParser(prog="test_cargo")
     parser.add_argument(
-        "-c",
-        "--cargo",
-        type=str,
-        default="cargo",
-        help="the program name (or full path) of the Cargo program to use",
-    )
-    parser.add_argument(
         "-p",
         "--program",
         type=pathlib.Path,
         required=True,
         help="the path to the trivver implementation to test",
     )
 
     args = parser.parse_args()
 
+    utf8_env = utf8_locale.UTF8Detect().detect().env
     return Config(
-        cachedir=find_cargo_cache(),
-        cargo=args.cargo,
+        cachedir=find_cargo_cache(cargo_index, utf8_env),
         program=args.program,
-        utf8_env=utf8_locale.UTF8Detect().detect().env,
+        utf8_env=utf8_env,
     )
 
 
 def main() -> None:
     """Parse command-line options, do stuff."""
-    if os.environ.get("RUN_TRIVVER_CARGO_TEST", "0") != "1":
-        print("Skipping the test, set RUN_TRIVVER_CARGO_TEST to 1 to run it")
+    cargo_index = os.environ.get("TEST_CARGO_INDEX_PATH")
+    if not cargo_index:
+        print("Skipping the test, set TEST_CARGO_INDEX_PATH to the path to a Git checkout")
         return
 
-    cfg = parse_args()
-    update_if_needed(cfg)
+    cfg = parse_args(pathlib.Path(cargo_index))
 
     for crate in CRATES:
         print(f"Testing {crate.name}")
         versions = get_crate_versions(cfg, crate.name)
         print(f"Got {len(versions)} versions for {crate.name}")
         missing = [vers for vers in crate.versions if vers not in versions]
         if missing:
```

### Comparing `trivver-2.2.2/src/trivver/trivver.1` & `trivver-2.2.3/src/trivver/trivver.1`

 * *Files identical despite different names*

### Comparing `trivver-2.2.2/unit_tests/test_main.sh` & `trivver-2.2.3/unit_tests/test_main.sh`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 #!/bin/sh
+#
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
 
 set -e
 
 if [ "$#" -ne 1 ]; then
 	echo 'Usage: test_main.sh trivver-command' 1>&2
 	exit 1
 fi
```

