# Comparing `tmp/all_repos-1.8.0.tar.gz` & `tmp/all_repos-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/all_repos-1.8.0.tar", last modified: Tue Jan 15 22:03:56 2019, max compression
+gzip compressed data, was "dist/all_repos-1.9.0.tar", last modified: Thu Jan 17 01:46:45 2019, max compression
```

## Comparing `all_repos-1.8.0.tar` & `all_repos-1.9.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 asottile   (501) wheel        (0)        0 2019-01-15 22:03:56.000000 all_repos-1.8.0/
--rw-r--r--   0 asottile   (501) wheel        (0)      429 2019-01-15 22:03:56.000000 all_repos-1.8.0/PKG-INFO
--rw-r--r--   0 asottile   (501) wheel        (0)    14688 2019-01-15 17:49:53.000000 all_repos-1.8.0/README.md
-drwxr-xr-x   0 asottile   (501) wheel        (0)        0 2019-01-15 22:03:56.000000 all_repos-1.8.0/all_repos/
--rw-r--r--   0 asottile   (501) wheel        (0)        0 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/__init__.py
-drwxr-xr-x   0 asottile   (501) wheel        (0)        0 2019-01-15 22:03:56.000000 all_repos-1.8.0/all_repos/autofix/
--rw-r--r--   0 asottile   (501) wheel        (0)        0 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/autofix/__init__.py
--rw-r--r--   0 asottile   (501) wheel        (0)     3025 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/autofix/pre_commit_autopep8_migrate.py
--rw-r--r--   0 asottile   (501) wheel        (0)     2579 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/autofix/pre_commit_autoupdate.py
--rw-r--r--   0 asottile   (501) wheel        (0)     1600 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/autofix/pre_commit_cache_dir.py
--rw-r--r--   0 asottile   (501) wheel        (0)     1821 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/autofix/pre_commit_migrate_config.py
--rw-r--r--   0 asottile   (501) wheel        (0)     8320 2019-01-15 21:32:23.000000 all_repos-1.8.0/all_repos/autofix_lib.py
--rw-r--r--   0 asottile   (501) wheel        (0)     1861 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/cli.py
--rw-r--r--   0 asottile   (501) wheel        (0)     4214 2019-01-15 22:03:27.000000 all_repos-1.8.0/all_repos/clone.py
--rw-r--r--   0 asottile   (501) wheel        (0)      451 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/color.py
--rw-r--r--   0 asottile   (501) wheel        (0)     2491 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/complete.py
--rw-r--r--   0 asottile   (501) wheel        (0)     1976 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/config.py
--rw-r--r--   0 asottile   (501) wheel        (0)     2645 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/find_files.py
--rw-r--r--   0 asottile   (501) wheel        (0)      169 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/git.py
--rw-r--r--   0 asottile   (501) wheel        (0)     2097 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/github_api.py
--rw-r--r--   0 asottile   (501) wheel        (0)     2904 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/grep.py
--rw-r--r--   0 asottile   (501) wheel        (0)      583 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/list_repos.py
--rw-r--r--   0 asottile   (501) wheel        (0)     1289 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/manual.py
--rw-r--r--   0 asottile   (501) wheel        (0)     1331 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/mapper.py
-drwxr-xr-x   0 asottile   (501) wheel        (0)        0 2019-01-15 22:03:56.000000 all_repos-1.8.0/all_repos/push/
--rw-r--r--   0 asottile   (501) wheel        (0)        0 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/push/__init__.py
--rw-r--r--   0 asottile   (501) wheel        (0)     1558 2019-01-15 21:32:23.000000 all_repos-1.8.0/all_repos/push/github_pull_request.py
--rw-r--r--   0 asottile   (501) wheel        (0)      452 2019-01-15 21:32:23.000000 all_repos-1.8.0/all_repos/push/merge_to_master.py
--rw-r--r--   0 asottile   (501) wheel        (0)     3202 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/sed.py
-drwxr-xr-x   0 asottile   (501) wheel        (0)        0 2019-01-15 22:03:56.000000 all_repos-1.8.0/all_repos/source/
--rw-r--r--   0 asottile   (501) wheel        (0)        0 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/source/__init__.py
--rw-r--r--   0 asottile   (501) wheel        (0)      615 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/source/github.py
--rw-r--r--   0 asottile   (501) wheel        (0)      625 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/source/github_org.py
--rw-r--r--   0 asottile   (501) wheel        (0)     1063 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/source/gitolite.py
--rw-r--r--   0 asottile   (501) wheel        (0)      237 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/source/json_file.py
--rw-r--r--   0 asottile   (501) wheel        (0)      148 2019-01-15 19:13:32.000000 all_repos-1.8.0/all_repos/util.py
-drwxr-xr-x   0 asottile   (501) wheel        (0)        0 2019-01-15 22:03:56.000000 all_repos-1.8.0/all_repos.egg-info/
--rw-r--r--   0 asottile   (501) wheel        (0)      429 2019-01-15 22:03:55.000000 all_repos-1.8.0/all_repos.egg-info/PKG-INFO
--rw-r--r--   0 asottile   (501) wheel        (0)     1010 2019-01-15 22:03:56.000000 all_repos-1.8.0/all_repos.egg-info/SOURCES.txt
--rw-r--r--   0 asottile   (501) wheel        (0)        1 2019-01-15 22:03:55.000000 all_repos-1.8.0/all_repos.egg-info/dependency_links.txt
--rw-r--r--   0 asottile   (501) wheel        (0)      314 2019-01-15 22:03:55.000000 all_repos-1.8.0/all_repos.egg-info/entry_points.txt
--rw-r--r--   0 asottile   (501) wheel        (0)        9 2019-01-15 22:03:55.000000 all_repos-1.8.0/all_repos.egg-info/requires.txt
--rw-r--r--   0 asottile   (501) wheel        (0)       10 2019-01-15 22:03:55.000000 all_repos-1.8.0/all_repos.egg-info/top_level.txt
--rw-r--r--   0 asottile   (501) wheel        (0)       70 2019-01-15 22:03:56.000000 all_repos-1.8.0/setup.cfg
--rw-r--r--   0 asottile   (501) wheel        (0)     1030 2019-01-15 22:03:42.000000 all_repos-1.8.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:46:45.000000 all_repos-1.9.0/
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4214 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/clone.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2491 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/complete.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      169 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/git.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos/autofix/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/autofix/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1600 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/autofix/pre_commit_cache_dir.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3025 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/autofix/pre_commit_autopep8_migrate.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2579 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/autofix/pre_commit_autoupdate.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1821 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/autofix/pre_commit_migrate_config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2904 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/grep.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      148 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/util.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3202 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/sed.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos/source/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      615 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/source/github.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/source/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1063 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/source/gitolite.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      625 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/source/github_org.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      237 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/source/json_file.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2097 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/github_api.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1289 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/manual.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos/push/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      536 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/push/merge_to_master.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/push/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1558 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/push/github_pull_request.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      144 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/push/readonly.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8320 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/autofix_lib.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      583 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/list_repos.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2645 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/find_files.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1861 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/cli.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1976 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1331 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/mapper.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      451 2019-01-17 01:45:33.000000 all_repos-1.9.0/all_repos/color.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    14902 2019-01-17 01:44:38.000000 all_repos-1.9.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1037 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      314 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      429 2019-01-17 01:46:45.000000 all_repos-1.9.0/all_repos.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1030 2019-01-17 01:46:31.000000 all_repos-1.9.0/setup.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       70 2019-01-17 01:46:45.000000 all_repos-1.9.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      429 2019-01-17 01:46:45.000000 all_repos-1.9.0/PKG-INFO
```

### Comparing `all_repos-1.8.0/README.md` & `all_repos-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -333,17 +333,18 @@
 ```bash
 git checkout master
 git pull
 git merge --no-ff $BRANCH
 git push origin HEAD
 ```
 
