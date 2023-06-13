# Comparing `tmp/ANBUtils-1.5.7.tar.gz` & `tmp/ANBUtils-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.5.7.tar", last modified: Tue Jun 13 05:26:25 2023, max compression
+gzip compressed data, was "dist/ANBUtils-1.5.8.tar", last modified: Tue Jun 13 06:11:14 2023, max compression
```

## Comparing `ANBUtils-1.5.7.tar` & `ANBUtils-1.5.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 05:26:25.325677 ANBUtils-1.5.7/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 05:26:25.324110 ANBUtils-1.5.7/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)      978 2023-06-13 05:25:45.000000 ANBUtils-1.5.7/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     2484 2023-06-13 05:24:45.000000 ANBUtils-1.5.7/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)    11142 2023-06-12 14:50:29.000000 ANBUtils-1.5.7/ANBUtils/db_worker.py
--rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.5.7/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)      917 2023-06-13 04:40:10.000000 ANBUtils-1.5.7/ANBUtils/environ_cheker.py
--rw-r--r--   0 redbson    (501) staff       (20)     3509 2023-06-06 05:12:32.000000 ANBUtils-1.5.7/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.5.7/ANBUtils/messenger.py
--rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.5.7/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 05:26:25.325201 ANBUtils-1.5.7/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      344 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 05:26:25.325457 ANBUtils-1.5.7/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)     4704 2023-06-13 04:40:56.000000 ANBUtils-1.5.7/README.md
--rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-13 05:26:25.325750 ANBUtils-1.5.7/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      893 2023-06-13 05:25:35.000000 ANBUtils-1.5.7/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 06:11:14.311587 ANBUtils-1.5.8/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 06:11:14.310127 ANBUtils-1.5.8/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)      881 2023-06-13 06:10:43.000000 ANBUtils-1.5.8/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     2484 2023-06-13 05:24:45.000000 ANBUtils-1.5.8/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)    11142 2023-06-12 14:50:29.000000 ANBUtils-1.5.8/ANBUtils/db_worker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.5.8/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)      917 2023-06-13 04:40:10.000000 ANBUtils-1.5.8/ANBUtils/environ_cheker.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3509 2023-06-06 05:12:32.000000 ANBUtils-1.5.8/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.5.8/ANBUtils/messenger.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.5.8/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 06:11:14.311116 ANBUtils-1.5.8/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      344 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 06:11:14.311379 ANBUtils-1.5.8/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4704 2023-06-13 06:05:52.000000 ANBUtils-1.5.8/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-13 06:11:14.311676 ANBUtils-1.5.8/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      892 2023-06-13 06:07:13.000000 ANBUtils-1.5.8/setup.py
```

### Comparing `ANBUtils-1.5.7/ANBUtils/__init__.py` & `ANBUtils-1.5.8/ANBUtils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 __title__ = 'ANBUtils'
-
-with open('version', 'r', encoding='utf-8') as f:
-    version = f.read()
-__version__ = version
-
 __author__ = 'redbson'
 __email__ = 'redbson@gmail.com'
 
 from .environ_cheker import environment_checker as _checker
 _checker()
```

### Comparing `ANBUtils-1.5.7/ANBUtils/a.py` & `ANBUtils-1.5.8/ANBUtils/a.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.7/ANBUtils/db_worker.py` & `ANBUtils-1.5.8/ANBUtils/db_worker.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.7/ANBUtils/easy_pickle.py` & `ANBUtils-1.5.8/ANBUtils/easy_pickle.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.7/ANBUtils/environ_cheker.py` & `ANBUtils-1.5.8/ANBUtils/environ_cheker.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.7/ANBUtils/id_work.py` & `ANBUtils-1.5.8/ANBUtils/id_work.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.7/ANBUtils/messenger.py` & `ANBUtils-1.5.8/ANBUtils/messenger.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.7/ANBUtils/tbox.py` & `ANBUtils-1.5.8/ANBUtils/tbox.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.7/ANBUtils.egg-info/PKG-INFO` & `ANBUtils-1.5.8/ANBUtils.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.5.7
+Version: 1.5.8
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: redbson
 Author-email: redbson@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# ANBUilts
+# ANBUtils
 
-ANBUilts is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
+ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
 ## Installation
 
