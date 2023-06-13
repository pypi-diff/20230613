# Comparing `tmp/skulk-2.0.3-py2.py3-none-any.whl.zip` & `tmp/skulk-2.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 9241 bytes, number of entries: 10
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-06 16:13 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 16:12 skulk/__init__.py
--rw-r--r--  2.0 unx     9548 b- defN 23-Jun-06 16:12 skulk/bumper.py
--rw-r--r--  2.0 unx     9801 b- defN 23-Jun-06 16:12 skulk/skulk.py
--rw-r--r--  2.0 unx     3363 b- defN 23-Jun-06 16:12 skulk/util.py
--rw-r--r--  2.0 unx      646 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      733 b- defN 23-Jun-06 16:13 skulk-2.0.3.dist-info/RECORD
-10 files, 24256 bytes uncompressed, 7999 bytes compressed:  67.0%
+Zip file size: 10429 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-13 17:57 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 17:56 skulk/__init__.py
+-rw-r--r--  2.0 unx    11487 b- defN 23-Jun-13 17:56 skulk/bumper.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-Jun-13 17:56 skulk/questions.py
+-rw-r--r--  2.0 unx    10044 b- defN 23-Jun-13 17:56 skulk/skulk.py
+-rw-r--r--  2.0 unx     3586 b- defN 23-Jun-13 17:56 skulk/util.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      810 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/RECORD
+11 files, 29025 bytes uncompressed, 9075 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -3,29 +3,32 @@
 
 Filename: skulk/__init__.py
 Comment: 
 
 Filename: skulk/bumper.py
 Comment: 
 
+Filename: skulk/questions.py
+Comment: 
+
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.0.3.dist-info/METADATA
+Filename: skulk-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.0.3.dist-info/WHEEL
+Filename: skulk-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.0.3.dist-info/entry_points.txt
+Filename: skulk-2.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.0.3.dist-info/top_level.txt
+Filename: skulk-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.0.3.dist-info/RECORD
+Filename: skulk-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.0.3
+2.1.0
```

## skulk/bumper.py

```diff
@@ -4,175 +4,207 @@
 import json
 import subprocess
 import semver
 import functools
 
 from . import util
 
-
+PROD_PYPI_INDEX = "https://pypi.org/simple/"
+TEST_PYPI_INDEX = "https://test.pypi.org/simple/"
 MOCKED = False
 MOCK_VERSIONS = {
-    "pypi": ["0.1.7", "1.4.3", "1.4.4", "1.4.5"],
+    "pypi": ["0.1.7", "1.4.3", "1.4.4", "1.4.5", "1.4.6-rc.1"],
+    "test": ["0.1.7", "1.4.3", "1.4.4", "1.4.5"],
     "tags": ["0.1.2", "0.1.3", "1.4.4", "1.4.5"],
 }
 
+RELEASE_SCOPE_BETA = "beta"
+RELEASE_SCOPE_RELEASE = "release"
+RELEASE_SCOPE_CANDIDATE = "candidate"
+
+RELEASE_TOKENS = {
+    RELEASE_SCOPE_BETA: "beta",
+    RELEASE_SCOPE_RELEASE: None,
+    RELEASE_SCOPE_CANDIDATE: "rc",
+}
+
+
+VERSION_POLICY = {
+    "patch": "A bug fix",
+    "minor": "A new feature",
+    "major": "A breaking change",
+}
+
 
 class Bumper(object):
     """A class to help the user bump the version."""
 
     def __init__(self, repo, pip_name):
         self.repo = repo
         self.pip_name = pip_name
         self.version_filename = os.path.join(self.repo.working_dir, "VERSION")
         self.current_version = _read_version_file(self.version_filename)
-        self.versions = None
-        self.next_version = None
-
-        self.latest_pypi_version = None
-        self.latest_tag_version = None
-        self.latest_version = None
-
-    def is_prerelease(self):
-        """Return True if the current version is a prerelease."""
-        return semver.Version.parse(self.current_version).prerelease is not None
-
-    def run(self):
-        """Wizard to choose a version."""
-
-        self._set_versions()
-
-        print("Versions:")
-        print(json.dumps(self.versions, indent=3))
-        print(f"The latest version on PyPi is: {self.latest_pypi_version}")
-        print(f"The latest tag in the repo is: {self.latest_tag_version}")
-        print(
-            "When you push this branch, we'll deploy to PyPi and we'll tag the repo with the version you choose."
-        )
-
-        if self.current_version not in self.versions["pypi"] + self.versions["tags"]:
-            print(
-                f"The local VERSION file contains a valid version: {self.current_version}."
-            )
-
-            print("You can use this version or you can bump to a new version.")
-            do_bump = util.yes_no("Do you wish to bump the version?")
-            if not do_bump:
-                return
-
-        else:
-            do_bump = True
-            print(
-                f"The local VERSION file contains an invalid version: {self.current_version}. It has been used already."
-            )
-            print("You'll need to bump the version.")
-
-        version_options = get_version_options(self.latest_version)
-
-        version_options += [
-            "Explicit: Specify a version manually. This is not recommended.",
-            "Cancel: I changed my mind. I don't want to tag or release. I just want to push.",
-            "Exit!"
-        ]
+        self.versions = self.get_versions()
 
