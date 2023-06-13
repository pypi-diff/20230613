# Comparing `tmp/commitizen-3.2.2.tar.gz` & `tmp/commitizen-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.2.2.tar", max compression
+gzip compressed data, was "commitizen-3.3.0.tar", max compression
```

## Comparing `commitizen-3.2.2.tar` & `commitizen-3.3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-05-11 12:35:10.600121 commitizen-3.2.2/LICENSE
--rw-r--r--   0        0        0      609 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/__version__.py
--rw-r--r--   0        0        0     8609 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/bump.py
--rw-r--r--   0        0        0    11956 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/changelog.py
--rw-r--r--   0        0        0     3431 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    16927 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    13932 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7266 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5067 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/info.py
--rw-r--r--   0        0        0    12930 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/commands/version.py
--rw-r--r--   0        0        0     1229 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/config/__init__.py
--rw-r--r--   0        0        0      915 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1575 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1753 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1438 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1226 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     3016 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7114 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3125 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      272 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3327 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/defaults.py
--rw-r--r--   0        0        0     4575 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/factory.py
--rw-r--r--   0        0        0     6916 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/out.py
--rw-r--r--   0        0        0     6657 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     2400 2023-05-11 12:35:10.600121 commitizen-3.2.2/commitizen/version_types.py
--rw-r--r--   0        0        0     5748 2023-05-11 12:35:10.600121 commitizen-3.2.2/docs/README.md
--rw-r--r--   0        0        0     3938 2023-05-11 12:35:10.616121 commitizen-3.2.2/pyproject.toml
--rw-r--r--   0        0        0     7581 1970-01-01 00:00:00.000000 commitizen-3.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-13 15:08:53.658482 commitizen-3.3.0/LICENSE
+-rw-r--r--   0        0        0      609 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/__version__.py
+-rw-r--r--   0        0        0     8543 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/bump.py
+-rw-r--r--   0        0        0    11894 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/changelog.py
+-rw-r--r--   0        0        0     3455 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    16940 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    13915 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7269 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5075 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12935 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1568 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1746 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1431 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7115 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3272 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/defaults.py
+-rw-r--r--   0        0        0     4575 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/factory.py
+-rw-r--r--   0        0        0     6900 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/out.py
+-rw-r--r--   0        0        0     7014 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     2376 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/version_types.py
+-rw-r--r--   0        0        0     5750 2023-06-13 15:08:53.658482 commitizen-3.3.0/docs/README.md
+-rw-r--r--   0        0        0     3938 2023-06-13 15:08:53.670482 commitizen-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.3.0/PKG-INFO
```

### Comparing `commitizen-3.2.2/LICENSE` & `commitizen-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/__init__.py` & `commitizen-3.3.0/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/bump.py` & `commitizen-3.3.0/commitizen/bump.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from __future__ import annotations
+
 import os
 import re
 import sys
 import typing
 from collections import OrderedDict
 from itertools import zip_longest
 from string import Template
-from typing import List, Optional, Tuple, Type, Union
 
 from packaging.version import Version
 
 from commitizen.defaults import MAJOR, MINOR, PATCH, bump_message
 from commitizen.exceptions import CurrentVersionNotFoundError
 from commitizen.git import GitCommit, smart_open
 
@@ -17,23 +18,23 @@
     from commitizen.version_types import VersionProtocol
 else:
     # workaround mypy issue for 3.7 python
     VersionProtocol = typing.Any
 
 
 def find_increment(
-    commits: List[GitCommit], regex: str, increments_map: Union[dict, OrderedDict]
-) -> Optional[str]:
+    commits: list[GitCommit], regex: str, increments_map: dict | OrderedDict
+) -> str | None:
     if isinstance(increments_map, dict):
         increments_map = OrderedDict(increments_map)
 
     # Most important cases are major and minor.
     # Everything else will be considered patch.
     select_pattern = re.compile(regex)
-    increment: Optional[str] = None
+    increment: str | None = None
 
     for commit in commits:
         for message in commit.message.split("\n"):
             result = select_pattern.search(message)
 
             if result:
                 found_keyword = result.group(1)
@@ -50,15 +51,15 @@
                 elif increment == "PATCH" or increment is None:
                     increment = new_increment
 
     return increment
 
 
 def prerelease_generator(
-    current_version: str, prerelease: Optional[str] = None, offset: int = 0
+    current_version: str, prerelease: str | None = None, offset: int = 0
 ) -> str:
     """Generate prerelease
 
     X.YaN   # Alpha release
     X.YbN   # Beta release
     X.YrcN  # Release Candidate
     X.Y  # Final
@@ -119,19 +120,19 @@
         f"{increments_version['PATCH']}"
     )
 
 
 def generate_version(
     current_version: str,
     increment: str,
-    prerelease: Optional[str] = None,
+    prerelease: str | None = None,
     prerelease_offset: int = 0,
-    devrelease: Optional[int] = None,
+    devrelease: int | None = None,
     is_local_version: bool = False,
-    version_type_cls: Optional[Type[VersionProtocol]] = None,
+    version_type_cls: type[VersionProtocol] | None = None,
 ) -> VersionProtocol:
     """Based on the given increment a proper semver will be generated.
 
     For now the rules and versioning scheme is based on
     python's PEP 0440.
     More info: https://www.python.org/dev/peps/pep-0440/
 
@@ -159,15 +160,15 @@
         semver = semver_generator(current_version, increment=increment)
 
         # TODO: post version
         return version_type_cls(f"{semver}{pre_version}{dev_version}")
 
 
 def update_version_in_files(
-    current_version: str, new_version: str, files: List[str], *, check_consistency=False
+    current_version: str, new_version: str, files: list[str], *, check_consistency=False
 ) -> None:
     """Change old version to the new one in every file given.
 
     Note that this version is not the tag formatted one.
     So for example, your tag could look like `v1.0.0` while your version in
     the package like `1.0.0`.
     """
@@ -193,15 +194,15 @@
         # Write the file out again
         with smart_open(filepath, "w") as file:
             file.write(version_file)
 
 
 def _bump_with_regex(
     version_filepath: str, current_version: str, new_version: str, regex: str
-) -> Tuple[bool, str]:
+) -> tuple[bool, str]:
     current_version_found = False
     lines = []
     pattern = re.compile(regex)
     with open(version_filepath, "r") as f:
         for line in f:
             if pattern.search(line):
                 bumped_line = line.replace(current_version, new_version)
@@ -214,17 +215,17 @@
 
 
 def _version_to_regex(version: str) -> str:
     return version.replace(".", r"\.").replace("+", r"\+")
 
 
 def normalize_tag(
-    version: Union[VersionProtocol, str],
-    tag_format: Optional[str] = None,
-    version_type_cls: Optional[Type[VersionProtocol]] = None,
+    version: VersionProtocol | str,
+    tag_format: str | None = None,
+    version_type_cls: type[VersionProtocol] | None = None,
 ) -> str:
     """The tag and the software version might be different.
 
     That's why this function exists.
 
     Example:
     | tag | version (PEP 0440) |
@@ -250,15 +251,15 @@
     t = Template(tag_format)
     return t.safe_substitute(
         version=version, major=major, minor=minor, patch=patch, prerelease=prerelease
     )
 
 
 def create_commit_message(
-    current_version: Union[Version, str],
-    new_version: Union[Version, str],
+    current_version: Version | str,
+    new_version: Version | str,
     message_template: str = None,
 ) -> str:
     if message_template is None:
         message_template = bump_message
     t = Template(message_template)
     return t.safe_substitute(current_version=current_version, new_version=new_version)
```

### Comparing `commitizen-3.2.2/commitizen/changelog.py` & `commitizen-3.3.0/commitizen/changelog.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,21 +21,23 @@
 - [x] Include in tree from file all the extra comments added manually
 - [x] Add unreleased value
 - [x] hook after message is parsed (add extra information like hyperlinks)
 - [x] hook after changelog is generated (api calls)
 - [x] add support for change_type maps
 """
 