-You can install ANBUilts using pip:
+You can install ANBUtils using pip:
 
 ```
-pip install ANBUilts
+pip install ANBUtils
 ```
 
 ## Functions
 
 ### MongoDB Operations
 
 - `DBWorker`: A class that provides convenient methods for working with MongoDB databases and collections. It allows you to perform operations such as querying data, inserting data, updating data, and more.
 
 ### Environment Checker
 
-- `environment_checker`: A function that checks the required environment variables for the ANBUilts package. It verifies the presence of the following environment variables: `MONGODB_URL`, `MONGODB_PUB_URI`, and `DINGTALK_WEBHOOK`.
+- `environment_checker`: A function that checks the required environment variables for the ANBUtils package. It verifies the presence of the following environment variables: `MONGODB_URL`, `MONGODB_PUB_URI`, and `DINGTALK_WEBHOOK`.
   - `MONGODB_URL`: URL of the MongoDB database.
   - `MONGODB_PUB_URI`: URL of the publicly accessible MongoDB database.
   - `DINGTALK_WEBHOOK`: Webhook address of the DingTalk bot.
   - `QYWECHAT_WEBHOOK`: Webhook address of the QiYe Wechat Work bot.
 
 ### DingTalk Message Sender
 
@@ -50,18 +50,18 @@
 - `ts2str`: A function that converts a timestamp to a formatted date string.
 - `date_format`: A function that formats a date string according to a specified format.
 
 ## Usage
 
 ### MongoDB Operations
 
-To use the MongoDB operations provided by ANBUilts, you need to instantiate a `DBWorker` object with the name of the database you want to work with. Here's an example:
+To use the MongoDB operations provided by ANBUtils, you need to instantiate a `DBWorker` object with the name of the database you want to work with. Here's an example:
 
 ```python
-from ANBUilts import DBWorker
+from ANBUtils import DBWorker
 
 # Instantiate a DBWorker object for the "mydb_key" database
 db = DBWorker("mydb_key")
 
 # Query data from a collection
 data = db.to_df("mycollection")
 
@@ -75,28 +75,28 @@
 ```
 
 ### Message Sender
 
 To send text messages to DingTalk or QiYe Wechat using the `dingtalk_text_message` or `qywechat_text_message` function, you need to set the `DINGTALK_WEBHOOK` environment variable to the webhook URL provided by DingTalk. Here's an example:
 
 ```python
-from ANBUilts import dingtalk_text_message, qywechat_text_message
+from ANBUtils import dingtalk_text_message, qywechat_text_message
 
 # Send a text message to DingTalk
-dingtalk_text_message("Hello from ANBUilts!")
-qywechat_text_message("Hello from ANBUilts!")
+dingtalk_text_message("Hello from ANBUtils!")
+qywechat_text_message("Hello from ANBUtils!")
 
 ```
 
 ### Date and Time Operations
 
-ANBUilts provides various functions for working with dates and times. Here are a few examples:
+ANBUtils provides various functions for working with dates and times. Here are a few examples:
 
 ```python
-from ANBUilts import future, utc2tz, today, tomorrow, yesterday, now, future_base, ts2str, date_format
+from ANBUtils import future, utc2tz, today, tomorrow, yesterday, now, future_base, ts2str, date_format
 
 # Get the date in the future
 future_date = future(5)
 
 # Convert UTC datetime to a specific time zone
 utc_datetime = ...
 tz_datetime = utc2tz(utc_datetime, tz="E8")
@@ -122,18 +122,18 @@
 date_string = ts2str(timestamp)
 
 # Format a date string according to a specified format
 date = "2023-06-06"
 formatted_date = date_format(date, date_format="YYYY_MM_DD")
 ```
 
-Please make sure to refer to the ANBUilts documentation for detailed information on each function and its parameters.
+Please make sure to refer to the ANBUtils documentation for detailed information on each function and its parameters.
 
 ## Contributions and Support
 
-ANBUilts is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUilts).
+ANBUtils is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUtils).
 
 For support or general questions, you can reach out to the project maintainers or the community through the GitHub repository.
 
 ## License
 
-ANBUilts is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
+ANBUtils is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
```

### Comparing `ANBUtils-1.5.7/PKG-INFO` & `ANBUtils-1.5.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.5.7
+Version: 1.5.8
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: redbson
 Author-email: redbson@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# ANBUilts
+# ANBUtils
 
-ANBUilts is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
+ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
 ## Installation
 
