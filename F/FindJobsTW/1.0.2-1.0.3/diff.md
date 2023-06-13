# Comparing `tmp/FindJobsTW-1.0.2.tar.gz` & `tmp/FindJobsTW-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-1.0.2.tar", last modified: Mon Jun 12 09:46:33 2023, max compression
+gzip compressed data, was "FindJobsTW-1.0.3.tar", last modified: Tue Jun 13 07:03:09 2023, max compression
```

## Comparing `FindJobsTW-1.0.2.tar` & `FindJobsTW-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.084308 FindJobsTW-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.037751 FindJobsTW-1.0.2/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 09:46:32.000000 FindJobsTW-1.0.2/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       72 2023-06-12 09:32:38.000000 FindJobsTW-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      591 2023-06-12 09:46:33.083305 FindJobsTW-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.046778 FindJobsTW-1.0.2/findJobs/
--rw-rw-rw-   0        0        0    17529 2023-06-12 09:45:45.000000 FindJobsTW-1.0.2/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0      133 2023-06-12 09:19:48.000000 FindJobsTW-1.0.2/findJobs/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-06-12 09:15:10.000000 FindJobsTW-1.0.2/findJobs/app.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.049778 FindJobsTW-1.0.2/findJobs/static/
--rw-rw-rw-   0        0        0      382 2023-06-12 08:30:14.000000 FindJobsTW-1.0.2/findJobs/static/styles.css
-drwxrwxrwx   0        0        0        0 2023-06-12 09:46:33.080307 FindJobsTW-1.0.2/findJobs/templates/
--rw-rw-rw-   0        0        0    27906 2023-06-12 09:45:41.000000 FindJobsTW-1.0.2/findJobs/templates/index.html
--rw-rw-rw-   0        0        0     4908 2023-06-12 04:00:23.000000 FindJobsTW-1.0.2/findJobs/url.py
--rw-rw-rw-   0        0        0       42 2023-06-12 09:46:33.084308 FindJobsTW-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      936 2023-06-12 09:46:17.000000 FindJobsTW-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.590001 FindJobsTW-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.565417 FindJobsTW-1.0.3/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 07:03:09.000000 FindJobsTW-1.0.3/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-06-12 09:32:38.000000 FindJobsTW-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      591 2023-06-13 07:03:09.588003 FindJobsTW-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.575422 FindJobsTW-1.0.3/findJobs/
+-rw-rw-rw-   0        0        0    17986 2023-06-13 06:58:13.000000 FindJobsTW-1.0.3/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0      133 2023-06-12 09:19:48.000000 FindJobsTW-1.0.3/findJobs/__init__.py
+-rw-rw-rw-   0        0        0     5369 2023-06-13 07:00:39.000000 FindJobsTW-1.0.3/findJobs/app.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.583007 FindJobsTW-1.0.3/findJobs/static/
+-rw-rw-rw-   0        0        0  1245103 2023-06-08 05:24:31.000000 FindJobsTW-1.0.3/findJobs/static/drake.png
+-rw-rw-rw-   0        0        0      382 2023-06-12 08:30:14.000000 FindJobsTW-1.0.3/findJobs/static/styles.css
+drwxrwxrwx   0        0        0        0 2023-06-13 07:03:09.584999 FindJobsTW-1.0.3/findJobs/templates/
+-rw-rw-rw-   0        0        0    29098 2023-06-13 03:43:41.000000 FindJobsTW-1.0.3/findJobs/templates/index.html
+-rw-rw-rw-   0        0        0     4908 2023-06-12 04:00:23.000000 FindJobsTW-1.0.3/findJobs/url.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:03:09.591002 FindJobsTW-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      936 2023-06-13 07:02:21.000000 FindJobsTW-1.0.3/setup.py
```

### Comparing `FindJobsTW-1.0.2/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-1.0.3/FindJobsTW.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.2/LICENSE` & `FindJobsTW-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.2/PKG-INFO` & `FindJobsTW-1.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.2/findJobs/FindJobs.py` & `FindJobsTW-1.0.3/findJobs/FindJobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,14 +289,15 @@
         for bar, percentage in zip(bars, percentages):
             plt.text(bar.get_width() + 0.2, bar.get_y() + bar.get_height()/2, 
                      '{0:.1f}%'.format(percentage), va='center')
 
         # 顯示圖形
         plt.gca().invert_yaxis()  # 倒轉y軸，讓最高的頻率在頂部
         plt.show()