+from __future__ import annotations
+
 import os
 import re
 import sys
 import typing
 from collections import OrderedDict, defaultdict
 from datetime import date
-from typing import Callable, Dict, Iterable, List, Optional, Tuple, Type
+from typing import Callable, Iterable
 
 from jinja2 import Environment, PackageLoader
 from packaging.version import InvalidVersion, Version
 
 from commitizen import defaults
 from commitizen.bump import normalize_tag
 from commitizen.exceptions import InvalidConfigurationError, NoCommitsFoundError
@@ -44,29 +46,29 @@
 if sys.version_info >= (3, 8):
     from commitizen.version_types import VersionProtocol
 else:
     # workaround mypy issue for 3.7 python
     VersionProtocol = typing.Any
 
 
-def get_commit_tag(commit: GitCommit, tags: List[GitTag]) -> Optional[GitTag]:
+def get_commit_tag(commit: GitCommit, tags: list[GitTag]) -> GitTag | None:
     return next((tag for tag in tags if tag.rev == commit.rev), None)
 
 
-def get_version(tag: GitTag) -> Optional[Version]:
+def get_version(tag: GitTag) -> Version | None:
     version = None
     try:
         version = Version(tag.name)
     except InvalidVersion:
         pass
     return version
 
 
 def tag_included_in_changelog(
-    tag: GitTag, used_tags: List, merge_prerelease: bool
+    tag: GitTag, used_tags: list, merge_prerelease: bool
 ) -> bool:
     if tag in used_tags:
         return False
 
     version = get_version(tag)
     if version is None:
         return False
@@ -74,43 +76,43 @@
     if merge_prerelease and version.is_prerelease:
         return False
 
     return True
 
 
 def generate_tree_from_commits(
-    commits: List[GitCommit],
-    tags: List[GitTag],
+    commits: list[GitCommit],
+    tags: list[GitTag],
     commit_parser: str,
     changelog_pattern: str,
-    unreleased_version: Optional[str] = None,
-    change_type_map: Optional[Dict[str, str]] = None,
-    changelog_message_builder_hook: Optional[Callable] = None,
+    unreleased_version: str | None = None,
+    change_type_map: dict[str, str] | None = None,
+    changelog_message_builder_hook: Callable | None = None,
     merge_prerelease: bool = False,
-) -> Iterable[Dict]:
+) -> Iterable[dict]:
     pat = re.compile(changelog_pattern)
     map_pat = re.compile(commit_parser, re.MULTILINE)
     body_map_pat = re.compile(commit_parser, re.MULTILINE | re.DOTALL)
-    current_tag: Optional[GitTag] = None
+    current_tag: GitTag | None = None
 
     # Check if the latest commit is not tagged
     if commits:
         latest_commit = commits[0]
         current_tag = get_commit_tag(latest_commit, tags)
 
     current_tag_name: str = unreleased_version or "Unreleased"
     current_tag_date: str = ""
     if unreleased_version is not None:
         current_tag_date = date.today().isoformat()
     if current_tag is not None and current_tag.name:
         current_tag_name = current_tag.name
         current_tag_date = current_tag.date
 
-    changes: Dict = defaultdict(list)
-    used_tags: List = [current_tag]
+    changes: dict = defaultdict(list)
+    used_tags: list = [current_tag]
     for commit in commits:
         commit_tag = get_commit_tag(commit, tags)
 
         if commit_tag is not None and tag_included_in_changelog(
             commit_tag, used_tags, merge_prerelease
         ):
             used_tags.append(commit_tag)
@@ -126,15 +128,15 @@
         matches = pat.match(commit.message)
         if not matches:
             continue
 
         # Process subject from commit message
         message = map_pat.match(commit.message)
         if message:
-            parsed_message: Dict = message.groupdict()
+            parsed_message: dict = message.groupdict()
             # change_type becomes optional by providing None
             change_type = parsed_message.pop("change_type", None)
 
             if change_type_map:
                 change_type = change_type_map.get(change_type, change_type)
             if changelog_message_builder_hook:
                 parsed_message = changelog_message_builder_hook(parsed_message, commit)
@@ -142,25 +144,25 @@
 
         # Process body from commit message
         body_parts = commit.body.split("\n\n")
         for body_part in body_parts:
             message_body = body_map_pat.match(body_part)
             if not message_body:
                 continue
-            parsed_message_body: Dict = message_body.groupdict()
+            parsed_message_body: dict = message_body.groupdict()
 
             change_type = parsed_message_body.pop("change_type", None)
             if change_type_map:
                 change_type = change_type_map.get(change_type, change_type)
             changes[change_type].append(parsed_message_body)
 
     yield {"version": current_tag_name, "date": current_tag_date, "changes": changes}
 
 
-def order_changelog_tree(tree: Iterable, change_type_order: List[str]) -> Iterable:
+def order_changelog_tree(tree: Iterable, change_type_order: list[str]) -> Iterable:
     if len(set(change_type_order)) != len(change_type_order):
         raise InvalidConfigurationError(
             f"Change types contain duplicates types ({change_type_order})"
         )
 
     sorted_tree = []
     for entry in tree:
@@ -180,50 +182,50 @@
     loader = PackageLoader("commitizen", "templates")
     env = Environment(loader=loader, trim_blocks=True)
     jinja_template = env.get_template("keep_a_changelog_template.j2")
     changelog: str = jinja_template.render(tree=tree)
     return changelog
 
 
-def parse_version_from_markdown(value: str) -> Optional[str]:
+def parse_version_from_markdown(value: str) -> str | None:
     if not value.startswith("#"):
         return None
     m = re.search(defaults.version_parser, value)
     if not m:
         return None
     return m.groupdict().get("version")
 
 
-def parse_title_type_of_line(value: str) -> Optional[str]:
+def parse_title_type_of_line(value: str) -> str | None:
     md_title_parser = r"^(?P<title>#+)"
     m = re.search(md_title_parser, value)
     if not m:
         return None
     return m.groupdict().get("title")
 
 
-def get_metadata(filepath: str) -> Dict:
-    unreleased_start: Optional[int] = None
-    unreleased_end: Optional[int] = None
-    unreleased_title: Optional[str] = None
-    latest_version: Optional[str] = None
-    latest_version_position: Optional[int] = None
+def get_metadata(filepath: str) -> dict:
+    unreleased_start: int | None = None
+    unreleased_end: int | None = None
+    unreleased_title: str | None = None
+    latest_version: str | None = None
+    latest_version_position: int | None = None
     if not os.path.isfile(filepath):
         return {
             "unreleased_start": None,
             "unreleased_end": None,
             "latest_version": None,
             "latest_version_position": None,
         }
 
     with open(filepath, "r") as changelog_file:
         for index, line in enumerate(changelog_file):
             line = line.strip().lower()
 
-            unreleased: Optional[str] = None
+            unreleased: str | None = None
             if "unreleased" in line:
                 unreleased = parse_title_type_of_line(line)
             # Try to find beginning and end lines of the unreleased block
             if unreleased:
                 unreleased_start = index
                 unreleased_title = unreleased
                 continue
@@ -245,15 +247,15 @@
         "unreleased_start": unreleased_start,
         "unreleased_end": unreleased_end,
         "latest_version": latest_version,
         "latest_version_position": latest_version_position,
     }
 
 
-def incremental_build(new_content: str, lines: List[str], metadata: Dict) -> List[str]:
+def incremental_build(new_content: str, lines: list[str], metadata: dict) -> list[str]:
     """Takes the original lines and updates with new_content.
 
     The metadata governs how to remove the old unreleased section and where to place the
     new content.
 
     Args:
         lines: The lines from the changelog
@@ -263,15 +265,15 @@
     Returns:
         Updated lines
     """
     unreleased_start = metadata.get("unreleased_start")
     unreleased_end = metadata.get("unreleased_end")
     latest_version_position = metadata.get("latest_version_position")
     skip = False
