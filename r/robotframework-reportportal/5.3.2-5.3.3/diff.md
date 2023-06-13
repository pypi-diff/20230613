# Comparing `tmp/robotframework-reportportal-5.3.2.tar.gz` & `tmp/robotframework-reportportal-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-reportportal-5.3.2.tar", last modified: Tue Mar 28 13:07:20 2023, max compression
+gzip compressed data, was "robotframework-reportportal-5.3.3.tar", last modified: Tue Jun 13 12:14:13 2023, max compression
```

## Comparing `robotframework-reportportal-5.3.2.tar` & `robotframework-reportportal-5.3.3.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:07:20.465991 robotframework-reportportal-5.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-03-28 13:07:20.465991 robotframework-reportportal-5.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:07:20.461991 robotframework-reportportal-5.3.2/robotframework_reportportal/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/post_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/result_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/time_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/robotframework_reportportal/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:07:20.465991 robotframework-reportportal-5.3.2/robotframework_reportportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-03-28 13:07:20.000000 robotframework-reportportal-5.3.2/robotframework_reportportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-28 13:07:20.000000 robotframework-reportportal-5.3.2/robotframework_reportportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:07:20.000000 robotframework-reportportal-5.3.2/robotframework_reportportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-28 13:07:20.000000 robotframework-reportportal-5.3.2/robotframework_reportportal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-28 13:07:20.000000 robotframework-reportportal-5.3.2/robotframework_reportportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-28 13:07:20.000000 robotframework-reportportal-5.3.2/robotframework_reportportal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-28 13:07:20.465991 robotframework-reportportal-5.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-28 13:07:14.000000 robotframework-reportportal-5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/robotframework_reportportal/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/post_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/result_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/result_visitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/time_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/robotframework_reportportal/variables.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 12:14:13.000000 robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 12:14:13.949376 robotframework-reportportal-5.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-13 12:14:09.000000 robotframework-reportportal-5.3.3/setup.py
```

### Comparing `robotframework-reportportal-5.3.2/CONTRIBUTING.rst` & `robotframework-reportportal-5.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.2/LICENSE.txt` & `robotframework-reportportal-5.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.2/PKG-INFO` & `robotframework-reportportal-5.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal
-Version: 5.3.2
+Version: 5.3.3
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/5.3.2
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/5.3.3
+Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -71,15 +72,15 @@
 For reporting results to Report Portal you need to pass some variables
 to `robot` run:
 
 REQUIRED:
 
 ```
 --listener robotframework_reportportal.listener
---variable RP_UUID:"your_user_uuid"
+--variable RP_API_KEY:"your_user_api_key"
 --variable RP_ENDPOINT:"your_reportportal_url"
 --variable RP_LAUNCH:"launch_name"
 --variable RP_PROJECT:"reportportal_project_name"
 ```
 
 NOT REQUIRED:
```

### Comparing `robotframework-reportportal-5.3.2/README.md` & `robotframework-reportportal-5.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 For reporting results to Report Portal you need to pass some variables
 to `robot` run:
 
 REQUIRED:
 
 ```
 --listener robotframework_reportportal.listener
---variable RP_UUID:"your_user_uuid"
+--variable RP_API_KEY:"your_user_api_key"
 --variable RP_ENDPOINT:"your_reportportal_url"
 --variable RP_LAUNCH:"launch_name"
 --variable RP_PROJECT:"reportportal_project_name"
 ```
 
 NOT REQUIRED:
```

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/__init__.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/exception.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/exception.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/listener.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/listener.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,27 +12,39 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 import os
+from functools import wraps
 from mimetypes import guess_type
 
 from reportportal_client.helpers import gen_attributes
 
 from .exception import RobotServiceException
 from .model import Keyword, Launch, Test, LogMessage, Suite
 from .service import RobotService
 from .static import MAIN_SUITE_ID, PABOT_WIHOUT_LAUNCH_ID_MSG
 from .variables import Variables
 
 logger = logging.getLogger(__name__)
 
 
+def check_rp_enabled(func):
+    """Verify is RP is enabled in config."""
+    @wraps(func)
+    def wrap(*args, **kwargs):
+        if args and isinstance(args[0], listener):
+            if not args[0].service:
+                return
+        func(*args, **kwargs)
+    return wrap
+
+
 class listener(object):
     """Robot Framework listener interface for reporting to Report Portal."""
 
     ROBOT_LISTENER_API_VERSION = 2
 
     def __init__(self):
         """Initialize listener attributes."""
@@ -60,23 +72,25 @@
 
     @property
     def current_item(self):
         """Get the last item from the self._items list."""
         if self._items:
             return self._items[-1]
 
+    @check_rp_enabled
     def log_message(self, message):
         """Send log message to the Report Portal.
 
         :param message: Message passed by the Robot Framework
         """
         msg = self._build_msg_struct(message)
         logger.debug('ReportPortal - Log Message: {0}'.format(message))
         self.service.log(message=msg)
 
+    @check_rp_enabled
     def log_message_with_image(self, msg, image):
         """Send log message to the Report Portal.
 
         :param msg:   Message passed by the Robot Framework
         :param image: Path to image
         """
         mes = self._build_msg_struct(msg)
@@ -94,20 +108,20 @@
     def parent_id(self):
         """Get rp_item_id attribute of the current item."""
         return getattr(self.current_item, 'rp_item_id', None)
 
     @property
     def service(self):
         """Initialize instance of the RobotService."""
-        if self._service is None:
+        if self.variables.enabled and self._service is None:
             self._service = RobotService()
             self._service.init_service(
                 endpoint=self.variables.endpoint,
                 project=self.variables.project,
-                uuid=self.variables.uuid,
+                api_key=self.variables.api_key,
                 log_batch_size=self.variables.log_batch_size,
                 pool_size=self.variables.pool_size,
                 skipped_issue=self.variables.skipped_issue,
                 verify_ssl=self.variables.verify_ssl,
                 log_batch_payload_size=self.variables.log_batch_payload_size,
                 launch_id=self.variables.launch_id,
             )
@@ -116,14 +130,15 @@
     @property
     def variables(self):
         """Get instance of the variables.Variables class."""
         if not self._variables:
             self._variables = Variables()
         return self._variables
 
+    @check_rp_enabled
     def start_launch(self, attributes, ts=None):
         """Start a new launch at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         launch = Launch(self.variables.launch_name, attributes)
@@ -139,14 +154,15 @@
                 mode=self.variables.mode,
                 ts=ts,
                 rerun=self.variables.rerun,
                 rerun_of=self.variables.rerun_of)
         else:
             self.service.rp.launch_id = self.variables.launch_id
 
+    @check_rp_enabled
     def start_suite(self, name, attributes, ts=None):
         """Start a new test suite at the Report Portal.
 
         :param name:       Test suite name
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
@@ -163,14 +179,15 @@
         else:
             logger.debug('ReportPortal - Start Suite: {0}'.format(attributes))
             suite = Suite(name, attributes)
             suite.rp_parent_item_id = self.parent_id
             suite.rp_item_id = self.service.start_suite(suite=suite, ts=ts)
             self._items.append(suite)
 
+    @check_rp_enabled
     def end_suite(self, _, attributes, ts=None):
         """Finish started test suite at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         if attributes['id'] == MAIN_SUITE_ID:
@@ -184,14 +201,15 @@
             self.service.finish_launch(launch=launch, ts=ts)
         else:
             suite = self._finish_current_item().update(attributes)
             logger.debug(
                 'ReportPortal - End Suite: {0}'.format(suite.attributes))
             self.service.finish_suite(suite=suite, ts=ts)
 
+    @check_rp_enabled
     def start_test(self, name, attributes, ts=None):
         """Start a new test case at the Report Portal.
 
         :param name:       Test case name
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
@@ -203,14 +221,15 @@
         logger.debug('ReportPortal - Start Test: {0}'.format(attributes))
         test.attributes = gen_attributes(
             self.variables.test_attributes + test.tags)
         test.rp_parent_item_id = self.parent_id
         test.rp_item_id = self.service.start_test(test=test, ts=ts)
         self._items.append(test)
 
+    @check_rp_enabled
     def end_test(self, _, attributes, ts=None):
         """Finish started test case at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         test = self.current_item.update(attributes)
@@ -220,28 +239,30 @@
             test.status = 'SKIP'
         if test.message:
             self.log_message({'message': test.message, 'level': 'DEBUG'})
         logger.debug('ReportPortal - End Test: {0}'.format(test.attributes))
         self._finish_current_item()
         self.service.finish_test(test=test, ts=ts)
 
+    @check_rp_enabled
     def start_keyword(self, name, attributes, ts=None):
         """Start a new keyword(test step) at the Report Portal.
 
         :param name:       Keyword name
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         kwd = Keyword(name=name, parent_type=self.current_item.type,
                       attributes=attributes)
         kwd.rp_parent_item_id = self.parent_id
         logger.debug('ReportPortal - Start Keyword: {0}'.format(attributes))
         kwd.rp_item_id = self.service.start_keyword(keyword=kwd, ts=ts)
         self._items.append(kwd)
 
+    @check_rp_enabled
     def end_keyword(self, _, attributes, ts=None):
         """Finish started keyword at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         kwd = self._finish_current_item().update(attributes)
@@ -271,10 +292,11 @@
 
         :param xunit_path: Path to the XUnit file
         """
         if self.variables.attach_xunit:
             message = {'message': 'XUnit result file', 'level': 'INFO'}
             self.log_message_with_image(message, xunit_path)
 
+    @check_rp_enabled
     def close(self):
         """Call service terminate when the whole test execution is done."""
         self.service.terminate_service()
```

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/logger.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/model.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/model.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/post_report.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/post_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 This will allow all the test results to be sent to ReportPortal, after the
 test is run. By doing this, we will not disturb the timing when the test is
 run. It also has the benefit of using the test result generated after running
 multiple parallel robot testing (eg. by using pabot).
 
 Command-line usage:
 
