# Comparing `tmp/canvaslms-2.8.tar.gz` & `tmp/canvaslms-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvaslms-2.8.tar", max compression
+gzip compressed data, was "canvaslms-2.9.tar", max compression
```

## Comparing `canvaslms-2.8.tar` & `canvaslms-2.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1074 2021-09-27 06:58:04.286703 canvaslms-2.8/LICENSE
--rw-r--r--   0        0        0     1450 2021-09-27 06:58:04.286703 canvaslms-2.8/README.md
--rw-r--r--   0        0        0     1505 2022-05-01 20:45:04.301240 canvaslms-2.8/experiments/quiz.py
--rw-r--r--   0        0        0     1102 2023-03-02 14:56:29.866669 canvaslms-2.8/pyproject.toml
--rw-r--r--   0        0        0      119 2022-03-12 06:43:50.183723 canvaslms-2.8/src/canvaslms/Makefile
--rw-r--r--   0        0        0        0 2022-01-18 09:45:09.014722 canvaslms-2.8/src/canvaslms/__init__.py
--rw-r--r--   0        0        0      251 2022-03-12 06:43:50.183723 canvaslms-2.8/src/canvaslms/cli/.gitignore
--rw-r--r--   0        0        0      589 2022-11-14 08:34:27.095839 canvaslms-2.8/src/canvaslms/cli/Makefile
--rw-r--r--   0        0        0     3109 2023-03-02 14:56:59.971006 canvaslms-2.8/src/canvaslms/cli/__init__.py
--rw-r--r--   0        0        0    11139 2023-01-05 20:59:17.162510 canvaslms-2.8/src/canvaslms/cli/assignments.nw
--rw-r--r--   0        0        0     5787 2023-01-05 20:59:18.074534 canvaslms-2.8/src/canvaslms/cli/assignments.py
--rw-r--r--   0        0        0     9146 2023-03-02 14:55:50.178357 canvaslms-2.8/src/canvaslms/cli/cli.nw
--rw-r--r--   0        0        0     4697 2022-12-21 07:01:28.846110 canvaslms-2.8/src/canvaslms/cli/courses.nw
--rw-r--r--   0        0        0     2165 2022-12-21 07:01:29.602113 canvaslms-2.8/src/canvaslms/cli/courses.py
--rw-r--r--   0        0        0     3078 2022-12-21 06:51:59.019526 canvaslms-2.8/src/canvaslms/cli/grade.nw
--rw-r--r--   0        0        0     1352 2022-12-21 06:57:05.392950 canvaslms-2.8/src/canvaslms/cli/grade.py
--rw-r--r--   0        0        0     3982 2023-02-16 10:21:27.688186 canvaslms-2.8/src/canvaslms/cli/login.nw
--rw-r--r--   0        0        0     2583 2023-02-16 12:42:26.949127 canvaslms-2.8/src/canvaslms/cli/login.py
--rw-r--r--   0        0        0     8714 2022-03-12 06:43:50.183723 canvaslms-2.8/src/canvaslms/cli/results.nw
--rw-r--r--   0        0        0     4907 2022-11-15 19:01:40.933352 canvaslms-2.8/src/canvaslms/cli/results.py
--rw-r--r--   0        0        0    18522 2023-03-02 14:45:52.976182 canvaslms-2.8/src/canvaslms/cli/submissions.nw
--rw-r--r--   0        0        0     9777 2023-03-02 14:49:47.600581 canvaslms-2.8/src/canvaslms/cli/submissions.py
--rw-r--r--   0        0        0    19745 2023-03-02 14:41:06.420817 canvaslms-2.8/src/canvaslms/cli/users.nw
--rw-r--r--   0        0        0    11638 2023-03-02 14:41:59.711483 canvaslms-2.8/src/canvaslms/cli/users.py
--rw-r--r--   0        0        0      162 2023-01-27 10:07:11.938313 canvaslms-2.8/src/canvaslms/grades/.gitignore
--rw-r--r--   0        0        0      690 2023-01-27 09:56:21.225027 canvaslms-2.8/src/canvaslms/grades/Makefile
--rw-r--r--   0        0        0      608 2022-03-12 06:43:50.183723 canvaslms-2.8/src/canvaslms/grades/__init__.py
--rw-r--r--   0        0        0     3329 2023-01-27 08:16:37.669974 canvaslms-2.8/src/canvaslms/grades/conjunctavg.nw
--rw-r--r--   0        0        0     2123 2023-01-27 09:50:54.412334 canvaslms-2.8/src/canvaslms/grades/conjunctavg.py
--rw-r--r--   0        0        0     2870 2023-01-27 09:58:14.366476 canvaslms-2.8/src/canvaslms/grades/conjunctavgsurvey.nw
--rw-r--r--   0        0        0     1748 2023-01-27 09:58:15.642448 canvaslms-2.8/src/canvaslms/grades/conjunctavgsurvey.py
--rw-r--r--   0        0        0     3135 2023-01-27 08:16:37.673974 canvaslms-2.8/src/canvaslms/grades/disjunctmax.nw
--rw-r--r--   0        0        0     1810 2023-01-27 09:50:54.412334 canvaslms-2.8/src/canvaslms/grades/disjunctmax.py
--rw-r--r--   0        0        0     1628 2023-01-27 08:17:49.806455 canvaslms-2.8/src/canvaslms/grades/grades.nw
--rw-r--r--   0        0        0     2689 2023-01-27 10:33:02.142932 canvaslms-2.8/src/canvaslms/grades/maxgradesurvey.nw
--rw-r--r--   0        0        0     1489 2023-01-27 10:33:05.895044 canvaslms-2.8/src/canvaslms/grades/maxgradesurvey.py
--rw-r--r--   0        0        0       27 2021-10-20 07:49:35.068703 canvaslms-2.8/src/canvaslms/hacks/.gitignore
--rw-r--r--   0        0        0      284 2021-10-20 07:49:35.068703 canvaslms-2.8/src/canvaslms/hacks/Makefile
--rw-r--r--   0        0        0        0 2021-10-20 07:49:35.068703 canvaslms-2.8/src/canvaslms/hacks/__init__.py
--rw-r--r--   0        0        0     3301 2022-03-05 19:23:21.489529 canvaslms-2.8/src/canvaslms/hacks/canvasapi.nw
--rw-r--r--   0        0        0     1466 2022-11-15 19:01:41.009351 canvaslms-2.8/src/canvaslms/hacks/canvasapi.py
--rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 canvaslms-2.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-09-27 06:58:04.286703 canvaslms-2.9/LICENSE
+-rw-r--r--   0        0        0     1450 2021-09-27 06:58:04.286703 canvaslms-2.9/README.md
+-rw-r--r--   0        0        0     1505 2022-05-01 20:45:04.301240 canvaslms-2.9/experiments/quiz.py
+-rw-r--r--   0        0        0     1102 2023-06-01 08:00:41.642157 canvaslms-2.9/pyproject.toml
+-rw-r--r--   0        0        0      119 2022-03-12 06:43:50.183723 canvaslms-2.9/src/canvaslms/Makefile
+-rw-r--r--   0        0        0        0 2022-01-18 09:45:09.014722 canvaslms-2.9/src/canvaslms/__init__.py
+-rw-r--r--   0        0        0      251 2022-03-12 06:43:50.183723 canvaslms-2.9/src/canvaslms/cli/.gitignore
+-rw-r--r--   0        0        0      589 2022-11-14 08:34:27.095839 canvaslms-2.9/src/canvaslms/cli/Makefile
+-rw-r--r--   0        0        0     3109 2023-03-02 14:56:59.971006 canvaslms-2.9/src/canvaslms/cli/__init__.py
+-rw-r--r--   0        0        0    11139 2023-01-05 20:59:17.162510 canvaslms-2.9/src/canvaslms/cli/assignments.nw
+-rw-r--r--   0        0        0     5787 2023-01-05 20:59:18.074534 canvaslms-2.9/src/canvaslms/cli/assignments.py
+-rw-r--r--   0        0        0     9146 2023-03-02 14:55:50.178357 canvaslms-2.9/src/canvaslms/cli/cli.nw
+-rw-r--r--   0        0        0     4697 2022-12-21 07:01:28.846110 canvaslms-2.9/src/canvaslms/cli/courses.nw
+-rw-r--r--   0        0        0     2165 2022-12-21 07:01:29.602113 canvaslms-2.9/src/canvaslms/cli/courses.py
+-rw-r--r--   0        0        0     3078 2022-12-21 06:51:59.019526 canvaslms-2.9/src/canvaslms/cli/grade.nw
+-rw-r--r--   0        0        0     1352 2022-12-21 06:57:05.392950 canvaslms-2.9/src/canvaslms/cli/grade.py
+-rw-r--r--   0        0        0     4415 2023-06-01 07:57:30.125695 canvaslms-2.9/src/canvaslms/cli/login.nw
+-rw-r--r--   0        0        0     2587 2023-06-01 08:01:30.013780 canvaslms-2.9/src/canvaslms/cli/login.py
+-rw-r--r--   0        0        0     8714 2022-03-12 06:43:50.183723 canvaslms-2.9/src/canvaslms/cli/results.nw
+-rw-r--r--   0        0        0     4907 2022-11-15 19:01:40.933352 canvaslms-2.9/src/canvaslms/cli/results.py
+-rw-r--r--   0        0        0    18522 2023-03-02 14:45:52.976182 canvaslms-2.9/src/canvaslms/cli/submissions.nw
+-rw-r--r--   0        0        0     9777 2023-03-02 14:49:47.600581 canvaslms-2.9/src/canvaslms/cli/submissions.py
+-rw-r--r--   0        0        0    19745 2023-03-02 14:41:06.420817 canvaslms-2.9/src/canvaslms/cli/users.nw
+-rw-r--r--   0        0        0    11638 2023-03-02 14:41:59.711483 canvaslms-2.9/src/canvaslms/cli/users.py
+-rw-r--r--   0        0        0      162 2023-01-27 10:07:11.938313 canvaslms-2.9/src/canvaslms/grades/.gitignore
+-rw-r--r--   0        0        0      690 2023-01-27 09:56:21.225027 canvaslms-2.9/src/canvaslms/grades/Makefile
+-rw-r--r--   0        0        0      608 2022-03-12 06:43:50.183723 canvaslms-2.9/src/canvaslms/grades/__init__.py
+-rw-r--r--   0        0        0     3329 2023-01-27 08:16:37.669974 canvaslms-2.9/src/canvaslms/grades/conjunctavg.nw
+-rw-r--r--   0        0        0     2123 2023-01-27 09:50:54.412334 canvaslms-2.9/src/canvaslms/grades/conjunctavg.py
+-rw-r--r--   0        0        0     2870 2023-01-27 09:58:14.366476 canvaslms-2.9/src/canvaslms/grades/conjunctavgsurvey.nw
+-rw-r--r--   0        0        0     1748 2023-01-27 09:58:15.642448 canvaslms-2.9/src/canvaslms/grades/conjunctavgsurvey.py
+-rw-r--r--   0        0        0     3135 2023-01-27 08:16:37.673974 canvaslms-2.9/src/canvaslms/grades/disjunctmax.nw
+-rw-r--r--   0        0        0     1810 2023-01-27 09:50:54.412334 canvaslms-2.9/src/canvaslms/grades/disjunctmax.py
+-rw-r--r--   0        0        0     1628 2023-01-27 08:17:49.806455 canvaslms-2.9/src/canvaslms/grades/grades.nw
+-rw-r--r--   0        0        0     2689 2023-01-27 10:33:02.142932 canvaslms-2.9/src/canvaslms/grades/maxgradesurvey.nw
+-rw-r--r--   0        0        0     1489 2023-01-27 10:33:05.895044 canvaslms-2.9/src/canvaslms/grades/maxgradesurvey.py
+-rw-r--r--   0        0        0       27 2021-10-20 07:49:35.068703 canvaslms-2.9/src/canvaslms/hacks/.gitignore
+-rw-r--r--   0        0        0      284 2021-10-20 07:49:35.068703 canvaslms-2.9/src/canvaslms/hacks/Makefile
+-rw-r--r--   0        0        0        0 2021-10-20 07:49:35.068703 canvaslms-2.9/src/canvaslms/hacks/__init__.py
+-rw-r--r--   0        0        0     3301 2022-03-05 19:23:21.489529 canvaslms-2.9/src/canvaslms/hacks/canvasapi.nw
+-rw-r--r--   0        0        0     1466 2022-11-15 19:01:41.009351 canvaslms-2.9/src/canvaslms/hacks/canvasapi.py
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 canvaslms-2.9/PKG-INFO
```

### Comparing `canvaslms-2.8/LICENSE` & `canvaslms-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/README.md` & `canvaslms-2.9/README.md`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/experiments/quiz.py` & `canvaslms-2.9/experiments/quiz.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/pyproject.toml` & `canvaslms-2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canvaslms"
-version = "2.8"
+version = "2.9"
 description = "Command-line interface to Canvas LMS"
 authors = ["Daniel Bosk <dbosk@kth.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/canvaslms"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `canvaslms-2.8/src/canvaslms/cli/Makefile` & `canvaslms-2.9/src/canvaslms/cli/Makefile`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/__init__.py` & `canvaslms-2.9/src/canvaslms/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/assignments.nw` & `canvaslms-2.9/src/canvaslms/cli/assignments.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/assignments.py` & `canvaslms-2.9/src/canvaslms/cli/assignments.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/cli.nw` & `canvaslms-2.9/src/canvaslms/cli/cli.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/courses.nw` & `canvaslms-2.9/src/canvaslms/cli/courses.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/courses.py` & `canvaslms-2.9/src/canvaslms/cli/courses.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/grade.nw` & `canvaslms-2.9/src/canvaslms/cli/grade.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/grade.py` & `canvaslms-2.9/src/canvaslms/cli/grade.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/login.nw` & `canvaslms-2.9/src/canvaslms/cli/login.nw`

 * *Files 7% similar despite different names*