-You can install ANBUilts using pip:
+You can install ANBUtils using pip:
 
 ```
-pip install ANBUilts
+pip install ANBUtils
 ```
 
 ## Functions
 
 ### MongoDB Operations
 
 - `DBWorker`: A class that provides convenient methods for working with MongoDB databases and collections. It allows you to perform operations such as querying data, inserting data, updating data, and more.
 
 ### Environment Checker
 
-- `environment_checker`: A function that checks the required environment variables for the ANBUilts package. It verifies the presence of the following environment variables: `MONGODB_URL`, `MONGODB_PUB_URI`, and `DINGTALK_WEBHOOK`.
+- `environment_checker`: A function that checks the required environment variables for the ANBUtils package. It verifies the presence of the following environment variables: `MONGODB_URL`, `MONGODB_PUB_URI`, and `DINGTALK_WEBHOOK`.
   - `MONGODB_URL`: URL of the MongoDB database.
   - `MONGODB_PUB_URI`: URL of the publicly accessible MongoDB database.
   - `DINGTALK_WEBHOOK`: Webhook address of the DingTalk bot.
   - `QYWECHAT_WEBHOOK`: Webhook address of the QiYe Wechat Work bot.
 
 ### DingTalk Message Sender
 
@@ -50,18 +50,18 @@
 - `ts2str`: A function that converts a timestamp to a formatted date string.
 - `date_format`: A function that formats a date string according to a specified format.
 
 ## Usage
 
 ### MongoDB Operations
 
-To use the MongoDB operations provided by ANBUilts, you need to instantiate a `DBWorker` object with the name of the database you want to work with. Here's an example:
+To use the MongoDB operations provided by ANBUtils, you need to instantiate a `DBWorker` object with the name of the database you want to work with. Here's an example:
 
 ```python
-from ANBUilts import DBWorker
+from ANBUtils import DBWorker
 
 # Instantiate a DBWorker object for the "mydb_key" database
 db = DBWorker("mydb_key")
 
 # Query data from a collection
 data = db.to_df("mycollection")
 
@@ -75,28 +75,28 @@
 ```
 
 ### Message Sender
 
 To send text messages to DingTalk or QiYe Wechat using the `dingtalk_text_message` or `qywechat_text_message` function, you need to set the `DINGTALK_WEBHOOK` environment variable to the webhook URL provided by DingTalk. Here's an example:
 
 ```python
-from ANBUilts import dingtalk_text_message, qywechat_text_message
+from ANBUtils import dingtalk_text_message, qywechat_text_message
 
 # Send a text message to DingTalk
-dingtalk_text_message("Hello from ANBUilts!")
-qywechat_text_message("Hello from ANBUilts!")
+dingtalk_text_message("Hello from ANBUtils!")
+qywechat_text_message("Hello from ANBUtils!")
 
 ```
 
 ### Date and Time Operations
 
-ANBUilts provides various functions for working with dates and times. Here are a few examples:
+ANBUtils provides various functions for working with dates and times. Here are a few examples:
 
 ```python
-from ANBUilts import future, utc2tz, today, tomorrow, yesterday, now, future_base, ts2str, date_format
+from ANBUtils import future, utc2tz, today, tomorrow, yesterday, now, future_base, ts2str, date_format
 
 # Get the date in the future
 future_date = future(5)
 
 # Convert UTC datetime to a specific time zone
 utc_datetime = ...
 tz_datetime = utc2tz(utc_datetime, tz="E8")
@@ -122,18 +122,18 @@
 date_string = ts2str(timestamp)
 
 # Format a date string according to a specified format
 date = "2023-06-06"
 formatted_date = date_format(date, date_format="YYYY_MM_DD")
 ```
 
-Please make sure to refer to the ANBUilts documentation for detailed information on each function and its parameters.
+Please make sure to refer to the ANBUtils documentation for detailed information on each function and its parameters.
 
 ## Contributions and Support
 
-ANBUilts is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUilts).
+ANBUtils is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUtils).
 
 For support or general questions, you can reach out to the project maintainers or the community through the GitHub repository.
 
 ## License
 
-ANBUilts is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
+ANBUtils is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
```

### Comparing `ANBUtils-1.5.7/README.md` & `ANBUtils-1.5.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# ANBUilts
+# ANBUtils
 
-ANBUilts is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
+ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
 ## Installation
 
