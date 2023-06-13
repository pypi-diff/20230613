# Comparing `tmp/FindJobsTW-1.0.3.tar.gz` & `tmp/FindJobsTW-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-1.0.3.tar", last modified: Tue Jun 13 07:03:09 2023, max compression
+gzip compressed data, was "FindJobsTW-1.0.4.tar", last modified: Tue Jun 13 13:25:16 2023, max compression
```

## Comparing `FindJobsTW-1.0.3.tar` & `FindJobsTW-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.590001 FindJobsTW-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.565417 FindJobsTW-1.0.3/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       72 2023-06-12 09:32:38.000000 FindJobsTW-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      591 2023-06-13 07:03:09.588003 FindJobsTW-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.575422 FindJobsTW-1.0.3/findJobs/
--rw-rw-rw-   0        0        0    17986 2023-06-13 06:58:13.000000 FindJobsTW-1.0.3/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0      133 2023-06-12 09:19:48.000000 FindJobsTW-1.0.3/findJobs/__init__.py
--rw-rw-rw-   0        0        0     5369 2023-06-13 07:00:39.000000 FindJobsTW-1.0.3/findJobs/app.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.583007 FindJobsTW-1.0.3/findJobs/static/
--rw-rw-rw-   0        0        0  1245103 2023-06-08 05:24:31.000000 FindJobsTW-1.0.3/findJobs/static/drake.png
--rw-rw-rw-   0        0        0      382 2023-06-12 08:30:14.000000 FindJobsTW-1.0.3/findJobs/static/styles.css
-drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.584999 FindJobsTW-1.0.3/findJobs/templates/
--rw-rw-rw-   0        0        0    29098 2023-06-13 03:43:41.000000 FindJobsTW-1.0.3/findJobs/templates/index.html
--rw-rw-rw-   0        0        0     4908 2023-06-12 04:00:23.000000 FindJobsTW-1.0.3/findJobs/url.py
--rw-rw-rw-   0        0        0       42 2023-06-13 07:03:09.591002 FindJobsTW-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      936 2023-06-13 07:02:21.000000 FindJobsTW-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.627336 FindJobsTW-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.618366 FindJobsTW-1.0.4/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 13:25:16.000000 FindJobsTW-1.0.4/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 16:16:15.000000 FindJobsTW-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      591 2023-06-13 13:25:16.626340 FindJobsTW-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 16:16:15.000000 FindJobsTW-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.622353 FindJobsTW-1.0.4/findJobs/
+-rw-rw-rw-   0        0        0    20125 2023-06-13 13:22:37.000000 FindJobsTW-1.0.4/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0      133 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/__init__.py
+-rw-rw-rw-   0        0        0     5368 2023-06-13 13:03:17.000000 FindJobsTW-1.0.4/findJobs/app.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.624346 FindJobsTW-1.0.4/findJobs/static/
+-rw-rw-rw-   0        0        0  1245103 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/static/drake.png
+-rw-rw-rw-   0        0        0      382 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/static/styles.css
+drwxrwxrwx   0        0        0        0 2023-06-13 13:25:16.625343 FindJobsTW-1.0.4/findJobs/templates/
+-rw-rw-rw-   0        0        0    29098 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/templates/index.html
+-rw-rw-rw-   0        0        0     4908 2023-06-13 11:41:35.000000 FindJobsTW-1.0.4/findJobs/url.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 13:25:16.627336 FindJobsTW-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      936 2023-06-13 13:24:57.000000 FindJobsTW-1.0.4/setup.py
```

### Comparing `FindJobsTW-1.0.3/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-1.0.4/FindJobsTW.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.3/LICENSE` & `FindJobsTW-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.3/PKG-INFO` & `FindJobsTW-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.3/findJobs/FindJobs.py` & `FindJobsTW-1.0.4/findJobs/FindJobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 import requests
 import time
 import pandas as pd
 import re
 from bs4 import BeautifulSoup
 from lxml import html
 from collections import Counter