-        # options = [f"{v[0]: <16} {v[1]}" for v in version_options]
-        num_options = len(version_options)
-        exit_option = num_options
-        no_tags_option = num_options - 1
-        custom_option = num_options - 2
-
-        bump_type = 0
-        msg = "Choose a new version"
-        while bump_type not in range(1, len(version_options) + 1):
-            print(msg)
-            for i, opt in enumerate(version_options):
-                n = i + 1
-                print(f"{n}: {opt}")
-            bump_type = input(util.green("Enter a number: "))
-            if not bump_type.isdigit():
-                bump_type = 0
-            bump_type = int(bump_type)
-            msg = f"Please choose a number between 1 and {num_options}."
-
-        if bump_type == exit_option:
-            sys.stderr.write("Exited:\n")
-            sys.exit(1)
-        msg = ""
-        if bump_type == custom_option:  # specify a version
-            custom_valid = False
-            while not custom_valid:
-                print(msg)
-                custom_version = input(
-                    util.green("Enter a version string or type 'exit' to exit: ")
-                )
-                if custom_version == "exit":
-                    sys.stderr.write("Exited:\n")
-                    sys.exit(1)
-                if not semver.Version.is_valid(custom_version):
-                    msg = f"Version {custom_version} is not a valid semver string."
-                elif custom_version in self.versions["pypi"]:
-                    msg = f"Version {custom_version} has already been released to PyPi."
-                elif custom_version in self.versions["tags"]:
-                    msg = (
-                        f"Version {custom_version} has already been tagged in the repo."
-                    )
-                else:
-                    custom_valid = True
-                    msg = f"Version {custom_version} is valid."
-                    self.next_version = custom_version
-        elif bump_type == no_tags_option:  # no tags
-            self.next_version = None
-        else:  # bump_type is one of the regular options
-            self.next_version = str(version_options[bump_type - 1])
-        print(self.next_version)
-        if self.next_version:
-            print(f"You bumped the version to: {self.next_version}")
-        else:
-            print("You chose to push with no tag or release.")
+    def latest_test_version(self):
+        """Return the latest version on test.pypi.org."""
+        return self.latest_version("test")
+
+    def latest_pypi_version(self):
+        """Return the latest version on pypi.org."""
+        return self.latest_version("pypi")
+
+    def latest_tag_version(self):
+        """Return the latest tag from github."""
+        return self.latest_version("tags")
+
+    def latest_version(self, *sources):
+        """Return the latest version from a list of versions."""
+        if not sources:
+            sources = ["test", "pypi", "tags"]
+        return sorted_versions(
+            [v for source in sources for v in self.versions[source]]
+        )[-1]
 
-    def _set_versions(self):
+    def get_versions(self):
         """Fetch the latest tags and PyPi versions."""
         if MOCKED:
-            self.versions = MOCK_VERSIONS
+            return MOCK_VERSIONS
         else:
-            self.versions = {"pypi": self.get_pypi_versions(), "tags": self.get_tags()}
+            return {
+                "test": self.get_pypi_versions(index=util.TEST_PYPI_INDEX),
+                "pypi": self.get_pypi_versions(),
+                "tags": self.get_tags(),
+            }
 
-        self.latest_pypi_version = _sorted_versions(self.versions["pypi"])[-1]
-        self.latest_tag_version = _sorted_versions(self.versions["tags"])[-1]
-        # These should be the same, but if they're not, we'll use the highest
-        self.latest_version = _sorted_versions(
-            [self.latest_pypi_version, self.latest_tag_version]
-        )[-1]
-
-    def get_pypi_versions(self):
+    def get_pypi_versions(self, index=util.PROD_PYPI_INDEX):
         """
         Return a list of all PyPi versions for the named package.
         """
-        return _get_pypi_versions(self.pip_name)
+        return _get_pypi_versions(self.pip_name, index=index)
 
     def get_tags(self):
         """Return a list of all tags in the repo."""