```diff
@@ -69,16 +69,15 @@
   print(f"""
 <<instructions how to get the token>>
 """)
 
   token = input("Canvas token: ")
 
   try:
-    keyring.set_password("canvaslms", "hostname", hostname)
-    keyring.set_password("canvaslms", "token", token)
+    <<save [[hostname]] and [[token]] to keyring>>
   except:
     canvaslms.cli.warn(f"You don't have a working keyring. "
                        f"Will write hostname and token to config file "
                        f"{args.config_file}.")
 
     config["canvas"]["host"] = hostname
     config["canvas"]["access_token"] = token
@@ -91,35 +90,49 @@
   https://{hostname}/profile/settings
 
 in your browser. Scroll down to approved integrations and click the
 '+ New access token' button. Fill in the required data and click the
 'Generate token' button. Enter the token here.
 @
 
+Now, to keep this data in the keyring, we simply use [[canvaslms]] as the 
+service, then we store the hostname as the password of user 
+\enquote{hostname}.
+And the same with the token.
+<<save [[hostname]] and [[token]] to keyring>>=
+keyring.set_password("canvaslms", "hostname", hostname)
+keyring.set_password("canvaslms", "token", token)
+@
+
+When we need these again, we simply load them.
+<<load [[hostname]] and [[token]] from keyring>>=
+hostname = keyring.get_password("canvaslms", "hostname")
+token = keyring.get_password("canvaslms", "token")
+@
+
 
 \section{Loading user credentials}
 
 The [[load_credentials]] function will try to get the user's LADOK credentials.
 There are three locations:
 \begin{enumerate}
 \item the system keyring,
-\item the environment variables [[LADOK_USER]] and [[LADOK_PASS]],
+\item the environment variables [[CANVAS_SERVER]] and [[CANVAS_TOKEN]],
 \item the configuration file.
 \end{enumerate}
 They are given the priority they are listed in above.
 It tries to fetch the credentials in the given order; if it succeeds, it 
 returns those credentials, otherwise it tries the next.
 If all fail, the function will return [[None]] for both.
 (This is due to how we handle the [[login]] command.)
 <<functions>>=
 def load_credentials(config):
   """Load credentials from keyring, environment or config dictionary"""
   try:
-    hostname = keyring.get_password("canvaslms", "host")
-    token = keyring.get_password("canvaslms", "token")
+    <<load [[hostname]] and [[token]] from keyring>>
     if hostname and token:
       return hostname, token
   except:
     pass
 
   try:
     hostname = os.environ["CANVAS_SERVER"]
```

