# Comparing `tmp/sqlalchemy-dlock-0.2b3.post4.tar.gz` & `tmp/sqlalchemy-dlock-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-dlock-0.2b3.post4.tar", last modified: Wed Mar 23 07:47:14 2022, max compression
+gzip compressed data, was "sqlalchemy-dlock-0.3.tar", last modified: Tue Jun 13 08:15:10 2023, max compression
```

## Comparing `sqlalchemy-dlock-0.2b3.post4.tar` & `sqlalchemy-dlock-0.3.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:14.530792 sqlalchemy-dlock-0.2b3.post4/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7164 2022-03-23 07:47:14.530792 sqlalchemy-dlock-0.2b3.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:14.526792 sqlalchemy-dlock-0.2b3.post4/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/scripts/run-test.sh
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/scripts/wait-for-mysql.sh
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/scripts/wait-for-postgres.sh
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-03-23 07:47:14.530792 sqlalchemy-dlock-0.2b3.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:14.522792 sqlalchemy-dlock-0.2b3.post4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:14.526792 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:14.526792 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:14.530792 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/impl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/impl/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     4852 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/impl/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:14.530792 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/impl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4570 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/impl/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     6534 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/impl/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (121)     6091 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-03-23 07:47:03.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-03-23 07:47:13.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 07:47:14.526792 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7164 2022-03-23 07:47:14.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-03-23 07:47:14.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 07:47:14.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-03-23 07:47:14.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-03-23 07:47:14.000000 sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.073943 sqlalchemy-dlock-0.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/scripts/run-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/scripts/wait-for-mysql.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/scripts/wait-for-postgres.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.073943 sqlalchemy-dlock-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 08:15:09.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/top_level.txt
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/CHANGELOG.md` & `sqlalchemy-dlock-0.3/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,38 @@
 # CHANGELOG
 
+## v0.3
+
+Date: 2023-06-13
+
+- Remove:
+  - Python 3.6 support
+
+- Tests:
+  - New docker compose based tests, from python 3.7 to 3.11, both SQLAlchemy 1.x and 2.x
+
+- Docs:
+  - Update to newer Sphinx docs
+
+- Build:
+  - Move all project meta to pyproject.toml, remove setup.cfg and setup.py
+
+## v0.2.1
+
+Date: 2023-02-25
+
+- New:
+  - support SQLAlchemy 2.0
+
+## v0.2
+
+Date: 2021-03-23
+
+First v0.2.x version released.
+
 ## v0.2b2/b3
 
 Date: 2021-03-23
 
 - Add:
   - More unit tests
   - Optimized CI
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/LICENSE` & `sqlalchemy-dlock-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.2b3.post4/PKG-INFO` & `sqlalchemy-dlock-0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,74 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-dlock
-Version: 0.2b3.post4
+Version: 0.3
 Summary: A distributed lock implementation based on SQLAlchemy
-Home-page: https://github.com/tanbro/sqlalchemy-dlock
-Author: liu xue yan
-Author-email: liu_xue_yan@foxmail.com
+Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD 3-Clause License
+        
+        Copyright (c) 2020, liu xue yan
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
+Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
 Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 License-File: LICENSE
+License-File: AUTHORS.md
 
 # SQLAlchemy-DLock
 