-        return _sorted_versions([str(tag) for tag in self.repo.tags])
+        return sorted_versions([str(tag) for tag in self.repo.tags])
+
+    def version_options(self, release_scope=RELEASE_SCOPE_BETA):
+        if release_scope == RELEASE_SCOPE_BETA:
+            sources = ["test", "pypi", "tags"]
+        else:
+            sources = ["pypi", "tags"]
+        token = RELEASE_TOKENS[release_scope]
+        reference_version = self.latest_version(*sources)
+        result = get_version_options(reference_version, token=token)
+        for i, v in enumerate(["patch", "minor", "major"]):
+            result[i] = {
+                "label": f"{result[i]} : {VERSION_POLICY[v]}",
+                "value": result[i],
+            }
+
+        return result
+
+    def versions_table(self, max_versions=10):
+        """Return a table of versions where the columns are the sources, and the rows are the versions."""
+        sources = ["test", "pypi", "tags"]
+        source_labels = [
+            util.blue("Internal PyPi"),
+            util.green("Production PyPi"),
+            util.magenta("Repository Tags"),
+        ]
+        table = {}
+        for source in sources:
+            for version in sorted_versions(self.versions[source])[-max_versions:]:
+                if version not in table:
+                    table[version] = {"tags": False, "pypi": False, "test": False}
+                table[version][source] = True
+
+        # now convert the table to a list of dicts sorted in reverse
+        result_table = [source_labels]
+        versions = sorted_versions(table.keys())
+        versions.reverse()
+        for version in versions:
+            result_table.append(
+                [
+                    util.blue(version) if table[version]["test"] else "",
+                    util.green(version) if table[version]["pypi"] else "",
+                    util.magenta(version) if table[version]["tags"] else "",
+                ]
+            )
+        return result_table
 
-    def is_released_version(self, version):
-        """Return True if the version has been released to PyPi or tagged in the repo."""
+    def validate_generic_version(self, version):
+        """Validate that the version is a valid semver string."""
         if not semver.Version.is_valid(version):
-            return None
-        release_version = str(
-            semver.Version.parse(version).replace(prerelease=None, build=None)
-        )
-        if release_version in self.versions["pypi"] + self.versions["tags"]:
-            return release_version
+            return f"Version {version} is not a valid semver string."
+        version = semver.Version.parse(version)
+        if version in self.versions["pypi"]:
+            return f"Version {version} has already been released to PyPi."
+        if version in self.versions["tags"]:
+            return f"Version {version} has already been tagged in the repo."
+        if version in self.versions["test"]:
+            return f"Version {version} has already been released to Test PyPi."
         return None
 
-def _pypi_to_semver(p):
+    def validate_beta_version(self, version):
+        """Validate that the version is a valid beta version."""
+        problem = self.validate_generic_version(version)
+        if problem:
+            return problem
+        version = semver.Version.parse(version)
+        regex = re.compile(r"beta\.\d+")
+        if not (version.prerelease and regex.match(version.prerelease)):
+            return f"Version {version} is not a beta version like '1.2.3-beta.4'."
+        return None
+
+    def validate_candidate_version(self, version):
+        """Validate that the version is a valid release candidate version."""
+        problem = self.validate_generic_version(version)
+        if problem:
+            return problem
+        version = semver.Version.parse(version)
+        regex = re.compile(r"rc\.\d+")
+        if not (version.prerelease and regex.match(version.prerelease)):
+            return f"Version {version} is not a release candidate version like '1.2.3-rc.4'."
+        return None
+
+    def validate_release_version(self, version):
+        """Validate that the version is a valid release version."""
+        problem = self.validate_generic_version(version)
+        if problem:
+            return problem
+        version = semver.Version.parse(version)
+        if not version.prerelease or version.build:
+            return f"Version {version} is not a release version like '1.2.3'."
+        return None
+
+
+def pypi_to_semver(version):
     """Convert a PyPi version to a semver."""
-    return p.replace("rc", "-rc.")
+    pypi_version_regex = re.compile(r"(\d+)\.(\d+)\.(\d+)((rc|a|b)(\d+))?")
+    match = pypi_version_regex.match(version)
+    if not match:
+        return None
+    major, minor, patch, prerelease, prerelease_type, prerelease_num = match.groups()
+    if prerelease_type:
+        prerelease_type = {"rc": "rc", "a": "alpha", "b": "beta"}[prerelease_type]
+        prerelease = f"-{prerelease_type}.{prerelease_num}"
+    return f"{major}.{minor}.{patch}{prerelease or ''}"
+
+
+def semver_to_pypi(version):
+    version = semver.Version.parse(version)
+    prerelease = ""
+    if version.prerelease:
+        prerelease_type, prerelease_num = version.prerelease.split(".")
+        prerelease_type = {"rc": "rc", "alpha": "a", "beta": "b"}[prerelease_type]
+        prerelease = f"{prerelease_type}{prerelease_num}"
+    return f"{version.major}.{version.minor}.{version.patch}{prerelease or ''}"
 
 
-def _sorted_versions(versions):
+def sorted_versions(versions):
     """Sort a list of versions."""
     return sorted(versions, key=functools.cmp_to_key(semver.compare))
 
 
 def _read_version_file(filename):
     """Pull the version from the VERSION file."""
     version = util.first_nonblank_line(filename)