-    post_report --variable RP_UUID:"your_user_uuid"
+    post_report --variable RP_API_KEY:"your_user_api_key"
                 --variable RP_ENDPOINT:"your_reportportal_url"
                 --variable RP_PROJECT:"reportportal_project_name"
                 [--variable RP_LAUNCH:"launch_name"]
                 [--variable RP_LAUNCH_DOC:"some_documentation_for_launch"]
                 [--variable RP_LAUNCH_ATTRIBUTES:"RF tag_name:tag_value"]
                 [--variable RP_TEST_ATTRIBUTES:"Long"]
                 [--variable RP_LOG_BATCH_SIZE:"10"]
```

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/result_visitor.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/result_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/service.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,43 +65,43 @@
         """
         attributes = cmd_attrs or []
         system_attributes = get_launch_sys_attrs()
         system_attributes['agent'] = (
             '{}|{}'.format(self.agent_name, self.agent_version))
         return attributes + dict_to_payload(system_attributes)
 
-    def init_service(self, endpoint, project, uuid, log_batch_size, pool_size,
-                     skipped_issue=True, verify_ssl=True,
+    def init_service(self, endpoint, project, api_key, log_batch_size,
+                     pool_size, skipped_issue=True, verify_ssl=True,
                      log_batch_payload_size=MAX_LOG_BATCH_PAYLOAD_SIZE,
                      launch_id=None):
         """Initialize common Report Portal client.
 
         :param endpoint:               Report Portal API endpoint
         :param project:                Report Portal project
-        :param uuid:                   API token
+        :param api_key:                API key
         :param log_batch_size:         Number of logs to be sent within one
                                        batch
         :param pool_size:              HTTPAdapter max pool size
         :param skipped_issue:          Mark skipped test items with
                                        'To Investigate', default value 'True'
         :param verify_ssl:             Disable SSL verification.
         :param log_batch_payload_size: Maximum size of logs to be sent within
                                        one batch
         :param launch_id:              a launch id to use instead of starting
                                        own one
         """
         if self.rp is None:
             logger.debug(
                 'ReportPortal - Init service: '
-                'endpoint={0}, project={1}, uuid={2}'
-                .format(endpoint, project, uuid))
+                'endpoint={0}, project={1}, api_key={2}'
+                .format(endpoint, project, api_key))
             self.rp = RPClient(
                 endpoint=endpoint,
                 project=project,
-                token=uuid,
+                api_key=api_key,
                 is_skipped_an_issue=skipped_issue,
                 log_batch_size=log_batch_size,
                 retries=True,
                 verify_ssl=verify_ssl,
                 max_pool_size=pool_size,
                 log_batch_payload_size=log_batch_payload_size,
                 launch_id=launch_id
```

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/static.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/static.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal/time_visitor.py` & `robotframework-reportportal-5.3.3/robotframework_reportportal/time_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal.egg-info/PKG-INFO` & `robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal
-Version: 5.3.2
+Version: 5.3.3
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/5.3.2
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/5.3.3
+Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -71,15 +72,15 @@
 For reporting results to Report Portal you need to pass some variables
 to `robot` run:
 
 REQUIRED:
 
 ```
 --listener robotframework_reportportal.listener
---variable RP_UUID:"your_user_uuid"
+--variable RP_API_KEY:"your_user_api_key"
 --variable RP_ENDPOINT:"your_reportportal_url"
 --variable RP_LAUNCH:"launch_name"
 --variable RP_PROJECT:"reportportal_project_name"
 ```
 
 NOT REQUIRED:
```

### Comparing `robotframework-reportportal-5.3.2/robotframework_reportportal.egg-info/SOURCES.txt` & `robotframework-reportportal-5.3.3/robotframework_reportportal.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -5,21 +5,27 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 robotframework_reportportal/__init__.py
 robotframework_reportportal/exception.py
 robotframework_reportportal/listener.py
+robotframework_reportportal/listener.pyi
 robotframework_reportportal/logger.py
 robotframework_reportportal/model.py
+robotframework_reportportal/model.pyi
 robotframework_reportportal/post_report.py
 robotframework_reportportal/result_visitor.py
+robotframework_reportportal/result_visitor.pyi
 robotframework_reportportal/service.py
+robotframework_reportportal/service.pyi
 robotframework_reportportal/static.py
+robotframework_reportportal/static.pyi
 robotframework_reportportal/time_visitor.py
 robotframework_reportportal/variables.py
+robotframework_reportportal/variables.pyi
 robotframework_reportportal.egg-info/PKG-INFO
 robotframework_reportportal.egg-info/SOURCES.txt
 robotframework_reportportal.egg-info/dependency_links.txt
 robotframework_reportportal.egg-info/entry_points.txt
 robotframework_reportportal.egg-info/requires.txt
 robotframework_reportportal.egg-info/top_level.txt
```

### Comparing `robotframework-reportportal-5.3.2/setup.py` & `robotframework-reportportal-5.3.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """Setup instructions for the package."""
 
 import os
-from setuptools import setup, find_packages
+from setuptools import setup
 
 
-__version__ = '5.3.2'
+__version__ = '5.3.3'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Name of the file to be read
     :return:      Output of the given file
     """
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name='robotframework-reportportal',
-    packages=find_packages(exclude=('tests', 'tests.*')),
+    packages=['robotframework_reportportal'],
+    package_data={'robotframework_reportportal': ['*.pyi']},
     version=__version__,
     description='Agent for reporting RobotFramework test results to '
                 'Report Portal',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
+    author='Report Portal Team',
     author_email='support@reportportal.io',
     url='https://github.com/reportportal/agent-Python-RobotFramework',
     download_url=(
         'https://github.com/reportportal/agent-Python-RobotFramework/'
         'tarball/{version}'.format(version=__version__)),
     keywords=['testing', 'reporting', 'robot framework', 'reportportal',
               'agent'],
```

