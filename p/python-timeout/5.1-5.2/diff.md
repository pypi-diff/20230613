# Comparing `tmp/python-timeout-5.1.tar.gz` & `tmp/python-timeout-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-timeout-5.1.tar", last modified: Tue Jun 13 00:02:03 2023, max compression
+gzip compressed data, was "python-timeout-5.2.tar", last modified: Tue Jun 13 00:03:11 2023, max compression
```

## Comparing `python-timeout-5.1.tar` & `python-timeout-5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 00:02:03.836792 python-timeout-5.1/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-5.1/.gitignore
--rw-rw-rw-   0        0        0      973 2023-06-13 00:02:03.836792 python-timeout-5.1/PKG-INFO
--rw-rw-rw-   0        0        0      757 2022-05-11 17:10:57.000000 python-timeout-5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 00:02:03.833795 python-timeout-5.1/python_timeout.egg-info/
--rw-rw-rw-   0        0        0      973 2023-06-13 00:02:03.000000 python-timeout-5.1/python_timeout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-13 00:02:03.000000 python-timeout-5.1/python_timeout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 00:02:03.000000 python-timeout-5.1/python_timeout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-13 00:02:03.000000 python-timeout-5.1/python_timeout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-13 00:02:03.000000 python-timeout-5.1/python_timeout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 00:02:03.837792 python-timeout-5.1/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-13 00:01:52.000000 python-timeout-5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:02:03.834794 python-timeout-5.1/timeout/
--rw-rw-rw-   0        0        0     9162 2023-06-13 00:01:45.000000 python-timeout-5.1/timeout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:02:03.835793 python-timeout-5.1/timeout/__pycache__/
--rw-rw-rw-   0        0        0     2743 2023-04-21 11:32:29.000000 python-timeout-5.1/timeout/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-13 00:03:11.916420 python-timeout-5.2/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-5.2/.gitignore
+-rw-rw-rw-   0        0        0      973 2023-06-13 00:03:11.916420 python-timeout-5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      757 2022-05-11 17:10:57.000000 python-timeout-5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 00:03:11.913423 python-timeout-5.2/python_timeout.egg-info/
+-rw-rw-rw-   0        0        0      973 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 00:03:11.917420 python-timeout-5.2/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-13 00:03:05.000000 python-timeout-5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:03:11.914422 python-timeout-5.2/timeout/
+-rw-rw-rw-   0        0        0     9145 2023-06-13 00:02:54.000000 python-timeout-5.2/timeout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:03:11.915421 python-timeout-5.2/timeout/__pycache__/
+-rw-rw-rw-   0        0        0     2743 2023-04-21 11:32:29.000000 python-timeout-5.2/timeout/__pycache__/__init__.cpython-39.pyc
```

### Comparing `python-timeout-5.1/PKG-INFO` & `python-timeout-5.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 5.1
+Version: 5.2
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
 
 ### Timeout
 Random timeout between minimum and maximum values
```

### Comparing `python-timeout-5.1/README.md` & `python-timeout-5.2/README.md`

 * *Files identical despite different names*

### Comparing `python-timeout-5.1/python_timeout.egg-info/PKG-INFO` & `python-timeout-5.2/python_timeout.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 5.1
+Version: 5.2
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
 
 ### Timeout
 Random timeout between minimum and maximum values
```

### Comparing `python-timeout-5.1/timeout/__init__.py` & `python-timeout-5.2/timeout/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from time import sleep
 from random import random, uniform, randrange
 from datetime import datetime, timedelta, time
 from dateutil.parser import parse
-from printr import printr
+from printr import print
 
 class sleep_timer:
     def __init__(self, hour_to_start_at, hour_to_stop_at, sleeping_message='Sleeping'):
         if type(hour_to_start_at) == int:
             self.hour_to_start_at = hour_to_start_at
             self.hour_to_stop_at = hour_to_stop_at
         else:
@@ -64,17 +64,17 @@
         # If we end at 11:13pm and start at 8:49am the difference between the minutes is more than 30 so add an exta hour
         if self.random_minute_to_start_at - current_minute > 30:
             number_of_hours_til_start += 1
 
         formatted_time_to_start_at = f'{self.hour_to_start_at}:{self.random_minute_to_start_at}' # 8:22, must use fstring due to integers
         
         if number_of_hours_til_start == 1:
-            printr(self.sleeping_message, '1 hour until', formatted_time_to_start_at)
+            print(self.sleeping_message, '1 hour until', formatted_time_to_start_at)
         else:
-            printr(self.sleeping_message, number_of_hours_til_start, 'hours until', formatted_time_to_start_at)
+            print(self.sleeping_message, number_of_hours_til_start, 'hours until', formatted_time_to_start_at)
 
         self.printed_sleeping_message = True
 
 class random_timeout:
     '''Random timeout between from and to values'''
     def __init__(self, from_seconds=None, to_seconds=None, from_minutes=None, to_minutes=None, from_hours=None, to_hours=None, from_days=None, to_days=None, silent=False):
         if from_seconds is not None:
@@ -117,39 +117,39 @@
                 maximum = (to_days + random()) * 86400
             else:
                 maximum = from_days + random()
                 
         timeout_in_seconds = uniform(minimum, maximum) # Random float between minimum and maximum
         if not silent:
             if timeout_in_seconds < 60:
-                printr('Sleeping', timeout_in_seconds, 'seconds', level='debug')
+                print('Sleeping', timeout_in_seconds, 'seconds', level='debug')
             elif timeout_in_seconds > 86400:
                 timeout_in_days = round(timeout_in_seconds / 86400) # Convert sleep time in seconds to days
                 til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%A, %B %e')
                 if timeout_in_days == 1:
-                    printr('Sleeping 1 day until', til)
+                    print('Sleeping 1 day until', til)
                 else:
-                    printr('Sleeping', timeout_in_days, 'days until', til)
+                    print('Sleeping', timeout_in_days, 'days until', til)
             elif timeout_in_seconds > 3600:
                 timeout_in_hours = round(timeout_in_seconds / 3600) # Convert sleep time in seconds to hours
                 til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_hours == 1:
-                    printr('Sleeping 1 hour until', til)
+                    print('Sleeping 1 hour until', til)
                 else:
-                    printr('Sleeping', timeout_in_hours, 'hours until', til)
+                    print('Sleeping', timeout_in_hours, 'hours until', til)
             elif timeout_in_seconds >= 60:
                 timeout_in_minutes = round(timeout_in_seconds / 60) # Convert sleep time in seconds to minutes
                 til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_minutes == 1:
-                    printr('Sleeping 1 minute until', til)
+                    print('Sleeping 1 minute until', til)
                 else:
-                    printr('Sleeping', timeout_in_minutes, 'minutes until', til)
+                    print('Sleeping', timeout_in_minutes, 'minutes until', til)
 
         sleep(timeout_in_seconds)
 
 class sleep_for:
     '''Sleep amount of time in minutes, hours or days and prints when it will continue'''
     def __init__(self, seconds=None, minutes=None, hours=None, days=None, silent=False):
         if seconds:
@@ -159,34 +159,34 @@
         elif hours:
             timeout_in_seconds = hours * 3600
         elif days:
             timeout_in_seconds = days * 86400
 
         if not silent:
             if timeout_in_seconds < 60:
-                printr('Sleeping', timeout_in_seconds, 'seconds', level='debug')
+                print('Sleeping', timeout_in_seconds, 'seconds', level='debug')
             elif timeout_in_seconds > 86400:
                 timeout_in_days = round(timeout_in_seconds / 86400) # Convert sleep time in seconds to days
                 til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%A, %B %e')
                 if timeout_in_days == 1:
-                    printr('Sleeping 1 day until', til)
+                    print('Sleeping 1 day until', til)
                 else:
-                    printr('Sleeping', timeout_in_days, 'days until', til)
+                    print('Sleeping', timeout_in_days, 'days until', til)
             elif timeout_in_seconds > 3600:
                 timeout_in_hours = round(timeout_in_seconds / 3600) # Convert sleep time in seconds to hours
                 til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_hours == 1:
-                    printr('Sleeping 1 hour until', til)
+                    print('Sleeping 1 hour until', til)
                 else:
-                    printr('Sleeping', timeout_in_hours, 'hours until', til)
+                    print('Sleeping', timeout_in_hours, 'hours until', til)
             elif timeout_in_seconds >= 60:
                 timeout_in_minutes = round(timeout_in_seconds / 60) # Convert sleep time in seconds to minutes
                 til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_minutes == 1:
-                    printr('Sleeping 1 minute until', til)
+                    print('Sleeping 1 minute until', til)
                 else:
-                    printr('Sleeping', timeout_in_minutes, 'minutes until', til)
+                    print('Sleeping', timeout_in_minutes, 'minutes until', til)
 
         sleep(timeout_in_seconds)
```

### Comparing `python-timeout-5.1/timeout/__pycache__/__init__.cpython-39.pyc` & `python-timeout-5.2/timeout/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