-#### `push_settings`
+#### Optional `push_settings`
 
-There are no configurable settings for `merge_to_master`.
+- `fast_forward` (default: `false`): if `true`, perform a fast-forward
+    merge (`--ff-only`). If `false`, create a merge commit (`--no-ff`).
 
 ### `all_repos.push.github_pull_request`
 
 Pushes the branch to `origin` and then creates a github pull request for the
 branch.
 
 #### Required `push_settings`
@@ -358,14 +359,22 @@
 #### Optional `push_settings`
 
 - `fork` (default: `false`): (if applicable) a fork will be created and pushed
   to instead of the upstream repository.  The pull request will then be made
   to the upstream repository.
 
 
+### `all_repos.push.readonly`
+
+Does nothing.
+
+#### `push_settings`
+
+There are no configurable settings for `readonly`.
+
 ## Writing your own push module
 
 First create a module.  This module must have the following api:
 
 ### A `Settings` class
 
 This class will receive keyword arguments for all values in the `push_settings`
```

### Comparing `all_repos-1.8.0/all_repos/autofix/pre_commit_autopep8_migrate.py` & `all_repos-1.9.0/all_repos/autofix/pre_commit_autopep8_migrate.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/autofix/pre_commit_autoupdate.py` & `all_repos-1.9.0/all_repos/autofix/pre_commit_autoupdate.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/autofix/pre_commit_cache_dir.py` & `all_repos-1.9.0/all_repos/autofix/pre_commit_cache_dir.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/autofix/pre_commit_migrate_config.py` & `all_repos-1.9.0/all_repos/autofix/pre_commit_migrate_config.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/autofix_lib.py` & `all_repos-1.9.0/all_repos/autofix_lib.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/cli.py` & `all_repos-1.9.0/all_repos/cli.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/clone.py` & `all_repos-1.9.0/all_repos/clone.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/complete.py` & `all_repos-1.9.0/all_repos/complete.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/config.py` & `all_repos-1.9.0/all_repos/config.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/find_files.py` & `all_repos-1.9.0/all_repos/find_files.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/github_api.py` & `all_repos-1.9.0/all_repos/github_api.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/grep.py` & `all_repos-1.9.0/all_repos/grep.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/list_repos.py` & `all_repos-1.9.0/all_repos/list_repos.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/manual.py` & `all_repos-1.9.0/all_repos/manual.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/mapper.py` & `all_repos-1.9.0/all_repos/mapper.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/push/github_pull_request.py` & `all_repos-1.9.0/all_repos/push/github_pull_request.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/sed.py` & `all_repos-1.9.0/all_repos/sed.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/source/github.py` & `all_repos-1.9.0/all_repos/source/github.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/source/github_org.py` & `all_repos-1.9.0/all_repos/source/github_org.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos/source/gitolite.py` & `all_repos-1.9.0/all_repos/source/gitolite.py`

 * *Files identical despite different names*

### Comparing `all_repos-1.8.0/all_repos.egg-info/SOURCES.txt` & `all_repos-1.9.0/all_repos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,13 @@
 all_repos/autofix/pre_commit_autopep8_migrate.py
 all_repos/autofix/pre_commit_autoupdate.py
 all_repos/autofix/pre_commit_cache_dir.py
 all_repos/autofix/pre_commit_migrate_config.py
 all_repos/push/__init__.py
 all_repos/push/github_pull_request.py
 all_repos/push/merge_to_master.py
+all_repos/push/readonly.py
 all_repos/source/__init__.py
 all_repos/source/github.py
 all_repos/source/github_org.py
 all_repos/source/gitolite.py
 all_repos/source/json_file.py
```

### Comparing `all_repos-1.8.0/setup.py` & `all_repos-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='all_repos',
     description='Clone all your repositories and apply sweeping changes.',
     url='https://github.com/asottile/all-repos',
-    version='1.8.0',
+    version='1.9.0',
     author='Anthony Sottile',
     author_email='asottile@umich.edu',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
     ],
```