@@ -180,84 +212,111 @@
         sys.stderr.write(
             f"Can't get version string from the version file: {filename}. using 0.0.1\n"
         )
         return "0.0.1"
     return version if semver.Version.is_valid(version) else "0.0.1"
 
 
-def _get_pypi_versions(pip_name):
+def _get_pypi_versions(pip_name, index):
     """
     Return a list of all PyPi versions for the named package.
 
     The package may not exist on PyPi, in which case we return an empty list. We
     don't error out, because it's perfectly valid for no package to exist. We
     can still deploy there.
     """
 
-    # notice this command says: Install version== (i.e. it requests an invalid
+    # NOTE: This command says: Install version== (i.e. it requests an invalid
     # version). It fails as intended, and the result is a message to say can't
     # find version in versions. It lists the existing versions which we split
     # and return. Check for py3 and py 27 compatible by using both pips.
     args = [
         "pip3",
         "install",
         "--index-url",
-        util.PROD_PYPI_INDEX,
+        index,
         f"{pip_name}==",
     ]
     output = subprocess.Popen(
         args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
     ).communicate()
     if len(output) < 2 or "none" in output[1].decode("utf-8"):
         args = [
             "pip2.7",
             "install",
             "--index-url",
-            util.PROD_PYPI_INDEX,
+            index,
             f"{pip_name}==",
         ]
         output = subprocess.Popen(
             args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         ).communicate()
         if len(output) < 2 or "none" in output[1].decode("utf-8"):
             return []
 
     output = output[1]
     regex = re.compile(
         r"^.*Could not find a version.*from versions:(.*)\).*", re.DOTALL
     )
     match = regex.match(output.decode("utf-8"))
     if match:
-        result = [_pypi_to_semver(v.strip()) for v in match.group(1).split(r", ")]
+        result = [pypi_to_semver(v.strip()) for v in match.group(1).split(r", ")]
 
-        return _sorted_versions([v for v in result if semver.Version.is_valid(v)])
+        return sorted_versions([v for v in result if semver.Version.is_valid(v)])
     return []
 
 
-def get_version_options(latest_version):
+def get_version_options(latest_version, token=None):
     """Return a list of the most likely versions to bump to
-    
+
     See the tests for examples.
     """
     latest = semver.Version.parse(latest_version)
+    if not token:
+        return _get_release_options(latest)
+    latest_version_token = latest.prerelease and latest.prerelease.split(".", 1)[0]
+    if latest_version_token and (latest_version_token != token):
+        if latest_version_token < token:
+            return _get_later_prerelease_options(latest, token)
+        return _get_earlier_prerelease_options(latest, token)
+    return _get_any_prerelease_options(latest, token)
+
+
+def _get_release_options(latest):
     if latest.prerelease:
-        version_options = [
-            str(latest.next_version(part="prerelease")),
-            str(latest.next_version(part="patch")),
-        ]
         latest = latest.replace(prerelease=None)
