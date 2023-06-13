# Comparing `tmp/cloudAgnosticPySqsListener-0.9.2.tar.gz` & `tmp/cloudAgnosticPySqsListener-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudAgnosticPySqsListener-0.9.2.tar", last modified: Mon Jun  5 13:04:15 2023, max compression
+gzip compressed data, was "cloudAgnosticPySqsListener-0.9.3.tar", last modified: Tue Jun 13 06:38:43 2023, max compression
```

## Comparing `cloudAgnosticPySqsListener-0.9.2.tar` & `cloudAgnosticPySqsListener-0.9.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:04:15.412770 cloudAgnosticPySqsListener-0.9.2/
--rw-r--r--   0 tom        (501) staff       (20)      643 2023-06-05 12:56:47.000000 cloudAgnosticPySqsListener-0.9.2/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     8068 2023-06-05 13:04:15.412603 cloudAgnosticPySqsListener-0.9.2/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     7420 2023-06-05 13:03:42.000000 cloudAgnosticPySqsListener-0.9.2/README.rst
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:04:15.411430 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     8068 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      349 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       26 2023-06-05 13:04:15.000000 cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-05 13:04:15.412815 cloudAgnosticPySqsListener-0.9.2/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     2403 2023-06-05 13:04:13.000000 cloudAgnosticPySqsListener-0.9.2/setup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:04:15.411581 cloudAgnosticPySqsListener-0.9.2/sqs_launcher/
--rw-r--r--   0 tom        (501) staff       (20)     4200 2023-06-05 12:23:15.000000 cloudAgnosticPySqsListener-0.9.2/sqs_launcher/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-05 13:04:15.412184 cloudAgnosticPySqsListener-0.9.2/sqs_listener/
--rw-r--r--   0 tom        (501) staff       (20)     9356 2023-06-05 12:24:49.000000 cloudAgnosticPySqsListener-0.9.2/sqs_listener/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4286 2023-06-05 12:21:12.000000 cloudAgnosticPySqsListener-0.9.2/sqs_listener/daemon.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 06:38:43.322971 cloudAgnosticPySqsListener-0.9.3/
+-rw-r--r--   0 tom        (501) staff       (20)      643 2023-06-05 12:56:47.000000 cloudAgnosticPySqsListener-0.9.3/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     8117 2023-06-13 06:38:43.322790 cloudAgnosticPySqsListener-0.9.3/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     7469 2023-06-13 06:38:32.000000 cloudAgnosticPySqsListener-0.9.3/README.rst
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 06:38:43.321250 cloudAgnosticPySqsListener-0.9.3/cloudAgnosticPySqsListener.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     8117 2023-06-13 06:38:43.000000 cloudAgnosticPySqsListener-0.9.3/cloudAgnosticPySqsListener.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      371 2023-06-13 06:38:43.000000 cloudAgnosticPySqsListener-0.9.3/cloudAgnosticPySqsListener.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-13 06:38:43.000000 cloudAgnosticPySqsListener-0.9.3/cloudAgnosticPySqsListener.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-06-13 06:38:43.000000 cloudAgnosticPySqsListener-0.9.3/cloudAgnosticPySqsListener.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       36 2023-06-13 06:38:43.000000 cloudAgnosticPySqsListener-0.9.3/cloudAgnosticPySqsListener.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-13 06:38:43.323020 cloudAgnosticPySqsListener-0.9.3/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2404 2023-06-13 06:21:23.000000 cloudAgnosticPySqsListener-0.9.3/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 06:38:43.321394 cloudAgnosticPySqsListener-0.9.3/sqs_launcher/
+-rw-r--r--   0 tom        (501) staff       (20)     4259 2023-06-06 09:14:22.000000 cloudAgnosticPySqsListener-0.9.3/sqs_launcher/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 06:38:43.322083 cloudAgnosticPySqsListener-0.9.3/sqs_listener/
+-rw-r--r--   0 tom        (501) staff       (20)    10283 2023-06-07 11:52:39.000000 cloudAgnosticPySqsListener-0.9.3/sqs_listener/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4286 2023-06-05 12:21:12.000000 cloudAgnosticPySqsListener-0.9.3/sqs_listener/daemon.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 06:38:43.322443 cloudAgnosticPySqsListener-0.9.3/sqs_queue/
+-rw-r--r--   0 tom        (501) staff       (20)     1642 2023-06-06 09:43:22.000000 cloudAgnosticPySqsListener-0.9.3/sqs_queue/__init__.py
```

### Comparing `cloudAgnosticPySqsListener-0.9.2/LICENSE` & `cloudAgnosticPySqsListener-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudAgnosticPySqsListener-0.9.2/PKG-INFO` & `cloudAgnosticPySqsListener-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: cloudAgnosticPySqsListener
-Version: 0.9.2
+Version: 0.9.3
 Summary: A simple cloud agnostic Python SQS utility package
 Home-page: https://github.com/phedone/python-sqs-listener
 Author: Tom HENEAULT
 Author-email: tom@phedone.com
 License: Apache Software License
 Keywords: aws sqs listener and message launcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 
