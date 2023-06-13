# Comparing `tmp/ANBUtils-1.5.5.tar.gz` & `tmp/ANBUtils-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.5.5.tar", last modified: Mon Jun 12 14:56:37 2023, max compression
+gzip compressed data, was "dist/ANBUtils-1.5.7.tar", last modified: Tue Jun 13 05:26:25 2023, max compression
```

## Comparing `ANBUtils-1.5.5.tar` & `ANBUtils-1.5.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-12 14:56:37.021179 ANBUtils-1.5.5/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-12 14:56:37.018973 ANBUtils-1.5.5/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)      860 2023-06-12 14:43:44.000000 ANBUtils-1.5.5/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     2483 2023-06-05 18:09:00.000000 ANBUtils-1.5.5/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)    11142 2023-06-12 14:50:29.000000 ANBUtils-1.5.5/ANBUtils/db_worker.py
--rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.5.5/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)      833 2023-06-12 14:42:50.000000 ANBUtils-1.5.5/ANBUtils/environ_cheker.py
--rw-r--r--   0 redbson    (501) staff       (20)     3509 2023-06-06 05:12:32.000000 ANBUtils-1.5.5/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)     1127 2023-06-06 05:13:30.000000 ANBUtils-1.5.5/ANBUtils/messager.py
--rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.5.5/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-12 14:56:37.020492 ANBUtils-1.5.5/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)      215 2023-06-12 14:56:36.000000 ANBUtils-1.5.5/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      343 2023-06-12 14:56:36.000000 ANBUtils-1.5.5/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-12 14:56:36.000000 ANBUtils-1.5.5/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-12 14:56:36.000000 ANBUtils-1.5.5/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-12 14:56:36.000000 ANBUtils-1.5.5/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)      215 2023-06-12 14:56:37.020956 ANBUtils-1.5.5/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)     4532 2023-06-12 14:19:28.000000 ANBUtils-1.5.5/README.md
--rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-12 14:56:37.021344 ANBUtils-1.5.5/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      405 2023-06-12 14:43:44.000000 ANBUtils-1.5.5/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 05:26:25.325677 ANBUtils-1.5.7/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 05:26:25.324110 ANBUtils-1.5.7/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)      978 2023-06-13 05:25:45.000000 ANBUtils-1.5.7/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     2484 2023-06-13 05:24:45.000000 ANBUtils-1.5.7/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)    11142 2023-06-12 14:50:29.000000 ANBUtils-1.5.7/ANBUtils/db_worker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.5.7/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)      917 2023-06-13 04:40:10.000000 ANBUtils-1.5.7/ANBUtils/environ_cheker.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3509 2023-06-06 05:12:32.000000 ANBUtils-1.5.7/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.5.7/ANBUtils/messenger.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.5.7/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 05:26:25.325201 ANBUtils-1.5.7/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      344 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-13 05:26:25.000000 ANBUtils-1.5.7/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 05:26:25.325457 ANBUtils-1.5.7/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4704 2023-06-13 04:40:56.000000 ANBUtils-1.5.7/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-13 05:26:25.325750 ANBUtils-1.5.7/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      893 2023-06-13 05:25:35.000000 ANBUtils-1.5.7/setup.py
```

### Comparing `ANBUtils-1.5.5/ANBUtils/__init__.py` & `ANBUtils-1.5.7/ANBUtils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 __title__ = 'ANBUtils'
-__version__ = '1.5.5'
+
+with open('version', 'r', encoding='utf-8') as f:
+    version = f.read()
+__version__ = version
+
 __author__ = 'redbson'
 __email__ = 'redbson@gmail.com'
 
 from .environ_cheker import environment_checker as _checker
 _checker()
 
 
+
 from .a import (
     print_rate_progress, set_date_index, digit, count, value, count2int
 )
 
 from .db_worker import (
     DBWorker, crawler_starter, log_db, read_log, dblink, dblink_add, dblink_remove, dblink_update, collection_show,
     df2mongo, mongo2df, get_db_info, get_mongodb, dblink_help, get_token,
@@ -21,14 +26,14 @@
     easy_dump, easy_load
 )
 
 from .id_work import (
     int_mark, id_analyst, matplot_set
 )
 