-    output_lines: List[str] = []
+    output_lines: list[str] = []
     for index, line in enumerate(lines):
         if index == unreleased_start:
             skip = True
         elif index == unreleased_end:
             skip = False
             if (
                 latest_version_position is None
@@ -293,16 +295,16 @@
             # Ensure at least one blank line between existing and new content.
             output_lines.append("\n")
         output_lines.append(new_content)
     return output_lines
 
 
 def get_smart_tag_range(
-    tags: List[GitTag], newest: str, oldest: Optional[str] = None
-) -> List[GitTag]:
+    tags: list[GitTag], newest: str, oldest: str | None = None
+) -> list[GitTag]:
     """Smart because it finds the N+1 tag.
 
     This is because we need to find until the next tag
     """
     accumulator = []
     keep = False
     if not oldest:
@@ -319,27 +321,27 @@
             except IndexError:
                 pass
             break
     return accumulator
 
 
 def get_oldest_and_newest_rev(
-    tags: List[GitTag],
+    tags: list[GitTag],
     version: str,
     tag_format: str,
-    version_type_cls: Optional[Type[VersionProtocol]] = None,
-) -> Tuple[Optional[str], Optional[str]]:
+    version_type_cls: type[VersionProtocol] | None = None,
+) -> tuple[str | None, str | None]:
     """Find the tags for the given version.
 
     `version` may come in different formats:
     - `0.1.0..0.4.0`: as a range
     - `0.3.0`: as a single version
     """
-    oldest: Optional[str] = None
-    newest: Optional[str] = None
+    oldest: str | None = None
+    newest: str | None = None
     try:
         oldest, newest = version.split("..")
     except ValueError:
         newest = version
 
     newest_tag = normalize_tag(
         newest, tag_format=tag_format, version_type_cls=version_type_cls
@@ -351,15 +353,15 @@
             oldest, tag_format=tag_format, version_type_cls=version_type_cls
         )
 
     tags_range = get_smart_tag_range(tags, newest=newest_tag, oldest=oldest_tag)
     if not tags_range:
         raise NoCommitsFoundError("Could not find a valid revision range.")
 
-    oldest_rev: Optional[str] = tags_range[-1].name
+    oldest_rev: str | None = tags_range[-1].name
     newest_rev = newest_tag
 
     # check if it's the first tag created
     # and it's also being requested as part of the range
     if oldest_rev == tags[-1].name and oldest_rev == oldest_tag:
         return None, newest_rev
```

### Comparing `commitizen-3.2.2/commitizen/changelog_parser.py` & `commitizen-3.3.0/commitizen/changelog_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 ## Parse CHANGELOG.md
 
 1. Get LATEST VERSION from CONFIG
 1. Parse the file version to version
 2. Build a dict (tree) of that particular version
 3. Transform tree into markdown again
 """
+from __future__ import annotations
+
 import re
 from collections import defaultdict
-from typing import Dict, Generator, Iterable, List
+from typing import Generator, Iterable
 
 MD_VERSION_RE = r"^##\s(?P<version>[a-zA-Z0-9.+]+)\s?\(?(?P<date>[0-9-]+)?\)?"
 MD_CHANGE_TYPE_RE = r"^###\s(?P<change_type>[a-zA-Z0-9.+\s]+)"
 MD_MESSAGE_RE = (
     r"^-\s(\*{2}(?P<scope>[a-zA-Z0-9]+)\*{2}:\s)?(?P<message>.+)(?P<breaking>!)?"
 )
 md_version_c = re.compile(MD_VERSION_RE)
@@ -63,29 +65,29 @@
                     yield block
                 block = [line]
             else:
                 block.append(line)
         yield block
 
 
-def parse_md_version(md_version: str) -> Dict:
+def parse_md_version(md_version: str) -> dict:
     m = md_version_c.match(md_version)
     if not m:
         return {}
     return m.groupdict()
 
 
-def parse_md_change_type(md_change_type: str) -> Dict:
+def parse_md_change_type(md_change_type: str) -> dict:
     m = md_change_type_c.match(md_change_type)
     if not m:
         return {}
     return m.groupdict()
 
 
-def parse_md_message(md_message: str) -> Dict:
+def parse_md_message(md_message: str) -> dict:
     m = md_message_c.match(md_message)
     if not m:
         return {}
     return m.groupdict()
 
 
 def transform_change_type(change_type: str) -> str:
@@ -95,18 +97,18 @@
     for match_value, output in CATEGORIES:
         if re.search(match_value, _change_type_lower):
             return output
     else:
         raise ValueError(f"Could not match a change_type with {change_type}")
 
 
-def generate_block_tree(block: List[str]) -> Dict:
+def generate_block_tree(block: list[str]) -> dict:
     # tree: Dict = {"commits": []}
-    changes: Dict = defaultdict(list)
-    tree: Dict = {"changes": changes}
+    changes: dict = defaultdict(list)
+    tree: dict = {"changes": changes}
 
     change_type = None
     for line in block:
         if line.startswith("## "):
             # version identified
             change_type = None
             tree = {**tree, **parse_md_version(line)}
@@ -122,10 +124,10 @@
             commit = parse_md_message(line)
             changes[change_type].append(commit)
         else:
             print("it's something else: ", line)
     return tree
 
 
-def generate_full_tree(blocks: Iterable) -> Iterable[Dict]:
+def generate_full_tree(blocks: Iterable) -> Iterable[dict]:
     for block in blocks:
         yield generate_block_tree(block)
```

### Comparing `commitizen-3.2.2/commitizen/cli.py` & `commitizen-3.3.0/commitizen/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
+
 import argparse
 import logging
 import sys
 from pathlib import Path
 from functools import partial
 from types import TracebackType
-from typing import List
 
 import argcomplete
 from decli import cli
 
 from commitizen import commands, config, out, version_types
 from commitizen.exceptions import (
     CommitizenException,
@@ -63,15 +64,15 @@
                         "action": "store_true",
                         "help": "show output to stdout, no commit, no modified files",
                     },
                     {
                         "name": "--write-message-to-file",
                         "type": Path,
                         "metavar": "FILE_PATH",
-                        "help": "write message to file before commiting (can be combined with --dry-run)",
+                        "help": "write message to file before committing (can be combined with --dry-run)",
                     },
                     {
                         "name": ["-s", "--signoff"],
                         "action": "store_true",
                         "help": "sign off the commit",
                     },
                 ],
@@ -349,15 +350,15 @@
     },
 }
 
 original_excepthook = sys.excepthook
 
 
 def commitizen_excepthook(
-    type, value, traceback, debug=False, no_raise: List[int] = None
+    type, value, traceback, debug=False, no_raise: list[int] = None
 ):
     traceback = traceback if isinstance(traceback, TracebackType) else None
     if not no_raise:
         no_raise = []
     if isinstance(value, CommitizenException):
         if value.message:
             value.output_method(value.message)
@@ -372,21 +373,21 @@
 
 
 commitizen_debug_excepthook = partial(commitizen_excepthook, debug=True)
 
 sys.excepthook = commitizen_excepthook
 
 
-def parse_no_raise(comma_separated_no_raise: str) -> List[int]:
+def parse_no_raise(comma_separated_no_raise: str) -> list[int]:
     """Convert the given string to exit codes.
 
     Receives digits and strings and outputs the parsed integer which
     represents the exit code found in exceptions.
     """
-    no_raise_items: List[str] = comma_separated_no_raise.split(",")
+    no_raise_items: list[str] = comma_separated_no_raise.split(",")
     no_raise_codes = []
     for item in no_raise_items:
         if item.isdecimal():
             no_raise_codes.append(int(item))
             continue
         try:
             exit_code = ExitCode[item.strip()]
```

### Comparing `commitizen-3.2.2/commitizen/cmd.py` & `commitizen-3.3.0/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/commands/bump.py` & `commitizen-3.3.0/commitizen/commands/bump.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+from __future__ import annotations
+
 import os
 from logging import getLogger
-from typing import List, Optional
 
 import questionary
-from packaging.version import InvalidVersion, Version
-
 from commitizen import bump, cmd, factory, git, hooks, out, version_types
 from commitizen.commands.changelog import Changelog
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     BumpCommitFailedError,
     BumpTagFailedError,
     DryRunExit,
@@ -18,14 +17,15 @@
     NoneIncrementExit,
     NoPatternMapError,
     NotAGitProjectError,
     NotAllowed,
     NoVersionSpecifiedError,
 )
 from commitizen.providers import get_provider
+from packaging.version import InvalidVersion, Version
 
 logger = getLogger("commitizen")
 
 
 class Bump:
     """Show prompt for the user to create a guided commit."""
 
@@ -81,15 +81,15 @@
                         "- version in configuration is not the current version\n"
                         "- tag_format is missing, check them using 'git tag --list'\n"
                     )
                 )
                 is_initial = questionary.confirm("Is this the first tag created?").ask()
         return is_initial
 
-    def find_increment(self, commits: List[git.GitCommit]) -> Optional[str]:
+    def find_increment(self, commits: list[git.GitCommit]) -> str | None:
         # Update the bump map to ensure major version doesn't increment.
         is_major_version_zero: bool = self.bump_settings["major_version_zero"]
         # self.cz.bump_map = defaults.bump_map_major_version_zero
         bump_map = (
             self.cz.bump_map_major_version_zero
             if is_major_version_zero
             else self.cz.bump_map
@@ -113,25 +113,25 @@
         try:
             current_version_instance: Version = Version(current_version)
         except TypeError:
             raise NoVersionSpecifiedError()
 
         tag_format: str = self.bump_settings["tag_format"]
         bump_commit_message: str = self.bump_settings["bump_message"]
-        version_files: List[str] = self.bump_settings["version_files"]
+        version_files: list[str] = self.bump_settings["version_files"]
         major_version_zero: bool = self.bump_settings["major_version_zero"]
         prerelease_offset: int = self.bump_settings["prerelease_offset"]
 
         dry_run: bool = self.arguments["dry_run"]
         is_yes: bool = self.arguments["yes"]
-        increment: Optional[str] = self.arguments["increment"]
-        prerelease: Optional[str] = self.arguments["prerelease"]
-        devrelease: Optional[int] = self.arguments["devrelease"]
-        is_files_only: Optional[bool] = self.arguments["files_only"]
-        is_local_version: Optional[bool] = self.arguments["local_version"]
+        increment: str | None = self.arguments["increment"]
+        prerelease: str | None = self.arguments["prerelease"]
+        devrelease: int | None = self.arguments["devrelease"]
+        is_files_only: bool | None = self.arguments["files_only"]
+        is_local_version: bool | None = self.arguments["local_version"]
         manual_version = self.arguments["manual_version"]
 
         if manual_version:
             if increment:
                 raise NotAllowed("--increment cannot be combined with MANUAL_VERSION")
 
             if prerelease:
```

### Comparing `commitizen-3.2.2/commitizen/commands/changelog.py` & `commitizen-3.3.0/commitizen/commands/changelog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+from __future__ import annotations
+
 import os.path
 from difflib import SequenceMatcher
 from operator import itemgetter
-from typing import Callable, Dict, List, Optional
-
-from packaging.version import parse
+from typing import Callable
 
 from commitizen import bump, changelog, defaults, factory, git, out, version_types
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     DryRunExit,
     NoCommitsFoundError,
     NoPatternMapError,
     NoRevisionError,
     NotAGitProjectError,
     NotAllowed,
 )
 from commitizen.git import GitTag, smart_open
+from packaging.version import parse
 
 
 class Changelog:
     """Generate a changelog based on the commit history."""
 
     def __init__(self, config: BaseConfig, args):
         if not git.is_git_project():
@@ -61,15 +62,15 @@
         self.merge_prerelease = args.get(
             "merge_prerelease"
         ) or self.config.settings.get("changelog_merge_prerelease")
 
         version_type = self.config.settings.get("version_type")
         self.version_type = version_type and version_types.VERSION_TYPES[version_type]
 
-    def _find_incremental_rev(self, latest_version: str, tags: List[GitTag]) -> str:
+    def _find_incremental_rev(self, latest_version: str, tags: list[GitTag]) -> str:
         """Try to find the 'start_rev'.
 
         We use a similarity approach. We know how to parse the version from the markdown
         changelog, but not the whole tag, we don't even know how's the tag made.
 
         This 'smart' function tries to find a similarity between the found version number
         and the available tag.