+import matplotlib
+matplotlib.use('Agg')#必須在之前設定，才可以在非main中調用
 import matplotlib.pyplot as plt
 import seaborn as sns
 #中文
 plt.rcParams['font.sans-serif'] = ['Microsoft JhengHei'] 
 plt.rcParams['axes.unicode_minus'] = False
 
 
+
+
+
 class Jobs:
     
     def __init__ (self, keyword):
         self.keyword = keyword
         self.job_links = []
         self.jobs = []
         self.data = []
@@ -212,15 +217,16 @@
                 data.append(job_data)
                 print(f"正在爬取第{i+1}/{min(self.job_links.shape[0], max_jobs)}個工作")
             except KeyboardInterrupt:
                 break
             except:
                 continue
             if i >= max_jobs-1:
-                break        
+                break 
+                   
         fields =['公司名稱', '職缺名稱', '職缺連結', '職務名稱', '職務類別', '工作待遇',
                  '薪資型態', '薪資下限', '薪資上限',
                  '工作性質', '上班地點', '遠端工作', '管理責任', '出差外派', '上班時段',
                  '休假制度', '可上班日', '需求人數', '語文條件', '工作經歷', '學歷要求',
                  '科系要求', '擅長工具', '工作技能', '具備駕照', '具備證照', '法定項目',
                  '其他福利', '招募福利']
         df = pd.DataFrame(columns = fields, data = data)
@@ -312,35 +318,36 @@
             return {"薪資型態": salary_type, "薪資下限": salary, "薪資上限": salary}
         elif re.match(pattern_4, s):
             return {"薪資型態": "待遇面議", "薪資下限": "面議", "薪資上限": "面議"}
         else:
             return {"薪資型態": "未知", "薪資下限": "未知", "薪資上限": "未知"}
     
     def draw_box(self, show = True):
-        plt.figure() #清空圖形，不然連續呼叫時會出錯
         df = self.jobs.copy()
         # Filter the dataframe
         df = df[df['薪資型態'] == '月薪']
         df = df[(df['薪資下限'] != '面議') & (df['薪資上限'] != '面議')]
         # Replace '無上限' with '薪資下限'
         df.loc[df['薪資上限'] == '無上限', '薪資上限'] = df.loc[df['薪資上限'] == '無上限', '薪資下限']
         # Convert to numeric values
         df['薪資下限'] = df['薪資下限'].str.replace(',', '').astype(float)
         df['薪資上限'] = df['薪資上限'].str.replace(',', '').astype(float)
         # Plot boxplot
         df[['薪資下限', '薪資上限']].plot(kind='box')
         plt.title(self.keyword + '月薪下限和上限的箱型圖')
         plt.ylabel('薪資')
-        plt.savefig("./static/temp/salary_boxplot.png", dpi=150, bbox_inches='tight')
-        if show:
+        if show:#show也會清空
             plt.show()
-        return plt
-    
+        else:
+            path = self.get_static_temp_path() + "/salary_boxplot.png"
+            print("儲存plt", path)
+            plt.savefig(path, dpi=150, bbox_inches='tight')
+        plt.clf()
+
     def draw_density(self, show = True):
-        plt.figure() #清空圖形，不然連續呼叫時會出錯
         df = self.jobs.copy()
         # Filter the dataframe
         df = df[df['薪資型態'] == '月薪']
         df = df[(df['薪資下限'] != '面議') & (df['薪資上限'] != '面議')]
 
         # Replace '無上限' with '薪資下限'
         df.loc[df['薪資上限'] == '無上限', '薪資上限'] = df.loc[df['薪資上限'] == '無上限', '薪資下限']
@@ -353,22 +360,78 @@
         df['薪資下限'].plot(kind='kde', label='薪資下限')
         df['薪資上限'].plot(kind='kde', label='薪資上限')
 
         plt.title(self.keyword + '月薪下限和上限的密度分佈')
         plt.xlabel('薪資')
         plt.ylabel('密度')
         plt.legend()
-        plt.savefig("./static/temp/salary_density.png", bbox_inches='tight')
         if show:
             plt.show()
