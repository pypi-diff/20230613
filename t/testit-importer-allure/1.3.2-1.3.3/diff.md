# Comparing `tmp/testit-importer-allure-1.3.2.tar.gz` & `tmp/testit-importer-allure-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-importer-allure-1.3.2.tar", last modified: Thu May 25 11:16:04 2023, max compression
+gzip compressed data, was "testit-importer-allure-1.3.3.tar", last modified: Tue Jun 13 14:29:14 2023, max compression
```

## Comparing `testit-importer-allure-1.3.2.tar` & `testit-importer-allure-1.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:16:04.548579 testit-importer-allure-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-25 11:16:04.548579 testit-importer-allure-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/connection_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:16:04.548579 testit-importer-allure-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:16:04.548579 testit-importer-allure-1.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/filedto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/filereader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/minioreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-25 11:15:50.000000 testit-importer-allure-1.3.2/src/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:16:04.548579 testit-importer-allure-1.3.2/testit_importer_allure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-25 11:16:04.000000 testit-importer-allure-1.3.2/testit_importer_allure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-25 11:16:04.000000 testit-importer-allure-1.3.2/testit_importer_allure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:16:04.000000 testit-importer-allure-1.3.2/testit_importer_allure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 11:16:04.000000 testit-importer-allure-1.3.2/testit_importer_allure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 11:16:04.000000 testit-importer-allure-1.3.2/testit_importer_allure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 11:16:04.000000 testit-importer-allure-1.3.2/testit_importer_allure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:29:14.205761 testit-importer-allure-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-13 14:29:14.205761 testit-importer-allure-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/connection_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:29:14.205761 testit-importer-allure-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:29:14.205761 testit-importer-allure-1.3.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/filedto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/minioreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 14:29:02.000000 testit-importer-allure-1.3.3/src/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:29:14.205761 testit-importer-allure-1.3.3/testit_importer_allure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-13 14:29:14.000000 testit-importer-allure-1.3.3/testit_importer_allure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-13 14:29:14.000000 testit-importer-allure-1.3.3/testit_importer_allure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:29:14.000000 testit-importer-allure-1.3.3/testit_importer_allure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 14:29:14.000000 testit-importer-allure-1.3.3/testit_importer_allure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 14:29:14.000000 testit-importer-allure-1.3.3/testit_importer_allure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 14:29:14.000000 testit-importer-allure-1.3.3/testit_importer_allure.egg-info/top_level.txt
```

### Comparing `testit-importer-allure-1.3.2/PKG-INFO` & `testit-importer-allure-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-importer-allure
-Version: 1.3.2
+Version: 1.3.3
 Summary: Allure report importer for Test IT
 Home-page: https://pypi.org/project/testit-importer-allure/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -63,17 +63,18 @@
 1. create a project  
 2. open DevTools -> network  
 3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests  
 4. GET-request configurations, Preview tab, copy id field 
 
 ### Importing
 
-Use the command `testit --resultsdir allure-results` to specify the directory with Allure report results and create new test run in TMS instance.  
-Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
-**Important:** This command initiates the import.
+Use the command `testit --resultsdir allure-results --testrunname <name>` to specify the directory with Allure report results and create new test run with the specified name in TMS instance.
+<br>The `--testrunname` parameter is optional. The default name of testrun is <em>"AllureRun"</em>
+<br>Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
+<br>**Important:** This command initiates the import.
 
 # Contributing
 
 You can help to develop the project. Any contributions are **greatly appreciated**.
 
 * If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testit-tms/importers/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
 * Please make sure you check your spelling and grammar.
```

### Comparing `testit-importer-allure-1.3.2/README.md` & `testit-importer-allure-1.3.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -48,17 +48,18 @@
 1. create a project  
 2. open DevTools -> network  
 3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests  
 4. GET-request configurations, Preview tab, copy id field 
 
 ### Importing
 
-Use the command `testit --resultsdir allure-results` to specify the directory with Allure report results and create new test run in TMS instance.  
-Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
-**Important:** This command initiates the import.
+Use the command `testit --resultsdir allure-results --testrunname <name>` to specify the directory with Allure report results and create new test run with the specified name in TMS instance.
+<br>The `--testrunname` parameter is optional. The default name of testrun is <em>"AllureRun"</em>
+<br>Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
+<br>**Important:** This command initiates the import.
 
 # Contributing
 
 You can help to develop the project. Any contributions are **greatly appreciated**.
 
 * If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testit-tms/importers/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
 * Please make sure you check your spelling and grammar.
```

### Comparing `testit-importer-allure-1.3.2/setup.py` & `testit-importer-allure-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='testit-importer-allure',
-    version='1.3.2',
+    version='1.3.3',
     description='Allure report importer for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://pypi.org/project/testit-importer-allure/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
```

### Comparing `testit-importer-allure-1.3.2/src/__main__.py` & `testit-importer-allure-1.3.3/src/__main__.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.3.2/src/apiclient.py` & `testit-importer-allure-1.3.3/src/apiclient.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.3.2/src/configurator.py` & `testit-importer-allure-1.3.3/src/configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 class Configurator:
     """Class representing a configurator"""
 
     path_to_results = None
     path_to_config = None
     specified_testrun = None
