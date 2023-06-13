# Comparing `tmp/livescore-api-0.0.1.tar.gz` & `tmp/livescore-api-0.0.2.linux-aarch64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livescore-api-0.0.1.tar", last modified: Mon Jun 12 13:08:45 2023, max compression
+gzip compressed data, was "livescore-api-0.0.2.linux-aarch64.tar", last modified: Tue Jun 13 16:21:12 2023, max compression
```

## Comparing `livescore-api-0.0.1.tar` & `livescore-api-0.0.2.linux-aarch64.tar`

### file list

```diff
@@ -1,17 +1,30 @@
-drwx------   0 bc03     (10204) bc03     (10205)        0 2023-06-12 13:08:45.641000 livescore-api-0.0.1/
--rw-------   0 bc03     (10204) bc03     (10205)     5328 2023-06-12 13:08:45.637000 livescore-api-0.0.1/PKG-INFO
--rw-------   0 bc03     (10204) bc03     (10205)     4266 2023-06-12 13:06:50.000000 livescore-api-0.0.1/README.md
-drwx------   0 bc03     (10204) bc03     (10205)        0 2023-06-12 13:08:45.609000 livescore-api-0.0.1/livescore_api/
--rw-------   0 bc03     (10204) bc03     (10205)      191 2023-06-12 12:02:20.000000 livescore-api-0.0.1/livescore_api/__init__.py
--rw-------   0 bc03     (10204) bc03     (10205)       34 2023-06-12 12:02:20.000000 livescore-api-0.0.1/livescore_api/__main__.py
--rw-------   0 bc03     (10204) bc03     (10205)     3908 2023-06-12 12:38:01.000000 livescore-api-0.0.1/livescore_api/console.py
--rw-------   0 bc03     (10204) bc03     (10205)     9143 2023-06-12 12:38:01.000000 livescore-api-0.0.1/livescore_api/main.py
-drwx------   0 bc03     (10204) bc03     (10205)        0 2023-06-12 13:08:45.633000 livescore-api-0.0.1/livescore_api.egg-info/
--rw-------   0 bc03     (10204) bc03     (10205)     5328 2023-06-12 13:08:44.000000 livescore-api-0.0.1/livescore_api.egg-info/PKG-INFO
--rw-------   0 bc03     (10204) bc03     (10205)      341 2023-06-12 13:08:45.000000 livescore-api-0.0.1/livescore_api.egg-info/SOURCES.txt
--rw-------   0 bc03     (10204) bc03     (10205)        1 2023-06-12 13:08:44.000000 livescore-api-0.0.1/livescore_api.egg-info/dependency_links.txt
--rw-------   0 bc03     (10204) bc03     (10205)       61 2023-06-12 13:08:44.000000 livescore-api-0.0.1/livescore_api.egg-info/entry_points.txt
--rw-------   0 bc03     (10204) bc03     (10205)       42 2023-06-12 13:08:44.000000 livescore-api-0.0.1/livescore_api.egg-info/requires.txt
--rw-------   0 bc03     (10204) bc03     (10205)       14 2023-06-12 13:08:44.000000 livescore-api-0.0.1/livescore_api.egg-info/top_level.txt
--rw-------   0 bc03     (10204) bc03     (10205)       38 2023-06-12 13:08:45.641000 livescore-api-0.0.1/setup.cfg
--rw-------   0 bc03     (10204) bc03     (10205)     1473 2023-06-12 12:38:01.000000 livescore-api-0.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.100987 ./
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.104987 ./data/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.108986 ./data/data/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.108986 ./data/data/com.termux/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.112986 ./data/data/com.termux/files/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:12.456987 ./data/data/com.termux/files/usr/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:12.464986 ./data/data/com.termux/files/usr/bin/
+-rw-rw----   0 root         (0) everybody  (9997)     1014 2023-06-13 16:21:12.468986 ./data/data/com.termux/files/usr/bin/livescore-api
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.116986 ./data/data/com.termux/files/usr/lib/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.116986 ./data/data/com.termux/files/usr/lib/python3.11/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:11.220986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.316986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/
+-rw-rw----   0 root         (0) everybody  (9997)      323 2023-06-13 15:59:50.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-12 02:52:21.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__main__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:10.572986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/
+-rw-rw----   0 root         (0) everybody  (9997)      606 2023-06-13 16:21:10.400987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/__init__.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)      274 2023-06-13 16:21:10.560986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/__main__.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    10107 2023-06-13 16:21:10.528987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/console.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)    20793 2023-06-13 16:21:10.328987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/main.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     4517 2023-06-13 16:21:10.364987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/__pycache__/predictor.cpython-311.pyc
+-rw-rw----   0 root         (0) everybody  (9997)     8243 2023-06-13 14:28:16.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    12712 2023-06-13 15:33:29.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/main.py
+-rw-rw----   0 root         (0) everybody  (9997)     2957 2023-06-13 15:12:23.000000 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api/predictor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 16:21:11.404986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     8545 2023-06-13 16:21:11.004986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      368 2023-06-13 16:21:11.208986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-13 16:21:11.024986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       61 2023-06-13 16:21:11.028987 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       80 2023-06-13 16:21:11.032986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-13 16:21:11.036986 ./data/data/com.termux/files/usr/lib/python3.11/site-packages/livescore_api-0.0.2-py3.11.egg-info/top_level.txt
```