-        return plt
+        else:
+            path = "./" + self.get_static_temp_path() + "/salary_density.png"
+            print("儲存plt", path)
+            plt.savefig(path, bbox_inches='tight')
+        plt.clf()
+
 
+    def get_static_temp_path(self):
+        # 獲取當前檔案的目錄
+        current_dir = os.path.dirname(os.path.realpath(__file__))
+
+        # 往上一層一層地搜尋，直到找到包含 'findJobs' 或 'FindJobsTW' 的路徑
+        while current_dir != os.path.sep:
+            if 'findJobs' in current_dir or 'FindJobsTW' in current_dir:
+                return os.path.relpath(os.path.join(current_dir, 'static/temp'))
+            current_dir = os.path.dirname(current_dir)
+    
+    def help(self):
+        print("在瀏覽器中執行請參考下列代碼:")
+        print()
+        text1 = '''
+            from threading import Timer
+            import webbrowser
+            from findJobs import create_app, hlep
+
+            def open_browser():
+                webbrowser.open_new('http://127.0.0.1:5000/')
+
+            app = create_app()
+
+            if __name__ == '__main__':
+                Timer(1, open_browser).start()
+                app.run(debug=True, use_reloader=False)
+            '''
+        print(text1)
+        print()
+        print()
+        print("直接於程式碼中執行，請參考下列代碼:")
+        print()
+        text2 = '''
+            from findJobs.FindJobs import Jobs
+            keyword = "ESG"
+            job = Jobs(keyword)
+            job.search_links(max_pages=1) #設定爬取的頁數，一頁20個
+            job.find_jobs()#找工作
+            job.save_jobs()#把找到的工作存成excel檔案
+            job.draw_box()
+            job.draw_density()
+            job.show(column = "all") #查看想統計的欄位，如果欄位名稱輸入"all"，會統計所有欄位，
+            #若要快速關閉視窗可按ctrl+w
+            '''
+        print(text2)
+        print()
+
+    
 if __name__ == "__main__":
-    keyword = "分析師"
+    a = Jobs("111")
+    a.help()
+    #print(os.path.relpath(a.get_static_temp_path()))
+''' keyword = "分析師"
     jobs = Jobs(keyword)
     jobs.search_links(max_pages = 1)#一頁是20個職缺
-    jobs.find_jobs()
+    jobs.find_jobs(max_jobs = 10)
     jobs.save_jobs()
-    jobs.draw_box()
-    jobs.draw_density()
+    jobs.draw_box(show = False)
+    jobs.draw_density(show = False)
     #jobs.show("all") #一次秀出全部
-    jobs.show("職務類別")
+    jobs.show("職務類別")
+    #help()'''
```

### Comparing `FindJobsTW-1.0.3/findJobs/app.py` & `FindJobsTW-1.0.4/findJobs/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         job.find_jobs(max_jobs = int(jobNumber))
         job.draw_box(show = False)
         job.draw_density(show = False)
         job.save_jobs()
         df = job.jobs.head(10)
         table = df.to_html(classes='data', header="true", index="false")
         image_filename = 'temp/salary_boxplot.png'
-        image_filename2 = 'temp/salary_density.png'
+        image_filename2 ='temp/salary_density.png'
     
     return render_template('index.html', message=message, 
                            table = table,
                            current_JobKeyword = JobKeyword,
                            current_JobNumber = jobNumber,
                            current_job_type=job_type, 
                            current_area_condition = area_condition,
```

### Comparing `FindJobsTW-1.0.3/findJobs/static/drake.png` & `FindJobsTW-1.0.4/findJobs/static/drake.png`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.3/findJobs/templates/index.html` & `FindJobsTW-1.0.4/findJobs/templates/index.html`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.3/findJobs/url.py` & `FindJobsTW-1.0.4/findJobs/url.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.3/setup.py` & `FindJobsTW-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='1.0.3',      
+    version='1.0.4',      
     packages=find_packages(),    
     install_requires=requirements,
     package_data={
         'findJobs': ['templates/*', 'static/*']
     },  
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
```

