# Comparing `tmp/FindJobsTW-1.0.4.tar.gz` & `tmp/FindJobsTW-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-1.0.4.tar", last modified: Tue Jun 13 13:25:16 2023, max compression
+gzip compressed data, was "FindJobsTW-1.0.5.tar", last modified: Tue Jun 13 13:46:33 2023, max compression
```

## Comparing `FindJobsTW-1.0.4.tar` & `FindJobsTW-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.627336 FindJobsTW-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.618366 FindJobsTW-1.0.4/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 16:16:15.000000 FindJobsTW-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       72 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      591 2023-06-13 13:25:16.626340 FindJobsTW-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 16:16:15.000000 FindJobsTW-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.622353 FindJobsTW-1.0.4/findJobs/
--rw-rw-rw-   0        0        0    20125 2023-06-13 13:22:37.000000 FindJobsTW-1.0.4/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0      133 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/__init__.py
--rw-rw-rw-   0        0        0     5368 2023-06-13 13:03:17.000000 FindJobsTW-1.0.4/findJobs/app.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.624346 FindJobsTW-1.0.4/findJobs/static/
--rw-rw-rw-   0        0        0  1245103 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/static/drake.png
--rw-rw-rw-   0        0        0      382 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/static/styles.css
-drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.625343 FindJobsTW-1.0.4/findJobs/templates/
--rw-rw-rw-   0        0        0    29098 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/templates/index.html
--rw-rw-rw-   0        0        0     4908 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/url.py
--rw-rw-rw-   0        0        0       42 2023-06-13 13:25:16.627336 FindJobsTW-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      936 2023-06-13 13:24:57.000000 FindJobsTW-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.297374 FindJobsTW-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.290397 FindJobsTW-1.0.5/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 16:16:15.000000 FindJobsTW-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      591 2023-06-13 13:46:33.296377 FindJobsTW-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 16:16:15.000000 FindJobsTW-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.292390 FindJobsTW-1.0.5/findJobs/
+-rw-rw-rw-   0        0        0    20125 2023-06-13 13:22:37.000000 FindJobsTW-1.0.5/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0      133 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/findJobs/__init__.py
+-rw-rw-rw-   0        0        0     5368 2023-06-13 13:03:17.000000 FindJobsTW-1.0.5/findJobs/app.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.294384 FindJobsTW-1.0.5/findJobs/static/
+-rw-rw-rw-   0        0        0  1245103 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/findJobs/static/drake.png
+-rw-rw-rw-   0        0        0      382 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/findJobs/static/styles.css
+drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.295380 FindJobsTW-1.0.5/findJobs/static/temp/
+-rw-rw-rw-   0        0        0        0 2023-06-13 13:43:36.000000 FindJobsTW-1.0.5/findJobs/static/temp/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.296377 FindJobsTW-1.0.5/findJobs/templates/
+-rw-rw-rw-   0        0        0    29098 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/findJobs/templates/index.html
+-rw-rw-rw-   0        0        0     5064 2023-06-13 13:34:51.000000 FindJobsTW-1.0.5/findJobs/url.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 13:46:33.297374 FindJobsTW-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-06-13 13:44:27.000000 FindJobsTW-1.0.5/setup.py
```

### Comparing `FindJobsTW-1.0.4/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-1.0.5/FindJobsTW.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.4/LICENSE` & `FindJobsTW-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.4/PKG-INFO` & `FindJobsTW-1.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.4/findJobs/FindJobs.py` & `FindJobsTW-1.0.5/findJobs/FindJobs.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.4/findJobs/app.py` & `FindJobsTW-1.0.5/findJobs/app.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.4/findJobs/static/drake.png` & `FindJobsTW-1.0.5/findJobs/static/drake.png`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.4/findJobs/templates/index.html` & `FindJobsTW-1.0.5/findJobs/templates/index.html`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.4/findJobs/url.py` & `FindJobsTW-1.0.5/findJobs/url.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 def search_url(submit):
     url = "https://www.104.com.tw/jobs/search/?jobsource=2018indexpoc&ro=0"
     ori_url = "https://www.104.com.tw/jobs/search/?jobsource=2018indexpoc&ro=0"
+    k = keyword(submit)
     j = jobtype(submit)
     a = area(submit)
     u = update_date(submit)
     s = salary_type(submit)
     s2 = salary_conditions(submit)
     e = experience(submit)
-    url = f"{ori_url}&{j}&{a}&{u}&{s}&{s2}&{e}"
+    url = f"{ori_url}&{k}&{j}&{a}&{u}&{s}&{s2}&{e}"
     while "&&" in url:
         url = url.replace("&&", "&")
     return url
 
 jdict = {
     "經營／人資類" : "2001000000" ,
     "行政／總務／法務類" : "2002000000" ,
@@ -29,14 +30,20 @@
     "學術／教育／輔導類" : "2016000000" ,
     "研發相關類" : "2008000000" ,
     "生產製造／品管／環衛類" : "2009000000" ,
     "軍警消／保全類" : "2017000000" ,
     "其他職類" : "2018000000" 
 }
 
+def keyword(submit):
+    keyword = ""
+    s1 = submit.get("關鍵字")
+    keyword = "keyword=" + s1
+    return keyword
+
 def salary_conditions(submit):
     salary = ""
     s1 = submit["薪資待遇"]
     s2 = submit["薪資下限"]
     s3 = submit["薪資上限"]
     if s1 == "default": #不限就沒東西
         return ""
```

### Comparing `FindJobsTW-1.0.4/setup.py` & `FindJobsTW-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='1.0.4',      
+    version='1.0.5',      
     packages=find_packages(),    
     install_requires=requirements,
     package_data={
-        'findJobs': ['templates/*', 'static/*']
+        'findJobs': ['templates/*', 'static/*', 'static/temp/*']
     },  
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
     description="A Python package to find jobs on 104.com.tw based on specific keywords.",
     long_description=open('README.md', 'r', encoding='utf-8').read(),# 若Discription.md中有中文 須加上 encoding="utf-8"
     long_description_content_type="text/markdown",
     url="https://github.com/DannyFin/FindJobsTW",
```