-AWS SQS Listener
-----------------
-
-.. image:: https://img.shields.io/pypi/v/pySqsListener.svg?style=popout
-   :alt: PyPI
-   :target: https://github.com/phedone/python-sqs-listener
-
+Cloud agnostic SQS Listener
+----------------------------
 
+| [WIP] DOC TO BE UPDATED TO LATEST CHANGES
+ This package takes care of the boilerplate involved in listening to an SQS
+ queue, as well as sending messages to a queue.  Works with python 2.7 & 3.6+.
 
+Publish new version
+~~~~~~~~~~~~~~~~~~~~
 
-This package takes care of the boilerplate involved in listening to an SQS
-queue, as well as sending messages to a queue.  Works with python 2.7 & 3.6+.
+- (if not yet done) Configure your ~/.pypirc : https://packaging.python.org/en/latest/specifications/pypirc/
+- Install build tool : ``python3 -m pip install --upgrade build && python3 -m pip install --upgrade twine``
+- Update version number in setup.py
+- ``python3 -m build && python3 -m twine upload --repository cloudAgnosticPySqsListener dist/*``
 
 Installation
 ~~~~~~~~~~~~
 
 ``pip install cloudAgnosticPySqsListener``
 
 Listening to a queue
@@ -164,19 +166,14 @@
     from sqs_launcher import SqsLauncher
 
     launcher = SqsLauncher('my-queue')
     response = launcher.launch_message({'param1': 'hello', 'param2': 'world'})
 
 Important Notes
 ~~~~~~~~~~~~~~~
-
--  The environment variable ``AWS_ACCOUNT_ID`` must be set, in addition
-   to the environment having valid AWS credentials (via environment variables
-   or a credentials file) or if running in an aws ec2 instance a role attached
-   with the required permissions.
 -  For both the main queue and the error queue, if the queue doesn’t
    exist (in the specified region), it will be created at runtime.
 -  The error queue receives only two values in the message body: ``exception_type`` and ``error_message``. Both are of type ``str``
 -  If the function that the listener executes involves connecting to a database, you should explicitly close the connection at the end of the function.  Otherwise, you're likely to get an error like this: ``OperationalError(2006, 'MySQL server has gone away')``
 -  Either the queue name or the queue url should be provided. When both are provided the queue url is used and the queue name is ignored.
 
 Contributing
```

### Comparing `cloudAgnosticPySqsListener-0.9.2/README.rst` & `cloudAgnosticPySqsListener-0.9.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-AWS SQS Listener
-----------------
-
-.. image:: https://img.shields.io/pypi/v/pySqsListener.svg?style=popout
-   :alt: PyPI
-   :target: https://github.com/phedone/python-sqs-listener
-
+Cloud agnostic SQS Listener
+----------------------------
 
+| [WIP] DOC TO BE UPDATED TO LATEST CHANGES
+ This package takes care of the boilerplate involved in listening to an SQS
+ queue, as well as sending messages to a queue.  Works with python 2.7 & 3.6+.
 
+Publish new version
+~~~~~~~~~~~~~~~~~~~~
 
-This package takes care of the boilerplate involved in listening to an SQS
-queue, as well as sending messages to a queue.  Works with python 2.7 & 3.6+.
+- (if not yet done) Configure your ~/.pypirc : https://packaging.python.org/en/latest/specifications/pypirc/
+- Install build tool : ``python3 -m pip install --upgrade build && python3 -m pip install --upgrade twine``
+- Update version number in setup.py
+- ``python3 -m build && python3 -m twine upload --repository cloudAgnosticPySqsListener dist/*``
 
 Installation
 ~~~~~~~~~~~~
 
 ``pip install cloudAgnosticPySqsListener``
 
 Listening to a queue
@@ -147,19 +149,14 @@
     from sqs_launcher import SqsLauncher
 
     launcher = SqsLauncher('my-queue')
     response = launcher.launch_message({'param1': 'hello', 'param2': 'world'})
 
 Important Notes
 ~~~~~~~~~~~~~~~
-
--  The environment variable ``AWS_ACCOUNT_ID`` must be set, in addition
-   to the environment having valid AWS credentials (via environment variables
-   or a credentials file) or if running in an aws ec2 instance a role attached
-   with the required permissions.
 -  For both the main queue and the error queue, if the queue doesn’t
    exist (in the specified region), it will be created at runtime.
 -  The error queue receives only two values in the message body: ``exception_type`` and ``error_message``. Both are of type ``str``
 -  If the function that the listener executes involves connecting to a database, you should explicitly close the connection at the end of the function.  Otherwise, you're likely to get an error like this: ``OperationalError(2006, 'MySQL server has gone away')``
 -  Either the queue name or the queue url should be provided. When both are provided the queue url is used and the queue name is ignored.
 
 Contributing
```

### Comparing `cloudAgnosticPySqsListener-0.9.2/cloudAgnosticPySqsListener.egg-info/PKG-INFO` & `cloudAgnosticPySqsListener-0.9.3/cloudAgnosticPySqsListener.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: cloudAgnosticPySqsListener
-Version: 0.9.2
+Version: 0.9.3
 Summary: A simple cloud agnostic Python SQS utility package
 Home-page: https://github.com/phedone/python-sqs-listener
 Author: Tom HENEAULT
 Author-email: tom@phedone.com
 License: Apache Software License
 Keywords: aws sqs listener and message launcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 
-AWS SQS Listener
-----------------
-
-.. image:: https://img.shields.io/pypi/v/pySqsListener.svg?style=popout
-   :alt: PyPI
-   :target: https://github.com/phedone/python-sqs-listener
-
+Cloud agnostic SQS Listener
+----------------------------
 
+| [WIP] DOC TO BE UPDATED TO LATEST CHANGES
+ This package takes care of the boilerplate involved in listening to an SQS
+ queue, as well as sending messages to a queue.  Works with python 2.7 & 3.6+.
 
+Publish new version
+~~~~~~~~~~~~~~~~~~~~
 
-This package takes care of the boilerplate involved in listening to an SQS
-queue, as well as sending messages to a queue.  Works with python 2.7 & 3.6+.
+- (if not yet done) Configure your ~/.pypirc : https://packaging.python.org/en/latest/specifications/pypirc/
+- Install build tool : ``python3 -m pip install --upgrade build && python3 -m pip install --upgrade twine``
+- Update version number in setup.py
+- ``python3 -m build && python3 -m twine upload --repository cloudAgnosticPySqsListener dist/*``
 
 Installation
 ~~~~~~~~~~~~
 
 ``pip install cloudAgnosticPySqsListener``
 
 Listening to a queue
@@ -164,19 +166,14 @@
     from sqs_launcher import SqsLauncher
 
     launcher = SqsLauncher('my-queue')
     response = launcher.launch_message({'param1': 'hello', 'param2': 'world'})
 
 Important Notes
 ~~~~~~~~~~~~~~~
-
--  The environment variable ``AWS_ACCOUNT_ID`` must be set, in addition
-   to the environment having valid AWS credentials (via environment variables
-   or a credentials file) or if running in an aws ec2 instance a role attached
-   with the required permissions.
 -  For both the main queue and the error queue, if the queue doesn’t
    exist (in the specified region), it will be created at runtime.
 -  The error queue receives only two values in the message body: ``exception_type`` and ``error_message``. Both are of type ``str``
 -  If the function that the listener executes involves connecting to a database, you should explicitly close the connection at the end of the function.  Otherwise, you're likely to get an error like this: ``OperationalError(2006, 'MySQL server has gone away')``
 -  Either the queue name or the queue url should be provided. When both are provided the queue url is used and the queue name is ignored.
 
 Contributing
```

### Comparing `cloudAgnosticPySqsListener-0.9.2/setup.py` & `cloudAgnosticPySqsListener-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from setuptools import setup, find_packages
 # To use a consistent encoding
 from codecs import open
 from os import path
 
+from setuptools import setup, find_packages
+
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cloudAgnosticPySqsListener',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.9.2',
+    version='0.9.3',
 
     description='A simple cloud agnostic Python SQS utility package',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/phedone/python-sqs-listener',
```

### Comparing `cloudAgnosticPySqsListener-0.9.2/sqs_launcher/__init__.py` & `cloudAgnosticPySqsListener-0.9.3/sqs_launcher/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,64 +9,67 @@
 
 # ================
 # start imports
 # ================
 
 import json
 import logging
-import os
 
 import boto3
 import boto3.session
 
 # ================
 # start class
 # ================
+from sqs_queue import SqsQueue
 
 sqs_logger = logging.getLogger('sqs_listener')
 
 
 class SqsLauncher(object):
 
-    def __init__(self, queue=None, queue_url=None, create_queue=False, visibility_timeout='600', serializer=json.dumps, **kwargs):
+    def __init__(self, queue: SqsQueue, create_queue=False, visibility_timeout='600', serializer=json.dumps, **kwargs):
         """
         :param queue: (str) name of queue to listen to
         :param queue_url: (str) url of queue to listen to
         :param create_queue (boolean) determines whether to create the queue if it doesn't exist.  If False, an
                                     Exception will be raised if the queue doesn't already exist
         :param visibility_timeout: (str) Relevant to queue creation.  Indicates the number of seconds for which the SQS will hide the message.
                                     Typically this should reflect the maximum amount of time your handler method will take
                                     to finish execution. See http://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-visibility-timeout.html
                                     for more information
         :param kwargs: options for fine tuning. see below
         """
-        if not any([queue, queue_url]):
+        if not queue.url:
             raise ValueError('Either `queue` or `queue_url` should be provided.')
-        
-        if (
-            not os.environ.get('AWS_ACCOUNT_ID', None) and 
-            not (boto3.Session().get_credentials().method in ['iam-role', 'assume-role', 'assume-role-with-web-identity'])
-        ):
-            raise EnvironmentError('Environment variable `AWS_ACCOUNT_ID` not set and no role found.')
-        
+
+        aws_access_key = queue.access_token or kwargs.get('aws_access_key', '')
+        aws_secret_key = queue.secret_token or kwargs.get('aws_secret_key', '')
+
+        if not aws_access_key or not aws_secret_key:
+            raise Exception("Access token and secret token are missing.")
+
         # new session for each instantiation
-        self._session = boto3.session.Session()
+        self._session = boto3.Session(
+            aws_access_key_id=aws_access_key,
+            aws_secret_access_key=aws_secret_key
+        )
 
-        self._queue_name = queue
-        self._queue_url = queue_url
+        self._queue_name = queue.name
+        self._queue_url = queue.url
         self._serializer = serializer
 
         self._endpoint_name = kwargs.get('endpoint_name', None)
         self._region_name = kwargs.get('region_name', self._session.region_name)
         if self._region_name and self._endpoint_name:
             self._client = self._session.client('sqs', region_name=self._region_name, endpoint_url=self._endpoint_name)
         else:
             self._client = self._session.client('sqs')
-            
-        if not queue_url:
+
+        if not self._queue_url:
             queues = self._client.list_queues(QueueNamePrefix=self._queue_name)
             exists = False
             for q in queues.get('QueueUrls', []):
                 qname = q.split('/')[-1]
                 if qname == self._queue_name:
                     exists = True
                     self._queue_url = q
@@ -79,15 +82,15 @@
                             'VisibilityTimeout': visibility_timeout  # 10 minutes
                         }
                     )
                     self._queue_url = q['QueueUrl']
                 else:
                     raise ValueError('No queue found with name ' + self._queue_name)
         else:
-            self._queue_name = self._get_queue_name_from_url(queue_url)
+            self._queue_name = self._get_queue_name_from_url(self._queue_url)
 
     def launch_message(self, message, **kwargs):
         """
         sends a message to the queue specified in the constructor
         :param message: (dict)
         :param kwargs: additional optional keyword arguments (DelaySeconds, MessageAttributes, MessageDeduplicationId, or MessageGroupId)
                         See http://boto3.readthedocs.io/en/latest/reference/services/sqs.html#SQS.Client.send_message for more information
```

### Comparing `cloudAgnosticPySqsListener-0.9.2/sqs_listener/__init__.py` & `cloudAgnosticPySqsListener-0.9.3/sqs_listener/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,151 +1,167 @@
 """
 Created December 21st, 2016
 @author: Yaakov Gesher
 @version: 0.9.0
 @license: Apache
 """
-from typing import Callable
-
-# ================
-# start imports
-# ================
-
 import json
 import logging
 import os
 import sys
 import time
 from abc import ABCMeta, abstractmethod
+from typing import Callable
 
 import boto3
 import boto3.session
 
-from sqs_launcher import SqsLauncher
-
 # ================
 # start class
 # ================
+from sqs_queue import SqsQueue
+
+# ================
+# start imports
+# ================
 
 sqs_logger = logging.getLogger('sqs_listener')
 
 
 class SqsListener(object):
     __metaclass__ = ABCMeta
 
-    def __init__(self, queue, **kwargs):
+    def __init__(self, queue: SqsQueue, **kwargs):
         """
-        :param queue: (str) name of queue to listen to
+        :param queue: (SQSQueue) queue to listen to
         :param kwargs: options for fine tuning. see below
         """
-        aws_access_key = kwargs.get('aws_access_key', '')
-        aws_secret_key = kwargs.get('aws_secret_key', '')
+        aws_access_key = queue.access_token or kwargs.get('aws_access_key', '')
+        aws_secret_key = queue.secret_token or kwargs.get('aws_secret_key', '')
 
-        boto3_session = None
-        if len(aws_access_key) != 0 and len(aws_secret_key) != 0:
-            boto3_session = boto3.Session(
-                aws_access_key_id=aws_access_key,
-                aws_secret_access_key=aws_secret_key
+        if not aws_access_key or not aws_secret_key:
+            raise Exception("Access token and secret token are missing.")
+
+        boto3_session = boto3.Session(
+            aws_access_key_id=aws_access_key,
+            aws_secret_access_key=aws_secret_key
+        )
+
+        boto3_dead_queue_session = None
+        if queue.dead_queue_secret_token and queue.dead_queue_access_token:
+            boto3_dead_queue_session = boto3.Session(
+                aws_access_key_id=queue.dead_queue_access_token,
+                aws_secret_access_key=queue.dead_queue_secret_token
             )
-        else:
-            boto3_session = None
-            if (
-                    not os.environ.get('AWS_ACCOUNT_ID', None) and
-                    not (boto3.Session().get_credentials().method in ['iam-role', 'assume-role', 'assume-role-with-web-identity'])
-            ):
-                raise EnvironmentError('Environment variable `AWS_ACCOUNT_ID` not set and no role found.')
 
-        self._queue_name = queue
+        self._queue_name = queue.name
         self._poll_interval = kwargs.get("interval", 60)
         self._queue_visibility_timeout = kwargs.get('visibility_timeout', '600')
-        self._error_queue_name = kwargs.get('error_queue', None)
-        self._error_queue_visibility_timeout = kwargs.get('error_visibility_timeout', '600')
-        self._queue_url = kwargs.get('queue_url', None)
+        self._dead_queue_visibility_timeout = kwargs.get('error_visibility_timeout', '10000')
+        self._queue_url = queue.url or kwargs.get('queue_url', None)  # use queue url if available
+        self._dead_queue_url = queue.dead_queue_url or None  # use dead queue url if available
+        self._dead_queue_name = queue.dead_queue_name or None  # use dead queue name if available
         self._message_attribute_names = kwargs.get('message_attribute_names', [])
         self._attribute_names = kwargs.get('attribute_names', [])
         self._force_delete = kwargs.get('force_delete', False)
         self._endpoint_name = kwargs.get('endpoint_name', None)
         self._wait_time = kwargs.get('wait_time', 0)
         self._max_number_of_messages = kwargs.get('max_number_of_messages', 1)
         self._deserializer = kwargs.get("deserializer", json.loads)
         self._run_while_idle = kwargs.get('run_while_idle', None)
+        self._listening = True
 
         # must come last
         if boto3_session:
             self._session = boto3_session
         else:
             self._session = boto3.session.Session()
+
+        if boto3_dead_queue_session or False:
+            self._dead_queue_session = boto3_dead_queue_session
+        else:
+            self._dead_queue_session = None
+
         self._region_name = kwargs.get('region_name', self._session.region_name)
-        self._client = self._initialize_client()
+        self._client, self._dead_queue_client = self._initialize_client()
 
     def _initialize_client(self):
         # new session for each instantiation
         ssl = True
         if self._region_name == 'elasticmq':
             ssl = False
 
         sqs = self._session.client('sqs', region_name=self._region_name, endpoint_url=self._endpoint_name, use_ssl=ssl)
+
+        dead_queue_sqs = None
+        if self._dead_queue_session:
+            dead_queue_sqs = self._dead_queue_session.client('sqs', region_name=self._region_name,
+                                                             endpoint_url=self._endpoint_name, use_ssl=ssl)
+
+        # Skip queue discovery process if queue_url and dead_queue_url are provided
+        if self._queue_url and (self._dead_queue_url or self._dead_queue_url is None):
+            return sqs, dead_queue_sqs
+
         queues = sqs.list_queues(QueueNamePrefix=self._queue_name)
         main_queue_exists = False
         error_queue_exists = False
         if 'QueueUrls' in queues:
             for q in queues['QueueUrls']:
                 qname = q.split('/')[-1]
                 if qname == self._queue_name:
                     main_queue_exists = True
-                if self._error_queue_name and qname == self._error_queue_name:
+                if self._dead_queue_name and qname == self._dead_queue_name:
                     error_queue_exists = True
 
-        # create queue if necessary.
-        # creation is idempotent, no harm in calling on a queue if it already exists.
-        if self._queue_url is None:
-            if not main_queue_exists:
-                sqs_logger.warning("main queue not found, creating now")
-
-                # is this a fifo queue?
-                if self._queue_name.endswith(".fifo"):
-                    fifo_queue = "true"
-                    q = sqs.create_queue(
-                        QueueName=self._queue_name,
-                        Attributes={
-                            'VisibilityTimeout': self._queue_visibility_timeout,  # 10 minutes
-                            'FifoQueue': fifo_queue
-                        }
-                    )
-                else:
-                    # need to avoid FifoQueue property for normal non-fifo queues
-                    q = sqs.create_queue(
-                        QueueName=self._queue_name,
-                        Attributes={
-                            'VisibilityTimeout': self._queue_visibility_timeout,  # 10 minutes
-                        }
-                    )
-                self._queue_url = q['QueueUrl']
+        if not main_queue_exists:
+            sqs_logger.warning("main queue not found, creating now")
+
+            # create queue if necessary.
+            if self._queue_name.endswith(".fifo"):
+                fifo_queue = "true"
+                q = sqs.create_queue(
+                    QueueName=self._queue_name,
+                    Attributes={
+                        'VisibilityTimeout': self._queue_visibility_timeout,  # 10 minutes
+                        'FifoQueue': fifo_queue
+                    }
+                )
+            else:
+                # need to avoid FifoQueue property for normal non-fifo queues
+                q = sqs.create_queue(
+                    QueueName=self._queue_name,
+                    Attributes={
+                        'VisibilityTimeout': self._queue_visibility_timeout,  # 10 minutes
+                    }
+                )
+            self._queue_url = q['QueueUrl']
 
-        if self._error_queue_name and not error_queue_exists:
+        if self._dead_queue_name and not error_queue_exists and dead_queue_sqs:
             sqs_logger.warning("error queue not found, creating now")
-            q = sqs.create_queue(
-                QueueName=self._error_queue_name,
+            q = dead_queue_sqs.create_queue(
+                QueueName=self._dead_queue_name,
                 Attributes={
                     'VisibilityTimeout': self._queue_visibility_timeout  # 10 minutes
                 }
             )
+            self._dead_queue_url = q['QueueUrl']  # update the error queue url
 
-        if self._queue_url is None:
+        if not self._queue_url:
             if os.environ.get('AWS_ACCOUNT_ID', None):
                 qs = sqs.get_queue_url(QueueName=self._queue_name,
                                        QueueOwnerAWSAccountId=os.environ.get('AWS_ACCOUNT_ID', None))
             else:
                 qs = sqs.get_queue_url(QueueName=self._queue_name)
             self._queue_url = qs['QueueUrl']
-        return sqs
+        return sqs, dead_queue_sqs
 
     def _start_listening(self):
         # TODO consider incorporating output processing from here: https://github.com/debrouwere/sqs-antenna/blob/master/antenna/__init__.py
-        while True:
+        self._listening = True
+        while self._listening:
             # calling with WaitTimeSecconds of zero show the same behavior as
             # not specifiying a wait time, ie: short polling
             messages = self._client.receive_message(
                 QueueUrl=self._queue_url,
                 MessageAttributeNames=self._message_attribute_names,
                 AttributeNames=self._attribute_names,
                 WaitTimeSeconds=self._wait_time,
@@ -182,38 +198,42 @@
                             self.handle_message(deserialized, message_attribs, attribs)
                             self._client.delete_message(
                                 QueueUrl=self._queue_url,
                                 ReceiptHandle=receipt_handle
                             )
                     except Exception as ex:
                         sqs_logger.exception(ex)
-                        if self._error_queue_name:
+                        if self._dead_queue_name:
                             exc_type, exc_obj, exc_tb = sys.exc_info()
 
-                            sqs_logger.info("Pushing exception to error queue")
-                            error_launcher = SqsLauncher(queue=self._error_queue_name, create_queue=True)
-                            error_launcher.launch_message(
-                                {
+                            sqs_logger.info("Pushing exception to dead queue")
+
+                            self._dead_queue_client.send_message(
+                                QueueUrl=self._dead_queue_url,
+                                MessageBody=json.dumps({
                                     'exception_type': str(exc_type),
                                     'error_message': str(ex.args)
-                                }
+                                }),
                             )
-
             else:
                 if isinstance(self._run_while_idle, Callable):
                     self._run_while_idle()
                 time.sleep(self._poll_interval)
+        sqs_logger.info("Stopped listening to queue " + self._queue_name)
 
     def listen(self):
         sqs_logger.info("Listening to queue " + self._queue_name)
-        if self._error_queue_name:
-            sqs_logger.info("Using error queue " + self._error_queue_name)
+        if self._dead_queue_name:
+            sqs_logger.info("Using error queue " + self._dead_queue_name)
 
         self._start_listening()
 
+    def stop_listening(self):
+        self._listening = False
+
     def _prepare_logger(self):
         logger = logging.getLogger('eg_daemon')
         logger.setLevel(logging.INFO)
 
         sh = logging.StreamHandler(sys.stdout)
         sh.setLevel(logging.INFO)
```

### Comparing `cloudAgnosticPySqsListener-0.9.2/sqs_listener/daemon.py` & `cloudAgnosticPySqsListener-0.9.3/sqs_listener/daemon.py`

 * *Files identical despite different names*