@@ -88,26 +89,26 @@
             raise NoRevisionError()
         if score < SIMILARITY_THRESHOLD:
             raise NoRevisionError()
         start_rev = tag.name
         return start_rev
 
     def write_changelog(
-        self, changelog_out: str, lines: List[str], changelog_meta: Dict
+        self, changelog_out: str, lines: list[str], changelog_meta: dict
     ):
         if not isinstance(self.file_name, str):
             raise NotAllowed(
                 "Changelog file name is broken.\n"
                 "Check the flag `--file-name` in the terminal "
                 f"or the setting `changelog_file` in {self.config.path}"
             )
 
-        changelog_hook: Optional[Callable] = self.cz.changelog_hook
+        changelog_hook: Callable | None = self.cz.changelog_hook
         with smart_open(self.file_name, "w") as changelog_file:
-            partial_changelog: Optional[str] = None
+            partial_changelog: str | None = None
             if self.incremental:
                 new_lines = changelog.incremental_build(
                     changelog_out, lines, changelog_meta
                 )
                 changelog_out = "".join(new_lines)
                 partial_changelog = changelog_out
 
@@ -116,19 +117,19 @@
             changelog_file.write(changelog_out)
 
     def __call__(self):
         commit_parser = self.cz.commit_parser
         changelog_pattern = self.cz.changelog_pattern
         start_rev = self.start_rev
         unreleased_version = self.unreleased_version
-        changelog_meta: Dict = {}
-        change_type_map: Optional[Dict] = self.change_type_map
-        changelog_message_builder_hook: Optional[
+        changelog_meta: dict = {}
+        change_type_map: dict | None = self.change_type_map
+        changelog_message_builder_hook: None | (
             Callable
-        ] = self.cz.changelog_message_builder_hook
+        ) = self.cz.changelog_message_builder_hook
         merge_prerelease = self.merge_prerelease
 
         if not changelog_pattern or not commit_parser:
             raise NoPatternMapError(
                 f"'{self.config.settings['name']}' rule does not support changelog"
             )
```

### Comparing `commitizen-3.2.2/commitizen/commands/check.py` & `commitizen-3.3.0/commitizen/commands/check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+from __future__ import annotations
+
 import os
 import re
 import sys
-from typing import Any, Dict, Optional
+from typing import Any
 
 from commitizen import factory, git, out
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     InvalidCommandArgumentError,
     InvalidCommitMessageError,
     NoCommitsFoundError,
 )
 
 
 class Check:
     """Check if the current commit msg matches the commitizen format."""
 
-    def __init__(self, config: BaseConfig, arguments: Dict[str, Any], cwd=os.getcwd()):
+    def __init__(self, config: BaseConfig, arguments: dict[str, Any], cwd=os.getcwd()):
         """Initial check command.
 
         Args:
             config: The config object required for the command to perform its action
             arguments: All the flags provided by the user
             cwd: Current work directory
         """