### Comparing `canvaslms-2.8/src/canvaslms/cli/login.py` & `canvaslms-2.9/src/canvaslms/cli/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     config["canvas"]["access_token"] = token
 
     canvaslms.cli.update_config_file(config, args.config_file)
 
 def load_credentials(config):
   """Load credentials from keyring, environment or config dictionary"""
   try:
-    hostname = keyring.get_password("canvaslms", "host")
+    hostname = keyring.get_password("canvaslms", "hostname")
     token = keyring.get_password("canvaslms", "token")
     if hostname and token:
       return hostname, token
   except:
     pass
 
   try:
```

### Comparing `canvaslms-2.8/src/canvaslms/cli/results.nw` & `canvaslms-2.9/src/canvaslms/cli/results.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/results.py` & `canvaslms-2.9/src/canvaslms/cli/results.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/submissions.nw` & `canvaslms-2.9/src/canvaslms/cli/submissions.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/submissions.py` & `canvaslms-2.9/src/canvaslms/cli/submissions.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/users.nw` & `canvaslms-2.9/src/canvaslms/cli/users.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/cli/users.py` & `canvaslms-2.9/src/canvaslms/cli/users.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/Makefile` & `canvaslms-2.9/src/canvaslms/grades/Makefile`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/__init__.py` & `canvaslms-2.9/src/canvaslms/grades/__init__.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/conjunctavg.nw` & `canvaslms-2.9/src/canvaslms/grades/conjunctavg.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/conjunctavg.py` & `canvaslms-2.9/src/canvaslms/grades/conjunctavg.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/conjunctavgsurvey.nw` & `canvaslms-2.9/src/canvaslms/grades/conjunctavgsurvey.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/conjunctavgsurvey.py` & `canvaslms-2.9/src/canvaslms/grades/conjunctavgsurvey.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/disjunctmax.nw` & `canvaslms-2.9/src/canvaslms/grades/disjunctmax.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/disjunctmax.py` & `canvaslms-2.9/src/canvaslms/grades/disjunctmax.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/grades.nw` & `canvaslms-2.9/src/canvaslms/grades/grades.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/maxgradesurvey.nw` & `canvaslms-2.9/src/canvaslms/grades/maxgradesurvey.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/grades/maxgradesurvey.py` & `canvaslms-2.9/src/canvaslms/grades/maxgradesurvey.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/hacks/canvasapi.nw` & `canvaslms-2.9/src/canvaslms/hacks/canvasapi.nw`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/src/canvaslms/hacks/canvasapi.py` & `canvaslms-2.9/src/canvaslms/hacks/canvasapi.py`

 * *Files identical despite different names*

### Comparing `canvaslms-2.8/PKG-INFO` & `canvaslms-2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvaslms
-Version: 2.8
+Version: 2.9
 Summary: Command-line interface to Canvas LMS
 Home-page: https://github.com/dbosk/canvaslms
 License: MIT
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