-You can install ANBUilts using pip:
+You can install ANBUtils using pip:
 
 ```
-pip install ANBUilts
+pip install ANBUtils
 ```
 
 ## Functions
 
 ### MongoDB Operations
 
 - `DBWorker`: A class that provides convenient methods for working with MongoDB databases and collections. It allows you to perform operations such as querying data, inserting data, updating data, and more.
 
 ### Environment Checker
 
-- `environment_checker`: A function that checks the required environment variables for the ANBUilts package. It verifies the presence of the following environment variables: `MONGODB_URL`, `MONGODB_PUB_URI`, and `DINGTALK_WEBHOOK`.
+- `environment_checker`: A function that checks the required environment variables for the ANBUtils package. It verifies the presence of the following environment variables: `MONGODB_URL`, `MONGODB_PUB_URI`, and `DINGTALK_WEBHOOK`.
   - `MONGODB_URL`: URL of the MongoDB database.
   - `MONGODB_PUB_URI`: URL of the publicly accessible MongoDB database.
   - `DINGTALK_WEBHOOK`: Webhook address of the DingTalk bot.
   - `QYWECHAT_WEBHOOK`: Webhook address of the QiYe Wechat Work bot.
 
 ### DingTalk Message Sender
 
@@ -40,18 +40,18 @@
 - `ts2str`: A function that converts a timestamp to a formatted date string.
 - `date_format`: A function that formats a date string according to a specified format.
 
 ## Usage
 
 ### MongoDB Operations
 
-To use the MongoDB operations provided by ANBUilts, you need to instantiate a `DBWorker` object with the name of the database you want to work with. Here's an example:
+To use the MongoDB operations provided by ANBUtils, you need to instantiate a `DBWorker` object with the name of the database you want to work with. Here's an example:
 
 ```python
-from ANBUilts import DBWorker
+from ANBUtils import DBWorker
 
 # Instantiate a DBWorker object for the "mydb_key" database
 db = DBWorker("mydb_key")
 
 # Query data from a collection
 data = db.to_df("mycollection")
 
@@ -65,28 +65,28 @@
 ```
 
 ### Message Sender
 
 To send text messages to DingTalk or QiYe Wechat using the `dingtalk_text_message` or `qywechat_text_message` function, you need to set the `DINGTALK_WEBHOOK` environment variable to the webhook URL provided by DingTalk. Here's an example:
 
 ```python
-from ANBUilts import dingtalk_text_message, qywechat_text_message
+from ANBUtils import dingtalk_text_message, qywechat_text_message
 
 # Send a text message to DingTalk
-dingtalk_text_message("Hello from ANBUilts!")
-qywechat_text_message("Hello from ANBUilts!")
+dingtalk_text_message("Hello from ANBUtils!")
+qywechat_text_message("Hello from ANBUtils!")
 
 ```
 
 ### Date and Time Operations
 
-ANBUilts provides various functions for working with dates and times. Here are a few examples:
+ANBUtils provides various functions for working with dates and times. Here are a few examples:
 
 ```python
-from ANBUilts import future, utc2tz, today, tomorrow, yesterday, now, future_base, ts2str, date_format
+from ANBUtils import future, utc2tz, today, tomorrow, yesterday, now, future_base, ts2str, date_format
 
 # Get the date in the future
 future_date = future(5)
 
 # Convert UTC datetime to a specific time zone
 utc_datetime = ...
 tz_datetime = utc2tz(utc_datetime, tz="E8")
@@ -112,18 +112,18 @@
 date_string = ts2str(timestamp)
 
 # Format a date string according to a specified format
 date = "2023-06-06"
 formatted_date = date_format(date, date_format="YYYY_MM_DD")
 ```
 
-Please make sure to refer to the ANBUilts documentation for detailed information on each function and its parameters.
+Please make sure to refer to the ANBUtils documentation for detailed information on each function and its parameters.
 
 ## Contributions and Support
 
-ANBUilts is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUilts).
+ANBUtils is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUtils).
 
 For support or general questions, you can reach out to the project maintainers or the community through the GitHub repository.
 
 ## License
 
-ANBUilts is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
+ANBUtils is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
```

### Comparing `ANBUtils-1.5.7/setup.py` & `ANBUtils-1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,9 @@
     install_requires=[
         "matplotlib>=3.0.0",
         "numpy>=1.0.0",
         "pandas>=1.0.0",
         "pymongo>=4.0.2",
         "requests>=2.0.0",
         "matplotlib>=3.0.0",
-
     ]
 )
```

