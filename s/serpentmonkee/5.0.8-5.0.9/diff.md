# Comparing `tmp/serpentmonkee-5.0.8.tar.gz` & `tmp/serpentmonkee-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serpentmonkee-5.0.8.tar", last modified: Thu Aug 12 09:38:02 2021, max compression
+gzip compressed data, was "serpentmonkee-5.0.9.tar", last modified: Sun Aug 15 04:54:39 2021, max compression
```

## Comparing `serpentmonkee-5.0.8.tar` & `serpentmonkee-5.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wverhoef   (501) staff       (20)        0 2021-08-12 09:38:02.601478 serpentmonkee-5.0.8/
--rw-r--r--   0 wverhoef   (501) staff       (20)      765 2021-08-12 09:38:02.601652 serpentmonkee-5.0.8/PKG-INFO
-drwxr-xr-x   0 wverhoef   (501) staff       (20)        0 2021-08-12 09:38:02.601242 serpentmonkee-5.0.8/serpentmonkee/
--rw-rw-r--   0 wverhoef   (501) staff       (20)     6058 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/CypherQueue.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)    20959 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/CypherTransaction.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)     5170 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/GcpDocMonkee.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)     9220 2021-08-12 09:35:52.721363 serpentmonkee-5.0.8/serpentmonkee/MonkeeRedis.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)    24183 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/MonkeeSQLblocks.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)     3007 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/NeoDriver.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)    11102 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/NeoMonkee.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)    11708 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/PubSubMonkee.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)     2233 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/SecretMonkee.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)      137 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/Serpent.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)     5261 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/UtilsMonkee.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)      806 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/__init__.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)     5205 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/testing pip installed.py
--rw-rw-r--   0 wverhoef   (501) staff       (20)     5180 2021-07-11 22:39:58.000000 serpentmonkee-5.0.8/serpentmonkee/xxMonkeeSqlMessenger.py
--rw-r--r--   0 wverhoef   (501) staff       (20)       61 2021-07-28 23:45:26.183938 serpentmonkee-5.0.8/setup.cfg
--rw-r--r--   0 wverhoef   (501) staff       (20)     1796 2021-08-12 09:36:20.027552 serpentmonkee-5.0.8/setup.py
+drwxr-xr-x   0 wverhoef   (501) staff       (20)        0 2021-08-15 04:54:39.437525 serpentmonkee-5.0.9/
+-rw-r--r--   0 wverhoef   (501) staff       (20)      765 2021-08-15 04:54:39.437755 serpentmonkee-5.0.9/PKG-INFO
+drwxr-xr-x   0 wverhoef   (501) staff       (20)        0 2021-08-15 04:54:39.437348 serpentmonkee-5.0.9/serpentmonkee/
+-rw-rw-r--   0 wverhoef   (501) staff       (20)     6058 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/CypherQueue.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)    20959 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/CypherTransaction.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)     5170 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/GcpDocMonkee.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)     9581 2021-08-15 04:53:07.422875 serpentmonkee-5.0.9/serpentmonkee/MonkeeRedis.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)    24183 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/MonkeeSQLblocks.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)     3007 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/NeoDriver.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)    11102 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/NeoMonkee.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)    11708 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/PubSubMonkee.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)     2233 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/SecretMonkee.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)      137 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/Serpent.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)     5261 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/UtilsMonkee.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)      806 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/__init__.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)     5205 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/testing pip installed.py
+-rw-rw-r--   0 wverhoef   (501) staff       (20)     5180 2021-07-11 22:39:58.000000 serpentmonkee-5.0.9/serpentmonkee/xxMonkeeSqlMessenger.py
+-rw-r--r--   0 wverhoef   (501) staff       (20)       61 2021-07-28 23:45:26.183938 serpentmonkee-5.0.9/setup.cfg
+-rw-r--r--   0 wverhoef   (501) staff       (20)     1796 2021-08-15 04:53:21.966953 serpentmonkee-5.0.9/setup.py
```

### Comparing `serpentmonkee-5.0.8/PKG-INFO` & `serpentmonkee-5.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: serpentmonkee
-Version: 5.0.8
+Version: 5.0.9
 Summary: works with neo4j x
 Home-page: https://github.com/anthromorphic-ai/serpentmonkee
 Author: author
 Author-email: serpentmonkee@monki.ii
 License: MIT