+        return plt
     
     def parse_salary(self, s):
         pattern_1 = r"(時薪|面議|月薪|年薪|論件計酬|日薪)([\d,]+)~([\d,]+)元"
         pattern_2 = r"(時薪|面議|月薪|年薪|論件計酬|日薪)([\d,]+)元以上"
         pattern_3 = r"(時薪|面議|月薪|年薪|論件計酬|日薪)([\d,]+)元"
         pattern_4 = r"待遇面議"
 
@@ -310,31 +311,36 @@
             salary_type, salary = re.match(pattern_3, s).groups()
             return {"薪資型態": salary_type, "薪資下限": salary, "薪資上限": salary}
         elif re.match(pattern_4, s):
             return {"薪資型態": "待遇面議", "薪資下限": "面議", "薪資上限": "面議"}
         else:
             return {"薪資型態": "未知", "薪資下限": "未知", "薪資上限": "未知"}
     
-    def draw_box(self):
+    def draw_box(self, show = True):
+        plt.figure() #清空圖形，不然連續呼叫時會出錯
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
-        plt.title('月薪下限和上限的箱型圖')
+        plt.title(self.keyword + '月薪下限和上限的箱型圖')
         plt.ylabel('薪資')
-        plt.show()
+        plt.savefig("./static/temp/salary_boxplot.png", dpi=150, bbox_inches='tight')
+        if show:
+            plt.show()
+        return plt
     
-    def draw_density(self):
+    def draw_density(self, show = True):
+        plt.figure() #清空圖形，不然連續呼叫時會出錯
         df = self.jobs.copy()
         # Filter the dataframe
         df = df[df['薪資型態'] == '月薪']
         df = df[(df['薪資下限'] != '面議') & (df['薪資上限'] != '面議')]
 
         # Replace '無上限' with '薪資下限'
         df.loc[df['薪資上限'] == '無上限', '薪資上限'] = df.loc[df['薪資上限'] == '無上限', '薪資下限']
@@ -343,23 +349,26 @@
         df['薪資下限'] = df['薪資下限'].str.replace(',', '').astype(float)
         df['薪資上限'] = df['薪資上限'].str.replace(',', '').astype(float)
 
         # Plot the kernel density estimation for salary lower and upper limit
         df['薪資下限'].plot(kind='kde', label='薪資下限')
         df['薪資上限'].plot(kind='kde', label='薪資上限')
 
-        plt.title('月薪下限和上限的密度分佈')
+        plt.title(self.keyword + '月薪下限和上限的密度分佈')
         plt.xlabel('薪資')
         plt.ylabel('密度')
         plt.legend()
-        plt.show()
+        plt.savefig("./static/temp/salary_density.png", bbox_inches='tight')
+        if show:
+            plt.show()
+        return plt
 
 if __name__ == "__main__":
-    keyword = "數據分析師"
+    keyword = "分析師"
     jobs = Jobs(keyword)
-    jobs.search_links(max_pages = 3)#一頁是20個職缺
+    jobs.search_links(max_pages = 1)#一頁是20個職缺
     jobs.find_jobs()
     jobs.save_jobs()
     jobs.draw_box()
     jobs.draw_density()
     #jobs.show("all") #一次秀出全部
     jobs.show("職務類別")
```

### Comparing `FindJobsTW-1.0.2/findJobs/app.py` & `FindJobsTW-1.0.3/findJobs/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     salary_condition = ''
     global custom_salary_min
     custom_salary_min = ''
     global custom_salary_max
     custom_salary_max = ''
     global experience
     experience = ''
+    image_filename = None
+    image_filename2 = None
     message = ""
     df = None
     table = None
     if request.method == 'POST':
         if 'clear' in request.form:
             # 如果按下了 "清除" 按鈕，將所有的模板變數設為空
             return render_template('index.html', message="", 
@@ -85,39 +87,52 @@
         url = search_url(conditions)
         print(url)
         message = findjobs(conditions)
         
         job = Jobs(JobKeyword)
         job.search_links(max_pages=int(int(jobNumber)/20)+1, ori_url = url)
         job.find_jobs(max_jobs = int(jobNumber))
+        job.draw_box(show = False)
+        job.draw_density(show = False)
         job.save_jobs()
         df = job.jobs.head(10)
         table = df.to_html(classes='data', header="true", index="false")
-        
+        image_filename = 'temp/salary_boxplot.png'
+        image_filename2 = 'temp/salary_density.png'
     
     return render_template('index.html', message=message, 
                            table = table,
                            current_JobKeyword = JobKeyword,
                            current_JobNumber = jobNumber,
                            current_job_type=job_type, 
                            current_area_condition = area_condition,
                            current_update_date = update_date,
                            current_attendance_system = attendance_system,
                            current_salarytype = salarytype,
                            current_salary_condition = salary_condition,
                            current_custom_salary_min = custom_salary_min,
                            current_custom_salary_max = custom_salary_max,
-                           current_experience = experience)
+                           current_experience = experience,
+                           image_filename=image_filename,
+                           image_filename2 = image_filename2)
 
 @app.route('/execute')
 def execute_findjobs():
     result = findjobs()
     if result is None:
         result = "No result returned from findjobs"
     return render_template('index.html', message=result)
 
 def open_browser():
     webbrowser.open_new('http://127.0.0.1:5000/')
 