-        version_options += [
-            str(latest.next_version(part="minor").bump_prerelease()),
+        return [
+            str(latest),
             str(latest.next_version(part="minor")),
-            str(latest.next_version(part="major").bump_prerelease()),
             str(latest.next_version(part="major")),
         ]
-    else:
-        version_options = [
-            str(latest.next_version(part="prerelease")),
-            str(latest.next_version(part="patch")),
-            str(latest.next_version(part="minor").bump_prerelease()),
-            str(latest.next_version(part="minor")),
-            str(latest.next_version(part="major").bump_prerelease()),
-            str(latest.next_version(part="major")),
-        ]
-    return version_options
+    return [
+        str(latest.next_version(part="patch")),
+        str(latest.next_version(part="minor")),
+        str(latest.next_version(part="major")),
+    ]
+
+
+def _get_any_prerelease_options(latest, token):
+    return [
+        str(latest.next_version(part="prerelease", prerelease_token=token)),
+        str(latest.bump_minor().bump_prerelease(token=token)),
+        str(latest.bump_major().bump_prerelease(token=token)),
+    ]
+
+
+def _get_later_prerelease_options(latest, token):
+    latest = latest.replace(prerelease=None)
+    return [
+        str(latest.bump_prerelease(token=token)),
+        str(latest.bump_minor().bump_prerelease(token=token)),
+        str(latest.bump_major().bump_prerelease(token=token)),
+    ]
+
+
+def _get_earlier_prerelease_options(latest, token):
+    latest = latest.replace(prerelease=None)
+    return [
+        str(latest.next_version(part="prerelease", prerelease_token=token)),
+        str(latest.bump_minor().bump_prerelease(token=token)),
+        str(latest.bump_major().bump_prerelease(token=token)),
+    ]
```

## skulk/skulk.py

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python3
-
 """
 Skulk.
 
 A tool to help get your repo in good shape for a release.
 
 It works for packages intended for PyPi.
 
@@ -28,20 +26,26 @@
     a. You'll be shown the current version and the latest version on PyPi.
     b. You'll be asked to choose a new version from the options.
 
 
 """
 
 from __future__ import print_function
-from builtins import input
 import datetime
 import os
 import sys
-from . import util
-from .bumper import Bumper
+from skulk import util
+from skulk.bumper import (
+    Bumper,
+    RELEASE_SCOPE_BETA,
+    RELEASE_SCOPE_CANDIDATE,
+    RELEASE_SCOPE_RELEASE,
+)
+from skulk import questions as q
+from tabulate import tabulate
 
 
 class Skulk(object):
     """A wizard to guide the user to a good version and changelog."""
 
     def __init__(self):
         self.repo = util.get_repo()
@@ -51,227 +55,237 @@
         self.hook_filename = os.path.join(self.working_dir, ".git", "hooks", "pre-push")
         self.changelog_filename = os.path.join(self.working_dir, "CHANGELOG.md")
         self.version_filename = os.path.join(self.working_dir, "VERSION")
         self.pip_name = util.get_pip_name(self.repo)
         self.bumper = None
         self.edit_changelog = False
         self.changelog_addition = ""
+        self.release_scope = None
+        self.next_version = None
 
     def run(self):
-        """
-        Guide the user to ensure version and changelog are valid.
-        """
-
         self.check_pre_push_hook()
-        self.check_clean()
         self.bumper = Bumper(self.repo, self.pip_name)
-        if self.ask_do_tag_release():
-            self.bumper.run()
-
-        self.ask_changelog_additions()
-
-        # Now we do the actual work.
-        # CHANGELOG
-        if self.edit_changelog:
-            self.resolve_changelog()
-
-        if self.bumper.next_version:
-            with open(self.version_filename, "w", encoding="utf-8") as vfn:
-                vfn.write(self.bumper.next_version)
-
+        self.check_clean()
+        self.release_scope = self.ask_release_scope()
+        self.show_recent_versions()
+        self.next_version = self.ask_version()
+        self.ask_changelog_update()
+        self.write_version()
         self.commit_version_changelog()
         tag = self.add_tag()
-        do_push = self.ask_push(tag)
-        if do_push:
-            self.push(tag)
-        else:
-            print("No worries. Use the following command to push later. Bye\n")
-            if tag:
-                print(f"git push --atomic origin {self.branch_name} {tag.name}")
-            else:
-                print(f"git push origin {self.branch_name}")
+        self.ask_push(tag)
         sys.exit(0)
 
-    # PRIVATE
-    def ask_push(self, tag=None):
-        """Ask the user if he wants to push the branch and tag."""
-        if tag:
-            question = f"Do you want me to push the branch and tag: {self.branch_name} + {tag.name}` for you?"
-        else:
-            question = f"Do you want me to push the branch: {self.branch_name} for you?"
-        return util.yes_no(question)
-
-    def push(self, tag=None):
-        """Push the branch and tag."""
-        origin = self.repo.remote("origin")
-        if tag:
-            origin.push(self.branch)
-            origin.push(tag)
-            print("Pushed branch and tag.\n")
-        else:
-            origin.push(self.branch)
-            print("Pushed branch.\n")
-
-    def add_tag(self):
-        """Add a tag to the repo."""
-        if self.bumper.next_version:
-            label = "Pre-release" if self.bumper.is_prerelease() else "Release"
-            tag = self.repo.create_tag(
-                self.bumper.next_version, message=f"{label}: {self.bumper.next_version}"
-            )
-            print(f"Created tag: {tag.name}")
-            return tag
-        return None
-
-    def commit_version_changelog(self):
-        """Commit the version and changelog files."""
-        if self.bumper.next_version:
-            if self.repo.is_dirty():
-                self.repo.index.add([self.changelog_filename, self.version_filename])
-                self.repo.index.commit(
-                    f"Update changelog and sets version to {self.bumper.next_version}"
-                )
-                print("Committed Version and Changelog\n")
-
-        elif self.edit_changelog:
-            if self.repo.is_dirty():
-                self.repo.index.add([self.changelog_filename])
-                self.repo.index.commit("Update changelog")
-                print("Committed Changelog\n")
-
     def check_clean(self):
         """Check that the repo is clean and give user a chance to clean it up.
 
-        User can continue with a dirty repo, but we at least want to warn them.
+        User can continue with a dirty repo, but we at least want to warn about it.
         """
         if not self.repo.is_dirty():
-            print("Repo clean. Good to go.")
+            print(util.green("Repo clean. Good to go."))
             return
 
+        print(util.red("Attention: Repository is dirty."))
+
         mods = [item.a_path for item in self.repo.index.diff(None)]
+        util.print_truncated_list(
+            mods,
+            "Modified files",
+            header_color=util.magenta,
+            item_color=util.default_color,
+        )
+
         untracked = self.repo.untracked_files
-        if mods:
-            print(util.magenta("Modified files:\n{}".format("\n".join(mods))))
-        if untracked:
-            print(util.magenta("Untracked files:\n{}".format("\n".join(untracked))))
+        util.print_truncated_list(
+            untracked,
+            "Untracked files",
+            header_color=util.blue,
+            item_color=util.default_color,
+        )
+
+        q.wait("If you want to include them, please commit them now.")
+
+    def ask_release_scope(self):
+        prompt = "What kind of deployment do you want to make?"
+        choices = [
+            {"label": "Beta release for internal testing", "value": RELEASE_SCOPE_BETA},
+            {
+                "label": "Candidate release for customer testing",
+                "value": RELEASE_SCOPE_CANDIDATE,
+            },
+        ]
+        if self.branch_name == "master":
+            choices.append({"label": "Full release", "value": RELEASE_SCOPE_RELEASE})
+        return q.choose(prompt, choices)
 
+    def show_recent_versions(self):
+        versions_table = self.bumper.versions_table()
         print(
-            "----------\nAttention: Repo is dirty. Uncommitted changes won't be included. Is this ok?"
+            util.yellow(
+                "Here's a table of recent versions on PyPi and in the repository"
+            )
         )
-        print("If you want to include them, please commit them now.")
-        cont = input(
-            util.green(
-                "When you are happy, press enter to continue or type 'exit' to exit."
+        print(
+            tabulate(
+                versions_table, headers="firstrow", tablefmt="pretty", stralign="left"
             )
         )
-        if cont == "exit":
-            sys.stderr.write("Exited.\n")
-            sys.exit(0)
-
-    def ask_do_tag_release(self):
-        """Ask the user if he wants to make a pre-release from this branch."""
-        return util.yes_no(
-            "Do you want to tag and deploy from this branch?",
-            "No, push only",
-            "Yes, push and deploy a tagged release.",
+        print("\n")
+
+    def ask_version(self):
+        choices = self.bumper.version_options(release_scope=self.release_scope)
+        choices.append({"label": "Custom (Not recommended)", "value": "custom"})
+        choice = q.choose(
+            f"What {self.release_scope} version do you want to deploy?", choices
         )
 
-    def ask_changelog_additions(self):
+        if choice == "custom":
+            if self.release_scope == RELEASE_SCOPE_BETA:
+                validator = self.bumper.validate_beta_version
+            elif self.release_scope == RELEASE_SCOPE_CANDIDATE:
+                validator = self.bumper.validate_candidate_version
+            else:
+                validator = self.bumper.validate_release_version
+
+            choice = q.input_string(
+                f"Enter a valid {self.release_scope} version number:",
+                validator=validator,
+            )
+
+        return choice
+
+    def ask_changelog_update(self):
         """Generate the reference additions to the changelog.
 
         Do not write anything to the changelog file yet."""
+
+        changelog_update = True
         stub = ""
-        if self.bumper.next_version:
-            self.edit_changelog = True
-            date_string = datetime.date.today().strftime("%d %b %Y")
-            stub = f"## Version:{self.bumper.next_version} -- {date_string}\n\n"
-        else:
-            self.edit_changelog = util.yes_no(
-                "No version bump. Do you want to add entries in the changelog anyway?"
+        if self.release_scope == RELEASE_SCOPE_BETA:
+            print(
+                util.yellow(
+                    "Since this is an internal beta release, an updated changelog is optional."
+                )
             )
-            stub = "## Unreleased\n\n"
+            changelog_update = q.yes_no("Do you want to update the changelog?")
+            if self.changelog_needs_unreleased_stub():
+                stub = f"## Unreleased: \n\n"
+        else:
+            date_string = datetime.date.today().strftime("%d %b %Y")
+            stub = f"## Version:{self.next_version} -- {date_string}\n\n"
 
-        if self.edit_changelog:
+        if changelog_update:
             terminal_advice = util.yellow(
                 "Here are some recent commit message for reference:\n"
             )
             terminal_advice += "-" * 30 + "\n"
-
             commits = util.get_recent_commits(self.repo)
- 
-            commit_messages = ([f"* {c.summary} [{c.hexsha[:7]}]" for c in commits])
-            terminal_advice += "\n".join(commit_messages) or ""
-            terminal_advice += "\n" + ("-" * 30) + "\n"
-
-            sections = [
-                "Added",
-                "Changed",
-                "Deprecated",
-                "Removed",
-                "Fixed",
-                "Security",
-            ]
-            terminal_advice += util.yellow(
-                "You may want to use these headngs to categorize your changelog entries:\n"
-            )
-            terminal_advice += "".join([f"### {s}\n" for s in sections])
-            terminal_advice += "-" * 30 + "\n\n"
-            print(terminal_advice)
-
-            if self.bumper.next_version or self.changelog_needs_unreleased_stub():
-                self.changelog_addition = stub
+            commit_messages = [f"* {c.summary}" for c in commits]
+            terminal_advice += "\n".join(commit_messages)
+            terminal_advice += "\n"
 
-    def resolve_changelog(self):
-        """Help the user to get the changelog file up-to-date."""
-        with open(self.changelog_filename, "r", encoding="utf-8") as clog:
-            content = clog.read() or "--"
+            print(terminal_advice)
 
-        content = self.changelog_addition + "\n\n" + content
+            if stub:
+                with open(self.changelog_filename, "r", encoding="utf-8") as clog:
+                    content = clog.read() or "--"
 
-        with open(self.changelog_filename, "w", encoding="utf-8") as clog:
-            clog.write(content)
+                content = stub + "\n\n" + content
 
-        print("Resolve CHANGELOG:")
+                with open(self.changelog_filename, "w", encoding="utf-8") as clog:
+                    clog.write(content)
 
-        input(
-            util.green(
-                "Please EDIT and SAVE your CHANGELOG (There's no need to commit), then press enter to continue."
+            q.wait(
+                "Please EDIT and SAVE your CHANGELOG now. (There's no need to commit)"
             )
-        )
 
     def changelog_needs_unreleased_stub(self):
         """Return True if the changelog needs an unreleased stub."""
         with open(self.changelog_filename, "r", encoding="utf-8") as f:
             datafile = f.readlines()
 
         for line in datafile:
             if line.startswith("## Unreleased"):
                 return False
             elif line.startswith("## Version"):
                 return True
         return True
 
+    def write_version(self):
+        """Write the new version number to the appropriate file."""
+        with open(self.version_filename, "w", encoding="utf-8") as vfn:
+            vfn.write(self.next_version)
+
+        # PRIVATE
 
+    def ask_push(self, tag):
+        """Ask the user if he wants to push the branch and tag."""
+        do_push = q.yes_no(
+            f"Do you want me to push the current branch and tag? ({self.branch_name}/{tag.name})"
+        )
+
+        origin = self.repo.remote("origin")
+        if do_push:
+            origin.push(self.branch)
+            origin.push(tag)
+            print("Pushed branch and tag.\n")
+        else:
+            print(
+                util.yellow(
+                    "No worries. Use the following command to push later. Bye\n"
+                )
+            )
+            print(util.green(f"git push --atomic origin {self.branch_name} {tag.name}"))
+
+    def add_tag(self):
+        """Add a tag to the repo."""
+        if self.release_scope == RELEASE_SCOPE_BETA:
+            label = "Pre-release"
+        elif self.release_scope == RELEASE_SCOPE_CANDIDATE:
+            label = "Release candidate"
+        else:
+            label = "Release"
+
+        tag = self.repo.create_tag(
+            self.next_version, message=f"{label}: {self.next_version}"
+        )
+        print(f"Created tag: {tag.name}")
+        return tag
+
+    def commit_version_changelog(self):
+        """Commit the version and changelog files."""
+
+        if self.repo.is_dirty():
+            self.repo.index.add([self.changelog_filename, self.version_filename])
+            self.repo.index.commit(
+                f"Update changelog and sets version to {self.next_version}"
+            )
+            print("Committed Version and Changelog\n")
 
     def check_pre_push_hook(self):
         """Check if there is a legacy pre-push hook and delete it."""
         hook_detection_line = "skulk.run_pre_push_checks()"
         delete_hook = False
-        if os.path.exists( self.hook_filename):
-            with open( self.hook_filename, "r", encoding="utf-8") as f:
+        if os.path.exists(self.hook_filename):
+            with open(self.hook_filename, "r", encoding="utf-8") as f:
                 for line in f:
                     if line.strip() == hook_detection_line:
                         delete_hook = True
         if delete_hook:
             print(f"Found legacy pre-push hook '{self.hook_filename}' - Deleting ...")
             try:
-                os.unlink( self.hook_filename)
+                os.unlink(self.hook_filename)
             except IOError as ex:
                 print(f"Error deleting '{self.hook_filename}': {ex}")
-                util.enter_to_continue_or_exit("Please delete it manually, then press enter")
+                util.enter_to_continue_or_exit(
+                    "Please delete it manually, then press enter"
+                )
+
+
 def main():
     """Run the wizard."""
     wizard = Skulk()
     wizard.run()
 
 
 if __name__ == "__main__":
```

## skulk/util.py

```diff
@@ -1,14 +1,16 @@
 import os
 import sys
 from git import InvalidGitRepositoryError, Repo
 
+from git import Repo
 
 MOCKED = True
 PROD_PYPI_INDEX = "https://pypi.org/simple/"
+TEST_PYPI_INDEX = "https://test.pypi.org/simple/"
 
 
 def yellow(rhs):
     """Return the rhs in red."""
     return f"\033[93m{rhs}\033[0m"
 
 
@@ -17,111 +19,124 @@
     return f"\033[92m{rhs}\033[0m"
 
 
 def red(rhs):
     """Return the rhs in red."""
     return f"\033[91m{rhs}\033[0m"
 
+
+def blue(rhs):
+    """Return the rhs in blue."""
+    return f"\033[94m{rhs}\033[0m"
+
+
 def magenta(rhs):
     """Return the rhs in magenta."""
     return f"\033[95m{rhs}\033[0m"
 
 
-def yes_no(question, *args):
-    """Ask a yes/no question and return True or False."""
-    options = args or ["No", "Yes"]
-
-    print(question)
-    for i, opt in enumerate(options):
-        print(f"{i}: {opt}")
-    while True:
-        inp = int(input(green("Enter a number: ")))
-        if inp in [0, 1]:
-            return [False, True][inp]
-        else:
-            print("You must choose 0 for {}, or 1 for {}..".format(*options))
+def default_color(rhs):
+    """Return the rhs in magenta."""
+    return rhs
+
 
 def get_repo():
     """Return the Repository object.
 
     Exit if not in a workable state.
     """
     try:
         repo = Repo(".")
     except InvalidGitRepositoryError:
         sys.stderr.write("Not a git repo. Can't continue.\n")
         sys.exit(1)
     if not MOCKED:
         if repo.is_dirty():
-            sys.stderr.write( red("Dirty repo. Can't continue. Commit or stash changes and try again.\n"))
+            sys.stderr.write(
+                red(
+                    "Dirty repo. Can't continue. Commit or stash changes and try again.\n"
+                )
+            )
             sys.exit(1)
     return repo
 
+
 def nonblank_lines(fileobject):
     """Generator to help search a file."""
     for line in fileobject:
         line = line.rstrip()
         if line:
             yield line
 
+
 def first_nonblank_line(filename):
     """Use a generator to return the first non blank line, or None."""
     try:
-        with open(filename, 'r', encoding='utf-8') as f:
+        with open(filename, "r", encoding="utf-8") as f:
             gen = nonblank_lines(f)
             return next(gen, None)
     except FileNotFoundError:
         print("The specified file was not found.")
         return None
     except PermissionError:
         print("You don't have permission to access this file.")
         return None
 
 
-
 def get_pip_name(repo):
     """
     Return the pip name, which may be different than the repo name.
 
     If the pip name is different, it should be the first line of the MANIFEST
     file as a comment.
     """
     manifest_file = os.path.join(repo.working_dir, "MANIFEST.in")
     base_name = os.path.basename(repo.working_dir)
     try:
         first_line = first_nonblank_line(manifest_file)
         if first_line[0] == "#":
             return first_line.split(" ")[1]
-    except IndexError: 
+    except IndexError:
         pass
     return base_name
-    
+
 
 def get_recent_commits(repo):
     """Get commits frm here back to the last tag on the master branch."""
     branch = repo.active_branch
-    master_shas = set(
-        [c.hexsha for c in repo.iter_commits(rev=repo.branches.master)]
-    )
+    try:
+        master_shas = set(
+            [c.hexsha for c in repo.iter_commits(rev=repo.branches.master)]
+        )
+    except AttributeError:
+        master_shas = set()
+
     tag_shas = [t.commit.hexsha for t in reversed(repo.tags)]
-    
     master_tag_sha = None
-    for sha in tag_shas:
-        if sha in master_shas:
-            master_tag_sha = sha
-            break
+    if master_shas == set():
+        for sha in tag_shas:
+            if sha in master_shas:
+                master_tag_sha = sha
+                break
     result = []
     for c in repo.iter_commits(rev=branch):
         result.append(c)
         if c.hexsha == master_tag_sha:
             break
     return result
 
-def enter_to_continue_or_exit(cont_message):
-    cont = input(
-        green(
-            "f{cont_message}. Type 'exit' to exit."
-        )
-    )
-    if cont.lower() == "exit":
-        sys.stderr.write("Exited.\n")
-        sys.exit(0)
+
+def print_truncated_list(
+    items, header, max_len=3, header_color=magenta, item_color=default_color
+):
+    """Return a truncated list of items."""
+    if not items:
+        return
+    lines = [header_color(header)]
+
+    if len(items) < max_len:
+        lines += [item_color(i) for i in items]
+    else:
+        lines += [item_color(i) for i in items[:max_len]]
+        lines.append(item_color("...and {} more.".format(len(items) - max_len)))
+
+    print("\n\t".join(lines))
```

## Comparing `skulk-2.0.3.dist-info/METADATA` & `skulk-2.1.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.0.3
+Version: 2.1.0
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Requires-Dist: GitPython (<4.0.0,>=3.1.31)
 Requires-Dist: semver (<4.0.0,>=3.0.0)
 Requires-Dist: twine (>=4.0.2)
 Requires-Dist: future (>=0.18.3)
 
 Streamline release for Conductor client tools and others
-
-
```