-        self.commit_msg_file: Optional[str] = arguments.get("commit_msg_file")
-        self.commit_msg: Optional[str] = arguments.get("message")
-        self.rev_range: Optional[str] = arguments.get("rev_range")
+        self.commit_msg_file: str | None = arguments.get("commit_msg_file")
+        self.commit_msg: str | None = arguments.get("message")
+        self.rev_range: str | None = arguments.get("rev_range")
         self.allow_abort: bool = bool(
             arguments.get("allow_abort", config.settings["allow_abort"])
         )
 
         self._valid_command_argument()
 
         self.config: BaseConfig = config
@@ -37,15 +39,15 @@
 
     def _valid_command_argument(self):
         num_exclusive_args_provided = sum(
             arg is not None
             for arg in (self.commit_msg_file, self.commit_msg, self.rev_range)
         )
         if num_exclusive_args_provided == 0 and not sys.stdin.isatty():
-            self.commit_msg: Optional[str] = sys.stdin.read()
+            self.commit_msg: str | None = sys.stdin.read()
         elif num_exclusive_args_provided != 1:
             raise InvalidCommandArgumentError(
                 (
                     "Only one of --rev-range, --message, and --commit-msg-file is permitted by check command! "
                     "See 'cz check -h' for more information"
                 )
             )
```

### Comparing `commitizen-3.2.2/commitizen/commands/commit.py` & `commitizen-3.3.0/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/commands/init.py` & `commitizen-3.3.0/commitizen/commands/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import os
 import shutil
-from typing import Any, Dict, List, Optional
+from typing import Any
 
 import questionary
 import yaml
 from commitizen import cmd, factory, out
 from commitizen.__version__ import __version__
 from commitizen.config import BaseConfig, JsonConfig, TomlConfig, YAMLConfig
 from commitizen.cz import registry
@@ -50,18 +52,18 @@
         return os.path.isfile("package.json")
 
     @property
     def is_php_composer(self) -> bool:
         return os.path.isfile("composer.json")
 
     @property
-    def latest_tag(self) -> Optional[str]:
+    def latest_tag(self) -> str | None:
         return get_latest_tag_name()
 
-    def tags(self) -> Optional[List]:
+    def tags(self) -> list | None:
         """Not a property, only use if necessary"""
         if self.latest_tag is None:
             return None
         return get_tag_names()
 
     @property
     def is_pre_commit_installed(self) -> bool:
@@ -281,36 +283,36 @@
         update_changelog_on_bump: bool = questionary.confirm(
             "Create changelog automatically on bump",
             default=True,
             auto_enter=True,
         ).unsafe_ask()
         return update_changelog_on_bump
 
-    def _exec_install_pre_commit_hook(self, hook_types: List[str]):
+    def _exec_install_pre_commit_hook(self, hook_types: list[str]):
         cmd_str = self._gen_pre_commit_cmd(hook_types)
         c = cmd.run(cmd_str)
         if c.return_code != 0:
             err_msg = (
                 f"Error running {cmd_str}."
                 "Outputs are attached below:\n"
                 f"stdout: {c.out}\n"
                 f"stderr: {c.err}"
             )
             raise InitFailedError(err_msg)
 
-    def _gen_pre_commit_cmd(self, hook_types: List[str]) -> str:
+    def _gen_pre_commit_cmd(self, hook_types: list[str]) -> str:
         """Generate pre-commit command according to given hook types"""
         if not hook_types:
             raise ValueError("At least 1 hook type should be provided.")
         cmd_str = "pre-commit install " + " ".join(
             f"--hook-type {ty}" for ty in hook_types
         )
         return cmd_str
 