+@app.route('/some_route')
+def some_route():
+    # Generate or select the image
+    image_filename = 'temp/salary_boxplot.png'
+    
+    # Render the template
+    return render_template('index.html', image_filename=image_filename)
+
 if __name__ == '__main__':
     Timer(1, open_browser).start()
     app.run(debug=True, use_reloader=False)
```

### Comparing `FindJobsTW-1.0.2/findJobs/templates/index.html` & `FindJobsTW-1.0.3/findJobs/templates/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -275,15 +275,15 @@
                                     <option value="1年以下"{% if current_experience == '1年以下' %}selected{% endif %}>1年以下</option>
                                     <option value="1-3年"{% if current_experience == '1-3年' %}selected{% endif %}>1-3年</option>
                                     <option value="3-5年"{% if current_experience == '3-5年' %}selected{% endif %}>3-5年</option>
                                     <option value="5-10年"{% if current_experience == '5-10年' %}selected{% endif %}>5-10年</option>
                                     <option value="10年以上"{% if current_experience == '10年以上' %}selected{% endif %}>10年以上</option>
                                 </select>
                             </div>
-                            <button type="submit" class="btn btn-primary btn-lg btn-block"  nclick="submitForm()">提交</button>
+                            <button type="submit" id="submitButton" class="btn btn-primary btn-lg btn-block">提交</button>
                             <style>
                                 /* 增加对 "薪資條件" 标签单独控制的能力 */
                                 .container {
                                     margin-top: 5em;
                                 }
                             </style>
                         </form>
@@ -293,16 +293,30 @@
                 <div class="card mt-3">
                     <div class="card-body">
                         <p class="card-text">{{ message | safe }}</p>
                     </div>
                 </div>
                 {% endif %}
                 <div class="container">
+                    {% if table %}
                     {{ table | safe }}
+                    {% endif %}
                 </div>
+                <img src="{{ url_for('static', filename='drake.png') }}" alt="My Image" style="width: 90%; height: auto;">
+                <h1>Your Plot</h1>
+                {% if image_filename %}
+                <img src="{{ url_for('static', filename= image_filename) }}" alt="Plot Image" style="width: 70%; height: auto;">
+                {% else %}
+                <p>The box plot is being generated, please wait...</p>
+                {% endif %}
+                {% if image_filename2 %}
+                <img src="{{ url_for('static', filename= image_filename2) }}" alt="Plot Image" style="width: 70%; height: auto;">
+                {% else %}
+                <p>The density plot is being generated, please wait...</p>
+                {% endif %}
             </div>
         </div>
     </div>
     <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
     <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
     <script>
         $(function() {
@@ -316,9 +330,17 @@
                 }
             });
         });
         function clearForm() {
             document.getElementById("myForm").reset();
         }
     </script>
+    <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
+    <script>
+    $(document).ready(function() {
+        $('#submitButton').click(function() {
+            alert("已送出資料，請至VS Code Terminal查看下載進度");  // 這行會顯示一個彈出窗口，並顯示文字"已送出資料"
+        });
+    });
+    </script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -93,8 +93,15 @@
 % if current_experience == '3-5å¹´' %}selected{% endif %}>3-5å¹´
 % if current_experience == '5-10å¹´' %}selected{% endif %}>5-10å¹´
 % if current_experience == '10å¹´ä»¥ä¸' %}selected{% endif %}>10å¹´ä»¥ä¸
 æäº¤
 {% if message %}
 {{ message | safe }}
 {% endif %}
-{{ table | safe }}
+{% if table %} {{ table | safe }} {% endif %}
+[My Image]
+****** Your Plot ******
+{% if image_filename %} [Plot Image] {% else %}
+The box plot is being generated, please wait...
+{% endif %} {% if image_filename2 %} [Plot Image] {% else %}
+The density plot is being generated, please wait...
+{% endif %}
```

### Comparing `FindJobsTW-1.0.2/findJobs/url.py` & `FindJobsTW-1.0.3/findJobs/url.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.2/setup.py` & `FindJobsTW-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='1.0.2',      
+    version='1.0.3',      
     packages=find_packages(),    
     install_requires=requirements,
     package_data={
         'findJobs': ['templates/*', 'static/*']
     },  
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
```