-[![GitHub](https://img.shields.io/github/license/tanbro/sqlalchemy-dlock)](https://github.com/tanbro/sqlalchemy-dlock)
-[![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/tanbro/sqlalchemy-dlock)](https://github.com/tanbro/sqlalchemy-dlock/tags)
 [![Python package](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml/badge.svg)](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
-[![PyPI - Status](https://img.shields.io/pypi/status/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
-[![PyPI - License](https://img.shields.io/pypi/l/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
 [![Documentation Status](https://readthedocs.org/projects/sqlalchemy-dlock/badge/?version=latest)](https://sqlalchemy-dlock.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/tanbro/sqlalchemy-dlock/branch/main/graph/badge.svg?token=GfcDT1ckFX)](https://codecov.io/gh/tanbro/sqlalchemy-dlock)
 
 Distributed lock based on Database and [SQLAlchemy][].
 
 It currently supports below locks:
 
-- `MySQL` - named lock: <https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html>
-- `PostgreSQL` - advisory lock: <https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS>
-
-> ❗ **Note**:
->
-> The project is not stable enough and **DO NOT** use it in production.
+ Database  |                                             Lock
+---------- | ---------------------------------------------------------------------------------------------
+MySQL      | [named lock](https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html)
+PostgreSQL | [advisory lock](https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS)
 
 ## Usages
 
-- Work with [SQLAlchemy][]'s `Connection` object:
+- Work with [SQLAlchemy][] `Connection`:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
@@ -66,15 +86,15 @@
   assert lock.acquired
 
   # un-lock
   lock.release()
   assert not lock.acquired
   ```
 
-- Use in `with` statement
+- `with` statement
 
   ```python
   from contextlib import closing
 
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
@@ -99,22 +119,15 @@
           lock2.acquire()
           assert lock2.acquired
 
       # Auto un-locked
       assert not lock2.acquired
   ```
 
-- Work with [SQLAlchemy][]'s `ORM` session:
-
-  > ❗ **Note**:
-  >
-  > According to <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>:
-  >
-  > - The asyncio extension as of SQLAlchemy 1.4.3 can now be considered to be **beta level** software.
-  > - The asyncio extension requires at least Python version 3.6
+- Work with [SQLAlchemy][] `ORM` session:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy.orm import sessionmaker
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
@@ -124,15 +137,20 @@
 
   with Session() as session:
     with create_sadlock(session, key) as lock:
         assert lock.acquired
     assert not lock.acquired
   ```
 
-- Work asynchronously
+- Asynchronous I/O Support
+
+  > ℹ️ **info**:
+  >
+  > - [SQLAlchemy][] `1.x`: <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>
+  > - [SQLAlchemy][] `2.x`: <https://docs.sqlalchemy.org/20/orm/extensions/asyncio.html>
 
   ```python
   from sqlalchemy.ext.asyncio import create_async_engine
   from sqlalchemy_dlock.asyncio import create_async_sadlock
 
   key = 'user/001'
 
@@ -145,107 +163,68 @@
           assert not lock.locked
           await lock.acquire()
       assert not lock.locked
   ```
 
 ## Tests
 
-Just `up` the docker-compose in `tests` directory:
-
-```bash
-(cd tests; docker-compose up --abort-on-container-exit --exit-code-from pytest; docker-compose down)
-```
-
-[SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
-
-# CHANGELOG
-
-## v0.2b2/b3
-
-Date: 2021-03-23
-
-- Add:
-  - More unit tests
-  - Optimized CI
-
-## v0.2b1
-
-Date: 2021-03-16
+Following [SQLAlchemy][] engines are tested:
 
-- Add:
+- MySQL:
 
-  - New unit tests
-  - CI by github workflows
+  - mysqlclient
+  - PyMySQL
+  - aiomysql ([asyncio][])
 
-## v0.2a3
+- Postgres:
 
-Date: 2021-03-14
+  - psycopg2
+  - asyncpg ([asyncio][])
 
-- Change:
+You can run unit-tests:
 
-  - Drop Python 3.5 support.
-  - Remove SQLAlchemy version requires earlier than 1.4 in setup, it's not supported actually.
-  - Adjust PostgreSQL lock's constructor arguments order
+- directly:
 
-- Add:
+  1. Install the project (A virtual environment ([venv][]) is strongly advised):
 
-  - More test cases, and add test/deploy workflow in github actions.
-  - Add docker-compose test scripts
+     ```bash
+     pip install -e .
+     ```
 
-## v0.2a2
+  1. Start up your mysql and postgresql
 
-Date: 2021-03-09
+  1. Set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
+     Multiple connections separated by space.
+     The test cases load environment variables in `tests/.env`.
 
-- Change:
+     eg (and also the defaults):
 
-  - Rename a lot of function/class:
+     ```ini
+     TEST_URLS=mysql://test:test@localhost/test postgresql://postgres:test@localhost/
+     TEST_ASYNC_URLS=mysql+aiomysql://test:test@localhost/test postgresql+asyncpg://postgres:test@localhost/
+     ```
 
-    - `sadlock` -> `create_sadlock`
-    - `asyncio.sadlock` -> `asyncio.create_async_sadlock`
-  
-    and some other ...
+  1. run unit-test
 
-## v0.2a1
+     ```bash
+     python -m unittest
+     ```
 
-Date: 2021-03-08
+- in docker-compose:
 
-- New:
+  1. build the project
 
-  - Asynchronous IO Support by:
+     ```bash
+     python -m pip install build && python -m build -w
+     ```
 
-    - [aiomysql](https://github.com/aio-libs/aiomysql) for MySQL
-
-      Connection URL is like: `"mysql+aiomysql://user:password@host:3306/schema?charset=utf8mb4"`
-
-    - [asyncpg](https://github.com/MagicStack/asyncpg) for PostgreSQL
-
-      Connection URL is like: `"postgresql+asyncpg://user:password@host:5432/db"`
-
-    Read <https://docs.sqlalchemy.org/en/14/orm/extensions/asyncio.html> for details
-
-## v0.1.2
-
-Date: 2021-01-26
-
-Still an early version, not for production.
-
-- Changes:
-  - Arguments and it's default value of `acquire` now similar to stdlib's `multiprossing.Lock`, instead of `Threading.Lock`
-  - MySQL lock now accepts float-point value as `timeout`
-- Adds
-  - Several new test cases
-- Other
-  - Many other small adjustment
-
-## v0.1.1
-
-- A very early version, maybe not stable enough.
-- Replace black2b with crc64-iso in PostgreSQL key convert function
-- Only named arguments as extra parameters allowed in Lock's implementation class
-
-# AUTHORS
-
-* Liu Xue Yan (<liu_xue_yan@foxmail.com>)
-
-  [![liu_xue_yan@foxmail.com](https://www.gravatar.com/avatar/049d2fae1fd2df6439e87d1383d0276b)](mailto:liu_xue_yan@foxmail.com)
+  1. run unit-test
 
+     ```bash
+     cd tests
+     docker compose up --abort-on-container-exit
+     docker compose rm -fsv
+     ```
 
+[SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
+[asyncio]: https://docs.python.org/library/asyncio.html "asyncio is a library to write concurrent code using the async/await syntax."
+[venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/functions.py` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/functions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from importlib import import_module
 
 from sqlalchemy.ext.asyncio import AsyncConnection
 
 from ..utils import safe_name
 from .types import BaseAsyncSadLock, TAsyncConnectionOrSession
 
-__all__ = ['create_async_sadlock']
+__all__ = ["create_async_sadlock"]
 
 
-def create_async_sadlock(
-        connection_or_engine: TAsyncConnectionOrSession,
-        key,
-        *args, **kwargs
-) -> BaseAsyncSadLock:
+def create_async_sadlock(connection_or_engine: TAsyncConnectionOrSession, key, *args, **kwargs) -> BaseAsyncSadLock:
     if isinstance(connection_or_engine, AsyncConnection):
         name = safe_name(connection_or_engine.sync_engine.engine.name)
     else:
         name = safe_name(connection_or_engine.get_bind().name)
     try:
-        mod = import_module('..impl.{}'.format(name), __name__)
+        mod = import_module("..impl.{}".format(name), __name__)
     except ImportError as exception:  # pragma: no cover
-        raise NotImplementedError('{}: {}'.format(name, exception))
-    lock_cls = getattr(mod, 'AsyncSadLock')
+        raise NotImplementedError("{}: {}".format(name, exception))
+    lock_cls = getattr(mod, "AsyncSadLock")
     return lock_cls(connection_or_engine, key, *args, **kwargs)
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/impl/mysql.py` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/mysql.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,63 +4,68 @@
 from sqlalchemy import text
 
 from ...exceptions import SqlAlchemyDLockDatabaseError
 from ..types import BaseAsyncSadLock, TAsyncConnectionOrSession
 
 MYSQL_LOCK_NAME_MAX_LENGTH = 64
 
-GET_LOCK = text(dedent('''
-SELECT GET_LOCK(:str, :timeout)
-''').strip())
-
-RELEASE_LOCK = text(dedent('''
-SELECT RELEASE_LOCK(:str)
-''').strip())
+GET_LOCK = text(
+    dedent(
+        """
+        SELECT GET_LOCK(:str, :timeout)
+        """
+    ).strip()
+)
+
+RELEASE_LOCK = text(
+    dedent(
+        """
+        SELECT RELEASE_LOCK(:str)
+        """
+    ).strip()
+)
 
 TConvertFunction = Callable[[Any], str]
 
 
 def default_convert(key: Union[bytearray, bytes, int, float]) -> str:
     if isinstance(key, (bytearray, bytes)):
         result = key.decode()
     elif isinstance(key, (int, float)):
         result = str(key)
     else:
-        raise TypeError('{}'.format(type(key)))
+        raise TypeError("{}".format(type(key)))
     return result
 
 
 class AsyncSadLock(BaseAsyncSadLock):
-    def __init__(self,
-                 connection_or_session: TAsyncConnectionOrSession,
-                 key,
-                 convert: Optional[TConvertFunction] = None,
-                 *args, **kwargs
-                 ):
+    def __init__(
+        self,
+        connection_or_session: TAsyncConnectionOrSession,
+        key,
+        convert: Optional[TConvertFunction] = None,
+        *args,
+        **kwargs,
+    ):
         if convert:
             key = convert(key)
         elif not isinstance(key, str):
             key = default_convert(key)
         if not isinstance(key, str):
-            raise TypeError(
-                'MySQL named lock requires the key given by string')
+            raise TypeError("MySQL named lock requires the key given by string")
         if len(key) > MYSQL_LOCK_NAME_MAX_LENGTH:
             raise ValueError(
-                'MySQL enforces a maximum length on lock names of {} characters.'.format(
-                    MYSQL_LOCK_NAME_MAX_LENGTH))
+                "MySQL enforces a maximum length on lock names of {} characters.".format(MYSQL_LOCK_NAME_MAX_LENGTH)
+            )
         #
         super().__init__(connection_or_session, key)
 
-    async def acquire(self,
-                      block: bool = True,
-                      timeout: Union[float, int, None] = None,
-                      *args, **kwargs
-                      ) -> bool:
+    async def acquire(self, block: bool = True, timeout: Union[float, int, None] = None, *args, **kwargs) -> bool:
         if self._acquired:
-            raise ValueError('invoked on a locked lock')
+            raise ValueError("invoked on a locked lock")
         if block:
             # None: set the timeout period to infinite.
             if timeout is None:
                 timeout = -1
             # negative value for `timeout` are equivalent to a `timeout` of zero
             elif timeout < 0:
                 timeout = 0
@@ -71,37 +76,34 @@
         ret_val = (await r.one())[0]
 
         if ret_val == 1:
             self._acquired = True
         elif ret_val == 0:
             pass  # 直到超时也没有成功锁定
         elif ret_val is None:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError(
-                'An error occurred while attempting to obtain the lock "{}"'.format(self._key))
+            raise SqlAlchemyDLockDatabaseError('An error occurred while attempting to obtain the lock "{}"'.format(self._key))
         else:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError(
-                'GET_LOCK("{}", {}) returns {}'.format(self._key, timeout, ret_val))
+            raise SqlAlchemyDLockDatabaseError('GET_LOCK("{}", {}) returns {}'.format(self._key, timeout, ret_val))
         return self._acquired
 
     async def release(self, *args, **kwargs):
         if not self._acquired:
-            raise ValueError('invoked on an unlocked lock')
+            raise ValueError("invoked on an unlocked lock")
         stmt = RELEASE_LOCK.params(str=self._key)
         r = await self.connection_or_session.stream(stmt)
         ret_val = (await r.one())[0]
         if ret_val == 1:
             self._acquired = False
         elif ret_val == 0:  # pragma: no cover
             self._acquired = False
             raise SqlAlchemyDLockDatabaseError(
-                'The named lock "{}" was not established by this thread, '
-                'and the lock is not released.'.format(self._key))
+                'The named lock "{}" was not established by this thread, ' "and the lock is not released.".format(self._key)
+            )
         elif ret_val is None:  # pragma: no cover
             self._acquired = False
             raise SqlAlchemyDLockDatabaseError(
                 'The named lock "{}" did not exist, '
-                'was never obtained by a call to GET_LOCK(), '
-                'or has previously been released.'.format(self._key)
+                "was never obtained by a call to GET_LOCK(), "
+                "or has previously been released.".format(self._key)
             )
         else:
-            raise SqlAlchemyDLockDatabaseError(
-                'RELEASE_LOCK("{}") returns {}'.format(self._key, ret_val))
+            raise SqlAlchemyDLockDatabaseError('RELEASE_LOCK("{}") returns {}'.format(self._key, ret_val))
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/impl/postgresql.py` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/postgresql.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,127 +9,166 @@
 from ...exceptions import SqlAlchemyDLockDatabaseError
 from ...utils import ensure_int64, to_int64_key
 from ..types import BaseAsyncSadLock, TAsyncConnectionOrSession
 
 SLEEP_INTERVAL_DEFAULT = 1
 
 STATEMENTS = {
-    'session': {
-        'lock': text(dedent('''
-            SELECT pg_advisory_lock(:key)
-            ''').strip()),
-        'trylock': text(dedent('''
-            SELECT pg_try_advisory_lock(:key)
-            ''').strip()),
-        'unlock': text(dedent('''
-            SELECT pg_advisory_unlock(:key)
-            ''').strip()),
+    "session": {
+        "lock": text(
+            dedent(
+                """
+                SELECT pg_advisory_lock(:key)
+                """
+            ).strip()
+        ),
+        "trylock": text(
+            dedent(
+                """
+                SELECT pg_try_advisory_lock(:key)
+                """
+            ).strip()
+        ),
+        "unlock": text(
+            dedent(
+                """
+                SELECT pg_advisory_unlock(:key)
+                """
+            ).strip()
+        ),
     },
-    'shared': {
-        'lock': text(dedent('''
-            SELECT pg_advisory_lock_shared(:key)
-            ''').strip()),
-        'trylock': text(dedent('''
-            SELECT pg_try_advisory_lock_shared(:key)
-            ''').strip()),
-        'unlock': text(dedent('''
-            SELECT pg_advisory_unlock_shared(:key)
-            ''').strip()),
+    "shared": {
+        "lock": text(
+            dedent(
+                """
+                SELECT pg_advisory_lock_shared(:key)
+                """
+            ).strip()
+        ),
+        "trylock": text(
+            dedent(
+                """
+                SELECT pg_try_advisory_lock_shared(:key)
+                """
+            ).strip()
+        ),
+        "unlock": text(
+            dedent(
+                """
+                SELECT pg_advisory_unlock_shared(:key)
+                """
+            ).strip()
+        ),
     },
-    'transaction': {
-        'lock': text(dedent('''
-            SELECT pg_advisory_xact_lock(:key)
-            ''').strip()),
-        'trylock': text(dedent('''
-            SELECT pg_try_advisory_xact_lock(:key)
-            ''').strip()),
-        'unlock': text(dedent('''
-            SELECT pg_advisory_xact_unlock(:key)
-            ''').strip()),
+    "transaction": {
+        "lock": text(
+            dedent(
+                """
+                SELECT pg_advisory_xact_lock(:key)
+                """
+            ).strip()
+        ),
+        "trylock": text(
+            dedent(
+                """
+                SELECT pg_try_advisory_xact_lock(:key)
+                """
+            ).strip()
+        ),
+        "unlock": text(
+            dedent(
+                """
+                SELECT pg_advisory_xact_unlock(:key)
+                """
+            ).strip()
+        ),
     },
 }
 
 
 TConvertFunction = Callable[[Any], int]
 
 
 class AsyncSadLock(BaseAsyncSadLock):
-    def __init__(self,
-                 connection_or_session: TAsyncConnectionOrSession,
-                 key,
-                 level: Optional[str] = None,
-                 interval: Union[float, int, None] = None,
-                 convert: Optional[TConvertFunction] = None,
-                 *args, **kwargs
-                 ):
+    def __init__(
+        self,
+        connection_or_session: TAsyncConnectionOrSession,
+        key,
+        level: Optional[str] = None,
+        interval: Union[float, int, None] = None,
+        convert: Optional[TConvertFunction] = None,
+        *args,
+        **kwargs,
+    ):
         if convert:
             key = ensure_int64(convert(key))
         elif isinstance(key, int):
             key = ensure_int64(key)
         else:
             key = to_int64_key(key)
         #
         self._interval = SLEEP_INTERVAL_DEFAULT if interval is None else interval
-        self._level = level or 'session'
+        self._level = level or "session"
         self._stmt_dict = STATEMENTS[self._level]
         #
         super().__init__(connection_or_session, key)
 
-    async def acquire(self,
-                      block: bool = True,
-                      timeout: Union[float, int, None] = None,
-                      interval: Union[float, int, None] = None,
-                      *args, **kwargs
-                      ) -> bool:
+    async def acquire(
+        self,
+        block: bool = True,
+        timeout: Union[float, int, None] = None,
+        interval: Union[float, int, None] = None,
+        *args,
+        **kwargs,
+    ) -> bool:
         if self._acquired:
-            raise ValueError('invoked on a locked lock')
+            raise ValueError("invoked on a locked lock")
         if block:
             if timeout is None:
                 # None: set the timeout period to infinite.
-                stmt = self._stmt_dict['lock'].params(key=self._key)
+                stmt = self._stmt_dict["lock"].params(key=self._key)
                 r = await self.connection_or_session.execute(stmt)
                 deque(r, maxlen=0)
                 self._acquired = True
             else:
                 # negative value for `timeout` are equivalent to a `timeout` of zero.
                 if timeout < 0:
                     timeout = 0
                 interval = self._interval if interval is None else interval
                 if interval < 0:
-                    raise ValueError('interval must not be smaller than 0')
-                stmt = self._stmt_dict['trylock'].params(key=self._key)
+                    raise ValueError("interval must not be smaller than 0")
+                stmt = self._stmt_dict["trylock"].params(key=self._key)
                 ts_begin = time()
                 while True:
                     r = await self.connection_or_session.stream(stmt)
                     ret_val = (await r.one())[0]
                     if ret_val:  # succeed
                         self._acquired = True
                         break
                     if time() - ts_begin > timeout:  # expired
                         break
                     await asyncio.sleep(interval)
         else:
             # This will either obtain the lock immediately and return true,
             # or return false without waiting if the lock cannot be acquired immediately.
-            stmt = self._stmt_dict['trylock'].params(key=self._key)
+            stmt = self._stmt_dict["trylock"].params(key=self._key)
             r = await self.connection_or_session.stream(stmt)
             ret_val = (await r.one())[0]
             self._acquired = bool(ret_val)
         #
         return self._acquired
 
     async def release(self, *args, **kwargs):
         if not self._acquired:
-            raise ValueError('invoked on an unlocked lock')
-        stmt = self._stmt_dict['unlock'].params(key=self._key)
+            raise ValueError("invoked on an unlocked lock")
+        stmt = self._stmt_dict["unlock"].params(key=self._key)
         r = await self.connection_or_session.stream(stmt)
         ret_val = (await r.one())[0]
         if ret_val:
             self._acquired = False
         else:
             self._acquired = False
-            raise SqlAlchemyDLockDatabaseError(
-                'The advisory lock "{}" was not held.'.format(self._key))
+            raise SqlAlchemyDLockDatabaseError('The advisory lock "{}" was not held.'.format(self._key))
 
     @property
     def level(self) -> str:
         return self._level
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/asyncio/types.py` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/functions.py` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 from importlib import import_module
 
 from sqlalchemy.engine import Connection
 
 from .types import BaseSadLock, TConnectionOrSession
 from .utils import safe_name
 
-__all__ = ['create_sadlock']
+__all__ = ["create_sadlock"]
 
 
-def create_sadlock(
-        connection_or_session: TConnectionOrSession,
-        key,
-        *args, **kwargs
-) -> BaseSadLock:
+def create_sadlock(connection_or_session: TConnectionOrSession, key, *args, **kwargs) -> BaseSadLock:
     """Create a database distributed lock object
 
     Parameters
     ----------
     connection_or_session :
-        sqlalchemy Connection or orm Session/ScopedSession object.
-        Database Connection on which the SQL locking functions will be invoked
+        Connection or Session object SQL locking functions will be invoked on it.
 
     key:
-        Key/name or sth like that used as SQL locking function's ID
+        ID or name of the SQL locking function
 
     Returns
     -------
-    BaseSadLock
         New created lock object, whose type is a subclass of :class:`BaseSadLock`.
 
         The actual type of the lock object depends on the type of `connection` object.
 
         MySQL and PostgreSQL are supported til now.
     """
     if isinstance(connection_or_session, Connection):
         name = safe_name(connection_or_session.engine.name)
     else:
         name = safe_name(connection_or_session.get_bind().name)
     try:
-        mod = import_module('..impl.{}'.format(name), __name__)
+        mod = import_module("..impl.{}".format(name), __name__)
     except ImportError as exception:  # pragma: no cover
-        raise NotImplementedError('{}: {}'.format(name, exception))
-    lock_cls = getattr(mod, 'SadLock')
+        raise NotImplementedError("{}: {}".format(name, exception))
+    lock_cls = getattr(mod, "SadLock")
     return lock_cls(connection_or_session, key, *args, **kwargs)
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/impl/mysql.py` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,47 +5,52 @@
 
 from ..types import BaseSadLock
 from ..exceptions import SqlAlchemyDLockDatabaseError
 from ..types import TConnectionOrSession
 
 MYSQL_LOCK_NAME_MAX_LENGTH = 64
 
-GET_LOCK = text(dedent('''
-SELECT GET_LOCK(:str, :timeout)
-''').strip())
-
-RELEASE_LOCK = text(dedent('''
-SELECT RELEASE_LOCK(:str)
-''').strip())
+GET_LOCK = text(
+    dedent(
+        """
+        SELECT GET_LOCK(:str, :timeout)
+        """
+    ).strip()
+)
+
+RELEASE_LOCK = text(
+    dedent(
+        """
+        SELECT RELEASE_LOCK(:str)
+        """
+    ).strip()
+)
 
 TConvertFunction = Callable[[Any], str]
 
 
 def default_convert(key: Union[bytearray, bytes, int, float]) -> str:
     if isinstance(key, (bytearray, bytes)):
         result = key.decode()
     elif isinstance(key, (int, float)):
         result = str(key)
     else:
-        raise TypeError('{}'.format(type(key)))
+        raise TypeError("{}".format(type(key)))
     return result
 
 
 class SadLock(BaseSadLock):
     """MySQL named-lock
 
     .. seealso:: https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html
     """
 
-    def __init__(self,
-                 connection_or_session: TConnectionOrSession,
-                 key,
-                 convert: Optional[TConvertFunction] = None,
-                 *args, **kwargs
-                 ):
+    def __init__(
+        self, connection_or_session: TConnectionOrSession, key, convert: Optional[TConvertFunction] = None, *args, **kwargs
+    ):
         """
         MySQL named lock requires the key given by string.
 
         If `key` is not a :class:`str`:
 
         - When :class:`int` or :class:`float`,
           the constructor will force convert it to :class:`str`::
@@ -65,30 +70,25 @@
                 return string
         """
         if convert:
             key = convert(key)
         elif not isinstance(key, str):
             key = default_convert(key)
         if not isinstance(key, str):
-            raise TypeError(
-                'MySQL named lock requires the key given by string')
+            raise TypeError("MySQL named lock requires the key given by string")
         if len(key) > MYSQL_LOCK_NAME_MAX_LENGTH:
             raise ValueError(
-                'MySQL enforces a maximum length on lock names of {} characters.'.format(
-                    MYSQL_LOCK_NAME_MAX_LENGTH))
+                "MySQL enforces a maximum length on lock names of {} characters.".format(MYSQL_LOCK_NAME_MAX_LENGTH)
+            )
         #
         super().__init__(connection_or_session, key)
 
-    def acquire(self,
-                block: bool = True,
-                timeout: Union[float, int, None] = None,
-                *args, **kwargs
-                ) -> bool:
+    def acquire(self, block: bool = True, timeout: Union[float, int, None] = None, *args, **kwargs) -> bool:
         if self._acquired:
-            raise ValueError('invoked on a locked lock')
+            raise ValueError("invoked on a locked lock")
         if block:
             # None: set the timeout period to infinite.
             if timeout is None:
                 timeout = -1
             # negative value for `timeout` are equivalent to a `timeout` of zero
             elif timeout < 0:
                 timeout = 0
@@ -97,36 +97,33 @@
         stmt = GET_LOCK.params(str=self._key, timeout=timeout)
         ret_val = self.connection_or_session.execute(stmt).scalar_one()
         if ret_val == 1:
             self._acquired = True
         elif ret_val == 0:
             pass  # 直到超时也没有成功锁定
         elif ret_val is None:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError(
-                'An error occurred while attempting to obtain the lock "{}"'.format(self._key))
+            raise SqlAlchemyDLockDatabaseError('An error occurred while attempting to obtain the lock "{}"'.format(self._key))
         else:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError(
-                'GET_LOCK("{}", {}) returns {}'.format(self._key, timeout, ret_val))
+            raise SqlAlchemyDLockDatabaseError('GET_LOCK("{}", {}) returns {}'.format(self._key, timeout, ret_val))
         return self._acquired
 
     def release(self, **kwargs):
         if not self._acquired:
-            raise ValueError('invoked on an unlocked lock')
+            raise ValueError("invoked on an unlocked lock")
         stmt = RELEASE_LOCK.params(str=self._key)
         ret_val = self.connection_or_session.execute(stmt).scalar_one()
         if ret_val == 1:
             self._acquired = False
         elif ret_val == 0:  # pragma: no cover
             self._acquired = False
             raise SqlAlchemyDLockDatabaseError(
-                'The named lock "{}" was not established by this thread, '
-                'and the lock is not released.'.format(self._key))
+                'The named lock "{}" was not established by this thread, ' "and the lock is not released.".format(self._key)
+            )
         elif ret_val is None:  # pragma: no cover
             self._acquired = False
             raise SqlAlchemyDLockDatabaseError(
                 'The named lock "{}" did not exist, '
-                'was never obtained by a call to GET_LOCK(), '
-                'or has previously been released.'.format(self._key)
+                "was never obtained by a call to GET_LOCK(), "
+                "or has previously been released.".format(self._key)
             )
         else:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError(
-                'RELEASE_LOCK("{}") returns {}'.format(self._key, ret_val))
+            raise SqlAlchemyDLockDatabaseError('RELEASE_LOCK("{}") returns {}'.format(self._key, ret_val))
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/types.py` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,24 +29,20 @@
         try:
             # do something...
             pass
         finally:
             some_lock.release()
     """
 
-    def __init__(self,
-                 connection_or_session: TConnectionOrSession,
-                 key,
-                 *args, **kwargs
-                 ):
+    def __init__(self, connection_or_session: TConnectionOrSession, key, *args, **kwargs):
         """
         Parameters
         ----------
-        connection_or_session : sqlalchemy Connection or orm Session/ScopedSession object
-            SQL locking functions will be invoked on it
+        connection_or_session :
+            Connection or Session object SQL locking functions will be invoked on it
 
         key
             ID or name of the SQL locking function
         """
         self._acquired = False
         self._connection_or_session = connection_or_session
         self._key = key
@@ -55,30 +51,26 @@
         self.acquire()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def __str__(self):  # pragma: no cover
-        return '<{} {} key={} at 0x{:x}>'.format(
-            'locked' if self._acquired else 'unlocked',
-            self.__class__.__name__,
-            self._key, id(self)
+        return "<{} {} key={} at 0x{:x}>".format(
+            "locked" if self._acquired else "unlocked", self.__class__.__name__, self._key, id(self)
         )
 
     @property
     def connection_or_session(self) -> TConnectionOrSession:
-        """Returns `connection_or_session` parameter of the constructor
-        """
+        """Returns `connection_or_session` parameter of the constructor"""
         return self._connection_or_session
 
     @property
     def key(self):
-        """Returns `key` parameter of the constructor
-        """
+        """Returns `key` parameter of the constructor"""
         return self._key
 
     @property
     def acquired(self) -> bool:
         """locked/unlocked state property
 
         As a `Getter`:
@@ -97,28 +89,22 @@
         if value:
             self.acquire()
         else:
             self.release()
 
     @property
     def locked(self) -> bool:
-        """Alias of :data:`acquired`
-        """
+        """Alias of :data:`acquired`"""
         return self.acquired
 
     @locked.setter
     def locked(self, value: bool):
         self.acquired = value
 
-    def acquire(self,
-                block: bool = True,
-                timeout: Union[float, int, None] = None,
-                *args,
-                **kwargs
-                ) -> bool:
+    def acquire(self, block: bool = True, timeout: Union[float, int, None] = None, *args, **kwargs) -> bool:
         """
         Acquire a lock, blocking or non-blocking.
 
         - With the `block` argument set to ``True`` (the default),
           the method call will block until the lock is in an unlocked state,
           then set it to locked and return ``True``.
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock/utils.py` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock.egg-info/PKG-INFO` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,74 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-dlock
-Version: 0.2b3.post4
+Version: 0.3
 Summary: A distributed lock implementation based on SQLAlchemy
-Home-page: https://github.com/tanbro/sqlalchemy-dlock
-Author: liu xue yan
-Author-email: liu_xue_yan@foxmail.com
+Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD 3-Clause License
+        
+        Copyright (c) 2020, liu xue yan
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
+Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
 Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 License-File: LICENSE
+License-File: AUTHORS.md
 
 # SQLAlchemy-DLock
 
-[![GitHub](https://img.shields.io/github/license/tanbro/sqlalchemy-dlock)](https://github.com/tanbro/sqlalchemy-dlock)
-[![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/tanbro/sqlalchemy-dlock)](https://github.com/tanbro/sqlalchemy-dlock/tags)
 [![Python package](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml/badge.svg)](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
-[![PyPI - Status](https://img.shields.io/pypi/status/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
-[![PyPI - License](https://img.shields.io/pypi/l/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
 [![Documentation Status](https://readthedocs.org/projects/sqlalchemy-dlock/badge/?version=latest)](https://sqlalchemy-dlock.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/tanbro/sqlalchemy-dlock/branch/main/graph/badge.svg?token=GfcDT1ckFX)](https://codecov.io/gh/tanbro/sqlalchemy-dlock)
 
 Distributed lock based on Database and [SQLAlchemy][].
 
 It currently supports below locks:
 
-- `MySQL` - named lock: <https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html>
-- `PostgreSQL` - advisory lock: <https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS>
-
-> ❗ **Note**:
->
-> The project is not stable enough and **DO NOT** use it in production.
+ Database  |                                             Lock
+---------- | ---------------------------------------------------------------------------------------------
+MySQL      | [named lock](https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html)
+PostgreSQL | [advisory lock](https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS)
 
 ## Usages
 
-- Work with [SQLAlchemy][]'s `Connection` object:
+- Work with [SQLAlchemy][] `Connection`:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
@@ -66,15 +86,15 @@
   assert lock.acquired
 
   # un-lock
   lock.release()
   assert not lock.acquired
   ```
 
-- Use in `with` statement
+- `with` statement
 
   ```python
   from contextlib import closing
 
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
@@ -99,22 +119,15 @@
           lock2.acquire()
           assert lock2.acquired
 
       # Auto un-locked
       assert not lock2.acquired
   ```
 
-- Work with [SQLAlchemy][]'s `ORM` session:
-
-  > ❗ **Note**:
-  >
-  > According to <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>:
-  >
-  > - The asyncio extension as of SQLAlchemy 1.4.3 can now be considered to be **beta level** software.
-  > - The asyncio extension requires at least Python version 3.6
+- Work with [SQLAlchemy][] `ORM` session:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy.orm import sessionmaker
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
@@ -124,15 +137,20 @@
 
   with Session() as session:
     with create_sadlock(session, key) as lock:
         assert lock.acquired
     assert not lock.acquired
   ```
 
-- Work asynchronously
+- Asynchronous I/O Support
+
+  > ℹ️ **info**:
+  >
+  > - [SQLAlchemy][] `1.x`: <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>
+  > - [SQLAlchemy][] `2.x`: <https://docs.sqlalchemy.org/20/orm/extensions/asyncio.html>
 
   ```python
   from sqlalchemy.ext.asyncio import create_async_engine
   from sqlalchemy_dlock.asyncio import create_async_sadlock
 
   key = 'user/001'
 
@@ -145,107 +163,68 @@
           assert not lock.locked
           await lock.acquire()
       assert not lock.locked
   ```
 
 ## Tests
 
-Just `up` the docker-compose in `tests` directory:
-
-```bash
-(cd tests; docker-compose up --abort-on-container-exit --exit-code-from pytest; docker-compose down)
-```
-
-[SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
-
-# CHANGELOG
-
-## v0.2b2/b3
-
-Date: 2021-03-23
-
-- Add:
-  - More unit tests
-  - Optimized CI
-
-## v0.2b1
-
-Date: 2021-03-16
+Following [SQLAlchemy][] engines are tested:
 
-- Add:
+- MySQL:
 
-  - New unit tests
-  - CI by github workflows
+  - mysqlclient
+  - PyMySQL
+  - aiomysql ([asyncio][])
 
-## v0.2a3
+- Postgres:
 
-Date: 2021-03-14
+  - psycopg2
+  - asyncpg ([asyncio][])
 
-- Change:
+You can run unit-tests:
 
-  - Drop Python 3.5 support.
-  - Remove SQLAlchemy version requires earlier than 1.4 in setup, it's not supported actually.
-  - Adjust PostgreSQL lock's constructor arguments order
+- directly:
 
-- Add:
+  1. Install the project (A virtual environment ([venv][]) is strongly advised):
 
-  - More test cases, and add test/deploy workflow in github actions.
-  - Add docker-compose test scripts
+     ```bash
+     pip install -e .
+     ```
 
-## v0.2a2
+  1. Start up your mysql and postgresql
 
-Date: 2021-03-09
+  1. Set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
+     Multiple connections separated by space.
+     The test cases load environment variables in `tests/.env`.
 
-- Change:
+     eg (and also the defaults):
 
-  - Rename a lot of function/class:
+     ```ini
+     TEST_URLS=mysql://test:test@localhost/test postgresql://postgres:test@localhost/
+     TEST_ASYNC_URLS=mysql+aiomysql://test:test@localhost/test postgresql+asyncpg://postgres:test@localhost/
+     ```
 
-    - `sadlock` -> `create_sadlock`
-    - `asyncio.sadlock` -> `asyncio.create_async_sadlock`
-  
-    and some other ...
+  1. run unit-test
 
-## v0.2a1
+     ```bash
+     python -m unittest
+     ```
 
-Date: 2021-03-08
+- in docker-compose:
 
-- New:
+  1. build the project
 
-  - Asynchronous IO Support by:
+     ```bash
+     python -m pip install build && python -m build -w
+     ```
 
-    - [aiomysql](https://github.com/aio-libs/aiomysql) for MySQL
-
-      Connection URL is like: `"mysql+aiomysql://user:password@host:3306/schema?charset=utf8mb4"`
-
-    - [asyncpg](https://github.com/MagicStack/asyncpg) for PostgreSQL
-
-      Connection URL is like: `"postgresql+asyncpg://user:password@host:5432/db"`
-
-    Read <https://docs.sqlalchemy.org/en/14/orm/extensions/asyncio.html> for details
-
-## v0.1.2
-
-Date: 2021-01-26
-
-Still an early version, not for production.
-
-- Changes:
-  - Arguments and it's default value of `acquire` now similar to stdlib's `multiprossing.Lock`, instead of `Threading.Lock`
-  - MySQL lock now accepts float-point value as `timeout`
-- Adds
-  - Several new test cases
-- Other
-  - Many other small adjustment
-
-## v0.1.1
-
-- A very early version, maybe not stable enough.
-- Replace black2b with crc64-iso in PostgreSQL key convert function
-- Only named arguments as extra parameters allowed in Lock's implementation class
-
-# AUTHORS
-
-* Liu Xue Yan (<liu_xue_yan@foxmail.com>)
-
-  [![liu_xue_yan@foxmail.com](https://www.gravatar.com/avatar/049d2fae1fd2df6439e87d1383d0276b)](mailto:liu_xue_yan@foxmail.com)
+  1. run unit-test
 
+     ```bash
+     cd tests
+     docker compose up --abort-on-container-exit
+     docker compose rm -fsv
+     ```
 
+[SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
+[asyncio]: https://docs.python.org/library/asyncio.html "asyncio is a library to write concurrent code using the async/await syntax."
+[venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
```

### Comparing `sqlalchemy-dlock-0.2b3.post4/src/sqlalchemy_dlock.egg-info/SOURCES.txt` & `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 codecov.yml
 pyproject.toml
-setup.cfg
-setup.py
 scripts/run-test.sh
 scripts/wait-for-mysql.sh
 scripts/wait-for-postgres.sh
 src/sqlalchemy_dlock/__init__.py
 src/sqlalchemy_dlock/exceptions.py
 src/sqlalchemy_dlock/functions.py
 src/sqlalchemy_dlock/types.py
```