-    def _install_pre_commit_hook(self, hook_types: Optional[List[str]] = None):
+    def _install_pre_commit_hook(self, hook_types: list[str] | None = None):
         pre_commit_config_filename = ".pre-commit-config.yaml"
         cz_hook_config = {
             "repo": "https://github.com/commitizen-tools/commitizen",
             "rev": f"v{__version__}",
             "hooks": [
                 {"id": "commitizen"},
                 {"id": "commitizen-branch", "stages": ["push"]},
@@ -344,10 +346,10 @@
         if not self.project_info.is_pre_commit_installed:
             raise InitFailedError("pre-commit is not installed in current environment.")
         if hook_types is None:
             hook_types = ["commit-msg", "pre-push"]
         self._exec_install_pre_commit_hook(hook_types)
         out.write("commitizen pre-commit hook is now installed in your '.git'\n")
 
-    def _update_config_file(self, values: Dict[str, Any]):
+    def _update_config_file(self, values: dict[str, Any]):
         for key, value in values.items():
             self.config.set_key(key, value)
```

### Comparing `commitizen-3.2.2/commitizen/commands/version.py` & `commitizen-3.3.0/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/config/__init__.py` & `commitizen-3.3.0/commitizen/config/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Union
 
 from commitizen import defaults, git
 
 from .base_config import BaseConfig
 from .json_config import JsonConfig
 from .toml_config import TomlConfig
 from .yaml_config import YAMLConfig
@@ -22,15 +23,15 @@
         for path in cfg_search_paths
         for filename in defaults.config_files
     )
     for filename in cfg_paths:
         if not filename.exists():
             continue
 
-        _conf: Union[TomlConfig, JsonConfig, YAMLConfig]
+        _conf: TomlConfig | JsonConfig | YAMLConfig
 
         with open(filename, "rb") as f:
             data: bytes = f.read()
 
         if "toml" in filename.suffix:
             _conf = TomlConfig(data=data, path=filename)
         elif "json" in filename.suffix:
```

### Comparing `commitizen-3.2.2/commitizen/config/base_config.py` & `commitizen-3.3.0/commitizen/config/base_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,36 @@
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Optional, Union
 
 from commitizen.defaults import DEFAULT_SETTINGS, Settings
 
 
 class BaseConfig:
     def __init__(self):
         self._settings: Settings = DEFAULT_SETTINGS.copy()
-        self._path: Optional[Path] = None
+        self._path: Path | None = None
 
     @property
     def settings(self) -> Settings:
         return self._settings
 
     @property
-    def path(self) -> Optional[Path]:
+    def path(self) -> Path | None:
         return self._path
 
     def set_key(self, key, value):
         """Set or update a key in the conf.
 
         For now only strings are supported.
         We use to update the version number.
         """
         raise NotImplementedError()
 
     def update(self, data: Settings) -> None:
         self._settings.update(data)
 
-    def add_path(self, path: Union[str, Path]) -> None:
+    def add_path(self, path: str | Path) -> None:
         self._path = Path(path)
 
-    def _parse_setting(self, data: Union[bytes, str]) -> None:
+    def _parse_setting(self, data: bytes | str) -> None:
         raise NotImplementedError()
```

### Comparing `commitizen-3.2.2/commitizen/config/json_config.py` & `commitizen-3.3.0/commitizen/config/json_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from __future__ import annotations
+
 import json
 from pathlib import Path
-from typing import Union
 from commitizen.exceptions import InvalidConfigurationError
 
 from commitizen.git import smart_open
 
 from .base_config import BaseConfig
 
 
 class JsonConfig(BaseConfig):
-    def __init__(self, *, data: Union[bytes, str], path: Union[Path, str]):
+    def __init__(self, *, data: bytes | str, path: Path | str):
         super(JsonConfig, self).__init__()
         self.is_empty_config = False
         self.add_path(path)
         self._parse_setting(data)
 
     def init_empty_config_content(self):
         with smart_open(self.path, "a") as json_file:
@@ -29,15 +30,15 @@
             parser = json.load(f)
 
         parser["commitizen"][key] = value
         with smart_open(self.path, "w") as f:
             json.dump(parser, f, indent=2)
         return self
 
-    def _parse_setting(self, data: Union[bytes, str]) -> None:
+    def _parse_setting(self, data: bytes | str) -> None:
         """We expect to have a section in .cz.json looking like
 
         ```
         {
             "commitizen": {
                 "name": "cz_conventional_commits"
             }
```

### Comparing `commitizen-3.2.2/commitizen/config/toml_config.py` & `commitizen-3.3.0/commitizen/config/toml_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from __future__ import annotations
+
 import os
 from pathlib import Path
-from typing import Union
 
 from tomlkit import exceptions, parse, table
 
 from .base_config import BaseConfig
 
 
 class TomlConfig(BaseConfig):
-    def __init__(self, *, data: Union[bytes, str], path: Union[Path, str]):
+    def __init__(self, *, data: bytes | str, path: Path | str):
         super(TomlConfig, self).__init__()
         self.is_empty_config = False
         self._parse_setting(data)
         self.add_path(path)
 
     def init_empty_config_content(self):
         if os.path.isfile(self.path):
@@ -37,15 +38,15 @@
             parser = parse(f.read())
 
         parser["tool"]["commitizen"][key] = value
         with open(self.path, "wb") as f:
             f.write(parser.as_string().encode("utf-8"))
         return self
 
-    def _parse_setting(self, data: Union[bytes, str]) -> None:
+    def _parse_setting(self, data: bytes | str) -> None:
         """We expect to have a section in pyproject looking like
 
         ```
         [tool.commitizen]
         name = "cz_conventional_commits"
         ```
         """
```

### Comparing `commitizen-3.2.2/commitizen/config/yaml_config.py` & `commitizen-3.3.0/commitizen/config/yaml_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Union
 
 import yaml
 
 from commitizen.git import smart_open
 
 from .base_config import BaseConfig
 
 
 class YAMLConfig(BaseConfig):
-    def __init__(self, *, data: Union[bytes, str], path: Union[Path, str]):
+    def __init__(self, *, data: bytes | str, path: Path | str):
         super(YAMLConfig, self).__init__()
         self.is_empty_config = False
         self._parse_setting(data)
         self.add_path(path)
 
     def init_empty_config_content(self):
         with smart_open(self.path, "a") as json_file:
             yaml.dump({"commitizen": {}}, json_file, explicit_start=True)
 
-    def _parse_setting(self, data: Union[bytes, str]) -> None:
+    def _parse_setting(self, data: bytes | str) -> None:
         """We expect to have a section in cz.yaml looking like
 
         ```
         commitizen:
           name: cz_conventional_commits
         ```
         """
```

### Comparing `commitizen-3.2.2/commitizen/cz/__init__.py` & `commitizen-3.3.0/commitizen/cz/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import importlib
 import pkgutil
 import warnings
-from typing import Iterable, Optional
+from typing import Iterable
 
 import importlib_metadata as metadata
 
 from commitizen.cz.base import BaseCommitizen
 
 
 def discover_plugins(
-    path: Optional[Iterable[str]] = None,
+    path: Iterable[str] | None = None,
 ) -> dict[str, type[BaseCommitizen]]:
     """Discover commitizen plugins on the path
 
     Args:
         path (Path, optional): If provided, 'path' should be either None or a list of paths to look for
     modules in. If path is None, all top-level modules on sys.path.. Defaults to None.
```

### Comparing `commitizen-3.2.2/commitizen/cz/base.py` & `commitizen-3.3.0/commitizen/cz/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
-from typing import Callable, Dict, List, Optional, Tuple
+from typing import Callable
 
 from prompt_toolkit.styles import Style, merge_styles
 
 from commitizen import git
 from commitizen.config.base_config import BaseConfig
 from commitizen.defaults import Questions
 
 
 class BaseCommitizen(metaclass=ABCMeta):
-    bump_pattern: Optional[str] = None
-    bump_map: Optional[Dict[str, str]] = None
-    bump_map_major_version_zero: Optional[Dict[str, str]] = None
-    default_style_config: List[Tuple[str, str]] = [
+    bump_pattern: str | None = None
+    bump_map: dict[str, str] | None = None
+    bump_map_major_version_zero: dict[str, str] | None = None
+    default_style_config: list[tuple[str, str]] = [
         ("qmark", "fg:#ff9d00 bold"),
         ("question", "bold"),
         ("answer", "fg:#ff9d00 bold"),
         ("pointer", "fg:#ff9d00 bold"),
         ("highlighted", "fg:#ff9d00 bold"),
         ("selected", "fg:#cc5454"),
         ("separator", "fg:#cc5454"),
@@ -24,26 +26,26 @@
         ("text", ""),
         ("disabled", "fg:#858585 italic"),
     ]
 
     # The whole subject will be parsed as message by default
     # This allows supporting changelog for any rule system.
     # It can be modified per rule
-    commit_parser: Optional[str] = r"(?P<message>.*)"
-    changelog_pattern: Optional[str] = r".*"
-    change_type_map: Optional[Dict[str, str]] = None
-    change_type_order: Optional[List[str]] = None
+    commit_parser: str | None = r"(?P<message>.*)"
+    changelog_pattern: str | None = r".*"
+    change_type_map: dict[str, str] | None = None
+    change_type_order: list[str] | None = None
 
     # Executed per message parsed by the commitizen
-    changelog_message_builder_hook: Optional[
-        Callable[[Dict, git.GitCommit], Dict]
-    ] = None
+    changelog_message_builder_hook: None | (
+        Callable[[dict, git.GitCommit], dict]
+    ) = None
 
     # Executed only at the end of the changelog generation
-    changelog_hook: Optional[Callable[[str, Optional[str]], str]] = None
+    changelog_hook: Callable[[str, str | None], str] | None = None
 
     def __init__(self, config: BaseConfig):
         self.config = config
         if not self.config.settings.get("style"):
             self.config.settings.update({"style": BaseCommitizen.default_style_config})
 
     @abstractmethod
@@ -59,27 +61,27 @@
         return merge_styles(
             [
                 Style(BaseCommitizen.default_style_config),
                 Style(self.config.settings["style"]),
             ]
         )
 
-    def example(self) -> Optional[str]:
+    def example(self) -> str | None:
         """Example of the commit message."""
         raise NotImplementedError("Not Implemented yet")
 
-    def schema(self) -> Optional[str]:
+    def schema(self) -> str | None:
         """Schema definition of the commit message."""
         raise NotImplementedError("Not Implemented yet")
 
-    def schema_pattern(self) -> Optional[str]:
+    def schema_pattern(self) -> str | None:
         """Regex matching the schema used for message validation."""
         raise NotImplementedError("Not Implemented yet")
 
-    def info(self) -> Optional[str]:
+    def info(self) -> str | None:
         """Information about the standardized commit message."""
         raise NotImplementedError("Not Implemented yet")
 
     def process_commit(self, commit: str) -> str:
         """Process commit for changelog.
 
         If not overwritten, it returns the first line of commit.
```

### Comparing `commitizen-3.2.2/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.3.0/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
             "<body>\n"
             "<BLANK LINE>\n"
             "(BREAKING CHANGE: )<footer>"
         )
 
     def schema_pattern(self) -> str:
         PATTERN = (
-            r"(?s)"  # To explictly make . match new line
+            r"(?s)"  # To explicitly make . match new line
             r"(build|ci|docs|feat|fix|perf|refactor|style|test|chore|revert|bump)"  # type
             r"(\(\S+\))?!?:"  # scope
             r"( [^\n\r]+)"  # subject
             r"((\n\n.*)|(\s*))?$"
         )
         return PATTERN
```

### Comparing `commitizen-3.2.2/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.3.0/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/cz/customize/customize.py` & `commitizen-3.3.0/commitizen/cz/customize/customize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from __future__ import annotations
+
 try:
     from jinja2 import Template
 except ImportError:
     from string import Template  # type: ignore
 
-from typing import Optional
 
 from commitizen import defaults
 from commitizen.config import BaseConfig
 from commitizen.cz.base import BaseCommitizen
 from commitizen.defaults import Questions
 from commitizen.exceptions import MissingCzCustomizeConfigError
 
@@ -63,24 +64,24 @@
     def message(self, answers: dict) -> str:
         message_template = Template(self.custom_settings.get("message_template", ""))
         if getattr(Template, "substitute", None):
             return message_template.substitute(**answers)  # type: ignore
         else:
             return message_template.render(**answers)
 
-    def example(self) -> Optional[str]:
+    def example(self) -> str | None:
         return self.custom_settings.get("example")
 
-    def schema_pattern(self) -> Optional[str]:
+    def schema_pattern(self) -> str | None:
         return self.custom_settings.get("schema_pattern")
 
-    def schema(self) -> Optional[str]:
+    def schema(self) -> str | None:
         return self.custom_settings.get("schema")
 
-    def info(self) -> Optional[str]:
+    def info(self) -> str | None:
         info_path = self.custom_settings.get("info_path")
         info = self.custom_settings.get("info")
         if info_path:
             with open(info_path, "r") as f:
                 content = f.read()
             return content
         elif info:
```

### Comparing `commitizen-3.2.2/commitizen/cz/jira/jira.py` & `commitizen-3.3.0/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/cz/jira/jira_info.txt` & `commitizen-3.3.0/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/defaults.py` & `commitizen-3.3.0/commitizen/defaults.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,66 @@
+from __future__ import annotations
+
 import pathlib
 import sys
 from collections import OrderedDict
-from typing import Any, Dict, Iterable, List, MutableMapping, Optional, Tuple, Union
+from typing import Any, Iterable, MutableMapping
 
 if sys.version_info < (3, 8):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 # Type
 Questions = Iterable[MutableMapping[str, Any]]
 
 
 class CzSettings(TypedDict, total=False):
     bump_pattern: str
-    bump_map: "OrderedDict[str, str]"
-    bump_map_major_version_zero: "OrderedDict[str, str]"
-    change_type_order: List[str]
+    bump_map: OrderedDict[str, str]
+    bump_map_major_version_zero: OrderedDict[str, str]
+    change_type_order: list[str]
 
     questions: Questions
-    example: Optional[str]
-    schema_pattern: Optional[str]
-    schema: Optional[str]
-    info_path: Union[str, pathlib.Path]
+    example: str | None
+    schema_pattern: str | None
+    schema: str | None
+    info_path: str | pathlib.Path
     info: str
     message_template: str
-    commit_parser: Optional[str]
-    changelog_pattern: Optional[str]
-    change_type_map: Optional[Dict[str, str]]
+    commit_parser: str | None
+    changelog_pattern: str | None
+    change_type_map: dict[str, str] | None
 
 
 class Settings(TypedDict, total=False):
     name: str
-    version: Optional[str]
-    version_files: List[str]
-    version_provider: Optional[str]
-    tag_format: Optional[str]
-    bump_message: Optional[str]
+    version: str | None
+    version_files: list[str]
+    version_provider: str | None
+    tag_format: str | None
+    bump_message: str | None
     allow_abort: bool
     changelog_file: str
     changelog_incremental: bool
-    changelog_start_rev: Optional[str]
+    changelog_start_rev: str | None
     changelog_merge_prerelease: bool
     update_changelog_on_bump: bool
     use_shortcuts: bool
-    style: Optional[List[Tuple[str, str]]]
+    style: list[tuple[str, str]] | None
     customize: CzSettings
     major_version_zero: bool
-    pre_bump_hooks: Optional[List[str]]
-    post_bump_hooks: Optional[List[str]]
+    pre_bump_hooks: list[str] | None
+    post_bump_hooks: list[str] | None
     prerelease_offset: int
-    version_type: Optional[str]
+    version_type: str | None
 
 
 name: str = "cz_conventional_commits"
-config_files: List[str] = [
+config_files: list[str] = [
     "pyproject.toml",
     ".cz.toml",
     ".cz.json",
     "cz.json",
     ".cz.yaml",
     "cz.yaml",
 ]
```

### Comparing `commitizen-3.2.2/commitizen/exceptions.py` & `commitizen-3.3.0/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/factory.py` & `commitizen-3.3.0/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/git.py` & `commitizen-3.3.0/commitizen/git.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from __future__ import annotations
+
 import os
 from enum import Enum
 from os import linesep
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import List, Optional
 
 from commitizen import cmd, out
 from commitizen.exceptions import GitCommandError
 
 UNIX_EOL = "\n"
 WINDOWS_EOL = "\r\n"
 
@@ -69,16 +70,15 @@
         return f"GitTag('{self.name}', '{self.rev}', '{self.date}')"
 
     @property
     def date(self):
         return self._date
 
     @classmethod
-    def from_line(cls, line: str, inner_delimiter: str) -> "GitTag":
-
+    def from_line(cls, line: str, inner_delimiter: str) -> GitTag:
         name, objectname, date, obj = line.split(inner_delimiter)
         if not obj:
             obj = objectname
 
         return cls(name=name, rev=obj, date=date)
 
 
@@ -98,19 +98,19 @@
     f.close()
     c = cmd.run(f"git commit {args} -F {f.name}")
     os.unlink(f.name)
     return c
 
 
 def get_commits(
-    start: Optional[str] = None,
+    start: str | None = None,
     end: str = "HEAD",
     *,
     args: str = "",
-) -> List[GitCommit]:
+) -> list[GitCommit]:
     """Get the commits between start and end."""
     git_log_entries = _get_log_as_str_list(start, end, args)
     git_commits = []
     for rev_and_commit in git_log_entries:
         if not rev_and_commit:
             continue
         rev, title, author, author_email, *body_list = rev_and_commit.split("\n")
@@ -136,15 +136,15 @@
     c = cmd.run(f"git show --name-only --pretty=format: {git_reference}")
     if c.return_code == 0:
         return c.out.strip().split("\n")
     else:
         raise GitCommandError(c.err)
 
 
-def get_tags(dateformat: str = "%Y-%m-%d") -> List[GitTag]:
+def get_tags(dateformat: str = "%Y-%m-%d") -> list[GitTag]:
     inner_delimiter = "---inner_delimiter---"
     formatter = (
         f'"%(refname:lstrip=2){inner_delimiter}'
         f"%(objectname){inner_delimiter}"
         f"%(creatordate:format:{dateformat}){inner_delimiter}"
         f'%(object)"'
     )
@@ -171,29 +171,29 @@
     return tag in c.out
 
 
 def is_signed_tag(tag: str) -> bool:
     return cmd.run(f"git tag -v {tag}").return_code == 0
 
 
-def get_latest_tag_name() -> Optional[str]:
+def get_latest_tag_name() -> str | None:
     c = cmd.run("git describe --abbrev=0 --tags")
     if c.err:
         return None
     return c.out.strip()
 
 
-def get_tag_names() -> List[Optional[str]]:
+def get_tag_names() -> list[str | None]:
     c = cmd.run("git tag --list")
     if c.err:
         return []
     return [tag.strip() for tag in c.out.split("\n") if tag.strip()]
 
 
-def find_git_project_root() -> Optional[Path]:
+def find_git_project_root() -> Path | None:
     c = cmd.run("git rev-parse --show-toplevel")
     if not c.err:
         return Path(c.out.strip())
     return None
 
 
 def is_staging_clean() -> bool:
@@ -212,15 +212,15 @@
 def get_eol_style() -> EOLTypes:
     c = cmd.run("git config core.eol")
     eol = c.out.strip().lower()
 
     # We enumerate the EOL types of the response of
     # `git config core.eol`, and map it to our enumration EOLTypes.
     #
-    # It is just like the varient of the "match" syntax.
+    # It is just like the variant of the "match" syntax.
     map = {
         "lf": EOLTypes.LF,
         "crlf": EOLTypes.CRLF,
         "native": EOLTypes.NATIVE,
     }
 
     # If the response of `git config core.eol` is in the map:
@@ -233,15 +233,15 @@
 
 
 def smart_open(*args, **kargs):
     """Open a file with the EOL style determined from Git."""
     return open(*args, newline=get_eol_style().get_eol_for_open(), **kargs)
 
 
-def _get_log_as_str_list(start: Optional[str], end: str, args: str) -> List[str]:
+def _get_log_as_str_list(start: str | None, end: str, args: str) -> list[str]:
     """Get string representation of each log entry"""
     delimiter = "----------commit-delimiter----------"
     log_format: str = "%H%n%s%n%an%n%ae%n%b"
     git_log_cmd = (
         f"git -c log.showSignature=False log --pretty={log_format}{delimiter} {args}"
     )
     if start:
```

### Comparing `commitizen-3.2.2/commitizen/hooks.py` & `commitizen-3.3.0/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/out.py` & `commitizen-3.3.0/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.2.2/commitizen/providers.py` & `commitizen-3.3.0/commitizen/providers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import json
 import re
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Callable, ClassVar, Optional, cast
+from typing import Any, Callable, ClassVar, cast
 
 import importlib_metadata as metadata
 import tomlkit
 from packaging.version import VERSION_PATTERN, Version
 
 from commitizen.config.base_config import BaseConfig
 from commitizen.exceptions import VersionProviderUnknown
@@ -111,22 +111,33 @@
     def set(self, pyproject: tomlkit.TOMLDocument, version: str):
         pyproject["tool"]["poetry"]["version"] = version  # type: ignore
 
 
 class CargoProvider(TomlProvider):
     """
     Cargo version management
+
+    With support for `workspaces`
     """
 
     filename = "Cargo.toml"
 
     def get(self, document: tomlkit.TOMLDocument) -> str:
-        return document["package"]["version"]  # type: ignore
+        try:
+            return document["package"]["version"]  # type: ignore
+        except tomlkit.exceptions.NonExistentKey:
+            ...
+        return document["workspace"]["package"]["version"]  # type: ignore
 
     def set(self, document: tomlkit.TOMLDocument, version: str):
+        try:
+            document["workspace"]["package"]["version"] = version  # type: ignore
+            return
+        except tomlkit.exceptions.NonExistentKey:
+            ...
         document["package"]["version"] = version  # type: ignore
 
 
 class JsonProvider(FileProvider):
     """
     Base class for JSON-based version providers
     """
@@ -180,22 +191,22 @@
         "$major": r"(?P<major>\d+)",
         "$minor": r"(?P<minor>\d+)",
         "$patch": r"(?P<patch>\d+)",
         "$prerelease": r"(?P<prerelease>\w+\d+)?",
         "$devrelease": r"(?P<devrelease>\.dev\d+)?",
     }
 
-    def _tag_format_matcher(self) -> Callable[[str], Optional[str]]:
+    def _tag_format_matcher(self) -> Callable[[str], str | None]:
         pattern = self.config.settings.get("tag_format") or VERSION_PATTERN
         for var, tag_pattern in self.TAG_FORMAT_REGEXS.items():
             pattern = pattern.replace(var, tag_pattern)
 
         regex = re.compile(f"^{pattern}$", re.VERBOSE)
 
-        def matcher(tag: str) -> Optional[str]:
+        def matcher(tag: str) -> str | None:
             match = regex.match(tag)
             if not match:
                 return None
             groups = match.groupdict()
             if "version" in groups:
                 return groups["version"]
             elif "major" in groups:
```

### Comparing `commitizen-3.2.2/commitizen/version_types.py` & `commitizen-3.3.0/commitizen/version_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,65 @@
+from __future__ import annotations
+
 import sys
-from typing import Optional, Tuple, Union
 
 if sys.version_info >= (3, 8):
     from typing import Protocol as _Protocol
 else:
     _Protocol = object
 
 from packaging.version import Version
 
 
 class VersionProtocol(_Protocol):
-    def __init__(self, _version: Union[Version, str]):
+    def __init__(self, _version: Version | str):
         raise NotImplementedError("must be implemented")
 
     def __str__(self) -> str:
         raise NotImplementedError("must be implemented")
 
     @property
-    def release(self) -> Tuple[int, ...]:
+    def release(self) -> tuple[int, ...]:
         raise NotImplementedError("must be implemented")
 
     @property
     def is_prerelease(self) -> bool:
         raise NotImplementedError("must be implemented")
 
     @property
-    def pre(self) -> Optional[Tuple[str, int]]:
+    def pre(self) -> tuple[str, int] | None:
         raise NotImplementedError("must be implemented")
 
     @property
-    def local(self) -> Optional[str]:
+    def local(self) -> str | None:
         raise NotImplementedError("must be implemented")
 
     @property
     def public(self) -> str:
         raise NotImplementedError("must be implemented")
 
 
 class SemVerVersion(VersionProtocol):
     def __init__(self, version: str):
         self._version = Version(version)
 
     @property
-    def release(self) -> Tuple[int, ...]:
+    def release(self) -> tuple[int, ...]:
         return self._version.release
 
     @property
     def is_prerelease(self) -> bool:
         return self._version.is_prerelease
 
     @property
-    def pre(self) -> Optional[Tuple[str, int]]:
+    def pre(self) -> tuple[str, int] | None:
         return self._version.pre
 
     @property
-    def local(self) -> Optional[str]:
+    def local(self) -> str | None:
         return self._version.local
 
     @property
     def public(self) -> str:
         return self._version.public
 
     def __str__(self) -> str:
```

### Comparing `commitizen-3.2.2/docs/README.md` & `commitizen-3.3.0/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 ---
 
 ## About
 
 Commitizen is release management tool designed for teams.
 
-Commitizen assumes your team uses a standard way of commiting rules
+Commitizen assumes your team uses a standard way of committing rules
 and from that foundation, it can bump your project's version, create
 the changelog, and update files.
 
 By default, commitizen uses [conventional commits][conventional_commits], but you
 can build your own set of rules, and publish them.
 
-Using a standarized set of rules to write commits, makes commits easier to read, and enforces writing
+Using a standardized set of rules to write commits, makes commits easier to read, and enforces writing
 descriptive commits.
 
 ### Features
 
 - Command-line utility to create commits with your rules. Defaults: [Conventional commits][conventional_commits]
 - Bump version automatically using [semantic versioning][semver] based on the commits. [Read More](./bump.md)
 - Generate a changelog using [Keep a changelog][keepchangelog]
```

### Comparing `commitizen-3.2.2/pyproject.toml` & `commitizen-3.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.2.2"
+version = "3.3.0"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.2.2"
+version = "3.3.0"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
```

### Comparing `commitizen-3.2.2/PKG-INFO` & `commitizen-3.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.2.2
+Version: 3.3.0
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -17,20 +17,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: argcomplete (>=1.12.1,<3.1)
 Requires-Dist: charset-normalizer (>=2.1.0,<4)
 Requires-Dist: colorama (>=0.4.1,<0.5.0)
 Requires-Dist: decli (>=0.6.0,<0.7.0)
 Requires-Dist: importlib_metadata (>=4.13,<7)
 Requires-Dist: jinja2 (>=2.10.3)
@@ -59,22 +53,22 @@
 
 ---
 
 ## About
 
 Commitizen is release management tool designed for teams.
 
-Commitizen assumes your team uses a standard way of commiting rules
+Commitizen assumes your team uses a standard way of committing rules
 and from that foundation, it can bump your project's version, create
 the changelog, and update files.
 
 By default, commitizen uses [conventional commits][conventional_commits], but you
 can build your own set of rules, and publish them.
 
-Using a standarized set of rules to write commits, makes commits easier to read, and enforces writing
+Using a standardized set of rules to write commits, makes commits easier to read, and enforces writing
 descriptive commits.
 
 ### Features
 
 - Command-line utility to create commits with your rules. Defaults: [Conventional commits][conventional_commits]
 - Bump version automatically using [semantic versioning][semver] based on the commits. [Read More](./bump.md)
 - Generate a changelog using [Keep a changelog][keepchangelog]
```