+    specified_testrun_name = None
 
     def __init__(self):
         self.__set_config()
         self.__set_parser()
         self.__parse_args()
         self.__load_env_properties()
 
@@ -139,14 +140,21 @@
             '--testrunid',
             action="store",
             dest="set_testrun",
             metavar="3802f329-190c-4617-8bb0-2c3696abeb8f",
             help='Set test run ID'
         )
         self.parser.add_argument(
+            '-tn',
+            '--testrunname',
+            action="store",
+            dest="set_testrun_name",
+            help='Set test run name'
+        )
+        self.parser.add_argument(
             '-cv',
             '--certvalidation',
             action="store",
             dest="set_cert_validation",
             metavar="false",
             help='Enables/disables certificate validation'
         )
@@ -302,14 +310,17 @@
             if not re.fullmatch(r'[a-zA-Z\d]{8}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{12}',
                                 args.set_testrun):
                 print('The wrong testrun ID!')
                 raise SystemExit
 
             self.specified_testrun = args.set_testrun
 
+        if args.set_testrun_name:
+            self.specified_testrun_name = args.set_testrun_name
+
         if args.set_cert_validation:
             self.config.set(CONFIG_SECTION, CONFIG_CERT_VALIDATION, args.set_cert_validation.lower())
 
         if args.alluredir:
             self.path_to_results = args.alluredir
 
         if args.set_rabbitmqhost:
```

### Comparing `testit-importer-allure-1.3.2/src/converter.py` & `testit-importer-allure-1.3.3/src/converter.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.3.2/src/filereader.py` & `testit-importer-allure-1.3.3/src/filereader.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.3.2/src/importer.py` & `testit-importer-allure-1.3.3/src/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     """Class representing an importer"""
 
     def __init__(self, parser: Parser, api_client: ApiClient, config: Configurator):
         self.__parser = parser
         self.__api_client = api_client
         self.__project_id = config.get_project_id()
         self.__testrun_id = config.specified_testrun
+        self.__testrun_name = config.specified_testrun_name
         self.__configuration_id = config.get_configuration_id()
 
     def send_result(self):
         """Function imports result to TMS."""
         data_tests, data_fixtures = self.__parser.parse_results()
 
         self.__set_test_run()
@@ -87,15 +88,18 @@
             self.__api_client.send_test_result(
                 self.__testrun_id,
                 Converter.test_result_to_testrun_result_post_model(test, self.__configuration_id)
             )
 
     def __set_test_run(self):
         if self.__testrun_id is None:
-            test_run_name = f'AllureRun {datetime.today().strftime("%d %b %Y %H:%M:%S")}'
+            if self.__testrun_name is not None:
+                test_run_name = f'{self.__testrun_name} {datetime.today().strftime("%d %b %Y %H:%M:%S")}'
+            else:
+                test_run_name = f'AllureRun {datetime.today().strftime("%d %b %Y %H:%M:%S")}'
             self.__testrun_id = self.__api_client.create_test_run(self.__project_id, test_run_name)
 
     def __send_attachments(self, attachments):
         ids = []
 
         if attachments:
             if 'attachment' in attachments:
```

### Comparing `testit-importer-allure-1.3.2/src/minioreader.py` & `testit-importer-allure-1.3.3/src/minioreader.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.3.2/src/parser.py` & `testit-importer-allure-1.3.3/src/parser.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.3.2/src/rabbitmq.py` & `testit-importer-allure-1.3.3/src/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.3.2/testit_importer_allure.egg-info/PKG-INFO` & `testit-importer-allure-1.3.3/testit_importer_allure.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-importer-allure
-Version: 1.3.2
+Version: 1.3.3
 Summary: Allure report importer for Test IT
 Home-page: https://pypi.org/project/testit-importer-allure/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -63,17 +63,18 @@
 1. create a project  
 2. open DevTools -> network  
 3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests  
 4. GET-request configurations, Preview tab, copy id field 
 
 ### Importing
 
-Use the command `testit --resultsdir allure-results` to specify the directory with Allure report results and create new test run in TMS instance.  
-Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
-**Important:** This command initiates the import.
+Use the command `testit --resultsdir allure-results --testrunname <name>` to specify the directory with Allure report results and create new test run with the specified name in TMS instance.
+<br>The `--testrunname` parameter is optional. The default name of testrun is <em>"AllureRun"</em>
+<br>Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
+<br>**Important:** This command initiates the import.
 
 # Contributing
 
 You can help to develop the project. Any contributions are **greatly appreciated**.
 
 * If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testit-tms/importers/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
 * Please make sure you check your spelling and grammar.
```

### Comparing `testit-importer-allure-1.3.2/testit_importer_allure.egg-info/SOURCES.txt` & `testit-importer-allure-1.3.3/testit_importer_allure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