-Download-URL: https://github.com/anthromorphic-ai/serpentmonkee/archive/5.0.8.tar.gz
+Download-URL: https://github.com/anthromorphic-ai/serpentmonkee/archive/5.0.9.tar.gz
 Description: UNKNOWN
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `serpentmonkee-5.0.8/serpentmonkee/CypherQueue.py` & `serpentmonkee-5.0.9/serpentmonkee/CypherQueue.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/CypherTransaction.py` & `serpentmonkee-5.0.9/serpentmonkee/CypherTransaction.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/GcpDocMonkee.py` & `serpentmonkee-5.0.9/serpentmonkee/GcpDocMonkee.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/MonkeeRedis.py` & `serpentmonkee-5.0.9/serpentmonkee/MonkeeRedis.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,16 +222,26 @@
             )
 
     def inferDTFormat(self, dtString):
         dtFormats = []
         dtFormats.append({"re": re.compile(
             r"\d{4}-\d{2}-\d{2}\s\d{2}:\d{2}:\d{2}\.\d*\+\d{2}:\d{2}$"), "fmt": "%Y-%m-%d %H:%M:%S.%f%z"})
         dtFormats.append({"re": re.compile(
+            r"\d{4}-\d{2}-\d{2}\s\d{2}:\d{2}:\d{2}\+\d{2}:\d{2}$"), "fmt": "%Y-%m-%d %H:%M:%S%z"})
+        dtFormats.append({"re": re.compile(
             r"\d{4}-\d{2}-\d{2}\s\d{2}:\d{2}:\d{2}\.\d*$"), "fmt": "%Y-%m-%d %H:%M:%S.%f"})
         dtFormats.append({"re": re.compile(
             r"\d{4}-\d{2}-\d{2}\s\d{2}:\d{2}:\d{2}$"), "fmt": "%Y-%m-%d %H:%M:%S"})
 
         for f in dtFormats:
             if len(re.findall(f["re"], dtString)) > 0:
                 return f["fmt"]
         logging.error(f'MonkeeRedis.inferDTFormat ERROR: "{dtString}"  does not match any preset format. Value encountered for self.userUid={self.userUid}, self.appUid={self.appUid}')
         return None
+
+if __name__=='__main__':
+    mr=MonkeeRedis(fb_db=None, cfName=None, redisClient=None)
+    val='2021-08-11 13:53:01+00:00'
+    fmt = mr.inferDTFormat(val)
+    dt = datetime.strptime(val, fmt)
+    print(fmt, str(dt))
+
```

### Comparing `serpentmonkee-5.0.8/serpentmonkee/MonkeeSQLblocks.py` & `serpentmonkee-5.0.9/serpentmonkee/MonkeeSQLblocks.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/NeoDriver.py` & `serpentmonkee-5.0.9/serpentmonkee/NeoDriver.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/NeoMonkee.py` & `serpentmonkee-5.0.9/serpentmonkee/NeoMonkee.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/PubSubMonkee.py` & `serpentmonkee-5.0.9/serpentmonkee/PubSubMonkee.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/SecretMonkee.py` & `serpentmonkee-5.0.9/serpentmonkee/SecretMonkee.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/UtilsMonkee.py` & `serpentmonkee-5.0.9/serpentmonkee/UtilsMonkee.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/__init__.py` & `serpentmonkee-5.0.9/serpentmonkee/__init__.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/testing pip installed.py` & `serpentmonkee-5.0.9/serpentmonkee/testing pip installed.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/serpentmonkee/xxMonkeeSqlMessenger.py` & `serpentmonkee-5.0.9/serpentmonkee/xxMonkeeSqlMessenger.py`

 * *Files identical despite different names*

### Comparing `serpentmonkee-5.0.8/setup.py` & `serpentmonkee-5.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from distutils.core import setup
 setup(
     name='serpentmonkee',  # How you named your package folder (MyLib)
     packages=['serpentmonkee'],  # Chose the same as "name"
-    version='5.0.8',  # Start with a small number and increase it with every change you make
+    version='5.0.9',  # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='works with neo4j x',
     author='author',  # Type in your name
     author_email='serpentmonkee@monki.ii',  # Type in your E-Mail
     # Provide either the link to your github or to your website
     url='https://github.com/anthromorphic-ai/serpentmonkee',
     # I explain this later on
-    download_url='https://github.com/anthromorphic-ai/serpentmonkee/archive/5.0.8.tar.gz',
+    download_url='https://github.com/anthromorphic-ai/serpentmonkee/archive/5.0.9.tar.gz',
     # Keywords that define your package best
     keywords=['SOME', 'MEANINGFULL', 'KEYWORDS'],
     install_requires=['redis', 'neo4j==4.2.1',
                       'requests==2.23.0',
                       'python-dateutil==2.8.1',
                       'SQLAlchemy==1.3.16',
                       'pg8000==1.15.2'],
```

