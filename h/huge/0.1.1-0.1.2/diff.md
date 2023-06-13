# Comparing `tmp/huge-0.1.1.tar.gz` & `tmp/huge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huge-0.1.1.tar", last modified: Thu Jun 18 12:28:22 2020, max compression
+gzip compressed data, was "huge-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `huge-0.1.1.tar` & `huge-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      772 2020-06-18 12:28:12.238033 huge-0.1.1/.github/workflows/package.yml
--rw-r--r--   0        0        0       13 2020-06-18 12:28:12.238033 huge-0.1.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-06-18 12:28:12.238033 huge-0.1.1/LICENSE
--rw-r--r--   0        0        0     3336 2020-06-18 12:28:12.238033 huge-0.1.1/README.md
--rw-r--r--   0        0        0     1942 2020-06-18 12:28:12.238033 huge-0.1.1/huge.py
--rw-r--r--   0        0        0      428 2020-06-18 12:28:12.238033 huge-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       11 2020-06-18 12:28:12.238033 huge-0.1.1/requirements.txt
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 huge-0.1.1/setup.py
--rw-r--r--   0        0        0      188 1970-01-01 00:00:00.000000 huge-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      775 2023-06-13 18:44:24.521849 huge-0.1.2/.github/workflows/package.yml
+-rw-r--r--   0        0        0       13 2023-06-13 18:44:24.521849 huge-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1069 2023-06-13 18:44:24.521849 huge-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3334 2023-06-13 18:44:24.521849 huge-0.1.2/README.md
+-rw-r--r--   0        0        0     2008 2023-06-13 18:44:24.521849 huge-0.1.2/huge.py
+-rw-r--r--   0        0        0      434 2023-06-13 18:44:24.521849 huge-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-13 18:44:24.521849 huge-0.1.2/requirements.txt
+-rw-r--r--   0        0        0     3708 1970-01-01 00:00:00.000000 huge-0.1.2/PKG-INFO
```

### Comparing `huge-0.1.1/.github/workflows/package.yml` & `huge-0.1.2/.github/workflows/package.yml`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: [3.6]
+        python-version: ["3.10"]
         os: [ubuntu-latest]
 
     steps:
     - name: Switch branch
       uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
```

### Comparing `huge-0.1.1/LICENSE` & `huge-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `huge-0.1.1/README.md` & `huge-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ```
 $ huge --help
 
 Usage: huge [OPTIONS]
 
 Options:
-  --branch TEXT          Which branch to scan.  [default: master]
+  --branch TEXT          Which branch to scan.  [default: main]
   --num-entries INTEGER  How many top entries to show.  [default: 20]
   --cutoff INTEGER       Cutoff (bytes) below which to ignore entries.
                          [default: 1000000]
 
   --help                 Show this message and exit.
 ```
```

### Comparing `huge-0.1.1/huge.py` & `huge-0.1.2/huge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Find huge additions in Git history."""
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 
 import subprocess
 import itertools
 from tqdm import tqdm
 import click
 from tabulate import tabulate
@@ -24,15 +24,15 @@
         .decode("utf8")
         .splitlines()
     )
 
 
 @click.command()
 @click.option(
-    "--branch", default="master", show_default=True, help="Which branch to scan."
+    "--branch", default="main", show_default=True, help="Which branch to scan."
 )
 @click.option(
     "--num-entries",
     default=20,
     type=int,
     show_default=True,
     help="How many top entries to show.",
@@ -52,29 +52,34 @@
     for commit in tqdm(commits):
         entries = get_file_entries(commit)
         for line in entries:
             s = line.split()
             size = s[3]
             if not "-" in size:
                 if int(size) > cutoff:
-                    path = ' '.join(s[4:])  # this is done for files with spaces
+                    path = " ".join(s[4:])  # this is done for files with spaces
                     if not (size, path) in additions_dict:
                         additions_dict[(size, path)] = commit
 
     additions = []
     for k, v in additions_dict.items():
         size_mb = float(k[0]) / 1000000.0
         additions.append((size_mb, k[1], v))
 
     additions = reversed(sorted(additions))
 
     print("\n")
 
     rows = list(itertools.islice(additions, num_entries))
     if len(rows) > 0:
-        print(tabulate(rows, headers=["size (MB)", "path", "commit"],))
+        print(
+            tabulate(
+                rows,
+                headers=["size (MB)", "path", "commit"],
+            )
+        )
     else:
         print("no additions found")
 
 
 if __name__ == "__main__":
     main()
```