-from .messager import (
-    dingtalk_message, dingtalk_text_message, message_mark_A, message_mark_B, message_mark_C, message_mark_D
+from .messenger import (
+    qywechat_message, qywechat_text_message, dingtalk_message, dingtalk_text_message, message_mark_A, message_mark_B, message_mark_C, message_mark_D
 )
 
 from .tbox import (
     future, future_base, date_format, today, yesterday, tomorrow, ts2str, now, utc2tz
 )
```

### Comparing `ANBUtils-1.5.5/ANBUtils/a.py` & `ANBUtils-1.5.7/ANBUtils/a.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,7 +111,8 @@
     _d = {'K': 1000, 'M': 1000000, 'B': 1000000000, 'T': 1000000000000}
     if isinstance(x, str):
         if x[-1] in _d.keys():
             x = float(x[:-1]) * _d[x[-1]]
         else:
             return 0
     return x
+
```

### Comparing `ANBUtils-1.5.5/ANBUtils/db_worker.py` & `ANBUtils-1.5.7/ANBUtils/db_worker.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.5/ANBUtils/easy_pickle.py` & `ANBUtils-1.5.7/ANBUtils/easy_pickle.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.5/ANBUtils/environ_cheker.py` & `ANBUtils-1.5.7/ANBUtils/environ_cheker.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,23 @@
     """
     检查环境变量是否设置。
 
     检查以下环境变量是否在系统环境变量中设置：
     - MONGODB_URL: MongoDB数据库的URL。
     - MONGODB_PUB_URI: 公共访问的MongoDB数据库的URL。
     - DINGTALK_WEBHOOK: 钉钉机器人的Webhook地址。
+    - QYWECHAT_WEBHOOK: 企业微信机器人的Webhook地址。
 
     如果环境变量未设置，则发出警告提示。
 
     参数:
         无
 
     返回:
         无
     """
-    for k in ['MONGODB_URL', 'MONGODB_PUB_URI', 'DINGTALK_WEBHOOK']:
+    for k in ['MONGODB_URL', 'MONGODB_PUB_URI', 'DINGTALK_WEBHOOK','QYWECHAT_WEBHOOK']:
         if k not in os.environ:
             warnings.warn( '\nPlease set %s in environment variable' % k )
             if k == 'MONGODB_URL':
                 warnings.warn(
                     'see <Setting Up DBWorker> https://second-cloche-446.notion.site/ANBUtils-Wiki-f3ba5d99b6904a56a3335aff927492ee' )
```

### Comparing `ANBUtils-1.5.5/ANBUtils/id_work.py` & `ANBUtils-1.5.7/ANBUtils/id_work.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.5/ANBUtils/messager.py` & `ANBUtils-1.5.7/ANBUtils/messenger.py`

 * *Files 27% similar despite different names*

```diff
@@ -37,14 +37,58 @@
     headers = {
         'Content-Type': 'application/json',
     }
     response = requests.post(webhook, headers=headers, data=data.encode("UTF-8"))
     return response.text
 
 
+
+
+def qywechat_message(data):
+    """
+    发送企业微信消息。
+
+    根据给定的数据，通过企业微信的机器人的Webhook发送消息。
+
+    参数：
+        data: 消息数据。
+
+    返回：
+        str: 发送结果。
+
+    异常：
+        None
+    """
+    webhook = os.environ.get('QYWECHAT_WEBHOOK')
+    headers = {
+        'Content-Type': 'application/json',
+    }
+    response = requests.post(webhook, headers=headers, data=data.encode("UTF-8"))
+    return response.text
+
+def qywechat_text_message(text: str):
+    """
+    发送企业微信文本消息。
+
+    根据给定的文本内容，通过企业微信机器人发送文本消息。
+
+    参数：
+        text (str): 文本内容。
+
+    返回：
+        None
+
+    异常：
+        None
+    """
+    qywechat_message(msg_text % text)
+
+
+
+
 def dingtalk_text_message(text: str):
     """
     发送钉钉文本消息。
 
     根据给定的文本内容，通过钉钉机器人发送文本消息。
 
     参数：
@@ -52,8 +96,8 @@
 
     返回：
         None
 
     异常：
         None
     """
-    dingtalk_message(msg_text % text)
+    dingtalk_message(msg_text % text)
```

### Comparing `ANBUtils-1.5.5/ANBUtils/tbox.py` & `ANBUtils-1.5.7/ANBUtils/tbox.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.5/README.md` & `ANBUtils-1.5.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 ### Environment Checker
 
 - `environment_checker`: A function that checks the required environment variables for the ANBUilts package. It verifies the presence of the following environment variables: `MONGODB_URL`, `MONGODB_PUB_URI`, and `DINGTALK_WEBHOOK`.
   - `MONGODB_URL`: URL of the MongoDB database.
   - `MONGODB_PUB_URI`: URL of the publicly accessible MongoDB database.
   - `DINGTALK_WEBHOOK`: Webhook address of the DingTalk bot.
+  - `QYWECHAT_WEBHOOK`: Webhook address of the QiYe Wechat Work bot.
 
 ### DingTalk Message Sender
 
 - `dingtalk_text_message`: A function that sends text messages to DingTalk. It requires the `DINGTALK_WEBHOOK` environment variable to be set. You can use this function to send notifications or alerts to a DingTalk group or chat.
 
 ### Date and Time Operations
 
@@ -59,23 +60,25 @@
 db.insert_df(df, "mycollection")
 
 # Update data in a collection
 df = ...
 db.update_df(df, "mycollection", key="id")
 ```
 
-### DingTalk Message Sender
+### Message Sender
 
-To send text messages to DingTalk using the `dingtalk_text_message` function, you need to set the `DINGTALK_WEBHOOK` environment variable to the webhook URL provided by DingTalk. Here's an example:
+To send text messages to DingTalk or QiYe Wechat using the `dingtalk_text_message` or `qywechat_text_message` function, you need to set the `DINGTALK_WEBHOOK` environment variable to the webhook URL provided by DingTalk. Here's an example:
 
 ```python
-from ANBUilts import dingtalk_text_message
+from ANBUilts import dingtalk_text_message, qywechat_text_message
 
 # Send a text message to DingTalk
 dingtalk_text_message("Hello from ANBUilts!")
+qywechat_text_message("Hello from ANBUilts!")
+
 ```
 
 ### Date and Time Operations
 
 ANBUilts provides various functions for working with dates and times. Here are a few examples:
 
 ```python
```

